# Comparing `tmp/mlaas_sdk-0.5.0.tar.gz` & `tmp/mlaas_sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlaas_sdk-0.5.0.tar", max compression
+gzip compressed data, was "mlaas_sdk-1.0.0.tar", max compression
```

## Comparing `mlaas_sdk-0.5.0.tar` & `mlaas_sdk-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0      303 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/README.md
--rwxr-xr-x   0        0        0        0 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/__init__.py
--rwxr-xr-x   0        0        0     1681 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/clients/__init__.py
--rwxr-xr-x   0        0        0     1894 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/clients/base.py
--rwxr-xr-x   0        0        0     3551 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/clients/blockchain.py
--rwxr-xr-x   0        0        0     4185 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/clients/sharing.py
--rwxr-xr-x   0        0        0     2058 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/clients/training.py
--rwxr-xr-x   0        0        0     1676 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/exceptions/MLaaSException.py
--rwxr-xr-x   0        0        0     1678 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/exceptions/__init__.py
--rwxr-xr-x   0        0        0     2812 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/exceptions/blockchain.py
--rwxr-xr-x   0        0        0     3046 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/exceptions/sharing.py
--rwxr-xr-x   0        0        0     2295 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/exceptions/training.py
--rwxr-xr-x   0        0        0     1776 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/models/DatasetContract.py
--rwxr-xr-x   0        0        0     1935 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/models/ModelContract.py
--rwxr-xr-x   0        0        0     1746 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/models/ModelContractUnverified.py
--rwxr-xr-x   0        0        0     1718 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/models/__init__.py
--rwxr-xr-x   0        0        0     1960 2023-07-25 12:37:44.120810 mlaas_sdk-0.5.0/mlaas_sdk/utils.py
--rwxr-xr-x   0        0        0      523 2023-08-01 09:56:56.917100 mlaas_sdk-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 mlaas_sdk-0.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0      303 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/README.md
+-rwxr-xr-x   0        0        0        0 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/mlaas_sdk/__init__.py
+-rwxr-xr-x   0        0        0     1681 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/mlaas_sdk/clients/__init__.py
+-rwxr-xr-x   0        0        0     1894 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/mlaas_sdk/clients/base.py
+-rwxr-xr-x   0        0        0     3733 2023-08-07 09:46:53.264172 mlaas_sdk-1.0.0/mlaas_sdk/clients/blockchain.py
+-rwxr-xr-x   0        0        0     4250 2023-08-07 09:44:10.798004 mlaas_sdk-1.0.0/mlaas_sdk/clients/sharing.py
+-rwxr-xr-x   0        0        0     2058 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/mlaas_sdk/clients/training.py
+-rwxr-xr-x   0        0        0     1676 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/mlaas_sdk/exceptions/MLaaSException.py
+-rwxr-xr-x   0        0        0     1678 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/mlaas_sdk/exceptions/__init__.py
+-rwxr-xr-x   0        0        0     2812 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/mlaas_sdk/exceptions/blockchain.py
+-rwxr-xr-x   0        0        0     3046 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/mlaas_sdk/exceptions/sharing.py
+-rwxr-xr-x   0        0        0     2295 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/mlaas_sdk/exceptions/training.py
+-rwxr-xr-x   0        0        0     1776 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/mlaas_sdk/models/DatasetContract.py
+-rwxr-xr-x   0        0        0     1935 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/mlaas_sdk/models/ModelContract.py
+-rwxr-xr-x   0        0        0     1746 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/mlaas_sdk/models/ModelContractUnverified.py
+-rwxr-xr-x   0        0        0     1718 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/mlaas_sdk/models/__init__.py
+-rwxr-xr-x   0        0        0     1960 2023-07-25 12:37:44.120810 mlaas_sdk-1.0.0/mlaas_sdk/utils.py
+-rwxr-xr-x   0        0        0      523 2023-08-07 12:44:13.336025 mlaas_sdk-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 mlaas_sdk-1.0.0/PKG-INFO
```

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/clients/__init__.py` & `mlaas_sdk-1.0.0/mlaas_sdk/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/clients/base.py` & `mlaas_sdk-1.0.0/mlaas_sdk/clients/base.py`

 * *Files identical despite different names*

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/clients/blockchain.py` & `mlaas_sdk-1.0.0/mlaas_sdk/clients/blockchain.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,64 +21,64 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-from typing import Union
+from typing import Literal, Union
 
 from .base import BaseClient
 from ..exceptions.blockchain import *
 from ..models import DatasetContract, ModelContract, ModelContractUnverified
 
 import requests
 
 
 class BlockchainClient(BaseClient):
     def __init__(self, blockchain_endpoint: str, secure: bool = False):
         super().__init__(blockchain_endpoint, secure)
 
     def read_contract(
-        self, contract_address: str
+        self,
+        contract_type: Literal["model", "model_unverified", "dataset"],
+        contract_address: str,
     ) -> Union[DatasetContract, ModelContract, ModelContractUnverified]:
         try:
             res = requests.get(
-                self.build_url("contract", contract_address)
+                self.build_url("contract", contract_type, contract_address)
             ).content
-            try:
-                return DatasetContract.parse_raw(res)
-            except ValueError:
-                pass
-            try:
-                return ModelContract.parse_raw(res)
-            except ValueError:
-                pass
-            try:
-                return ModelContractUnverified.parse_raw(res)
-            except ValueError:
-                raise ContractNotFoundException(contract_address)
+            match contract_type:
+                case "model":
+                    return ModelContract.parse_raw(res)
+                case "model_unverified":
+                    return ModelContractUnverified.parse_raw(res)
+                case "dataset":
+                    return DatasetContract.parse_raw(res)
+                case _:
+                    raise ContractNotFoundException(contract_address)
         except requests.exceptions.RequestException as e:
             raise ContractNotFoundException(contract_address)
 
     def verify_contract(self, contract_address: str, res_hash: str) -> None:
         try:
             requests.post(
                 self.build_url("contract", contract_address, "verify"),
                 params={"res_hash": res_hash},
             )
         except requests.exceptions.RequestException as e:
             raise ContractVerificationException(contract_address)
 
     def deploy_contract(
         self,
+        contract_type: Literal["model", "model_unverified", "dataset"],
         payload: Union[
             DatasetContract, ModelContract, ModelContractUnverified
         ],
     ) -> str:
         try:
             return requests.post(
-                self.build_url("contract"),
+                self.build_url("contract", contract_type),
                 json=payload.dict(exclude_none=True),
             ).json()["contract_address"]
         except requests.exceptions.RequestException as e:
             raise ContractDeploymentException(payload)
```

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/clients/sharing.py` & `mlaas_sdk-1.0.0/mlaas_sdk/clients/sharing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Copyright 2023, Atos Spain S.A.
 # All rights reserved.
-# 
+#
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
-# 
+#
 #     * Redistributions of source code must retain the above copyright notice,
 #       this list of conditions and the following disclaimer.
 #     * Redistributions in binary form must reproduce the above copyright
 #       notice, this list of conditions and the following disclaimer in the
 #       documentation and/or other materials provided with the distribution.
 #     * Neither the name of the copyright holder nor the names of its
 #       contributors may be used to endorse or promote products derived from
 #       this software without specific prior written permission.
-# 
+#
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 # AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 # IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
 # ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE
 # LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
@@ -40,22 +40,26 @@
         try:
             return requests.get(self.build_url("model", model_id), stream=True)
         except requests.exceptions.RequestException as e:
             raise ModelNotFoundException(model_id)
 
     def get_dataset(self, dataset_id: str) -> requests.Response:
         try:
-            return requests.get(self.build_url("dataset", dataset_id), stream=True)
+            return requests.get(
+                self.build_url("dataset", dataset_id), stream=True
+            )
         except requests.exceptions.RequestException as e:
             raise DatasetNotFoundException(dataset_id)
 
     def get_model_metadata(self, model_id: str) -> ModelContract:
         try:
             return ModelContract.parse_raw(
-                requests.get(self.build_url("model", model_id, "metadata")).content
+                requests.get(
+                    self.build_url("model", model_id, "metadata")
+                ).content
             )
         except requests.exceptions.RequestException as e:
             raise ModelException(model_id)
 
     def add_model(self, model: ModelContract) -> str:
         try:
             return requests.post(
```

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/clients/training.py` & `mlaas_sdk-1.0.0/mlaas_sdk/clients/training.py`

 * *Files identical despite different names*

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/exceptions/MLaaSException.py` & `mlaas_sdk-1.0.0/mlaas_sdk/exceptions/MLaaSException.py`

 * *Files identical despite different names*

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/exceptions/__init__.py` & `mlaas_sdk-1.0.0/mlaas_sdk/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/exceptions/blockchain.py` & `mlaas_sdk-1.0.0/mlaas_sdk/exceptions/blockchain.py`

 * *Files identical despite different names*

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/exceptions/sharing.py` & `mlaas_sdk-1.0.0/mlaas_sdk/exceptions/sharing.py`

 * *Files identical despite different names*

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/exceptions/training.py` & `mlaas_sdk-1.0.0/mlaas_sdk/exceptions/training.py`

 * *Files identical despite different names*

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/models/DatasetContract.py` & `mlaas_sdk-1.0.0/mlaas_sdk/models/DatasetContract.py`

 * *Files identical despite different names*

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/models/ModelContract.py` & `mlaas_sdk-1.0.0/mlaas_sdk/models/ModelContract.py`

 * *Files identical despite different names*

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/models/ModelContractUnverified.py` & `mlaas_sdk-1.0.0/mlaas_sdk/models/ModelContractUnverified.py`

 * *Files identical despite different names*

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/models/__init__.py` & `mlaas_sdk-1.0.0/mlaas_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mlaas_sdk-0.5.0/mlaas_sdk/utils.py` & `mlaas_sdk-1.0.0/mlaas_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `mlaas_sdk-0.5.0/pyproject.toml` & `mlaas_sdk-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 include = '\.pyi?$'
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "mlaas-sdk"
-version = "0.5.0"
+version = "1.0.0"
 description = "IoT-NGIN MLaaS Polyglot Model Sharing Framework Python SDK"
 authors = ["ivanvmoreno <ivan@ivan.build>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["iot-ngin"]
 packages = [{include = "mlaas_sdk"}]
```

### Comparing `mlaas_sdk-0.5.0/PKG-INFO` & `mlaas_sdk-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlaas-sdk
-Version: 0.5.0
+Version: 1.0.0
 Summary: IoT-NGIN MLaaS Polyglot Model Sharing Framework Python SDK
 License: MIT
 Keywords: iot-ngin
 Author: ivanvmoreno
 Author-email: ivan@ivan.build
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

