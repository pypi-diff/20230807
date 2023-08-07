# Comparing `tmp/scribeauth-1.0.6-py3-none-any.whl.zip` & `tmp/scribeauth-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 8053 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat       66 b- defN 23-May-17 09:44 scribeauth/__init__.py
 -rw-rw-rw-  2.0 fat      664 b- defN 23-Jun-20 10:33 scribeauth/__main__.py
 -rw-rw-rw-  2.0 fat    14309 b- defN 23-Jun-20 10:12 scribeauth/scribeauth.py
 -rw-rw-rw-  2.0 fat     1351 b- defN 23-May-15 17:21 scribeauth/scribeauthfederation.py
--rw-rw-rw-  2.0 fat     1097 b- defN 23-Jun-20 10:34 scribeauth-1.0.6.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat     5008 b- defN 23-Jun-20 10:34 scribeauth-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-20 10:34 scribeauth-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-20 10:34 scribeauth-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      732 b- defN 23-Jun-20 10:34 scribeauth-1.0.6.dist-info/RECORD
+-rw-rw-rw-  2.0 fat     1097 b- defN 23-Aug-07 12:36 scribeauth-1.0.8.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat     5008 b- defN 23-Aug-07 12:36 scribeauth-1.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-07 12:36 scribeauth-1.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Aug-07 12:36 scribeauth-1.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      732 b- defN 23-Aug-07 12:36 scribeauth-1.0.8.dist-info/RECORD
 9 files, 23330 bytes uncompressed, 6789 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: scribeauth/scribeauth.py
 Comment: 
 
 Filename: scribeauth/scribeauthfederation.py
 Comment: 
 
-Filename: scribeauth-1.0.6.dist-info/LICENSE.md
+Filename: scribeauth-1.0.8.dist-info/LICENSE.md
 Comment: 
 
-Filename: scribeauth-1.0.6.dist-info/METADATA
+Filename: scribeauth-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: scribeauth-1.0.6.dist-info/WHEEL
+Filename: scribeauth-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: scribeauth-1.0.6.dist-info/top_level.txt
+Filename: scribeauth-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: scribeauth-1.0.6.dist-info/RECORD
+Filename: scribeauth-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `scribeauth-1.0.6.dist-info/LICENSE.md` & `scribeauth-1.0.8.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `scribeauth-1.0.6.dist-info/METADATA` & `scribeauth-1.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scribeauth
-Version: 1.0.6
+Version: 1.0.8
 Summary: Library to authenticate to Scribe's platform
 Home-page: https://github.com/ScribeLabsAI/ScribeAuth
 Author: Ailin Venerus
 Author-email: ailin@scribelabs.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

## Comparing `scribeauth-1.0.6.dist-info/RECORD` & `scribeauth-1.0.8.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 scribeauth/__init__.py,sha256=2-RDsb4wzEH_M6fa1C_QVx5qQylNuMw0I1K1tNDtz8o,66
 scribeauth/__main__.py,sha256=G5QJGPflFoSlMPoUNyP9y9xKmDy2udBUeDOZyF_-RpE,664
 scribeauth/scribeauth.py,sha256=5_egs_T1zO291rM9mLFsyVz_OM6_6JVPrKIauRmOWwI,14309
 scribeauth/scribeauthfederation.py,sha256=hcuxU437ejJVDgzxoClSemUwlNfVEXBhB52ETfhTxRk,1351
-scribeauth-1.0.6.dist-info/LICENSE.md,sha256=UxWtngnKh5L97bck8adZy5mU_kPYjXQmpzoQW3UBZgA,1097
-scribeauth-1.0.6.dist-info/METADATA,sha256=tjjjZktV1pC29Xpb5K61ucyqaRlM5Fz6cyzJ8t6Kr2I,5008
-scribeauth-1.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-scribeauth-1.0.6.dist-info/top_level.txt,sha256=u_gWgkGGrMYmNcBINraxlpw1j0QerxKxy9dTD9yXgnE,11
-scribeauth-1.0.6.dist-info/RECORD,,
+scribeauth-1.0.8.dist-info/LICENSE.md,sha256=UxWtngnKh5L97bck8adZy5mU_kPYjXQmpzoQW3UBZgA,1097
+scribeauth-1.0.8.dist-info/METADATA,sha256=ajtW-T9cIx9Xbs-MWZKXSBhKIlsmKReCPdLtM1MR3Wg,5008
+scribeauth-1.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+scribeauth-1.0.8.dist-info/top_level.txt,sha256=u_gWgkGGrMYmNcBINraxlpw1j0QerxKxy9dTD9yXgnE,11
+scribeauth-1.0.8.dist-info/RECORD,,
```

