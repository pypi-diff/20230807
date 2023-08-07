# Comparing `tmp/econia_sdk-1.0.2.tar.gz` & `tmp/econia_sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econia_sdk-1.0.2.tar", max compression
+gzip compressed data, was "econia_sdk-1.0.3.tar", max compression
```

## Comparing `econia_sdk-1.0.2.tar` & `econia_sdk-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0       61 2023-07-27 18:10:49.224251 econia_sdk-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-07-21 16:14:17.854900 econia_sdk-1.0.2/econia_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 16:14:17.854950 econia_sdk-1.0.2/econia_sdk/entry/__init__.py
--rw-r--r--   0        0        0     4144 2023-07-21 16:14:17.855021 econia_sdk-1.0.2/econia_sdk/entry/incentives.py
--rw-r--r--   0        0        0     9305 2023-07-27 18:56:10.502928 econia_sdk-1.0.2/econia_sdk/entry/market.py
--rw-r--r--   0        0        0     3637 2023-07-21 16:14:17.855149 econia_sdk-1.0.2/econia_sdk/entry/registry.py
--rw-r--r--   0        0        0     3883 2023-07-21 16:14:17.855205 econia_sdk-1.0.2/econia_sdk/entry/user.py
--rw-r--r--   0        0        0     3534 2023-07-26 14:37:08.196402 econia_sdk-1.0.2/econia_sdk/lib.py
--rw-r--r--   0        0        0      551 2023-07-27 00:22:09.389353 econia_sdk-1.0.2/econia_sdk/types.py
--rw-r--r--   0        0        0        0 2023-07-26 14:37:08.196805 econia_sdk-1.0.2/econia_sdk/view/__init__.py
--rw-r--r--   0        0        0     2640 2023-07-27 18:56:10.506615 econia_sdk-1.0.2/econia_sdk/view/incentives.py
--rw-r--r--   0        0        0     6790 2023-07-27 18:56:10.513134 econia_sdk-1.0.2/econia_sdk/view/market.py
--rw-r--r--   0        0        0     8509 2023-07-27 18:56:26.619749 econia_sdk-1.0.2/econia_sdk/view/registry.py
--rw-r--r--   0        0        0      264 2023-07-27 18:56:10.514681 econia_sdk-1.0.2/econia_sdk/view/resource_account.py
--rw-r--r--   0        0        0    17151 2023-07-27 18:56:10.509675 econia_sdk-1.0.2/econia_sdk/view/user.py
--rw-r--r--   0        0        0      409 2023-07-27 19:04:47.825946 econia_sdk-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      589 1970-01-01 00:00:00.000000 econia_sdk-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      543 2023-08-07 16:28:45.544810 econia_sdk-1.0.3/README.md
+-rw-r--r--   0        0        0      118 2023-08-04 16:51:43.612860 econia_sdk-1.0.3/econia_sdk/README.md
+-rw-r--r--   0        0        0       31 2023-08-02 13:21:36.047375 econia_sdk-1.0.3/econia_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:14:17.854950 econia_sdk-1.0.3/econia_sdk/entry/__init__.py
+-rw-r--r--   0        0        0     4144 2023-07-21 16:14:17.855021 econia_sdk-1.0.3/econia_sdk/entry/incentives.py
+-rw-r--r--   0        0        0     9305 2023-08-04 16:52:42.145623 econia_sdk-1.0.3/econia_sdk/entry/market.py
+-rw-r--r--   0        0        0     3637 2023-07-21 16:14:17.855149 econia_sdk-1.0.3/econia_sdk/entry/registry.py
+-rw-r--r--   0        0        0     3883 2023-07-21 16:14:17.855205 econia_sdk-1.0.3/econia_sdk/entry/user.py
+-rw-r--r--   0        0        0     3566 2023-08-04 16:52:39.413263 econia_sdk-1.0.3/econia_sdk/lib.py
+-rw-r--r--   0        0        0      604 2023-07-28 20:52:31.009030 econia_sdk-1.0.3/econia_sdk/types.py
+-rw-r--r--   0        0        0        0 2023-08-07 17:44:07.609900 econia_sdk-1.0.3/econia_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     4965 2023-08-07 17:44:07.610413 econia_sdk-1.0.3/econia_sdk/utils/decimals.py
+-rw-r--r--   0        0        0        0 2023-07-28 20:52:31.009074 econia_sdk-1.0.3/econia_sdk/view/__init__.py
+-rw-r--r--   0        0        0     4629 2023-08-04 16:52:46.287202 econia_sdk-1.0.3/econia_sdk/view/incentives.py
+-rw-r--r--   0        0        0    10293 2023-08-04 16:52:49.008392 econia_sdk-1.0.3/econia_sdk/view/market.py
+-rw-r--r--   0        0        0    10203 2023-08-07 16:28:45.544957 econia_sdk-1.0.3/econia_sdk/view/registry.py
+-rw-r--r--   0        0        0      317 2023-08-04 16:52:54.531890 econia_sdk-1.0.3/econia_sdk/view/resource_account.py
+-rw-r--r--   0        0        0    21253 2023-08-04 16:52:57.326492 econia_sdk-1.0.3/econia_sdk/view/user.py
+-rw-r--r--   0        0        0      587 2023-08-07 17:46:45.745263 econia_sdk-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1029 1970-01-01 00:00:00.000000 econia_sdk-1.0.3/PKG-INFO
```

### Comparing `econia_sdk-1.0.2/econia_sdk/entry/incentives.py` & `econia_sdk-1.0.3/econia_sdk/entry/incentives.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-1.0.2/econia_sdk/entry/market.py` & `econia_sdk-1.0.3/econia_sdk/entry/market.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-1.0.2/econia_sdk/entry/registry.py` & `econia_sdk-1.0.3/econia_sdk/entry/registry.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-1.0.2/econia_sdk/entry/user.py` & `econia_sdk-1.0.3/econia_sdk/entry/user.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-1.0.2/econia_sdk/lib.py` & `econia_sdk-1.0.3/econia_sdk/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,17 @@
         type_arguments: List[str] = [],
         arguments: List = [],  # string encoded args i.e "12345" or "0xabcdef" or "abracadabra"
         ledger_version: int = -1,
     ) -> List:
         if ledger_version < 0:
             request = f"{self.aptos_client.base_url}/view"
         else:
-            request = f"{self.aptos_client.base_url}/view?ledger_version={ledger_version}"
+            request = (
+                f"{self.aptos_client.base_url}/view?ledger_version={ledger_version}"
+            )
 
         response = self.aptos_client.client.post(
             request,
             json={
                 "function": f"{self.econia_address}::{module}::{function}",
                 "type_arguments": type_arguments,
                 "arguments": arguments,
```

### Comparing `econia_sdk-1.0.2/econia_sdk/types.py` & `econia_sdk-1.0.3/econia_sdk/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,7 +29,9 @@
     Eviction = 1
     ImmediateOrCancel = 2
     ManualCancel = 3
     MaxQuoteTraded = 4
     NotEnoughLiquidity = 5
     SelfMatchMaker = 6
     SelfMatchTaker = 7
+    TooSmallToFillLot = 8
+    ViolatedLimitPrice = 9
```

### Comparing `econia_sdk-1.0.2/econia_sdk/view/user.py` & `econia_sdk-1.0.3/econia_sdk/view/user.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,71 +3,96 @@
 from aptos_sdk.account_address import AccountAddress
 
 from econia_sdk.lib import EconiaViewer
 from econia_sdk.types import CancelReason, Restriction, SelfMatchBehavior, Side
 
 
 def get_ASK(view: EconiaViewer) -> bool:
+    """
+    Public constant getter for `ASK`.
+    """
     returns = view.get_returns("user", "get_ASK")
     return bool(returns[0])
 
 
 def get_BID(view: EconiaViewer) -> bool:
+    """
+    Public constant getter for `BID`.
+    """
     returns = view.get_returns("user", "get_BID")
     return bool(returns[0])
 
 
 def get_NO_CUSTODIAN(view: EconiaViewer) -> int:
+    """
+    Public constant getter for `NO_CUSTODIAN`.
+    """
     returns = view.get_returns("user", "get_NO_CUSTODIAN")
     return int(returns[0])
 
 
 def get_CANCEL_REASON_EVICTION(view: EconiaViewer) -> int:
+    """
+    Public constant getter for `CANCEL_REASON_EVICTION`.
+    """
     returns = view.get_returns("user", "get_CANCEL_REASON_EVICTION")
     return int(returns[0])
 
 
 def get_CANCEL_REASON_IMMEDIATE_OR_CANCEL(view: EconiaViewer) -> int:
+    """
+    Public constant getter for `CANCEL_REASON_IMMEDIATE_OR_CANCEL`.
+    """
     returns = view.get_returns("user", "get_CANCEL_REASON_IMMEDIATE_OR_CANCEL")
     return int(returns[0])
 
 
 def get_CANCEL_REASON_MANUAL_CANCEL(view: EconiaViewer) -> int:
+    """
+    Public constant getter for `CANCEL_REASON_MANUAL_CANCEL`.
+    """
     returns = view.get_returns("user", "get_CANCEL_REASON_MANUAL_CANCEL")
     return int(returns[0])
 
 
 def get_CANCEL_REASON_MAX_QUOTE_TRADED(view: EconiaViewer) -> int:
+    """
+    Public constant getter for `CANCEL_REASON_MAX_QUOTE_TRADED`.
+    """
     returns = view.get_returns("user", "get_CANCEL_REASON_MAX_QUOTE_TRADED")
     return int(returns[0])
 
 
 def get_CANCEL_REASON_NOT_ENOUGH_LIQUIDITY(view: EconiaViewer) -> int:
+    """
+    Public constant getter for `CANCEL_REASON_NOT_ENOUGH_LIQUIDITY`.
+    """
     returns = view.get_returns("user", "get_CANCEL_REASON_NOT_ENOUGH_LIQUIDITY")
     return int(returns[0])
 
 
 def get_CANCEL_REASON_SELF_MATCH_TAKER(view: EconiaViewer) -> int:
+    """
+    Public constant getter for `CANCEL_REASON_SELF_MATCH_TAKER`.
+    """
     returns = view.get_returns("user", "get_CANCEL_REASON_SELF_MATCH_TAKER")
     return int(returns[0])
 
 
-def get_CANCEL_REASON_TOO_SMALL_AFTER_MATCHING(view: EconiaViewer) -> int:
-    returns = view.get_returns(
-        "user", "get_CANCEL_REASON_TOO_SMALL_AFTER_MATCHING"
-    )
-    return int(returns[0])
-
-
 def get_market_event_handle_creation_numbers(
     view: EconiaViewer,
     user: AccountAddress,
     market_id: int,
     custodian_id: int,
 ) -> Optional[dict]:
+    """
+    Return the market event handle creation numbers for `market_id` and
+    `custodian_id`, if `user` has event handles for indicated market
+    account.
+    """
     returns = view.get_returns(
         "user",
         "get_market_event_handle_creation_numbers",
         [],
         [serialize_address(user), str(market_id), str(custodian_id)],
     )
     opt_val = returns[0]["vec"]
@@ -98,14 +123,25 @@
     view: EconiaViewer,
     user: AccountAddress,
     market_id: int,
     custodian_id: int,
     limit: Optional[int] = None,
     start: Optional[int] = None,
 ) -> List[dict]:
+    """
+    Get all (or some) of the order size change events by a given user, market_id,
+    and custodian_id.
+
+    Parameters:
+    * `user`: the account address to which the events will have been emitted;
+    * `market_id`: the market id to which the events pertain.
+    * `custodian_id`: the custodian id associated with the event, usually 0.
+    * `limit`: the maximum number of events to be returned.
+    * `start`: the lowest sequence number of event to be returned
+    """
     creation_numbers = get_market_event_handle_creation_numbers(
         view, user, market_id, custodian_id
     )
     if creation_numbers is not None:
         events = view.get_events_by_creation_number(
             user,
             creation_numbers["change_order_size_events_handle_creation_num"],
@@ -114,17 +150,15 @@
         )
         returns = []
         for event in events:
             returns.append(
                 {
                     "version": int(event["version"]),
                     "guid": {
-                        "creation_number": int(
-                            event["guid"]["creation_number"]
-                        ),
+                        "creation_number": int(event["guid"]["creation_number"]),
                         "account_address": AccountAddress.from_hex(
                             event["guid"]["account_address"]
                         ),
                     },
                     "sequence_number": int(event["sequence_number"]),
                     "type": event["type"],
                     "data": {
@@ -167,14 +201,25 @@
     view: EconiaViewer,
     user: AccountAddress,
     market_id: int,
     custodian_id: int,
     limit: Optional[int] = None,
     start: Optional[int] = None,
 ) -> List[dict]:
+    """
+    Get all (or some) of the order cancel events by a given user, market_id,
+    and custodian_id.
+
+    Parameters:
+    * `user`: the account address to which the events will have been emitted;
+    * `market_id`: the market id to which the events pertain.
+    * `custodian_id`: the custodian id associated with the event, usually 0.
+    * `limit`: the maximum number of events to be returned.
+    * `start`: the lowest sequence number of event to be returned
+    """
     creation_numbers = get_market_event_handle_creation_numbers(
         view, user, market_id, custodian_id
     )
     if creation_numbers is not None:
         events = view.get_events_by_creation_number(
             user,
             creation_numbers["cancel_order_events_handle_creation_num"],
@@ -210,29 +255,38 @@
             "sequence_number_for_trade": int(
                 event["data"]["sequence_number_for_trade"]
             ),
             "size": int(event["data"]["size"]),
             "taker": AccountAddress.from_hex(event["data"]["taker"]),
             "taker_custodian_id": int(event["data"]["taker_custodian_id"]),
             "taker_order_id": int(event["data"]["taker_order_id"]),
-            "taker_quote_fees_paid": int(
-                event["data"]["taker_quote_fees_paid"]
-            ),
+            "taker_quote_fees_paid": int(event["data"]["taker_quote_fees_paid"]),
         },
     }
 
 
 def get_fill_events(
     view: EconiaViewer,
     user: AccountAddress,
     market_id: int,
     custodian_id: int,
     limit: Optional[int] = None,
     start: Optional[int] = None,
 ) -> List[dict]:
+    """
+    Get all (or some) of the order fill events by/for a given user, market_id,
+    and custodian_id.
+
+    Parameters:
+    * `user`: the account address to which the events will have been emitted;
+    * `market_id`: the market id to which the events pertain.
+    * `custodian_id`: the custodian id associated with the event, usually 0.
+    * `limit`: the maximum number of events to be returned.
+    * `start`: the lowest sequence number of event to be returned
+    """
     creation_numbers = get_market_event_handle_creation_numbers(
         view, user, market_id, custodian_id
     )
     if creation_numbers is not None:
         events = view.get_events_by_creation_number(
             user,
             creation_numbers["fill_events_handle_creation_num"],
@@ -251,14 +305,25 @@
     view: EconiaViewer,
     user: AccountAddress,
     market_id: int,
     custodian_id: int,
     limit: Optional[int] = None,
     start: Optional[int] = None,
 ) -> List[dict]:
+    """
+    Get all (or some) of the market order placement events by a given user,
+    market_id, and custodian_id.
+
+    Parameters:
+    * `user`: the account address to which the events will have been emitted;
+    * `market_id`: the market id to which the events pertain.
+    * `custodian_id`: the custodian id associated with the event, usually 0.
+    * `limit`: the maximum number of events to be returned.
+    * `start`: the lowest sequence number of event to be returned
+    """
     creation_numbers = get_market_event_handle_creation_numbers(
         view, user, market_id, custodian_id
     )
     if creation_numbers is not None:
         events = view.get_events_by_creation_number(
             user,
             creation_numbers["place_market_order_events_handle_creation_num"],
@@ -267,17 +332,15 @@
         )
         returns = []
         for event in events:
             returns.append(
                 {
                     "version": int(event["version"]),
                     "guid": {
-                        "creation_number": int(
-                            event["guid"]["creation_number"]
-                        ),
+                        "creation_number": int(event["guid"]["creation_number"]),
                         "account_address": AccountAddress.from_hex(
                             event["guid"]["account_address"]
                         ),
                     },
                     "sequence_number": int(event["sequence_number"]),
                     "type": event["type"],
                     "data": {
@@ -307,14 +370,25 @@
     view: EconiaViewer,
     user: AccountAddress,
     market_id: int,
     custodian_id: int,
     limit: Optional[int] = None,
     start: Optional[int] = None,
 ) -> List[dict]:
+    """
+    Get all (or some) of the limit order placement events by a given user,
+    market_id, and custodian_id.
+
+    Parameters:
+    * `user`: the account address to which the events will have been emitted;
+    * `market_id`: the market id to which the events pertain.
+    * `custodian_id`: the custodian id associated with the event, usually 0.
+    * `limit`: the maximum number of events to be returned.
+    * `start`: the lowest sequence number of event to be returned
+    """
     creation_numbers = get_market_event_handle_creation_numbers(
         view, user, market_id, custodian_id
     )
     if creation_numbers is not None:
         events = view.get_events_by_creation_number(
             user,
             creation_numbers["place_limit_order_events_handle_creation_num"],
@@ -323,17 +397,15 @@
         )
         returns = []
         for event in events:
             returns.append(
                 {
                     "version": int(event["version"]),
                     "guid": {
-                        "creation_number": int(
-                            event["guid"]["creation_number"]
-                        ),
+                        "creation_number": int(event["guid"]["creation_number"]),
                         "account_address": AccountAddress.from_hex(
                             event["guid"]["account_address"]
                         ),
                     },
                     "sequence_number": int(event["sequence_number"]),
                     "type": event["type"],
                     "data": {
@@ -341,23 +413,19 @@
                         "integrator": AccountAddress.from_hex(
                             event["data"]["integrator"]
                         ),
                         "market_id": int(event["data"]["market_id"]),
                         "order_id": int(event["data"]["order_id"]),
                         "price": int(event["data"]["price"]),
                         "remaining_size": int(event["data"]["remaining_size"]),
-                        "restriction": Restriction(
-                            int(event["data"]["restriction"])
-                        ),
+                        "restriction": Restriction(int(event["data"]["restriction"])),
                         "self_match_behavior": SelfMatchBehavior(
                             int(event["data"]["self_match_behavior"])
                         ),
-                        "side": Side.ASK
-                        if bool(event["data"]["side"])
-                        else Side.BID,
+                        "side": Side.ASK if bool(event["data"]["side"]) else Side.BID,
                         "size": int(event["data"]["size"]),
                         "user": AccountAddress.from_hex(event["data"]["user"]),
                     },
                 }
             )
         return returns
     else:
@@ -369,14 +437,25 @@
 
 
 def get_all_market_account_ids_for_market_id(
     view: EconiaViewer,
     user: AccountAddress,
     market_id: int,
 ) -> list[int]:
+    """
+    Return all market account IDs associated with market ID.
+
+    Parameters:
+    * `user`: Address of user to check market account IDs for.
+    * `market_id`: Market ID to check market accounts for.
+
+    Returns:
+    * `list[int]`: Vector of user's market account IDs for given
+      market, empty if no market accounts.
+    """
     returns = view.get_returns(
         "user",
         "get_all_market_account_ids_for_market_id",
         [],
         [serialize_address(user), str(market_id)],
     )
     ids = []
@@ -385,39 +464,54 @@
     return ids
 
 
 def get_all_market_account_ids_for_user(
     view: EconiaViewer,
     user: AccountAddress,
 ) -> list[int]:
+    """
+    Return all of a user's market account IDs.
+
+    Parameters:
+    * `user`: Address of user to check market account IDs for.
+
+    Returns:
+    * `list[int]`: Vector of user's market account IDs, empty if
+      no market accounts.
+    """
     returns = view.get_returns(
         "user",
         "get_all_market_account_ids_for_user",
         [],
         [serialize_address(user)],
     )
     ids = []
     for id in returns[0]:
         ids.append(int(id))
     return ids
 
 
 def get_custodian_id(view: EconiaViewer, market_account_id: int) -> int:
-    returns = view.get_returns(
-        "user", "get_custodian_id", [], [str(market_account_id)]
-    )
+    """
+    Return custodian ID encoded in market account ID.
+    """
+    returns = view.get_returns("user", "get_custodian_id", [], [str(market_account_id)])
     return int(returns[0])
 
 
 def get_market_account(
     view: EconiaViewer,
     user: AccountAddress,
     market_id: int,
     custodian_id: int,
 ) -> dict:
+    """
+    Return the open "bids" and "asks" amongst other information, for
+    the account associated with a user, market id, and custodian id.
+    """
     returns = view.get_returns(
         "user",
         "get_market_account",
         [],
         [serialize_address(user), str(market_id), str(custodian_id)],
     )
     return _convert_market_account_value(returns[0])
@@ -455,27 +549,33 @@
 
 
 def get_market_account_id(
     view: EconiaViewer,
     market_id: int,
     custodian_id: int,
 ) -> int:
+    """
+    Return market account ID with encoded market and custodian IDs.
+    """
     returns = view.get_returns(
         "user",
         "get_market_account_id",
         [],
         [
             str(market_id),
             str(custodian_id),
         ],
     )
     return int(returns[0])
 
 
 def get_market_accounts(view: EconiaViewer, user: AccountAddress) -> list[dict]:
+    """
+    Get user-friendly views of all of a `user`'s market accounts.
+    """
     returns = view.get_returns(
         "user",
         "get_market_accounts",
         [],
         [serialize_address(user)],
     )
     value = returns[0]
@@ -485,40 +585,51 @@
     return accounts
 
 
 def get_market_id(
     view: EconiaViewer,
     market_account_id: int,
 ) -> int:
+    """
+    Return market ID encoded in market account ID.
+    """
     returns = view.get_returns(
         "user",
         "get_market_id",
         [],
         [str(market_account_id)],
     )
     return int(returns[0])
 
 
 def has_market_account(
     view: EconiaViewer, user: AccountAddress, market_id: int, custodian_id: int
 ) -> bool:
+    """
+    Return `True` if `user` has market account registered with
+    given `market_id` and `custodian_id`.
+    """
     returns = view.get_returns(
         "user",
         "has_market_account",
         [],
         [serialize_address(user), str(market_id), str(custodian_id)],
     )
     return bool(returns[0])
 
 
 def has_market_account_by_market_account_id(
     view: EconiaViewer,
     user: AccountAddress,
     market_account_id: int,
 ) -> bool:
+    """
+    Return `True` if `user` has market account registered with
+    given `market_account_id`.
+    """
     returns = view.get_returns(
         "user",
         "has_market_account",
         [],
         [
             serialize_address(user),
             str(market_account_id),
@@ -528,14 +639,18 @@
 
 
 def has_market_account_by_market_id(
     view: EconiaViewer,
     user: AccountAddress,
     market_id: int,
 ) -> bool:
+    """
+    Return `True` if `user` has at least one market account
+    registered with given `market_id`.
+    """
     returns = view.get_returns(
         "user",
         "has_market_account_by_market_id",
         [],
         [
             serialize_address(user),
             str(market_id),
```

