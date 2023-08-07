# Comparing `tmp/rivian_python_client-1.0.1.tar.gz` & `tmp/rivian_python_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rivian_python_client-1.0.1.tar", max compression
+gzip compressed data, was "rivian_python_client-1.0.2.tar", max compression
```

## Comparing `rivian_python_client-1.0.1.tar` & `rivian_python_client-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      325 2023-08-05 18:02:19.088641 rivian_python_client-1.0.1/README.md
--rw-r--r--   0        0        0      775 2023-08-05 18:02:40.152866 rivian_python_client-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      155 2023-08-05 18:02:19.096641 rivian_python_client-1.0.1/src/rivian/__init__.py
--rw-r--r--   0        0        0     5766 2023-08-05 18:02:19.096641 rivian_python_client-1.0.1/src/rivian/const.py
--rw-r--r--   0        0        0      969 2023-08-05 18:02:19.096641 rivian_python_client-1.0.1/src/rivian/exceptions.py
--rw-r--r--   0        0        0        0 2023-08-05 18:02:19.096641 rivian_python_client-1.0.1/src/rivian/py.typed
--rw-r--r--   0        0        0    26156 2023-08-05 18:02:19.096641 rivian_python_client-1.0.1/src/rivian/rivian.py
--rw-r--r--   0        0        0     3031 2023-08-05 18:02:19.096641 rivian_python_client-1.0.1/src/rivian/utils.py
--rw-r--r--   0        0        0     7509 2023-08-05 18:02:19.096641 rivian_python_client-1.0.1/src/rivian/ws_monitor.py
--rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 rivian_python_client-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      325 2023-08-07 03:11:05.575780 rivian_python_client-1.0.2/README.md
+-rw-r--r--   0        0        0      775 2023-08-07 03:11:22.371650 rivian_python_client-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-08-07 03:11:05.579780 rivian_python_client-1.0.2/src/rivian/__init__.py
+-rw-r--r--   0        0        0     5766 2023-08-07 03:11:05.579780 rivian_python_client-1.0.2/src/rivian/const.py
+-rw-r--r--   0        0        0      969 2023-08-07 03:11:05.579780 rivian_python_client-1.0.2/src/rivian/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-07 03:11:05.579780 rivian_python_client-1.0.2/src/rivian/py.typed
+-rw-r--r--   0        0        0    26218 2023-08-07 03:11:05.579780 rivian_python_client-1.0.2/src/rivian/rivian.py
+-rw-r--r--   0        0        0     3031 2023-08-07 03:11:05.579780 rivian_python_client-1.0.2/src/rivian/utils.py
+-rw-r--r--   0        0        0     7509 2023-08-07 03:11:05.579780 rivian_python_client-1.0.2/src/rivian/ws_monitor.py
+-rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 rivian_python_client-1.0.2/PKG-INFO
```

### Comparing `rivian_python_client-1.0.1/pyproject.toml` & `rivian_python_client-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rivian-python-client"
-version = "1.0.1"
+version = "1.0.2"
 description = "Rivian API Client (Unofficial)"
 readme = "README.md"
 authors = ["Brian Retterer <bretterer@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "rivian", from = "src" },
 ]
```

### Comparing `rivian_python_client-1.0.1/src/rivian/const.py` & `rivian_python_client-1.0.2/src/rivian/const.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.0.1/src/rivian/exceptions.py` & `rivian_python_client-1.0.2/src/rivian/exceptions.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.0.1/src/rivian/rivian.py` & `rivian_python_client-1.0.2/src/rivian/rivian.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
         url = GRAPHQL_GATEWAY
 
         headers = BASE_HEADERS | {
             "A-Sess": self._app_session_token,
             "U-Sess": self._user_session_token,
         }
 
-        vehicles_fragment = "vehicles { id vin name vas { __typename vasVehicleId vehiclePublicKey } roles state createdAt updatedAt vehicle { __typename id vin modelYear make model expectedBuildDate plannedBuildDate expectedGeneralAssemblyStartDate actualGeneralAssemblyDate } }"
+        vehicles_fragment = "vehicles { id vin name vas { __typename vasVehicleId vehiclePublicKey } roles state createdAt updatedAt vehicle { __typename id vin modelYear make model expectedBuildDate plannedBuildDate expectedGeneralAssemblyStartDate actualGeneralAssemblyDate vehicleState { supportedFeatures { __typename name status } } } }"
         phones_fragment = "enrolledPhones { __typename vas { __typename vasPhoneId publicKey } enrolled { __typename deviceType deviceName vehicleId identityId shortName } }"
 
         graphql_json = {
             "operationName": "getUserInfo",
             "query": f"query getUserInfo {{ currentUser {{ __typename id {vehicles_fragment} {phones_fragment if include_phones else ''} }} }}",
             "variables": None,
         }
```

### Comparing `rivian_python_client-1.0.1/src/rivian/utils.py` & `rivian_python_client-1.0.2/src/rivian/utils.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.0.1/src/rivian/ws_monitor.py` & `rivian_python_client-1.0.2/src/rivian/ws_monitor.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.0.1/PKG-INFO` & `rivian_python_client-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rivian-python-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: Rivian API Client (Unofficial)
 License: MIT
 Author: Brian Retterer
 Author-email: bretterer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

