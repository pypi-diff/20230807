# Comparing `tmp/symbol-sdk-python-3.0.7.tar.gz` & `tmp/symbol_sdk_python-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbol-sdk-python-3.0.7.tar", max compression
+gzip compressed data, was "symbol_sdk_python-3.1.0.tar", max compression
```

## Comparing `symbol-sdk-python-3.0.7.tar` & `symbol_sdk_python-3.1.0.tar`

### file list

```diff
@@ -1,55 +1,54 @@
--rw-r--r--   0        0        0     4585 2023-04-27 18:15:06.272392 symbol-sdk-python-3.0.7/README.md
--rw-r--r--   0        0        0      674 2023-04-27 18:44:29.145353 symbol-sdk-python-3.0.7/pyproject.toml
--rw-r--r--   0        0        0     2508 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/AccountDescriptorRepository.py
--rw-r--r--   0        0        0     3728 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/ArrayHelpers.py
--rw-r--r--   0        0        0     1482 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/BaseValue.py
--rw-r--r--   0        0        0     1787 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/Bip32.py
--rw-r--r--   0        0        0      723 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/BlockchainSettings.py
--rw-r--r--   0        0        0      883 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/BufferReader.py
--rw-r--r--   0        0        0      639 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/BufferWriter.py
--rw-r--r--   0        0        0     1059 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/ByteArray.py
--rw-r--r--   0        0        0     2158 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/Cipher.py
--rw-r--r--   0        0        0     1233 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/CodeWordsEncoder.py
--rw-r--r--   0        0        0     1844 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/CryptoTypes.py
--rw-r--r--   0        0        0     1848 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/DiceMnemonicGenerator.py
--rw-r--r--   0        0        0     3368 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/Network.py
--rw-r--r--   0        0        0     1594 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/NetworkTimestamp.py
--rw-r--r--   0        0        0     1019 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/NodeDescriptorRepository.py
--rw-r--r--   0        0        0      397 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/Ordered.py
--rw-r--r--   0        0        0     1606 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/PrivateKeyStorage.py
--rw-r--r--   0        0        0     1348 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/QrSignatureStorage.py
--rw-r--r--   0        0        0     1494 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/QrStorage.py
--rw-r--r--   0        0        0     4992 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/RuleBasedTransactionFactory.py
--rw-r--r--   0        0        0      593 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/SharedKey.py
--rw-r--r--   0        0        0     1809 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/TransactionDescriptorProcessor.py
--rw-r--r--   0        0        0      226 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/Transforms.py
--rw-r--r--   0        0        0        0 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/external/__init__.py
--rw-r--r--   0        0        0     7833 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/external/ed25519.py
--rw-r--r--   0        0        0     2983 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/facade/BatchOperations.py
--rw-r--r--   0        0        0     2801 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/facade/NemFacade.py
--rw-r--r--   0        0        0     4940 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/facade/SymbolFacade.py
--rw-r--r--   0        0        0        0 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/facade/__init__.py
--rw-r--r--   0        0        0     2152 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/impl/CipherHelpers.py
--rw-r--r--   0        0        0        0 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/impl/__init__.py
--rw-r--r--   0        0        0   178806 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/nc/__init__.py
--rw-r--r--   0        0        0     3712 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/nem/KeyPair.py
--rw-r--r--   0        0        0     2374 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/nem/MessageEncoder.py
--rw-r--r--   0        0        0     1746 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/nem/Network.py
--rw-r--r--   0        0        0     1094 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/nem/SharedKey.py
--rw-r--r--   0        0        0     3748 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/nem/TransactionFactory.py
--rw-r--r--   0        0        0        0 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/nem/__init__.py
--rw-r--r--   0        0        0      378 2023-04-27 18:15:06.276392 symbol-sdk-python-3.0.7/symbolchain/ripemd160.py
--rw-r--r--   0        0        0   477679 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/sc/__init__.py
--rw-r--r--   0        0        0     1696 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/IdGenerator.py
--rw-r--r--   0        0        0     1506 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/KeyPair.py
--rw-r--r--   0        0        0     7243 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/Merkle.py
--rw-r--r--   0        0        0     2476 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/MessageEncoder.py
--rw-r--r--   0        0        0      567 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/Metadata.py
--rw-r--r--   0        0        0     2229 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/Network.py
--rw-r--r--   0        0        0      334 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/SharedKey.py
--rw-r--r--   0        0        0     3355 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/TransactionFactory.py
--rw-r--r--   0        0        0     1686 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/VotingKeysGenerator.py
--rw-r--r--   0        0        0        0 2023-04-27 18:15:06.280392 symbol-sdk-python-3.0.7/symbolchain/symbol/__init__.py
--rw-r--r--   0        0        0     5609 2023-04-27 18:44:42.719073 symbol-sdk-python-3.0.7/setup.py
--rw-r--r--   0        0        0     5567 2023-04-27 18:44:42.719560 symbol-sdk-python-3.0.7/PKG-INFO
+-rw-r--r--   0        0        0     4585 2023-08-07 15:06:24.834947 symbol_sdk_python-3.1.0/README.md
+-rw-r--r--   0        0        0      842 2023-08-07 15:37:11.426322 symbol_sdk_python-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2508 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/AccountDescriptorRepository.py
+-rw-r--r--   0        0        0     3728 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/ArrayHelpers.py
+-rw-r--r--   0        0        0     1482 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/BaseValue.py
+-rw-r--r--   0        0        0     1787 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/Bip32.py
+-rw-r--r--   0        0        0      723 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/BlockchainSettings.py
+-rw-r--r--   0        0        0      883 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/BufferReader.py
+-rw-r--r--   0        0        0      639 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/BufferWriter.py
+-rw-r--r--   0        0        0     1059 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/ByteArray.py
+-rw-r--r--   0        0        0     2158 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/Cipher.py
+-rw-r--r--   0        0        0     1233 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/CodeWordsEncoder.py
+-rw-r--r--   0        0        0     1844 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/CryptoTypes.py
+-rw-r--r--   0        0        0     1848 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/DiceMnemonicGenerator.py
+-rw-r--r--   0        0        0     3368 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/Network.py
+-rw-r--r--   0        0        0     1594 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/NetworkTimestamp.py
+-rw-r--r--   0        0        0     1019 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/NodeDescriptorRepository.py
+-rw-r--r--   0        0        0      397 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/Ordered.py
+-rw-r--r--   0        0        0     1606 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/PrivateKeyStorage.py
+-rw-r--r--   0        0        0     1348 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/QrSignatureStorage.py
+-rw-r--r--   0        0        0     1494 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/QrStorage.py
+-rw-r--r--   0        0        0     4992 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/RuleBasedTransactionFactory.py
+-rw-r--r--   0        0        0      593 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/SharedKey.py
+-rw-r--r--   0        0        0     1806 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/TransactionDescriptorProcessor.py
+-rw-r--r--   0        0        0      226 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/Transforms.py
+-rw-r--r--   0        0        0        0 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/external/__init__.py
+-rw-r--r--   0        0        0     7833 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/external/ed25519.py
+-rw-r--r--   0        0        0     2983 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/facade/BatchOperations.py
+-rw-r--r--   0        0        0     2801 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/facade/NemFacade.py
+-rw-r--r--   0        0        0     4940 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/facade/SymbolFacade.py
+-rw-r--r--   0        0        0        0 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/facade/__init__.py
+-rw-r--r--   0        0        0     2152 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/impl/CipherHelpers.py
+-rw-r--r--   0        0        0        0 2023-08-07 15:06:24.838947 symbol_sdk_python-3.1.0/symbolchain/impl/__init__.py
+-rw-r--r--   0        0        0   178770 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/nc/__init__.py
+-rw-r--r--   0        0        0     3712 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/nem/KeyPair.py
+-rw-r--r--   0        0        0     2583 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/nem/MessageEncoder.py
+-rw-r--r--   0        0        0     1746 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/nem/Network.py
+-rw-r--r--   0        0        0     1094 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/nem/SharedKey.py
+-rw-r--r--   0        0        0     4017 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/nem/TransactionFactory.py
+-rw-r--r--   0        0        0        0 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/nem/__init__.py
+-rw-r--r--   0        0        0      378 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/ripemd160.py
+-rw-r--r--   0        0        0   477679 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/sc/__init__.py
+-rw-r--r--   0        0        0     1696 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/symbol/IdGenerator.py
+-rw-r--r--   0        0        0     1506 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/symbol/KeyPair.py
+-rw-r--r--   0        0        0     7243 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/symbol/Merkle.py
+-rw-r--r--   0        0        0     3766 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/symbol/MessageEncoder.py
+-rw-r--r--   0        0        0      567 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/symbol/Metadata.py
+-rw-r--r--   0        0        0     2229 2023-08-07 15:06:24.842947 symbol_sdk_python-3.1.0/symbolchain/symbol/Network.py
+-rw-r--r--   0        0        0      334 2023-08-07 15:06:24.846947 symbol_sdk_python-3.1.0/symbolchain/symbol/SharedKey.py
+-rw-r--r--   0        0        0     3624 2023-08-07 15:06:24.846947 symbol_sdk_python-3.1.0/symbolchain/symbol/TransactionFactory.py
+-rw-r--r--   0        0        0     1686 2023-08-07 15:06:24.846947 symbol_sdk_python-3.1.0/symbolchain/symbol/VotingKeysGenerator.py
+-rw-r--r--   0        0        0        0 2023-08-07 15:06:24.846947 symbol_sdk_python-3.1.0/symbolchain/symbol/__init__.py
+-rw-r--r--   0        0        0     5584 1970-01-01 00:00:00.000000 symbol_sdk_python-3.1.0/PKG-INFO
```

### Comparing `symbol-sdk-python-3.0.7/README.md` & `symbol_sdk_python-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/AccountDescriptorRepository.py` & `symbol_sdk_python-3.1.0/symbolchain/AccountDescriptorRepository.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/ArrayHelpers.py` & `symbol_sdk_python-3.1.0/symbolchain/ArrayHelpers.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/BaseValue.py` & `symbol_sdk_python-3.1.0/symbolchain/BaseValue.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/Bip32.py` & `symbol_sdk_python-3.1.0/symbolchain/Bip32.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/BlockchainSettings.py` & `symbol_sdk_python-3.1.0/symbolchain/BlockchainSettings.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/BufferReader.py` & `symbol_sdk_python-3.1.0/symbolchain/BufferReader.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/BufferWriter.py` & `symbol_sdk_python-3.1.0/symbolchain/BufferWriter.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/ByteArray.py` & `symbol_sdk_python-3.1.0/symbolchain/ByteArray.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/Cipher.py` & `symbol_sdk_python-3.1.0/symbolchain/Cipher.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/CodeWordsEncoder.py` & `symbol_sdk_python-3.1.0/symbolchain/CodeWordsEncoder.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/CryptoTypes.py` & `symbol_sdk_python-3.1.0/symbolchain/CryptoTypes.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/DiceMnemonicGenerator.py` & `symbol_sdk_python-3.1.0/symbolchain/DiceMnemonicGenerator.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/Network.py` & `symbol_sdk_python-3.1.0/symbolchain/Network.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/NetworkTimestamp.py` & `symbol_sdk_python-3.1.0/symbolchain/NetworkTimestamp.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/NodeDescriptorRepository.py` & `symbol_sdk_python-3.1.0/symbolchain/NodeDescriptorRepository.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/PrivateKeyStorage.py` & `symbol_sdk_python-3.1.0/symbolchain/PrivateKeyStorage.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/QrSignatureStorage.py` & `symbol_sdk_python-3.1.0/symbolchain/QrSignatureStorage.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/QrStorage.py` & `symbol_sdk_python-3.1.0/symbolchain/QrStorage.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/RuleBasedTransactionFactory.py` & `symbol_sdk_python-3.1.0/symbolchain/RuleBasedTransactionFactory.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/SharedKey.py` & `symbol_sdk_python-3.1.0/symbolchain/SharedKey.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/TransactionDescriptorProcessor.py` & `symbol_sdk_python-3.1.0/symbolchain/TransactionDescriptorProcessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 			value = self.type_parsing_rules[type_hint](value)
 
 		return value
 
 	def lookup_value(self, key):
 		"""Looks up the value for key."""
 		value = self._lookup_value_and_apply_type_hints(key)
-		if not any(isinstance(value, type_class) for type_class in [str, bytes, tuple]) and hasattr(value, '__iter__'):
+		if not any(isinstance(value, type_class) for type_class in [str, bytes, tuple]) and isinstance(value, list):
 			return [self.type_converter(item) for item in value]
 
 		return self.type_converter(value)
 
 	def copy_to(self, transaction, ignore_keys=None):
 		"""Copies all descriptor information to a transaction."""
 		for key in self.transaction_descriptor.keys():
```

### Comparing `symbol-sdk-python-3.0.7/symbolchain/external/ed25519.py` & `symbol_sdk_python-3.1.0/symbolchain/external/ed25519.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/facade/BatchOperations.py` & `symbol_sdk_python-3.1.0/symbolchain/facade/BatchOperations.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/facade/NemFacade.py` & `symbol_sdk_python-3.1.0/symbolchain/facade/NemFacade.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/facade/SymbolFacade.py` & `symbol_sdk_python-3.1.0/symbolchain/facade/SymbolFacade.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/impl/CipherHelpers.py` & `symbol_sdk_python-3.1.0/symbolchain/impl/CipherHelpers.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/nc/__init__.py` & `symbol_sdk_python-3.1.0/symbolchain/nc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
 
 class TransactionType(Enum):
 	TRANSFER = 257
 	ACCOUNT_KEY_LINK = 2049
 	MULTISIG_ACCOUNT_MODIFICATION = 4097
 	MULTISIG_COSIGNATURE = 4098
-	MULTISIG_TRANSACTION = 4100
+	MULTISIG = 4100
 	NAMESPACE_REGISTRATION = 8193
 	MOSAIC_DEFINITION = 16385
 	MOSAIC_SUPPLY_CHANGE = 16386
 
 	@property
 	def size(self) -> int:
 		return 4
@@ -3702,15 +3702,15 @@
 		result += f'cosignature: {self._cosignature.__str__()}, '
 		result += ')'
 		return result
 
 
 class MultisigTransactionV1:
 	TRANSACTION_VERSION: int = 1
-	TRANSACTION_TYPE: TransactionType = TransactionType.MULTISIG_TRANSACTION
+	TRANSACTION_TYPE: TransactionType = TransactionType.MULTISIG
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
 		'signature': 'pod:Signature',
 		'fee': 'pod:Amount',
@@ -3921,15 +3921,15 @@
 		result += f'cosignatures: {list(map(str, self._cosignatures))}, '
 		result += ')'
 		return result
 
 
 class NonVerifiableMultisigTransactionV1:
 	TRANSACTION_VERSION: int = 1
-	TRANSACTION_TYPE: TransactionType = TransactionType.MULTISIG_TRANSACTION
+	TRANSACTION_TYPE: TransactionType = TransactionType.MULTISIG
 	TYPE_HINTS = {
 		'type_': 'enum:TransactionType',
 		'network': 'enum:NetworkType',
 		'timestamp': 'pod:Timestamp',
 		'signer_public_key': 'pod:PublicKey',
 		'fee': 'pod:Amount',
 		'deadline': 'pod:Timestamp',
```

### Comparing `symbol-sdk-python-3.0.7/symbolchain/nem/KeyPair.py` & `symbol_sdk_python-3.1.0/symbolchain/nem/KeyPair.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/nem/MessageEncoder.py` & `symbol_sdk_python-3.1.0/symbolchain/nem/MessageEncoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+import warnings
+
 import cryptography
 
 from symbolchain.CryptoTypes import PublicKey
 from symbolchain.impl.CipherHelpers import decode_aes_cbc, decode_aes_gcm, encode_aes_cbc, encode_aes_gcm
 from symbolchain.nc import Message, MessageType
 from symbolchain.nem.KeyPair import KeyPair
 from symbolchain.nem.SharedKey import SharedKey
 
 
 class MessageEncoder:
 	"""Encrypts and encodes messages between two parties."""
 
 	def __init__(self, key_pair: KeyPair):
 		"""Creates message encoder around key pair."""
+
 		self.key_pair = key_pair
 
 	def try_decode(self, recipient_public_key, encoded_message: Message):
 		"""Tries to decode encoded message, returns tuple:
 		* True, message - if message has been decoded and decrypted
 		* False, encoded_message - otherwise
 		"""
@@ -38,26 +41,32 @@
 				'Invalid IV size',
 				'The length of the provided data is not a multiple of the block length']
 			if not any(map(lambda message: message in str(exception), exceptions)):
 				raise
 
 		return False, encoded_message
 
-	def encode_deprecated(self, recipient_public_key: PublicKey, message: bytes):
-		"""Encodes message to recipient using deprecated encryption and key derivation."""
+	def encode(self, recipient_public_key: PublicKey, message: bytes):
+		"""Encodes message to recipient using recommended format."""
 
-		salt, initialization_vector, cipher_text = encode_aes_cbc(SharedKey, self.key_pair, recipient_public_key, message)
+		tag, initialization_vector, cipher_text = encode_aes_gcm(SharedKey, self.key_pair, recipient_public_key, message)
 
 		encoded_messsage = Message()
 		encoded_messsage.message_type = MessageType.ENCRYPTED
-		encoded_messsage.message = salt + initialization_vector + cipher_text
+		encoded_messsage.message = tag + initialization_vector + cipher_text
 		return encoded_messsage
 
-	def encode(self, recipient_public_key: PublicKey, message: bytes):
-		"""Encodes message to recipient using recommended format."""
+	def encode_deprecated(self, recipient_public_key: PublicKey, message: bytes):
+		"""Encodes message to recipient using deprecated encryption and key derivation."""
 
-		tag, initialization_vector, cipher_text = encode_aes_gcm(SharedKey, self.key_pair, recipient_public_key, message)
+		warnings.warn(
+			'This function is only provided for compatability with older NEM messages.\n'
+			'Please use `encode` in any new code.',
+			category=DeprecationWarning,
+			stacklevel=2)
+
+		salt, initialization_vector, cipher_text = encode_aes_cbc(SharedKey, self.key_pair, recipient_public_key, message)
 
 		encoded_messsage = Message()
 		encoded_messsage.message_type = MessageType.ENCRYPTED
-		encoded_messsage.message = tag + initialization_vector + cipher_text
+		encoded_messsage.message = salt + initialization_vector + cipher_text
 		return encoded_messsage
```

### Comparing `symbol-sdk-python-3.0.7/symbolchain/nem/Network.py` & `symbol_sdk_python-3.1.0/symbolchain/nem/Network.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/nem/SharedKey.py` & `symbol_sdk_python-3.1.0/symbolchain/nem/SharedKey.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/nem/TransactionFactory.py` & `symbol_sdk_python-3.1.0/symbolchain/nem/TransactionFactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 	"""Factory for creating NEM transactions."""
 
 	def __init__(self, network, type_rule_overrides=None):
 		"""Creates a factory for the specified network."""
 		self.factory = self._build_rules(type_rule_overrides)
 		self.network = network
 
+	@staticmethod
+	def lookup_transaction_name(transaction_type, transaction_version):
+		"""Looks up the friendly name for the specified transaction."""
+		return f'{str(transaction_type)[str(transaction_type).index(".") + 1:].lower()}_transaction_v{transaction_version}'
+
 	def create(self, transaction_descriptor, autosort=True):
 		"""
 		Creates a transaction from a transaction descriptor.
 		When autosort is set (default), descriptor arrays requiring ordering will be automatically sorted.
 		When unset, descriptor arrays will be presumed to be already sorted.
 		"""
 		transaction = self.factory.create_from_factory(nc.TransactionFactory.create_by_name, {
```

### Comparing `symbol-sdk-python-3.0.7/symbolchain/sc/__init__.py` & `symbol_sdk_python-3.1.0/symbolchain/sc/__init__.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/symbol/IdGenerator.py` & `symbol_sdk_python-3.1.0/symbolchain/symbol/IdGenerator.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/symbol/KeyPair.py` & `symbol_sdk_python-3.1.0/symbolchain/symbol/KeyPair.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/symbol/Merkle.py` & `symbol_sdk_python-3.1.0/symbolchain/symbol/Merkle.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/symbol/Metadata.py` & `symbol_sdk_python-3.1.0/symbolchain/symbol/Metadata.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/symbol/Network.py` & `symbol_sdk_python-3.1.0/symbolchain/symbol/Network.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/symbolchain/symbol/TransactionFactory.py` & `symbol_sdk_python-3.1.0/symbolchain/symbol/TransactionFactory.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 	"""Factory for creating Symbol transactions."""
 
 	def __init__(self, network, type_rule_overrides=None):
 		"""Creates a factory for the specified network."""
 		self.factory = self._build_rules(type_rule_overrides)
 		self.network = network
 
+	@staticmethod
+	def lookup_transaction_name(transaction_type, transaction_version):
+		"""Looks up the friendly name for the specified transaction."""
+		return f'{str(transaction_type)[str(transaction_type).index(".") + 1:].lower()}_transaction_v{transaction_version}'
+
 	def _create_and_extend(self, transaction_descriptor, autosort, factory_class):
 		transaction = self.factory.create_from_factory(factory_class.create_by_name, {
 			**transaction_descriptor,
 			'network': self.network.identifier
 		})
 		if autosort:
 			transaction.sort()
```

### Comparing `symbol-sdk-python-3.0.7/symbolchain/symbol/VotingKeysGenerator.py` & `symbol_sdk_python-3.1.0/symbolchain/symbol/VotingKeysGenerator.py`

 * *Files identical despite different names*

### Comparing `symbol-sdk-python-3.0.7/setup.py` & `symbol_sdk_python-3.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,132 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: symbol-sdk-python
+Version: 3.1.0
+Summary: Symbol SDK
+Home-page: https://github.com/symbol/symbol/tree/main/sdk/python
+License: MIT
+Keywords: symbol,sdk,Symbol SDK
+Author: Symbol Contributors
+Author-email: contributors@symbol.dev
+Maintainer: Symbol Contributors
+Maintainer-email: contributors@symbol.dev
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cryptography (>=41.0.3,<41.1.0)
+Requires-Dist: mnemonic (>=0.20,<1.0)
+Requires-Dist: pillow (>=10.0.0,<10.1.0)
+Requires-Dist: pynacl (>=1.5.0,<1.6.0)
+Requires-Dist: pyyaml (>=6.0.1,<6.1.0)
+Requires-Dist: pyzbar (>=0.1.9,<0.2.0)
+Requires-Dist: qrcode (>=7.4.2,<7.5.0)
+Requires-Dist: ripemd-hash (>=1.0.1,<1.1.0)
+Requires-Dist: safe-pysha3 (>=1.0.4,<1.1.0)
+Project-URL: Repository, https://github.com/symbol/symbol/tree/main/sdk/python
+Description-Content-Type: text/markdown
+
+# Symbol-SDK
+
+[![lint][sdk-python-lint]][sdk-python-job] [![test][sdk-python-test]][sdk-python-job] [![vectors][sdk-python-vectors]][sdk-python-job] [![][sdk-python-cov]][sdk-python-cov-link] [![][sdk-python-package]][sdk-python-package-link]
+
+[sdk-python-job]: https://jenkins.symboldev.com/blue/organizations/jenkins/Symbol%2Fgenerated%2Fsymbol%2Fpython/activity?branch=dev
+[sdk-python-lint]: https://jenkins.symboldev.com/buildStatus/icon?job=Symbol%2Fgenerated%2Fsymbol%2Fpython%2Fdev%2F&config=sdk-python-lint
+[sdk-python-build]: https://jenkins.symboldev.com/buildStatus/icon?job=Symbol%2Fgenerated%2Fsymbol%2Fpython%2Fdev%2F&config=sdk-python-build
+[sdk-python-test]: https://jenkins.symboldev.com/buildStatus/icon?job=Symbol%2Fgenerated%2Fsymbol%2Fpython%2Fdev%2F&config=sdk-python-test
+[sdk-python-examples]: https://jenkins.symboldev.com/buildStatus/icon?job=Symbol%2Fgenerated%2Fsymbol%2Fpython%2Fdev%2F&config=sdk-python-examples
+[sdk-python-vectors]: https://jenkins.symboldev.com/buildStatus/icon?job=Symbol%2Fgenerated%2Fsymbol%2Fpython%2Fdev%2F&config=sdk-python-vectors
+[sdk-python-cov]: https://codecov.io/gh/symbol/symbol/branch/dev/graph/badge.svg?token=SSYYBMK0M7&flag=sdk-python
+[sdk-python-cov-link]: https://codecov.io/gh/symbol/symbol/tree/dev/sdk/python
+[sdk-python-package]: https://img.shields.io/pypi/v/symbol-sdk-python
+[sdk-python-package-link]: https://pypi.org/project/symbol-sdk-python
+
+Python SDK for interacting with the Symbol and NEM blockchains.
+
+Most common functionality is grouped under facades so that the same programming paradigm can be used for interacting with both Symbol and NEM.
+
+## Sending a Transaction
+
+To send a transaction, first create a facade for the desired network:
+
+_Symbol_
+```python
+from symbolchain.CryptoTypes import PrivateKey
+from symbolchain.facade.SymbolFacade import SymbolFacade
+
+
+facade = SymbolFacade('testnet')
+```
+
+_NEM_
+```python
+from symbolchain.CryptoTypes import PrivateKey
+from symbolchain.facade.SymbolFacade import SymbolFacade
+
+facade = SymbolFacade('testnet')
+````
+
+Second, describe the transaction using a Python dictionary. For example, a transfer transaction can be described as follows:
+
+_Symbol_
+```python
+transaction = facade.transaction_factory.create({
+	'type': 'transfer_transaction_v1',
+	'signer_public_key': '87DA603E7BE5656C45692D5FC7F6D0EF8F24BB7A5C10ED5FDA8C5CFBC49FCBC8',
+	'fee': 1000000,
+	'deadline': 41998024783,
+	'recipient_address': 'TCHBDENCLKEBILBPWP3JPB2XNY64OE7PYHHE32I',
+	'mosaics': [
+		{'mosaic_id': 0x7CDF3B117A3C40CC, 'amount': 1000000}
+	]
+})
+```
+
+_NEM_
+```python
+transaction = facade.transaction_factory.create({
+	'type': 'transfer_transaction_v1',
+	'signer_public_key': 'A59277D56E9F4FA46854F5EFAAA253B09F8AE69A473565E01FD9E6A738E4AB74',
+	'fee': 0x186A0,
+	'timestamp': 191205516,
+	'deadline': 191291916,
+	'recipient_address': 'TALICE5VF6J5FYMTCB7A3QG6OIRDRUXDWJGFVXNW',
+	'amount': 5100000
+})
+````
+
+Third, sign the transaction and attach the signature:
+
+
+```python
+private_key = PrivateKey('EDB671EB741BD676969D8A035271D1EE5E75DF33278083D877F23615EB839FEC')
+signature = facade.sign_transaction(facade.KeyPair(private_key), transaction)
+
+json_payload = facade.transactionFactory.attachSignature(transaction, signature)
+```
+
+Finally, send the payload to the desired network using the specified node endpoint:
+
+_Symbol_: PUT `/transactions`
+<br>
+_NEM_: POST `/transaction/announce`
+
+
+## NEM Cheat Sheet
+
+In order to simplify the learning curve for NEM and Symbol usage, the SDK uses Symbol terminology for shared Symbol and NEM concepts.
+Where appropriate, NEM terminology is replaced with Symbol terminology, including the names of many of the NEM transactions.
+The mapping of NEM transactions to SDK descriptors can be found in the following table:
+
+| NEM name (used in docs) | SDK descriptor name|
+|--- |--- |
+| ImportanceTransfer transaction | `account_key_link_transaction_v1` |
+| MosaicDefinitionCreation transaction | `mosaic_definition_transaction_v1` |
+| MosaicSupplyChange transaction | `mosaic_supply_change_transaction_v1` |
+| MultisigAggregateModification transaction | `multisig_account_modification_transaction_v1`<br>`multisig_account_modification_transaction_v2` |
+| MultisigSignature transaction or Cosignature transaction | `cosignature_v1` |
+| Multisig transaction | `multisig_transaction_v1` |
+| ProvisionNamespace transaction | `namespace_registration_transaction_v1` |
+| Transfer transaction | `transfer_transaction_v1`<br>`transfer_transaction_v2` |
 
-packages = \
-['symbolchain',
- 'symbolchain.external',
- 'symbolchain.facade',
- 'symbolchain.impl',
- 'symbolchain.nc',
- 'symbolchain.nem',
- 'symbolchain.sc',
- 'symbolchain.symbol']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Pillow==9.5.0',
- 'PyNaCl==1.5.0',
- 'PyYAML==6.0',
- 'cryptography==40.0.2',
- 'mnemonic==0.20',
- 'pyzbar==0.1.9',
- 'qrcode==7.4.2',
- 'ripemd-hash==1.0.0',
- 'safe-pysha3==1.0.3']
-
-setup_kwargs = {
-    'name': 'symbol-sdk-python',
-    'version': '3.0.7',
-    'description': 'Symbol SDK',
-    'long_description': "# Symbol-SDK\n\n[![lint][sdk-python-lint]][sdk-python-job] [![test][sdk-python-test]][sdk-python-job] [![vectors][sdk-python-vectors]][sdk-python-job] [![][sdk-python-cov]][sdk-python-cov-link] [![][sdk-python-package]][sdk-python-package-link]\n\n[sdk-python-job]: https://jenkins.symboldev.com/blue/organizations/jenkins/Symbol%2Fgenerated%2Fsymbol%2Fpython/activity?branch=dev\n[sdk-python-lint]: https://jenkins.symboldev.com/buildStatus/icon?job=Symbol%2Fgenerated%2Fsymbol%2Fpython%2Fdev%2F&config=sdk-python-lint\n[sdk-python-build]: https://jenkins.symboldev.com/buildStatus/icon?job=Symbol%2Fgenerated%2Fsymbol%2Fpython%2Fdev%2F&config=sdk-python-build\n[sdk-python-test]: https://jenkins.symboldev.com/buildStatus/icon?job=Symbol%2Fgenerated%2Fsymbol%2Fpython%2Fdev%2F&config=sdk-python-test\n[sdk-python-examples]: https://jenkins.symboldev.com/buildStatus/icon?job=Symbol%2Fgenerated%2Fsymbol%2Fpython%2Fdev%2F&config=sdk-python-examples\n[sdk-python-vectors]: https://jenkins.symboldev.com/buildStatus/icon?job=Symbol%2Fgenerated%2Fsymbol%2Fpython%2Fdev%2F&config=sdk-python-vectors\n[sdk-python-cov]: https://codecov.io/gh/symbol/symbol/branch/dev/graph/badge.svg?token=SSYYBMK0M7&flag=sdk-python\n[sdk-python-cov-link]: https://codecov.io/gh/symbol/symbol/tree/dev/sdk/python\n[sdk-python-package]: https://img.shields.io/pypi/v/symbol-sdk-python\n[sdk-python-package-link]: https://pypi.org/project/symbol-sdk-python\n\nPython SDK for interacting with the Symbol and NEM blockchains.\n\nMost common functionality is grouped under facades so that the same programming paradigm can be used for interacting with both Symbol and NEM.\n\n## Sending a Transaction\n\nTo send a transaction, first create a facade for the desired network:\n\n_Symbol_\n```python\nfrom symbolchain.CryptoTypes import PrivateKey\nfrom symbolchain.facade.SymbolFacade import SymbolFacade\n\n\nfacade = SymbolFacade('testnet')\n```\n\n_NEM_\n```python\nfrom symbolchain.CryptoTypes import PrivateKey\nfrom symbolchain.facade.SymbolFacade import SymbolFacade\n\nfacade = SymbolFacade('testnet')\n````\n\nSecond, describe the transaction using a Python dictionary. For example, a transfer transaction can be described as follows:\n\n_Symbol_\n```python\ntransaction = facade.transaction_factory.create({\n\t'type': 'transfer_transaction_v1',\n\t'signer_public_key': '87DA603E7BE5656C45692D5FC7F6D0EF8F24BB7A5C10ED5FDA8C5CFBC49FCBC8',\n\t'fee': 1000000,\n\t'deadline': 41998024783,\n\t'recipient_address': 'TCHBDENCLKEBILBPWP3JPB2XNY64OE7PYHHE32I',\n\t'mosaics': [\n\t\t{'mosaic_id': 0x7CDF3B117A3C40CC, 'amount': 1000000}\n\t]\n})\n```\n\n_NEM_\n```python\ntransaction = facade.transaction_factory.create({\n\t'type': 'transfer_transaction_v1',\n\t'signer_public_key': 'A59277D56E9F4FA46854F5EFAAA253B09F8AE69A473565E01FD9E6A738E4AB74',\n\t'fee': 0x186A0,\n\t'timestamp': 191205516,\n\t'deadline': 191291916,\n\t'recipient_address': 'TALICE5VF6J5FYMTCB7A3QG6OIRDRUXDWJGFVXNW',\n\t'amount': 5100000\n})\n````\n\nThird, sign the transaction and attach the signature:\n\n\n```python\nprivate_key = PrivateKey('EDB671EB741BD676969D8A035271D1EE5E75DF33278083D877F23615EB839FEC')\nsignature = facade.sign_transaction(facade.KeyPair(private_key), transaction)\n\njson_payload = facade.transactionFactory.attachSignature(transaction, signature)\n```\n\nFinally, send the payload to the desired network using the specified node endpoint:\n\n_Symbol_: PUT `/transactions`\n<br>\n_NEM_: POST `/transaction/announce`\n\n\n## NEM Cheat Sheet\n\nIn order to simplify the learning curve for NEM and Symbol usage, the SDK uses Symbol terminology for shared Symbol and NEM concepts.\nWhere appropriate, NEM terminology is replaced with Symbol terminology, including the names of many of the NEM transactions.\nThe mapping of NEM transactions to SDK descriptors can be found in the following table:\n\n| NEM name (used in docs) | SDK descriptor name|\n|--- |--- |\n| ImportanceTransfer transaction | `account_key_link_transaction_v1` |\n| MosaicDefinitionCreation transaction | `mosaic_definition_transaction_v1` |\n| MosaicSupplyChange transaction | `mosaic_supply_change_transaction_v1` |\n| MultisigAggregateModification transaction | `multisig_account_modification_transaction_v1`<br>`multisig_account_modification_transaction_v2` |\n| MultisigSignature transaction or Cosignature transaction | `cosignature_v1` |\n| Multisig transaction | `multisig_transaction_v1` |\n| ProvisionNamespace transaction | `namespace_registration_transaction_v1` |\n| Transfer transaction | `transfer_transaction_v1`<br>`transfer_transaction_v2` |\n",
-    'author': 'Symbol Contributors',
-    'author_email': 'contributors@symbol.dev',
-    'maintainer': 'Symbol Contributors',
-    'maintainer_email': 'contributors@symbol.dev',
-    'url': 'https://github.com/symbol/symbol/tree/main/sdk/python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

