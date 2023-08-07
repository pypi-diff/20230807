# Comparing `tmp/django_query_tools-0.3.0-py3-none-any.whl.zip` & `tmp/django_query_tools-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 8201 bytes, number of entries: 13
+Zip file size: 8222 bytes, number of entries: 13
 -rw-r--r--  2.0 unx        0 b- defN 23-May-10 16:12 django_query_tools/__init__.py
 -rw-r--r--  2.0 unx     3192 b- defN 23-Aug-07 13:16 django_query_tools/client.py
--rw-r--r--  2.0 unx     4756 b- defN 23-Aug-07 14:42 django_query_tools/server.py
--rw-r--r--  2.0 unx       22 b- defN 23-Aug-07 11:45 django_query_tools/version.py
+-rw-r--r--  2.0 unx     5102 b- defN 23-Aug-07 15:38 django_query_tools/server.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Aug-07 15:39 django_query_tools/version.py
 -rw-r--r--  2.0 unx       39 b- defN 23-May-10 15:25 djangoquerytools/__init__.py
 -rw-r--r--  2.0 unx     2823 b- defN 23-May-10 15:30 djangoquerytools/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-10 15:26 djangoquerytools/server.py
 -rw-r--r--  2.0 unx       22 b- defN 23-May-10 15:24 djangoquerytools/version.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Aug-07 15:18 django_query_tools-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2299 b- defN 23-Aug-07 15:18 django_query_tools-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 15:18 django_query_tools-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Aug-07 15:18 django_query_tools-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1107 b- defN 23-Aug-07 15:18 django_query_tools-0.3.0.dist-info/RECORD
-13 files, 15440 bytes uncompressed, 6319 bytes compressed:  59.1%
+-rw-r--r--  2.0 unx     1069 b- defN 23-Aug-07 15:42 django_query_tools-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2299 b- defN 23-Aug-07 15:42 django_query_tools-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 15:42 django_query_tools-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Aug-07 15:42 django_query_tools-0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1107 b- defN 23-Aug-07 15:42 django_query_tools-0.3.1.dist-info/RECORD
+13 files, 15786 bytes uncompressed, 6340 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: djangoquerytools/server.py
 Comment: 
 
 Filename: djangoquerytools/version.py
 Comment: 
 
-Filename: django_query_tools-0.3.0.dist-info/LICENSE
+Filename: django_query_tools-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: django_query_tools-0.3.0.dist-info/METADATA
+Filename: django_query_tools-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: django_query_tools-0.3.0.dist-info/WHEEL
+Filename: django_query_tools-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: django_query_tools-0.3.0.dist-info/top_level.txt
+Filename: django_query_tools-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: django_query_tools-0.3.0.dist-info/RECORD
+Filename: django_query_tools-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_query_tools/server.py

```diff
@@ -47,14 +47,18 @@
     Returns a list of these `QueryAtom` objects.
     """
 
     key, value = next(iter(data.items()))
     operators = {"&", "|", "^"}
 
     if key in operators:
+        if not isinstance(value, list):
+            raise QueryException(
+                f"Expected list when parsing query but received type: {type(value)}"
+            )
         atoms = [make_atoms(k_v) for k_v in value]
         return functools.reduce(operator.add, atoms)
 
     elif key == "~":
         return make_atoms(value)
 
     else:
@@ -78,14 +82,18 @@
     Traverses the provided `data` and forms the corresponding Q object.
     """
 
     key, value = next(iter(data.items()))
     operators = {"&": operator.and_, "|": operator.or_, "^": operator.xor}
 
     if key in operators:
+        if not isinstance(value, list):
+            raise QueryException(
+                f"Expected list when parsing query but received type: {type(value)}"
+            )
         q_objects = [make_query(k_v) for k_v in value]
         return functools.reduce(operators[key], q_objects)
 
     elif key == "~":
         return ~make_query(value)
 
     else:
```

## django_query_tools/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

## Comparing `django_query_tools-0.3.0.dist-info/LICENSE` & `django_query_tools-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_query_tools-0.3.0.dist-info/METADATA` & `django_query_tools-0.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-query-tools
-Version: 0.3.0
+Version: 0.3.1
 Author: Thomas Brier
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `django-query-tools`
 Tools for building queries in Django.
```

