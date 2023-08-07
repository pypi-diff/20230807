# Comparing `tmp/cosmian_anonymization-1.2.0-py3-none-any.whl.zip` & `tmp/cosmian_anonymization-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20456 bytes, number of entries: 11
+Zip file size: 20507 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 cosmian_anonymization/__init__.py
 -rw-r--r--  2.0 unx     8273 b- defN 80-Jan-01 00:00 cosmian_anonymization/anonymize.py
 -rw-r--r--  2.0 unx     1954 b- defN 80-Jan-01 00:00 cosmian_anonymization/conversion_helper.py
--rw-r--r--  2.0 unx     3628 b- defN 80-Jan-01 00:00 cosmian_anonymization/method_parser.py
--rw-r--r--  2.0 unx     3784 b- defN 80-Jan-01 00:00 cosmian_anonymization/noise_correlation.py
--rw-r--r--  2.0 unx     3887 b- defN 80-Jan-01 00:00 cosmian_anonymization/noise_parser.py
--rw-r--r--  2.0 unx    32275 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.2.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1500 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       73 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.2.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1030 b- defN 16-Jan-01 00:00 cosmian_anonymization-1.2.0.dist-info/RECORD
-11 files, 56754 bytes uncompressed, 18676 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx     3824 b- defN 80-Jan-01 00:00 cosmian_anonymization/method_parser.py
+-rw-r--r--  2.0 unx     3842 b- defN 80-Jan-01 00:00 cosmian_anonymization/noise_correlation.py
+-rw-r--r--  2.0 unx     3979 b- defN 80-Jan-01 00:00 cosmian_anonymization/noise_parser.py
+-rw-r--r--  2.0 unx    32275 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.2.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1500 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.2.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1030 b- defN 16-Jan-01 00:00 cosmian_anonymization-1.2.1.dist-info/RECORD
+11 files, 57100 bytes uncompressed, 18727 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: cosmian_anonymization/noise_correlation.py
 Comment: 
 
 Filename: cosmian_anonymization/noise_parser.py
 Comment: 
 
-Filename: cosmian_anonymization-1.2.0.dist-info/LICENSE.md
+Filename: cosmian_anonymization-1.2.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: cosmian_anonymization-1.2.0.dist-info/METADATA
+Filename: cosmian_anonymization-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: cosmian_anonymization-1.2.0.dist-info/WHEEL
+Filename: cosmian_anonymization-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: cosmian_anonymization-1.2.0.dist-info/entry_points.txt
+Filename: cosmian_anonymization-1.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: cosmian_anonymization-1.2.0.dist-info/RECORD
+Filename: cosmian_anonymization-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cosmian_anonymization/method_parser.py

```diff
@@ -1,16 +1,14 @@
 # -*- coding: utf-8 -*-
 import os
 from typing import Callable, Dict, Optional
 
-from cloudproof_py.anonymization import DateAggregator
-from cloudproof_py.anonymization import (
-    Hasher as AnoHasher,  # Avoid builtin.Hasher name override
-)
 from cloudproof_py.anonymization import (
+    DateAggregator,
+    Hasher,
     NumberAggregator,
     NumberScaler,
     WordMasker,
     WordPatternMasker,
     WordTokenizer,
 )
 from cloudproof_py.fpe import Alphabet, Float, Integer
@@ -22,34 +20,50 @@
 def parse_date_aggregation_options(time_unit: str) -> Callable[[str], str]:
     """
     Parses the date aggregation options and returns a function that applies the aggregation.
 
     Args:
         time_unit (str): The time unit for rounding.
     """
-    return lambda date_str: DateAggregator(time_unit).apply_on_date(
-        date_to_rfc3339(date_str)
-    )
+    date_aggregator = DateAggregator(time_unit)
+
+    def apply_date_aggregation(date_str: str) -> str:
+        return date_aggregator.apply_on_date(date_to_rfc3339(date_str))
+
+    return apply_date_aggregation
 
 
 def parse_fpe_string_options(alphabet: str) -> Callable[[str], str]:
     # TODO: get key and tweak from dedicated file
-    return lambda val: Alphabet(alphabet).encrypt(os.urandom(32), os.urandom(32), val)
+    fpe_string = Alphabet(alphabet)
+
+    def fpe_string_encrypt(val: str) -> str:
+        return fpe_string.encrypt(os.urandom(32), os.urandom(32), val)
+
+    return fpe_string_encrypt
 
 
 def parse_fpe_integer_options(radix: int, digit: int) -> Callable[[int], int]:
     # TODO: get key and tweak from dedicated file
-    return lambda val: Integer(radix, digit).encrypt(
-        os.urandom(32), os.urandom(32), val
-    )
+    fpe_int = Integer(radix, digit)
+
+    def fpe_int_encrypt(val: int) -> int:
+        return fpe_int.encrypt(os.urandom(32), os.urandom(32), val)
+
+    return fpe_int_encrypt
 
 
 def parse_fpe_float_options() -> Callable[[float], float]:
     # TODO: get key and tweak from dedicated file
-    return lambda val: Float().encrypt(os.urandom(32), os.urandom(32), val)
+    fpe_float = Float()
+
+    def fpe_float_encrypt(val: float) -> float:
+        return fpe_float.encrypt(os.urandom(32), os.urandom(32), val)
+
+    return fpe_float_encrypt
 
 
 def parse_hash_options(
     hash_type: str, salt_value: Optional[str] = None, encoding="utf-8"
 ) -> Callable[[str], str]:
     """
     Returns a function that takes a string and applies a hash function to it.
@@ -58,17 +72,16 @@
         hash_type (str): The name of the hash function to use.
         salt_value (Optional[str]): An optional salt to use for hashing.
         encoding (str): The encoding to use when converting the input string to bytes.
     """
     salt = None
     if salt_value:
         salt = salt_value.encode(encoding)
-    hasher = AnoHasher(hash_type, salt)
 
-    return lambda val: hasher.apply_str(val)
+    return Hasher(hash_type, salt).apply_str
 
 
 def create_transformation_function(method_name: str, method_opts: Dict) -> Callable:
     """
     Given a method name and options, returns a callable that applies the desired transformation.
     """
     parsing_functions: Dict[str, Callable] = {
```

## cosmian_anonymization/noise_correlation.py

```diff
@@ -57,16 +57,20 @@
         if noise_generator_func is None:
             raise ValueError(f"Cannot apply correlation for method: {self.method}.")
 
         # Scale noise by 1 for now
         correlation_factors = [1] * len(self.column_names)
         # Create a noise generator instance with the specified options
         noise_generator = noise_generator_func(**self.options)
-        # Return a lambda function that applies the noise generator to the data vector
-        return lambda data_vec: noise_generator(data_vec, correlation_factors)
+
+        # Return a function that applies the noise generator to the data vector
+        def apply_noise(data_vec: List) -> List:
+            return noise_generator(data_vec, correlation_factors)
+
+        return apply_noise
 
 
 def parse_noise_correlation_config(config: Dict) -> Dict[str, NoiseCorrelationTask]:
     """
     Parse the noise correlation configuration and return the dictionary of correlation tasks.
 
     Args:
```

## cosmian_anonymization/noise_parser.py

```diff
@@ -82,12 +82,15 @@
         lower_boundary=lower_boundary_secs,
         upper_boundary=upper_boundary_secs,
     )
 
 
 def parse_date_noise_options(**kwargs) -> Callable[[str], str]:
     """
-    Returns a lambda function that takes a date string and returns a noisy version of that date.
+    Returns a function that takes a date string and returns a noisy version of that date.
     """
-    return lambda date_str: create_date_noise_generator(**kwargs).apply_on_date(
-        date_to_rfc3339(date_str)
-    )
+    date_noise_generator = create_date_noise_generator(**kwargs)
+
+    def apply_date_noise(date_str: str) -> str:
+        return date_noise_generator.apply_on_date(date_to_rfc3339(date_str))
+
+    return apply_date_noise
```

## Comparing `cosmian_anonymization-1.2.0.dist-info/LICENSE.md` & `cosmian_anonymization-1.2.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `cosmian_anonymization-1.2.0.dist-info/METADATA` & `cosmian_anonymization-1.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmian-anonymization
-Version: 1.2.0
+Version: 1.2.1
 Summary: Cosmian Anonymization library in Python
 Author: Hugo Rosenkranz-Costa
 Author-email: hugo.rosenkranz@cosmian.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `cosmian_anonymization-1.2.0.dist-info/RECORD` & `cosmian_anonymization-1.2.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cosmian_anonymization/__init__.py,sha256=I2KNlDp6w9J0ZC8D8CBGxuAG5tD6mlLzme3tMuVqCjQ,262
 cosmian_anonymization/anonymize.py,sha256=Ib3c5k5oz9d81t05Encuhj1-IiJxKewJrgFl7NWbNs0,8273
 cosmian_anonymization/conversion_helper.py,sha256=WiT2AVz9_eR0KdR1hHx79U8wS_rDPy9_8hXolvWB-gg,1954
-cosmian_anonymization/method_parser.py,sha256=JoDKER4MZVYbOcRzsNcXZTe7DADZzWA9H4oHaBeJXbA,3628
-cosmian_anonymization/noise_correlation.py,sha256=GCmDJKpmB3p1DxeaQA_y6BcVLuB_tXxtCfBVJauwQmE,3784
-cosmian_anonymization/noise_parser.py,sha256=l6G9qjwPXNf43Rb9PvawFriF1AcDzSz0_nBNAqBz1Q4,3887
-cosmian_anonymization-1.2.0.dist-info/LICENSE.md,sha256=_zfsPgqYDWuqWECzE0w-LQfkkgg28_DMNj87xgn6OUI,32275
-cosmian_anonymization-1.2.0.dist-info/METADATA,sha256=UlzF4_5fs7k86OzzMBfQW0rtNLbYgF-larMHAJths6E,1500
-cosmian_anonymization-1.2.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-cosmian_anonymization-1.2.0.dist-info/entry_points.txt,sha256=8zwjT9vbjKsVxtbgIOOw9YY0zzI7PE9y06fEsILeAyA,73
-cosmian_anonymization-1.2.0.dist-info/RECORD,,
+cosmian_anonymization/method_parser.py,sha256=u5sQdtBOQ2zpA-CHKTm8T9K4fPrXhI3rw6pZxXEkTeo,3824
+cosmian_anonymization/noise_correlation.py,sha256=f-Ai61USedgqBGfpInyKZ-xAaE7raVFzH8_o455iFps,3842
+cosmian_anonymization/noise_parser.py,sha256=PezCycfOPqLtI4Sb2MfJSrm0RHA6SKs0wo1Qu5WLaOk,3979
+cosmian_anonymization-1.2.1.dist-info/LICENSE.md,sha256=_zfsPgqYDWuqWECzE0w-LQfkkgg28_DMNj87xgn6OUI,32275
+cosmian_anonymization-1.2.1.dist-info/METADATA,sha256=byufgCHPif1YzjSL-C6_EgP7qvGGu2lzgjtCtlOlLU4,1500
+cosmian_anonymization-1.2.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+cosmian_anonymization-1.2.1.dist-info/entry_points.txt,sha256=8zwjT9vbjKsVxtbgIOOw9YY0zzI7PE9y06fEsILeAyA,73
+cosmian_anonymization-1.2.1.dist-info/RECORD,,
```

