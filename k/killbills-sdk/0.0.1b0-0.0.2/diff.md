# Comparing `tmp/killbills_sdk-0.0.1b0.tar.gz` & `tmp/killbills_sdk-0.0.2.tar.gz`

## Comparing `killbills_sdk-0.0.1b0.tar` & `killbills_sdk-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/cryptoService.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/getStores.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/sendDataWithHmac.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/sendReceipt.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/sendTransaction.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/validatorService.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_crypto_service.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_get_stores.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_send_receipt.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_send_transaction.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_validator_service.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/LICENSE
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/README.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/pyproject.toml
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 killbills_sdk-0.0.1b0/PKG-INFO
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/Makefile
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/src/killbills_sdk/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/src/killbills_sdk/cryptoService.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/src/killbills_sdk/getStores.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/src/killbills_sdk/sendDataWithHmac.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/src/killbills_sdk/sendReceipt.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/src/killbills_sdk/sendTransaction.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/src/killbills_sdk/validatorService.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/src/killbills_sdk/tests/test_crypto_service.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/src/killbills_sdk/tests/test_get_stores.py
+-rw-r--r--   0        0        0     9179 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/src/killbills_sdk/tests/test_send_receipt.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/src/killbills_sdk/tests/test_send_transaction.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/src/killbills_sdk/tests/test_validator_service.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/LICENSE
+-rw-r--r--   0        0        0     6843 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/README.md
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 killbills_sdk-0.0.2/PKG-INFO
```

### Comparing `killbills_sdk-0.0.1b0/src/killbills_sdk/getStores.py` & `killbills_sdk-0.0.2/src/killbills_sdk/getStores.py`

 * *Files identical despite different names*

### Comparing `killbills_sdk-0.0.1b0/src/killbills_sdk/sendDataWithHmac.py` & `killbills_sdk-0.0.2/src/killbills_sdk/sendDataWithHmac.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 
     hashed_payload = cipher_hmac_payload(data, hmac_signature)
     headers = {
         'Authorization': f'hmac {hashed_payload}',
         'Content-Type': 'application/json'
     }
 
-    url = f'https://in.{env + "." if env != "prod" else "."}killbills.{"dev" if env != "prod" else "co"}/{endpoint}'
+    url = f'https://in.{env + "." if env != "prod" else ""}killbills.{"dev" if env != "prod" else "co"}/{endpoint}'
     response = requests.post(url, data=json.dumps(data), headers=headers)
     response.raise_for_status()  # Raise an exception for HTTP errors (4xx, 5xx)
 
     return response.json()
```

### Comparing `killbills_sdk-0.0.1b0/src/killbills_sdk/validatorService.py` & `killbills_sdk-0.0.2/src/killbills_sdk/validatorService.py`

 * *Files identical despite different names*

### Comparing `killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_crypto_service.py` & `killbills_sdk-0.0.2/src/killbills_sdk/tests/test_crypto_service.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import hashlib
 import unittest
-from cryptoService import cipher_hmac_payload
+from killbills_sdk.cryptoService import cipher_hmac_payload
 
 class TestCryptoService(unittest.TestCase):
 
     def test_sanity_check(self):
         self.assertTrue(True)
 
     def test_cipher_hmac_payload(self):
```

### Comparing `killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_get_stores.py` & `killbills_sdk-0.0.2/src/killbills_sdk/tests/test_get_stores.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 import os,time
 from dotenv import load_dotenv
+
 load_dotenv()
 
 from getStores import get_stores
 
 def test_get_stores_returns_list_of_dicts():
     env = 'dev'
     api_key = os.environ.get("TEST_API_KEY")
```

### Comparing `killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_send_receipt.py` & `killbills_sdk-0.0.2/src/killbills_sdk/tests/test_send_receipt.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     ],
     "partner_name": os.environ['TEST_POS_PARTNER_NAME'],
     "reference_id": "1221554511",
   }
 
 
 validPayload2 = {
-    "date": "2023-07-16T09:04:08",
+    "date": "2023-07-30T09:04:08",
     "mode": 0,
     "items": [
       {
         "tax": {
           "rate": 1000,
           "amount": 85,
           "description": "TVA",
@@ -216,15 +216,15 @@
         "bin": "0",
         "amount": 871741,
         "scheme": "",
         "auth_code": "",
         "last_four": "0",
         "payment_type": "CB",
         "transaction_id": "null",
-        "transaction_date": "2023-07-16T09:04:08",
+        "transaction_date": "2023-07-30T09:04:08",
       },
     ],
     "partner_name": os.environ['TEST_POS_PARTNER_NAME'] ,
     "reference_id": "1221554511",
   }
 
 def test_send_receipt_empty_payload():
@@ -241,54 +241,54 @@
 def test_send_receipt_Invalid_payload():
     with pytest.raises(ValueError) as exc_info:
         send_receipt("dev", {'tt':'toto'}, "hmac")
     expected_error_message = (
         "14 validation errors for ReceiptPayload\n"
         "reference_id\n"
         "  Field required [type=missing, input_value={'tt': 'toto'}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing\n"
         "amount\n"
         "  Field required [type=missing, input_value={'tt': 'toto'}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing\n"
         "currency\n"
         "  Field required [type=missing, input_value={'tt': 'toto'}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing\n"
         "date\n"
         "  Field required [type=missing, input_value={'tt': 'toto'}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing\n"
         "covers\n"
         "  Field required [type=missing, input_value={'tt': 'toto'}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing\n"
         "table\n"
         "  Field required [type=missing, input_value={'tt': 'toto'}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing\n"
         "invoice\n"
         "  Field required [type=missing, input_value={'tt': 'toto'}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing\n"
         "mode\n"
         "  Field required [type=missing, input_value={'tt': 'toto'}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing\n"
         "partner_name\n"
         "  Field required [type=missing, input_value={'tt': 'toto'}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing\n"
         "merchant\n"
         "  Field required [type=missing, input_value={'tt': 'toto'}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing\n"
         "store\n"
         "  Field required [type=missing, input_value={'tt': 'toto'}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing\n"
         "taxes\n"
         "  Field required [type=missing, input_value={'tt': 'toto'}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing\n"
         "items\n"
         "  Field required [type=missing, input_value={'tt': 'toto'}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing\n"
         "payments\n"
         "  Field required [type=missing, input_value={'tt': 'toto'}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing"
         
     )
     assert str(exc_info.value) == expected_error_message
     
 def test_send_receipt_valid_payload():
     result = send_receipt("dev", validPayload2, os.environ.get("TEST_POS_HMAC"))
     assert result['status'] == 'success'
```

### Comparing `killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_send_transaction.py` & `killbills_sdk-0.0.2/src/killbills_sdk/tests/test_send_transaction.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,26 +54,26 @@
 
     with pytest.raises(ValueError) as exc_info:
         send_transaction('dev', invalid_payload, os.environ.get("TEST_HMAC"))
     expected_error_message = (
         "5 validation errors for TransactionPayload\n"
         "bank_id\n"
         "  String should have at least 36 characters [type=string_too_short, input_value='1234', input_type=str]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/string_too_short\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/string_too_short\n"
         "partner_name\n"
         "  Field required [type=missing, input_value={'bank_id': '1234', 'call...illing_descriptor': ''}}, input_type=dict]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/missing\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/missing\n"
         "receipt_format\n"
         "  Input should be 'json','pdf','svg' or 'png' [type=enum, input_value='INVALID_FORMAT', input_type=str]\n"
         "transaction.amount\n"
         "  Input should be a valid integer, got a number with a fractional part [type=int_from_float, input_value=-10.5, input_type=float]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/int_from_float\n"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/int_from_float\n"
         "transaction.transaction_date\n"
         "  Input should be a valid integer, unable to parse string as an integer [type=int_parsing, input_value='INVALID_DATE', input_type=str]\n"
-        "    For further information visit https://errors.pydantic.dev/2.0.3/v/int_parsing"
+        "    For further information visit https://errors.pydantic.dev/2.1/v/int_parsing"
     )
 
     assert str(exc_info.value) == expected_error_message
```

### Comparing `killbills_sdk-0.0.1b0/src/killbills_sdk/tests/test_validator_service.py` & `killbills_sdk-0.0.2/src/killbills_sdk/tests/test_validator_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 import os,time
-from validatorService import validate_receipt_payload, validate_transaction_payload
+from killbills_sdk.validatorService import validate_receipt_payload, validate_transaction_payload
 from dotenv import load_dotenv
 load_dotenv()
 
 
 invalidPayload = {
     "bank_id": '1234',
     "callback_url": 'data:text/plain',
```

### Comparing `killbills_sdk-0.0.1b0/.gitignore` & `killbills_sdk-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `killbills_sdk-0.0.1b0/LICENSE` & `killbills_sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `killbills_sdk-0.0.1b0/pyproject.toml` & `killbills_sdk-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "killbills_sdk"
-version = "0.0.1-beta.0"
+version = "0.0.2"
 authors = [
     { name = "killbillsdev", email = "cto@killbills.co" }
 ]
 description = "KillBills e-receipt sdk"
 logo_url = "https://a.storyblok.com/f/149852/x/797a4a2b7e/dark_logo.svg"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "requests>=2.26.0",
     "pydantic>=2.0.3",
-    "pytest>=7.4.0"
+    "pytest>=7.4.0",
+    "python-dotenv>=1.0.0"
 ]
 
 [project.urls]
 Homepage = "https://github.com/killbillsdev/killbills-sdk-python"
 "Bug Tracker" = "https://github.com/killbillsdev/killbills-sdk-python/issues"
 
 [dependencies]
 python = ">=3.7"
 requests = ">=2.26.0"
+python-dotenv = ">=1.0.0"
 pydantic = ">=2.0.3"
 hmac = "20101005"
```

