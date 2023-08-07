# Comparing `tmp/python_sample_03_08_2023-0.1.0-py3-none-any.whl.zip` & `tmp/python_sample_03_08_2023-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2450 bytes, number of entries: 6
--rw-r--r--  2.0 fat       49 b- defN 80-Jan-01 00:00 python_sample_03_08_2023/__init__.py
--rw-r--r--  2.0 fat      212 b- defN 80-Jan-01 00:00 python_sample_03_08_2023/basic_math.py
--rw-r--r--  2.0 fat     1098 b- defN 80-Jan-01 00:00 python_sample_03_08_2023-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 fat      463 b- defN 80-Jan-01 00:00 python_sample_03_08_2023-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 python_sample_03_08_2023-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 fat      546 b- defN 16-Jan-01 00:00 python_sample_03_08_2023-0.1.0.dist-info/RECORD
-6 files, 2456 bytes uncompressed, 1444 bytes compressed:  41.2%
+Zip file size: 2748 bytes, number of entries: 6
+-rw-r--r--  2.0 fat       54 b- defN 80-Jan-01 00:00 python_sample_03_08_2023/__init__.py
+-rw-r--r--  2.0 fat     1869 b- defN 80-Jan-01 00:00 python_sample_03_08_2023/basic_math.py
+-rw-r--r--  2.0 fat     1098 b- defN 80-Jan-01 00:00 python_sample_03_08_2023-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 fat      463 b- defN 80-Jan-01 00:00 python_sample_03_08_2023-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 python_sample_03_08_2023-0.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 fat      547 b- defN 16-Jan-01 00:00 python_sample_03_08_2023-0.1.1.dist-info/RECORD
+6 files, 4119 bytes uncompressed, 1742 bytes compressed:  57.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: python_sample_03_08_2023/__init__.py
 Comment: 
 
 Filename: python_sample_03_08_2023/basic_math.py
 Comment: 
 
-Filename: python_sample_03_08_2023-0.1.0.dist-info/LICENSE
+Filename: python_sample_03_08_2023-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: python_sample_03_08_2023-0.1.0.dist-info/METADATA
+Filename: python_sample_03_08_2023-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: python_sample_03_08_2023-0.1.0.dist-info/WHEEL
+Filename: python_sample_03_08_2023-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: python_sample_03_08_2023-0.1.0.dist-info/RECORD
+Filename: python_sample_03_08_2023-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## python_sample_03_08_2023/__init__.py

```diff
@@ -1 +1 @@
-from python_sample_03_08_2023.basic_math import *
+"""The package has basic mathematical operations."""
```

## python_sample_03_08_2023/basic_math.py

```diff
@@ -1,17 +1,78 @@
+"""
+Basic mathematical operations.
+
+This module provides useful functions for performing math operations.
+
+Functions:
+    - add(arg1, arg2): Perform addition of two numbers.
+    - sub(arg1, arg2): Perform subtraction of two numbers.
+    - multiply(arg1, arg2): Perform multiplication of two numbers.
+    - divide(arg1, arg2): Perform division of two numbers.
+    - squareroot(arg): Perform square root of the given number.
+"""
+
 from math import sqrt
 
 
-def add(a, b):
+def add(a: float, b: float) -> float:
+    """Perform addition of two numbers.
+
+    Parameters:
+    a (int or float): The first number.
+    b (int or float): The second number.
+
+    Returns:
+    int or float: The sum of the two input numbers.
+    """
     return a+b
 
-def sub(a, b):
+
+def sub(a: float, b: float) -> float:
+    """Perform subtraction of two numbers.
+
+    Parameters:
+    a (int or float): The first number.
+    b (int or float): The second number.
+
+    Returns:
+    int or float: The subtraction of the two input numbers.
+    """
     return a-b
 
-def multiply(a, b):
+
+def multiply(a: float, b: float) -> float:
+    """Perform multiplication of two numbers.
+
+    Parameters:
+    a (int or float): The first number.
+    b (int or float): The second number.
+
+    Returns:
+    int or float: The product of the two input numbers.
+    """
     return a*b
 
-def divide(a, b):
+
+def divide(a: float, b: float) -> float:
+    """Perform division of two numbers.
+
+    Parameters:
+    a (int or float): The first number.
+    b (int or float): The second number.
+
+    Returns:
+    int or float: The division of the two input numbers.
+    """
     return a/b
 
-def square_root(a):
+
+def square_root(a: float) -> float:
+    """Perform square root of the given number.
+
+    Parameters:
+    a (int or float): The first number.
+
+    Returns:
+    int or float: The square root of the input number.
+    """
     return sqrt(a)
```

## Comparing `python_sample_03_08_2023-0.1.0.dist-info/LICENSE` & `python_sample_03_08_2023-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `python_sample_03_08_2023-0.1.0.dist-info/RECORD` & `python_sample_03_08_2023-0.1.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-python_sample_03_08_2023/__init__.py,sha256=eWG91LJx1f3HF6CcxmenGIPXVCQNyEyuvaoPakL2-uw,49
-python_sample_03_08_2023/basic_math.py,sha256=QvNuEUetPgB6v-QOcpguVtMCmAFzgkiY5_Yjg5ntGYE,212
-python_sample_03_08_2023-0.1.0.dist-info/LICENSE,sha256=jIrRAkIWFTv_LCwvdgQxqdNu8k8vMt2Pj5sIbYxtTnM,1098
-python_sample_03_08_2023-0.1.0.dist-info/METADATA,sha256=KfmH-eMepUAVAp6fkhy8nJVkuKxifG9Eib3Th8ZGM3Y,463
-python_sample_03_08_2023-0.1.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-python_sample_03_08_2023-0.1.0.dist-info/RECORD,,
+python_sample_03_08_2023/__init__.py,sha256=leg2w-MIEAd7pPSv1V0rStaO6kUUl4gKlCszLBJBkzY,54
+python_sample_03_08_2023/basic_math.py,sha256=Pt-urDio5CITyMpyRk9aDEsGQYeo54heavzeg3-MFvo,1869
+python_sample_03_08_2023-0.1.1.dist-info/LICENSE,sha256=jIrRAkIWFTv_LCwvdgQxqdNu8k8vMt2Pj5sIbYxtTnM,1098
+python_sample_03_08_2023-0.1.1.dist-info/METADATA,sha256=1JjyLL-DBBQDJSRwKZTE4Xev7GJPEf_p8ItTxlBWs1o,463
+python_sample_03_08_2023-0.1.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+python_sample_03_08_2023-0.1.1.dist-info/RECORD,,
```

