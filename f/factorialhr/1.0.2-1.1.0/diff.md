# Comparing `tmp/factorialhr-1.0.2-py3-none-any.whl.zip` & `tmp/factorialhr-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8690 bytes, number of entries: 7
--rw-r--r--  2.0 unx      256 b- defN 23-Mar-27 16:30 factorialhr/__init__.py
--rw-r--r--  2.0 unx    35510 b- defN 23-Mar-27 16:30 factorialhr/endpoints.py
--rw-r--r--  2.0 unx    10071 b- defN 23-Mar-27 16:30 factorialhr/models.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-27 16:30 factorialhr/py.typed
-?rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 factorialhr-1.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     3837 b- defN 16-Jan-01 00:00 factorialhr-1.0.2.dist-info/METADATA
-?rw-r--r--  2.0 unx      532 b- defN 16-Jan-01 00:00 factorialhr-1.0.2.dist-info/RECORD
-7 files, 50287 bytes uncompressed, 7754 bytes compressed:  84.6%
+Zip file size: 8691 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      256 b- defN 23-Aug-07 06:58 factorialhr/__init__.py
+-rw-r--r--  2.0 unx    35510 b- defN 23-Aug-07 06:58 factorialhr/endpoints.py
+-rw-r--r--  2.0 unx    10074 b- defN 23-Aug-07 06:58 factorialhr/models.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-07 06:58 factorialhr/py.typed
+-rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 factorialhr-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx     3837 b- defN 16-Jan-01 00:00 factorialhr-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      532 b- defN 16-Jan-01 00:00 factorialhr-1.1.0.dist-info/RECORD
+7 files, 50290 bytes uncompressed, 7755 bytes compressed:  84.6%
```

## zipnote {}

```diff
@@ -6,17 +6,17 @@
 
 Filename: factorialhr/models.py
 Comment: 
 
 Filename: factorialhr/py.typed
 Comment: 
 
-Filename: factorialhr-1.0.2.dist-info/WHEEL
+Filename: factorialhr-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: factorialhr-1.0.2.dist-info/METADATA
+Filename: factorialhr-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: factorialhr-1.0.2.dist-info/RECORD
+Filename: factorialhr-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## factorialhr/models.py

```diff
@@ -11,15 +11,15 @@
 
 class Employee(pydantic.BaseModel):
     id: int
     first_name: str
     last_name: str
     full_name: str
     email: str
-    birthday: datetime.date | None
+    birthday_on: datetime.date | None
     terminated_on: datetime.date | None
     termination_reason: str | None
     termination_reason_type: str | None
     termination_observations: str | None
     identifier: str | None
     identifier_type: str | None
     gender: str | None
```

## Comparing `factorialhr-1.0.2.dist-info/METADATA` & `factorialhr-1.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factorialhr
-Version: 1.0.2
+Version: 1.1.0
 Summary: Python package for the api of FactorialHR 
 Keywords: FactorialHR,HR
 Author-email: Leon Budnick <y6q6ea9w@mail-proxy.org>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

## Comparing `factorialhr-1.0.2.dist-info/RECORD` & `factorialhr-1.1.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 factorialhr/__init__.py,sha256=m6IeDqIm1HIokIB8Gm8Mugb71eD4G2nGlDTg5-NPcsE,256
 factorialhr/endpoints.py,sha256=nh6zpzN3Zmh6RqRfBDrtTUWGISPPTzp0YhpfO_tAOuw,35510
-factorialhr/models.py,sha256=QXYIIfdqjfkXaPTMyBnj7yp44lST4Tw1jLhbt3IgTb8,10071
+factorialhr/models.py,sha256=1XA9gm1ji_NMYSFFUD39JEahNuJGAb5xLPvfidS337I,10074
 factorialhr/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-factorialhr-1.0.2.dist-info/WHEEL,sha256=rSgq_JpHF9fHR1lx53qwg_1-2LypZE_qmcuXbVUq948,81
-factorialhr-1.0.2.dist-info/METADATA,sha256=Opqq455_udUOORNVSMjE9ZXuN-wZVh3GFftYwo_V660,3837
-factorialhr-1.0.2.dist-info/RECORD,,
+factorialhr-1.1.0.dist-info/WHEEL,sha256=EZbGkh7Ie4PoZfRQ8I0ZuP9VklN_TvcZ6DSE5Uar4z4,81
+factorialhr-1.1.0.dist-info/METADATA,sha256=XaHbDLU6VmNhfyL8bhG0xB47ivTEboyEbGyneASs-ZA,3837
+factorialhr-1.1.0.dist-info/RECORD,,
```

