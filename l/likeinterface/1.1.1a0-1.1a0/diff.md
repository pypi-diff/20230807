# Comparing `tmp/likeinterface-1.1.1a0.tar.gz` & `tmp/likeinterface-1.1a0.tar.gz`

## Comparing `likeinterface-1.1.1a0.tar` & `likeinterface-1.1a0.tar`

### file list

```diff
@@ -1,41 +1,36 @@
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/Makefile
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/.github/dependabot.yml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/.github/workflows/pre-commit-updater.yml
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/licenses/LICENSE.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/__meta__.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/constants.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/exceptions.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/interface.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/network.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/session.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/methods/__init__.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/methods/base.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/methods/auth/__init__.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/methods/auth/get_authorization_information.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/methods/auth/get_user_information.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/methods/auth/root_auth.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/methods/auth/sign_in.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/methods/balance/__init__.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/methods/balance/get_balance.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/methods/balance/root_balance.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/methods/like/__init__.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/methods/like/evaluator.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/methods/like/root_like.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/types/__init__.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/types/base.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/types/auth/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/types/auth/authorization.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/types/auth/user.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/types/balance/__init__.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/types/balance/balance.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/types/like/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/types/like/hand.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/utils/__init__.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/utils/pydantic.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/likeinterface/utils/response_validator.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/.gitignore
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/pyproject.toml
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 likeinterface-1.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 likeinterface-1.1a0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 likeinterface-1.1a0/Makefile
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 likeinterface-1.1a0/.github/dependabot.yml
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 likeinterface-1.1a0/.github/workflows/pre-commit-updater.yml
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 likeinterface-1.1a0/licenses/LICENSE.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/__meta__.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/constants.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/exceptions.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/interface.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/network.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/session.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/methods/__init__.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/methods/base.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/methods/auth/__init__.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/methods/auth/get_authorization_information.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/methods/auth/get_user_information.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/methods/auth/root_auth.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/methods/auth/sign_in.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/methods/like/__init__.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/methods/like/evaluator.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/methods/like/root_like.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/types/__init__.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/types/base.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/types/auth/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/types/auth/authorization.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/types/auth/user.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/types/like/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/types/like/hand.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/utils/__init__.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/utils/pydantic.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 likeinterface-1.1a0/likeinterface/utils/response_validator.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 likeinterface-1.1a0/.gitignore
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 likeinterface-1.1a0/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 likeinterface-1.1a0/pyproject.toml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 likeinterface-1.1a0/PKG-INFO
```

### Comparing `likeinterface-1.1.1a0/Makefile` & `likeinterface-1.1a0/Makefile`

 * *Files identical despite different names*

### Comparing `likeinterface-1.1.1a0/.github/workflows/pre-commit-updater.yml` & `likeinterface-1.1a0/.github/workflows/pre-commit-updater.yml`

 * *Files identical despite different names*

### Comparing `likeinterface-1.1.1a0/licenses/LICENSE.txt` & `likeinterface-1.1a0/licenses/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `likeinterface-1.1.1a0/likeinterface/interface.py` & `likeinterface-1.1a0/likeinterface/interface.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.1.1a0/likeinterface/session.py` & `likeinterface-1.1a0/likeinterface/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 from collections import defaultdict
 from typing import TYPE_CHECKING, Any, Dict, Optional, cast
 
-from aiohttp.client import ClientError, ClientSession
+from aiohttp.client import ClientSession, ClientError
 
 from likeinterface.constants import REQUEST_TIMEOUT
 from likeinterface.exceptions import LikeNetworkError
 from likeinterface.methods import LikeType, Method
 from likeinterface.utils.response_validator import response_validator
 
 if TYPE_CHECKING:
@@ -54,22 +54,23 @@
         self, interface: Interface, method: Method[LikeType], timeout: Optional[int] = None
     ) -> LikeType:
         await self.create()
 
         request = method.request(interface=interface)
 
         try:
-            async with self.session.post(
+            response = await self.session.post(  # type: ignore[union-attr]
                 url=interface.network.url(method=method.__name__),
                 json=request.data,
                 timeout=REQUEST_TIMEOUT if not timeout else timeout,
-            ) as response:
-                content = await response.text()
+            )
         except asyncio.TimeoutError:
             raise LikeNetworkError("Exception %s: %s." % (method, "request timeout error"))
         except ClientError as e:
             raise LikeNetworkError(
                 "Exception for method %s: %s." % (method.__name__, f"{type(e).__name__}: {e}")
             )
 
-        response = response_validator(method=method, status_code=response.status, content=content)
+        response = response_validator(
+            method=method, status_code=response.status, content=response.text
+        )
         return cast(LikeType, response.result)
```

### Comparing `likeinterface-1.1.1a0/likeinterface/methods/base.py` & `likeinterface-1.1a0/likeinterface/methods/base.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.1.1a0/likeinterface/methods/auth/get_authorization_information.py` & `likeinterface-1.1a0/likeinterface/methods/auth/get_authorization_information.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.1.1a0/likeinterface/methods/auth/get_user_information.py` & `likeinterface-1.1a0/likeinterface/methods/auth/get_user_information.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.1.1a0/likeinterface/methods/auth/root_auth.py` & `likeinterface-1.1a0/likeinterface/methods/auth/root_auth.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.1.1a0/likeinterface/methods/auth/sign_in.py` & `likeinterface-1.1a0/likeinterface/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.1.1a0/likeinterface/methods/balance/get_balance.py` & `likeinterface-1.1a0/likeinterface/methods/like/evaluator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, List
 
 from likeinterface.methods.base import Method, Request
-from likeinterface.types import Balance
+from likeinterface.types import Hand
 
 if TYPE_CHECKING:
     from likeinterface.interface import Interface
 
 
-class GetBalanceMethod(Method[Balance]):
+class EvaluatorMethod(Method[List[Hand]]):
     """
-    Use this method to get balance for user.
+    Use this method to evaluate hands.
 
     Parameters
-      Name            | Type    | Required | Description
+      Name     | Type            | Required | Description
 
-      1. user_id      | Integer | Yes      | User ID in the system. Send user_id=0 for get current user balance and provide access_token parameter.
-      2. access_token | String  | No       | Auth access token
+      1. board | Array of String | Yes      | Card table, for example, ["Ac", "As", "Ah", "Ad", "Td"]
+
+      2. hands | Array Of String | Yes      | Player hand, for example, ["2c2h", "2d2s"]
 
     Result
-      :class:`likeinterface.types.balance.balance.Balance`
+      Array of :class:`likeinterface.types.like.hand.Hand`
     """
 
-    __name__ = "balance.getBalance"
-    __returning__ = Balance
+    __name__ = "like.evaluator"
+    __returning__ = List[Hand]
 
-    user_id: int
-    access_token: Optional[str] = None
+    board: List[str]
+    hands: List[str]
 
     def request(self, interface: Interface) -> Request:
         return Request(method=self.__name__, data=self.model_dump())
```

### Comparing `likeinterface-1.1.1a0/likeinterface/methods/balance/root_balance.py` & `likeinterface-1.1a0/likeinterface/methods/like/root_like.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 from likeinterface.methods.base import Method, Request
 
 if TYPE_CHECKING:
     from likeinterface.interface import Interface
 
 
-class RootBalanceMethod(Method[bool]):
+class RootLikeMethod(Method[bool]):
     """
     Use this method to get service health.
 
     Parameters
       This constructor does not require any parameters.
 
     Result
       :class:`bool`
     """
 
-    __name__ = "balance"
+    __name__ = "like"
     __returning__ = bool
 
     def request(self, interface: Interface) -> Request:
         return Request(method=self.__name__, data=self.model_dump())
```

### Comparing `likeinterface-1.1.1a0/likeinterface/types/auth/user.py` & `likeinterface-1.1a0/likeinterface/types/auth/user.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.1.1a0/likeinterface/utils/pydantic.py` & `likeinterface-1.1a0/likeinterface/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.1.1a0/likeinterface/utils/response_validator.py` & `likeinterface-1.1a0/likeinterface/utils/response_validator.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.1.1a0/.gitignore` & `likeinterface-1.1a0/.gitignore`

 * *Files identical despite different names*

### Comparing `likeinterface-1.1.1a0/pyproject.toml` & `likeinterface-1.1a0/pyproject.toml`

 * *Files identical despite different names*

