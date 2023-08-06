# Comparing `tmp/logical_rush-0.0.3-py3-none-any.whl.zip` & `tmp/logical_rush-0.0.4-cp310-cp310-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,8 @@
-Zip file size: 1274367 bytes, number of entries: 9
+Zip file size: 199239 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat      131 b- defN 23-Jun-16 01:14 logical_rush/__init__.py
--rw-rw-rw-  2.0 fat  1508352 b- defN 23-Jun-16 01:14 logical_rush/_logical_rush.pyd
--rw-rw-rw-  2.0 fat  1508352 b- defN 23-Jun-16 01:14 logical_rush/logical_rush.cp310-win_amd64.pyd
--rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-05 19:13 logical_rush/logical_rush.py
--rw-rw-rw-  2.0 fat   793088 b- defN 23-May-02 17:20 logical_rush/logical_rush.so
--rw-rw-rw-  2.0 fat     3409 b- defN 23-Aug-05 19:17 logical_rush-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-05 19:17 logical_rush-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-05 19:17 logical_rush-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      762 b- defN 23-Aug-05 19:17 logical_rush-0.0.3.dist-info/RECORD
-9 files, 3814199 bytes uncompressed, 1273055 bytes compressed:  66.6%
+-rw-rw-rw-  2.0 fat   457728 b- defN 23-Aug-06 17:48 logical_rush/logical_rush.cp310-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     3466 b- defN 23-Aug-06 17:48 logical_rush-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Aug-06 17:48 logical_rush-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-06 17:48 logical_rush-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      503 b- defN 23-Aug-06 17:48 logical_rush-0.0.4.dist-info/RECORD
+6 files, 461943 bytes uncompressed, 198327 bytes compressed:  57.1%
```

## zipnote {}

```diff
@@ -1,28 +1,19 @@
 Filename: logical_rush/__init__.py
 Comment: 
 
-Filename: logical_rush/_logical_rush.pyd
-Comment: 
-
 Filename: logical_rush/logical_rush.cp310-win_amd64.pyd
 Comment: 
 
-Filename: logical_rush/logical_rush.py
-Comment: 
-
-Filename: logical_rush/logical_rush.so
-Comment: 
-
-Filename: logical_rush-0.0.3.dist-info/METADATA
+Filename: logical_rush-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: logical_rush-0.0.3.dist-info/WHEEL
+Filename: logical_rush-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: logical_rush-0.0.3.dist-info/top_level.txt
+Filename: logical_rush-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: logical_rush-0.0.3.dist-info/RECORD
+Filename: logical_rush-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `logical_rush-0.0.3.dist-info/METADATA` & `logical_rush-0.0.4.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: logical-rush
-Version: 0.0.3
+Version: 0.0.4
 Summary: Batch-computing solution for cashflow calculations.
 Author: Blasser Analytica (Rodolfo Blasser)
 Author-email: <rodolfoblasser@gmail.com>
-Keywords: python,panama,finance,stocks,fixed income,data,api,market data,latinex
+Keywords: batch-computing,cashflows,ammortization
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 # logical_rush
 Batch-computing solution for cashflow calculations.
```

