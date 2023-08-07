# Comparing `tmp/bk-crypto-python-sdk-1.0.4.tar.gz` & `tmp/bk-crypto-python-sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bk-crypto-python-sdk-1.0.4.tar", max compression
+gzip compressed data, was "bk-crypto-python-sdk-1.1.0.tar", max compression
```

## Comparing `bk-crypto-python-sdk-1.0.4.tar` & `bk-crypto-python-sdk-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
--rw-r--r--   0        0        0     1068 2023-07-20 14:38:00.335918 bk-crypto-python-sdk-1.0.4/LICENSE.txt
--rw-r--r--   0        0        0      757 2023-07-20 14:38:00.335918 bk-crypto-python-sdk-1.0.4/bkcrypto/__init__.py
--rw-r--r--   0        0        0      757 2023-07-20 14:38:00.335918 bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/__init__.py
--rw-r--r--   0        0        0      953 2023-07-20 14:38:00.335918 bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/ciphers/__init__.py
--rw-r--r--   0        0        0     9481 2023-07-20 14:38:00.335918 bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/ciphers/base.py
--rw-r--r--   0        0        0     5426 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/ciphers/rsa.py
--rw-r--r--   0        0        0     4464 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/ciphers/sm2.py
--rw-r--r--   0        0        0     2543 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/configs.py
--rw-r--r--   0        0        0     1240 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/interceptors.py
--rw-r--r--   0        0        0     1114 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/options.py
--rw-r--r--   0        0        0     2324 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/constants.py
--rw-r--r--   0        0        0      757 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/contrib/__init__.py
--rw-r--r--   0        0        0      757 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/contrib/django/__init__.py
--rw-r--r--   0        0        0     4791 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/contrib/django/ciphers.py
--rw-r--r--   0        0        0     4856 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/contrib/django/fields.py
--rw-r--r--   0        0        0     2680 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/contrib/django/init_configs.py
--rw-r--r--   0        0        0     7422 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/contrib/django/settings.py
--rw-r--r--   0        0        0      757 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/contrib/drf/__init__.py
--rw-r--r--   0        0        0      757 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/__init__.py
--rw-r--r--   0        0        0      947 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/ciphers/__init__.py
--rw-r--r--   0        0        0     3817 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/ciphers/aes.py
--rw-r--r--   0        0        0    11066 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/ciphers/base.py
--rw-r--r--   0        0        0     4158 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/ciphers/sm4.py
--rw-r--r--   0        0        0     3041 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/configs.py
--rw-r--r--   0        0        0      881 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/interceptors.py
--rw-r--r--   0        0        0     1106 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/options.py
--rw-r--r--   0        0        0     1866 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/types.py
--rw-r--r--   0        0        0      757 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/utils/__init__.py
--rw-r--r--   0        0        0     1203 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/utils/base_interceptors.py
--rw-r--r--   0        0        0     2024 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/utils/convertors.py
--rw-r--r--   0        0        0     1539 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/bkcrypto/utils/module_loding.py
--rw-r--r--   0        0        0     1756 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     7505 2023-07-20 14:38:00.339918 bk-crypto-python-sdk-1.0.4/readme.md
--rw-r--r--   0        0        0     8741 1970-01-01 00:00:00.000000 bk-crypto-python-sdk-1.0.4/setup.py
--rw-r--r--   0        0        0     8286 1970-01-01 00:00:00.000000 bk-crypto-python-sdk-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-07 04:20:14.172812 bk-crypto-python-sdk-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      757 2023-08-07 04:20:14.172812 bk-crypto-python-sdk-1.1.0/bkcrypto/__init__.py
+-rw-r--r--   0        0        0      757 2023-08-07 04:20:14.172812 bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/__init__.py
+-rw-r--r--   0        0        0      953 2023-08-07 04:20:14.172812 bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/ciphers/__init__.py
+-rw-r--r--   0        0        0     9536 2023-08-07 04:20:14.172812 bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/ciphers/base.py
+-rw-r--r--   0        0        0     5491 2023-08-07 04:20:14.172812 bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/ciphers/rsa.py
+-rw-r--r--   0        0        0     4540 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/ciphers/sm2.py
+-rw-r--r--   0        0        0     2543 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/configs.py
+-rw-r--r--   0        0        0     1240 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/interceptors.py
+-rw-r--r--   0        0        0     1114 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/options.py
+-rw-r--r--   0        0        0     2324 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/constants.py
+-rw-r--r--   0        0        0      757 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/__init__.py
+-rw-r--r--   0        0        0      757 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/basic/__init__.py
+-rw-r--r--   0        0        0     3706 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/basic/ciphers.py
+-rw-r--r--   0        0        0      757 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/django/__init__.py
+-rw-r--r--   0        0        0     5405 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/django/ciphers.py
+-rw-r--r--   0        0        0     2953 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/django/fields.py
+-rw-r--r--   0        0        0     2680 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/django/init_configs.py
+-rw-r--r--   0        0        0     5011 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/django/selectors.py
+-rw-r--r--   0        0        0     7422 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/django/settings.py
+-rw-r--r--   0        0        0      757 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/drf/__init__.py
+-rw-r--r--   0        0        0      757 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/__init__.py
+-rw-r--r--   0        0        0      947 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/ciphers/__init__.py
+-rw-r--r--   0        0        0     3881 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/ciphers/aes.py
+-rw-r--r--   0        0        0    11095 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/ciphers/base.py
+-rw-r--r--   0        0        0     4222 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/ciphers/sm4.py
+-rw-r--r--   0        0        0     3041 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/configs.py
+-rw-r--r--   0        0        0      881 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/interceptors.py
+-rw-r--r--   0        0        0     1106 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/options.py
+-rw-r--r--   0        0        0     1866 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/types.py
+-rw-r--r--   0        0        0      757 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/utils/__init__.py
+-rw-r--r--   0        0        0     1203 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/utils/base_interceptors.py
+-rw-r--r--   0        0        0     2024 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/utils/convertors.py
+-rw-r--r--   0        0        0     1539 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/bkcrypto/utils/module_loding.py
+-rw-r--r--   0        0        0     1756 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12951 2023-08-07 04:20:14.176812 bk-crypto-python-sdk-1.1.0/readme.md
+-rw-r--r--   0        0        0    14367 1970-01-01 00:00:00.000000 bk-crypto-python-sdk-1.1.0/setup.py
+-rw-r--r--   0        0        0    13732 1970-01-01 00:00:00.000000 bk-crypto-python-sdk-1.1.0/PKG-INFO
```

### Comparing `bk-crypto-python-sdk-1.0.4/LICENSE.txt` & `bk-crypto-python-sdk-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/__init__.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/__init__.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/ciphers/__init__.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/ciphers/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/ciphers/base.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/ciphers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,16 @@
         return wrapped(*args, **kwargs)
 
     return handle
 
 
 class BaseAsymmetricCipher:
 
+    CIPHER_TYPE: str = None
+
     CONFIG_DATA_CLASS: typing.Type[BaseAsymmetricRuntimeConfig] = BaseAsymmetricRuntimeConfig
 
     OPTIONS_DATA_CLASS: typing.Type[AsymmetricOptions] = AsymmetricOptions
 
     config: BaseAsymmetricRuntimeConfig = None
 
     @staticmethod
@@ -198,24 +200,24 @@
         :param plaintext: 待加密的字符串
         :return: 密文
         """
         plaintext: str = self.config.interceptor.before_encrypt(plaintext)
         plaintext_bytes: bytes = self.config.convertor.encode_plaintext(plaintext, encoding=self.config.encoding)
         ciphertext_bytes: bytes = self._encrypt(plaintext_bytes)
         ciphertext: str = self.config.convertor.to_string(ciphertext_bytes)
-        return self.config.interceptor.after_encrypt(ciphertext)
+        return self.config.interceptor.after_encrypt(ciphertext, cipher=self)
 
     @key_obj_checker(constants.AsymmetricKeyAttribute.PRIVATE_KEY)
     def decrypt(self, ciphertext: str) -> str:
         """
         解密
         :param ciphertext: 密文
         :return: 解密后的信息
         """
-        ciphertext: str = self.config.interceptor.before_decrypt(ciphertext)
+        ciphertext: str = self.config.interceptor.before_decrypt(ciphertext, cipher=self)
         ciphertext_bytes: bytes = self.config.convertor.from_string(ciphertext)
         plaintext_bytes: bytes = self._decrypt(ciphertext_bytes)
         plaintext: str = self.config.convertor.decode_plaintext(plaintext_bytes, encoding=self.config.encoding)
         return self.config.interceptor.after_decrypt(plaintext)
 
     @key_obj_checker(constants.AsymmetricKeyAttribute.PRIVATE_KEY)
     def sign(self, plaintext: str) -> str:
```

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/ciphers/rsa.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/ciphers/rsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
         self.sig_scheme_maker = constants.RSASigScheme.get_sig_scheme_maker_by_member(self.sig_scheme)
 
         super().__post_init__()
 
 
 class RSAAsymmetricCipher(base.BaseAsymmetricCipher):
 
+    CIPHER_TYPE: str = constants.AsymmetricCipherType.RSA.value
+
     CONFIG_DATA_CLASS: typing.Type[RSAAsymmetricRuntimeConfig] = RSAAsymmetricRuntimeConfig
 
     OPTIONS_DATA_CLASS: typing.Type[RSAAsymmetricOptions] = RSAAsymmetricOptions
 
     config: RSAAsymmetricRuntimeConfig = None
 
     def export_public_key(self) -> str:
```

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/ciphers/sm2.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/ciphers/sm2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,31 @@
 import typing
 from dataclasses import dataclass
 
 from tongsuopy.crypto import exceptions, hashes, serialization
 from tongsuopy.crypto.asymciphers import ec
 from tongsuopy.crypto.asymciphers import types as tongsuopy_types
 
-from bkcrypto import types
+from bkcrypto import constants, types
 
 from .. import configs
 from ..options import SM2AsymmetricOptions
 from . import base
 
 
 @dataclass
 class SM2AsymmetricRuntimeConfig(configs.BaseSM2AsymmetricConfig, base.BaseAsymmetricRuntimeConfig):
     public_key: typing.Optional[tongsuopy_types.PUBLIC_KEY_TYPES] = None
     private_key: typing.Optional[tongsuopy_types.PRIVATE_KEY_TYPES] = None
 
 
 class SM2AsymmetricCipher(base.BaseAsymmetricCipher):
 
+    CIPHER_TYPE: str = constants.AsymmetricCipherType.SM2.value
+
     CONFIG_DATA_CLASS: typing.Type[SM2AsymmetricRuntimeConfig] = SM2AsymmetricRuntimeConfig
 
     OPTIONS_DATA_CLASS: typing.Type[SM2AsymmetricOptions] = SM2AsymmetricOptions
 
     config: SM2AsymmetricRuntimeConfig = None
 
     def export_public_key(self) -> str:
```

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/configs.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/configs.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/interceptors.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/interceptors.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/asymmetric/options.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/asymmetric/options.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/constants.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/constants.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/contrib/__init__.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/contrib/django/__init__.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/contrib/django/ciphers.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/basic/ciphers.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,107 +5,68 @@
 Copyright (C) 2017-2023 THL A29 Limited, a Tencent company. All rights reserved.
 Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License at https://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
+
+
 import typing
 from dataclasses import asdict
 
-from bkcrypto.asymmetric.ciphers import BaseAsymmetricCipher
+from bkcrypto import constants
+from bkcrypto.asymmetric.ciphers import BaseAsymmetricCipher, RSAAsymmetricCipher, SM2AsymmetricCipher
 from bkcrypto.asymmetric.options import AsymmetricOptions
-from bkcrypto.symmetric.ciphers import BaseSymmetricCipher
+from bkcrypto.symmetric.ciphers import AESSymmetricCipher, BaseSymmetricCipher, SM4SymmetricCipher
 from bkcrypto.symmetric.options import SymmetricOptions
 
-from .init_configs import AsymmetricCipherInitConfig, SymmetricCipherInitConfig
-from .settings import crypto_settings
+SYMMETRIC_CIPHER_CLASSES: typing.Dict[str, typing.Type[BaseSymmetricCipher]] = {
+    constants.SymmetricCipherType.AES.value: AESSymmetricCipher,
+    constants.SymmetricCipherType.SM4.value: SM4SymmetricCipher,
+}
+
+
+ASYMMETRIC_CIPHER_CLASSES: typing.Dict[str, typing.Type[BaseAsymmetricCipher]] = {
+    constants.AsymmetricCipherType.RSA.value: RSAAsymmetricCipher,
+    constants.AsymmetricCipherType.SM2.value: SM2AsymmetricCipher,
+}
 
 
 def get_asymmetric_cipher(
     cipher_type: typing.Optional[str] = None,
     common: typing.Optional[typing.Dict[str, typing.Any]] = None,
     cipher_options: typing.Optional[typing.Dict[str, typing.Optional[AsymmetricOptions]]] = None,
+    asymmetric__cipher_classes: typing.Optional[typing.Dict[str, BaseAsymmetricCipher]] = None,
 ) -> BaseAsymmetricCipher:
-
-    cipher_type: str = cipher_type or crypto_settings.ASYMMETRIC_CIPHER_TYPE
-    asymmetric_cipher_class: typing.Type[BaseAsymmetricCipher] = crypto_settings.ASYMMETRIC_CIPHER_CLASSES[cipher_type]
+    cipher_type: str = cipher_type or constants.AsymmetricCipherType.RSA.value
+    asymmetric__cipher_classes: typing.Optional[typing.Dict[str, typing.Type[BaseAsymmetricCipher]]] = (
+        asymmetric__cipher_classes or ASYMMETRIC_CIPHER_CLASSES
+    )
+    asymmetric_cipher_class: typing.Type[BaseAsymmetricCipher] = asymmetric__cipher_classes[cipher_type]
 
     common = common or {}
     cipher_options: typing.Dict[str, typing.Optional[AsymmetricOptions]] = cipher_options or {}
     options: AsymmetricOptions = cipher_options.get(cipher_type) or asymmetric_cipher_class.OPTIONS_DATA_CLASS()
 
     # 同参数优先级：common > options
     return asymmetric_cipher_class(**{**asdict(options), **common})
 
 
 def get_symmetric_cipher(
     cipher_type: typing.Optional[str] = None,
     common: typing.Optional[typing.Dict[str, typing.Any]] = None,
     cipher_options: typing.Optional[typing.Dict[str, typing.Optional[SymmetricOptions]]] = None,
+    symmetric_cipher_classes: typing.Optional[typing.Dict[str, BaseSymmetricCipher]] = None,
 ) -> BaseSymmetricCipher:
-
-    cipher_type: str = cipher_type or crypto_settings.SYMMETRIC_CIPHER_TYPE
-    symmetric_cipher_class: typing.Type[BaseSymmetricCipher] = crypto_settings.SYMMETRIC_CIPHER_CLASSES[cipher_type]
+    cipher_type: str = cipher_type or constants.SymmetricCipherType.AES.value
+    symmetric_cipher_classes: typing.Optional[typing.Dict[str, typing.Type[BaseSymmetricCipher]]] = (
+        symmetric_cipher_classes or SYMMETRIC_CIPHER_CLASSES
+    )
+    symmetric_cipher_class: typing.Type[BaseSymmetricCipher] = symmetric_cipher_classes[cipher_type]
 
     common = common or {}
     cipher_options: typing.Dict[str, typing.Optional[SymmetricOptions]] = cipher_options or {}
     options: SymmetricOptions = cipher_options.get(cipher_type) or symmetric_cipher_class.OPTIONS_DATA_CLASS()
 
     # 同参数优先级：common > options
     return symmetric_cipher_class(**{**asdict(options), **common})
-
-
-class SymmetricCipherManager:
-    _cache: typing.Optional[typing.Dict[str, BaseSymmetricCipher]] = None
-
-    def __init__(self):
-        self._cache: [str, BaseSymmetricCipher] = {}
-
-    def cipher(
-        self, using: typing.Optional[str] = None, cipher_type: typing.Optional[str] = None
-    ) -> BaseSymmetricCipher:
-
-        using: str = using or "default"
-        if using not in crypto_settings.SYMMETRIC_CIPHERS:
-            raise RuntimeError(f"Invalid using {using}")
-
-        cipher_type: str = cipher_type or crypto_settings.SYMMETRIC_CIPHER_TYPE
-        cache_key: str = f"{using}-{cipher_type}"
-        if cache_key in self._cache:
-            return self._cache[cache_key]
-
-        init_config: SymmetricCipherInitConfig = crypto_settings.SYMMETRIC_CIPHERS[using]
-        cipher: BaseSymmetricCipher = get_symmetric_cipher(**init_config.as_get_cipher_params(cipher_type))
-        self._cache[cache_key] = cipher
-        return cipher
-
-
-class AsymmetricCipherManager:
-    _cache: typing.Optional[typing.Dict[str, BaseAsymmetricCipher]] = None
-
-    def __init__(self):
-        self._cache: [str, BaseAsymmetricCipher] = {}
-
-    def cipher(
-        self, using: typing.Optional[str] = None, cipher_type: typing.Optional[str] = None
-    ) -> BaseAsymmetricCipher:
-
-        using: str = using or "default"
-        if using not in crypto_settings.ASYMMETRIC_CIPHERS:
-            raise RuntimeError(f"Invalid using {using}")
-
-        cipher_type: str = cipher_type or crypto_settings.ASYMMETRIC_CIPHER_TYPE
-        cache_key: str = f"{using}-{cipher_type}"
-        if cache_key in self._cache:
-            return self._cache[cache_key]
-
-        init_config: AsymmetricCipherInitConfig = crypto_settings.ASYMMETRIC_CIPHERS[using]
-        cipher: BaseAsymmetricCipher = get_asymmetric_cipher(**init_config.as_get_cipher_params(cipher_type))
-        self._cache[cache_key] = cipher
-        return cipher
-
-
-symmetric_cipher_manager = SymmetricCipherManager()
-
-
-asymmetric_cipher_manager = AsymmetricCipherManager()
```

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/contrib/django/init_configs.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/django/init_configs.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/contrib/django/settings.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/django/settings.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/contrib/drf/__init__.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/__init__.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/contrib/drf/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/ciphers/__init__.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/ciphers/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/ciphers/aes.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/ciphers/aes.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 
         except KeyError:
             raise ValueError(f"Unsupported mode: {self.mode}")
 
 
 class AESSymmetricCipher(base.BaseSymmetricCipher):
 
+    CIPHER_TYPE: str = constants.SymmetricCipherType.AES.value
+
     CONFIG_DATA_CLASS: typing.Type[AESSymmetricRuntimeConfig] = AESSymmetricRuntimeConfig
 
     OPTIONS_DATA_CLASS: typing.Type[options.AESSymmetricOptions] = options.AESSymmetricOptions
 
     config: AESSymmetricRuntimeConfig = None
 
     def get_block_size(self) -> int:
```

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/ciphers/base.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/ciphers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 
         if self.aad and self.enable_aad:
             self.aad_size = len(self.aad)
 
 
 class BaseSymmetricCipher:
 
+    CIPHER_TYPE: str = None
+
     CONFIG_DATA_CLASS: typing.Type[BaseSymmetricRuntimeConfig] = BaseSymmetricRuntimeConfig
 
     OPTIONS_DATA_CLASS: typing.Type[SymmetricOptions] = SymmetricOptions
 
     config: BaseSymmetricRuntimeConfig = None
 
     @abc.abstractmethod
```

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/ciphers/sm4.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/ciphers/sm4.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 
         except KeyError:
             raise ValueError(f"Unsupported mode: {self.mode}")
 
 
 class SM4SymmetricCipher(base.BaseSymmetricCipher):
 
+    CIPHER_TYPE: str = constants.SymmetricCipherType.SM4.value
+
     CONFIG_DATA_CLASS: typing.Type[SM4SymmetricRuntimeConfig] = SM4SymmetricRuntimeConfig
 
     OPTIONS_DATA_CLASS: typing.Type[SM4SymmetricOptions] = SM4SymmetricOptions
 
     config: SM4SymmetricRuntimeConfig = None
 
     def __init__(
```

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/configs.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/configs.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/interceptors.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/interceptors.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/symmetric/options.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/options.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/types.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/types.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/utils/__init__.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/symmetric/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/utils/base_interceptors.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/utils/base_interceptors.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/utils/convertors.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/utils/convertors.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/bkcrypto/utils/module_loding.py` & `bk-crypto-python-sdk-1.1.0/bkcrypto/utils/module_loding.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.4/pyproject.toml` & `bk-crypto-python-sdk-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bk-crypto-python-sdk"
-version = "1.0.4"
+version = "1.1.0"
 description = "bk-crypto-python-sdk is a lightweight cryptography toolkit for Python applications based on Cryptodome / tongsuopy and other encryption libraries."
 authors = ["TencentBlueKing <contactus_bk@tencent.com>"]
 readme = "readme.md"
 packages = [
     { include = "bkcrypto" },
 ]
```

### Comparing `bk-crypto-python-sdk-1.0.4/readme.md` & `bk-crypto-python-sdk-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: bk-crypto-python-sdk
+Version: 1.1.0
+Summary: bk-crypto-python-sdk is a lightweight cryptography toolkit for Python applications based on Cryptodome / tongsuopy and other encryption libraries.
+Author: TencentBlueKing
+Author-email: contactus_bk@tencent.com
+Requires-Python: >=3.6.2,<3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: dacite (>=1.8.1,<2.0.0)
+Requires-Dist: pycryptodomex (>=3.18.0,<4.0.0)
+Requires-Dist: tongsuopy-crayon (>=1.0.2b5,<2.0.0)
+Requires-Dist: wrapt (>=1.15.0,<2.0.0)
+Description-Content-Type: text/markdown
+
 # BlueKing crypto-python-sdk
 
 ---
 
 ![Python](https://badgen.net/badge/python/%3E=3.6.2,%3C3.11/green?icon=github)
 ![Django](https://badgen.net/badge/django/%3E=3.1.5,%3C=4.2.1/yellow?icon=github)
 [![License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](LICENSE.txt)
@@ -34,15 +52,101 @@
 $ pip install bk-crypto-python-sdk
 ```
 
 ### Usage
 
 > 更多用法参考：[使用文档](https://github.com/TencentBlueKing/crypto-python-sdk/blob/main/docs/usage.md)
 
-在项目中配置
+#### 1. 基础用法
+
+**非对称加密**
+
+```python
+import os
+
+from bkcrypto import constants
+from bkcrypto.symmetric.ciphers import BaseSymmetricCipher
+from bkcrypto.contrib.basic.ciphers import get_symmetric_cipher
+
+symmetric_cipher: BaseSymmetricCipher = get_symmetric_cipher(
+    cipher_type=constants.SymmetricCipherType.SM4.value,
+    common={"key": os.urandom(16)},
+)
+assert "123" == symmetric_cipher.decrypt(symmetric_cipher.encrypt("123"))
+```
+
+**对称加密**
+
+````python
+from bkcrypto import constants
+from bkcrypto.asymmetric import options
+from bkcrypto.asymmetric.ciphers import BaseAsymmetricCipher
+from bkcrypto.contrib.basic.ciphers import get_asymmetric_cipher
+
+asymmetric_cipher: BaseAsymmetricCipher = get_asymmetric_cipher(
+    cipher_type=constants.AsymmetricCipherType.SM2.value,
+    # 传入 None 将随机生成密钥，业务可以根据场景选择传入密钥或随机生成
+    cipher_options={
+        constants.AsymmetricCipherType.SM2.value: options.SM2AsymmetricOptions(
+            private_key_string=None
+        ),
+        constants.AsymmetricCipherType.RSA.value: options.SM2AsymmetricOptions(
+            private_key_string=None
+        ),
+    }
+)
+
+# 加解密
+assert "123" == asymmetric_cipher.decrypt(asymmetric_cipher.encrypt("123"))
+# 验签
+assert asymmetric_cipher.verify(plaintext="123", signature=asymmetric_cipher.sign("123"))
+````
+
+#### 2. 结合 Django 使用
+
+在 Django Settings 中配置加密算法类型
+
+```python
+from bkcrypto import constants
+
+BKCRYPTO = {
+    # 声明项目所使用的非对称加密算法
+    "ASYMMETRIC_CIPHER_TYPE": constants.AsymmetricCipherType.SM2.value,
+    # 声明项目所使用的对称加密算法
+    "SYMMETRIC_CIPHER_TYPE": constants.SymmetricCipherType.SM4.value,
+}
+```
+
+**非对称加密**
+
+```python
+from bkcrypto.asymmetric.ciphers import BaseAsymmetricCipher
+from bkcrypto.contrib.django.ciphers import get_asymmetric_cipher
+
+asymmetric_cipher: BaseAsymmetricCipher = get_asymmetric_cipher()
+
+# 加解密
+assert "123" == asymmetric_cipher.decrypt(asymmetric_cipher.encrypt("123"))
+# 验签
+assert asymmetric_cipher.verify(plaintext="123", signature=asymmetric_cipher.sign("123"))
+```
+
+**对称加密**
+
+```python
+from bkcrypto.symmetric.ciphers import BaseSymmetricCipher
+from bkcrypto.contrib.django.ciphers import get_symmetric_cipher
+
+symmetric_cipher: BaseSymmetricCipher = get_symmetric_cipher()
+assert "123" == symmetric_cipher.decrypt(symmetric_cipher.encrypt("123"))
+```
+
+#### 3. 使用 Django CipherManager
+
+在 Django Settings 中配置加密算法类型
 
 ```python
 from bkcrypto import constants
 from bkcrypto.symmetric.options import AESSymmetricOptions, SM4SymmetricOptions
 from bkcrypto.asymmetric.options import RSAAsymmetricOptions
 
 BKCRYPTO = {
@@ -81,76 +185,141 @@
                 constants.AsymmetricCipherType.SM2.value: SM4SymmetricOptions()
             },
         },
     }
 }
 ```
 
-#### 非对称加密
+**非对称加密**
 
-使用 `get_asymmetric_cipher` 获取 `cipher`
+使用 `asymmetric_cipher_manager` 获取 `BKCRYPTO.ASYMMETRIC_CIPHERS` 配置的 `cipher`
 
 ```python
 from bkcrypto.asymmetric.ciphers import BaseAsymmetricCipher
-from bkcrypto.contrib.django.ciphers import get_asymmetric_cipher
+from bkcrypto.contrib.django.ciphers import asymmetric_cipher_manager
 
-asymmetric_cipher: BaseAsymmetricCipher = get_asymmetric_cipher()
+asymmetric_cipher: BaseAsymmetricCipher = asymmetric_cipher_manager.cipher(using="default")
 
 # 加解密
 assert "123" == asymmetric_cipher.decrypt(asymmetric_cipher.encrypt("123"))
 # 验签
 assert asymmetric_cipher.verify(plaintext="123", signature=asymmetric_cipher.sign("123"))
 ```
 
-使用 `asymmetric_cipher_manager` 获取 `BKCRYPTO.ASYMMETRIC_CIPHERS` 配置的 `cipher`
+**对称加密**
+
+使用 `symmetric_cipher_manager` 获取 `BKCRYPTO.SYMMETRIC_CIPHERS` 配置的 `cipher`
 
 ```python
-from bkcrypto.asymmetric.ciphers import BaseAsymmetricCipher
-from bkcrypto.contrib.django.ciphers import asymmetric_cipher_manager
+from bkcrypto.symmetric.ciphers import BaseSymmetricCipher
+from bkcrypto.contrib.django.ciphers import symmetric_cipher_manager
 
-asymmetric_cipher: BaseAsymmetricCipher = asymmetric_cipher_manager.cipher(using="default")
+# using - 指定对称加密实例，默认使用 `default`
+symmetric_cipher: BaseSymmetricCipher = symmetric_cipher_manager.cipher(using="default")
+assert "123" == symmetric_cipher.decrypt(symmetric_cipher.encrypt("123"))
+```
 
-# 加解密
-assert "123" == asymmetric_cipher.decrypt(asymmetric_cipher.encrypt("123"))
-# 验签
-assert asymmetric_cipher.verify(plaintext="123", signature=asymmetric_cipher.sign("123"))
+**Django ModelField**
+
+```python
+from django.db import models
+from bkcrypto.contrib.django.fields import SymmetricTextField
+
+
+class IdentityData(models.Model):
+    password = SymmetricTextField("密码", blank=True, null=True)
 ```
 
-#### 对称加密
+#### 3. Using Django CipherManager
 
-使用 `get_symmetric_cipher` 获取 `cipher`
+Configure the encryption algorithm type in Django Settings
 
 ```python
-from bkcrypto.symmetric.ciphers import BaseSymmetricCipher
-from bkcrypto.contrib.django.ciphers import get_symmetric_cipher
+from bkcrypto import constants
+from bkcrypto.symmetric.options import AESSymmetricOptions, SM4SymmetricOptions
+from bkcrypto.asymmetric.options import RSAAsymmetricOptions
 
-symmetric_cipher: BaseSymmetricCipher = get_symmetric_cipher()
-assert "123" == symmetric_cipher.decrypt(symmetric_cipher.encrypt("123"))
+BKCRYPTO = {
+    # Declare the asymmetric encryption algorithm used by the project
+    "ASYMMETRIC_CIPHER_TYPE": constants.AsymmetricCipherType.SM2.value,
+    # Declare the symmetric encryption algorithm used by the project
+    "SYMMETRIC_CIPHER_TYPE": constants.SymmetricCipherType.SM4.value,
+    "SYMMETRIC_CIPHERS": {
+        # default - The configured symmetric encryption instance can be configured with multiple instances depending on the project requirements
+        "default": {
+            # Optional, used in cases where settings cannot directly obtain the key
+            # "get_key_config": "apps.utils.encrypt.key.get_key_config",
+            # Optional, used for ModelField, encrypted with this prefix to store the database, decrypting and analyzing the prefix and selecting the appropriate decryption algorithm
+            # ⚠️ The prefix and cipher type must be in one-to-one correspondence, and there can be no prefix matching relationship
+            # "db_prefix_map": {
+            #     SymmetricCipherType.AES.value: "aes_str:::",
+            #     SymmetricCipherType.SM4.value: "sm4_str:::"
+            # },
+            # Common parameter configuration, sharing these parameters when initializing different ciphers
+            "common": {"key": "your key"},
+            "cipher_options": {
+                constants.SymmetricCipherType.AES.value: AESSymmetricOptions(key_size=16),
+                # Blue Whale recommended configuration
+                constants.SymmetricCipherType.SM4.value: SM4SymmetricOptions(mode=constants.SymmetricMode.CTR)
+            }
+        },
+    },
+    "ASYMMETRIC_CIPHERS": {
+        # Configuration same as SYMMETRIC_CIPHERS
+        "default": {
+            "common": {"public_key_string": "your key"},
+            "cipher_options": {
+                constants.AsymmetricCipherType.RSA.value: RSAAsymmetricOptions(
+                    padding=constants.RSACipherPadding.PKCS1_OAEP
+                ),
+                constants.AsymmetricCipherType.SM2.value: SM4SymmetricOptions()
+            },
+        },
+    }
+}
 ```
 
-使用 `symmetric_cipher_manager` 获取 `BKCRYPTO.SYMMETRIC_CIPHERS` 配置的 `cipher`
+**Asymmetric Encryption**
+
+Use `asymmetric_cipher_manager` to get the `cipher` configured for `BKCRYPTO.ASYMMETRIC_CIPHERS`
+
+```python
+from bkcrypto.asymmetric.ciphers import BaseAsymmetricCipher
+from bkcrypto.contrib.django.ciphers import asymmetric_cipher_manager
+
+asymmetric_cipher: BaseAsymmetricCipher = asymmetric_cipher_manager.cipher(using="default")
+
+# Encrypt and Decrypt
+assert "123" == asymmetric_cipher.decrypt(asymmetric_cipher.encrypt("123"))
+# Signature verification
+assert asymmetric_cipher.verify(plaintext="123", signature=asymmetric_cipher.sign("123"))
+```
+
+**Symmetric Encryption**
+
+Use `symmetric_cipher_manager` to get the `cipher` configured for `BKCRYPTO.SYMMETRIC_CIPHERS`
 
 ```python
 from bkcrypto.symmetric.ciphers import BaseSymmetricCipher
 from bkcrypto.contrib.django.ciphers import symmetric_cipher_manager
 
-# using - 指定对称加密实例，默认使用 `default`
+# using - Specifies a symmetric encryption instance, defaults to 'default'
 symmetric_cipher: BaseSymmetricCipher = symmetric_cipher_manager.cipher(using="default")
 assert "123" == symmetric_cipher.decrypt(symmetric_cipher.encrypt("123"))
 ```
 
-#### SymmetricTextField
+**Django ModelField**
 
 ```python
 from django.db import models
 from bkcrypto.contrib.django.fields import SymmetricTextField
 
 
 class IdentityData(models.Model):
-    password = SymmetricTextField("密码", blank=True, null=True)
+    password = SymmetricTextField("Password", blank=True, null=True)
 ```
 
 ## Roadmap
 
 - [版本日志](https://github.com/TencentBlueKing/crypto-python-sdk/blob/main/release.md)
 
 ## Support
@@ -174,7 +343,8 @@
 
 如果你有好的意见或建议，欢迎给我们提 Issues 或 Pull Requests，为蓝鲸开源社区贡献力量。   
 [腾讯开源激励计划](https://opensource.tencent.com/contribution) 鼓励开发者的参与和贡献，期待你的加入。
 
 ## License
 
 基于 MIT 协议， 详细请参考 [LICENSE](https://github.com/TencentBlueKing/crypto-python-sdk/blob/main/LICENSE.txt)
+
```

