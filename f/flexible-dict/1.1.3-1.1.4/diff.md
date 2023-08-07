# Comparing `tmp/flexible_dict-1.1.3.tar.gz` & `tmp/flexible_dict-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexible_dict-1.1.3.tar", last modified: Fri Aug  4 12:12:47 2023, max compression
+gzip compressed data, was "flexible_dict-1.1.4.tar", last modified: Mon Aug  7 07:47:51 2023, max compression
```

## Comparing `flexible_dict-1.1.3.tar` & `flexible_dict-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-04 12:12:47.511976 flexible_dict-1.1.3/
--rw-r--r--   0 bytedance   (501) staff       (20)     2080 2023-08-04 12:12:47.511819 flexible_dict-1.1.3/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)     1791 2023-08-04 11:30:22.000000 flexible_dict-1.1.3/README.md
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-04 12:12:47.510379 flexible_dict-1.1.3/flexible_dict/
--rw-r--r--   0 bytedance   (501) staff       (20)      208 2023-07-28 02:13:43.000000 flexible_dict-1.1.3/flexible_dict/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      508 2023-07-24 09:58:30.000000 flexible_dict-1.1.3/flexible_dict/__main__.py
--rw-r--r--   0 bytedance   (501) staff       (20)       88 2023-08-04 12:10:37.000000 flexible_dict-1.1.3/flexible_dict/about.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9856 2023-08-04 12:10:20.000000 flexible_dict-1.1.3/flexible_dict/json_object.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-04 12:12:47.511200 flexible_dict-1.1.3/flexible_dict/script/
--rw-r--r--   0 bytedance   (501) staff       (20)       24 2023-07-26 03:47:11.000000 flexible_dict-1.1.3/flexible_dict/script/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5360 2023-07-25 03:14:12.000000 flexible_dict-1.1.3/flexible_dict/script/class_builder.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-04 12:12:47.510932 flexible_dict-1.1.3/flexible_dict.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)     2080 2023-08-04 12:12:47.000000 flexible_dict-1.1.3/flexible_dict.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      393 2023-08-04 12:12:47.000000 flexible_dict-1.1.3/flexible_dict.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-08-04 12:12:47.000000 flexible_dict-1.1.3/flexible_dict.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       14 2023-08-04 12:12:47.000000 flexible_dict-1.1.3/flexible_dict.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-08-04 12:12:47.512038 flexible_dict-1.1.3/setup.cfg
--rw-r--r--   0 bytedance   (501) staff       (20)      970 2023-07-24 10:52:09.000000 flexible_dict-1.1.3/setup.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-04 12:12:47.511540 flexible_dict-1.1.3/tests/
--rw-r--r--   0 bytedance   (501) staff       (20)      625 2023-07-25 03:17:01.000000 flexible_dict-1.1.3/tests/test_build_class.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1112 2023-07-28 02:13:43.000000 flexible_dict-1.1.3/tests/test_json_object.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-07 07:47:51.600681 flexible_dict-1.1.4/
+-rw-r--r--   0 bytedance   (501) staff       (20)     2080 2023-08-07 07:47:51.600565 flexible_dict-1.1.4/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)     1791 2023-08-04 11:30:22.000000 flexible_dict-1.1.4/README.md
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-07 07:47:51.598735 flexible_dict-1.1.4/flexible_dict/
+-rw-r--r--   0 bytedance   (501) staff       (20)      208 2023-07-28 02:13:43.000000 flexible_dict-1.1.4/flexible_dict/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      532 2023-08-07 04:45:15.000000 flexible_dict-1.1.4/flexible_dict/__main__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)       88 2023-08-07 07:45:43.000000 flexible_dict-1.1.4/flexible_dict/about.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    10591 2023-08-07 07:44:08.000000 flexible_dict-1.1.4/flexible_dict/json_object.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-07 07:47:51.599736 flexible_dict-1.1.4/flexible_dict/script/
+-rw-r--r--   0 bytedance   (501) staff       (20)       24 2023-07-26 03:47:11.000000 flexible_dict-1.1.4/flexible_dict/script/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5360 2023-07-25 03:14:12.000000 flexible_dict-1.1.4/flexible_dict/script/class_builder.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-07 07:47:51.599249 flexible_dict-1.1.4/flexible_dict.egg-info/
+-rw-r--r--   0 bytedance   (501) staff       (20)     2080 2023-08-07 07:47:51.000000 flexible_dict-1.1.4/flexible_dict.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)      393 2023-08-07 07:47:51.000000 flexible_dict-1.1.4/flexible_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-08-07 07:47:51.000000 flexible_dict-1.1.4/flexible_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       14 2023-08-07 07:47:51.000000 flexible_dict-1.1.4/flexible_dict.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-08-07 07:47:51.600719 flexible_dict-1.1.4/setup.cfg
+-rw-r--r--   0 bytedance   (501) staff       (20)      970 2023-07-24 10:52:09.000000 flexible_dict-1.1.4/setup.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-07 07:47:51.600284 flexible_dict-1.1.4/tests/
+-rw-r--r--   0 bytedance   (501) staff       (20)      625 2023-07-25 03:17:01.000000 flexible_dict-1.1.4/tests/test_build_class.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1112 2023-07-28 02:13:43.000000 flexible_dict-1.1.4/tests/test_json_object.py
```

### Comparing `flexible_dict-1.1.3/PKG-INFO` & `flexible_dict-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible_dict
-Version: 1.1.3
+Version: 1.1.4
 Summary: A flexible way to access dict data instead of built-in dict.
 Home-page: https://github.com/darkpeath/flexible_dict
 Author: darkpeath
 Author-email: darkpeath@gmail.com
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `flexible_dict-1.1.3/README.md` & `flexible_dict-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `flexible_dict-1.1.3/flexible_dict/json_object.py` & `flexible_dict-1.1.4/flexible_dict/json_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Same code is copied from dataclasses.
 # Code of dataclasses is pretty.
 
-from typing import Any, Callable, Dict
+from typing import Any, Callable, Dict, Tuple, Iterable
 import warnings
 import dataclasses
 import types
 
 # A sentinel object to detect if a parameter is supplied or not.  Use
 # a class to give it a better repr.
 class _MISSING_TYPE:
@@ -235,20 +235,45 @@
     return wrap(cls)
 
 # Another way to define a json_object class, just inherit this class.
 class JsonObject(dict):
     def __init_subclass__(cls):
         super().__init_subclass__()
         JsonObjectClassProcessor()(cls)
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         fields = getattr(self, _FIELDS, {})
         for f in fields.values():
             f: Field
             value = self.get(f.key)
             if value is None or not isinstance(f.type, type) or isinstance(value, f.type):
                 continue
             adapt_data_type = f.adapt_data_type
             if adapt_data_type is None or adapt_data_type:
                 adapt_data_type = hasattr(f.type, _FIELDS)
             if adapt_data_type and isinstance(value, dict):
                 self[f.key] = f.type(value)
+
+    def field_items(self) -> Iterable[Tuple[str, Any]]:
+        """
+        iter of defined field values
+        """
+        # one should not define a field use the reserved name
+        fields = getattr(self, _FIELDS, {})
+        for name, field in fields.items():
+            if field.key in self:
+                yield name, self[field.key]
+
+    @property
+    def _iter_field_items_only(self) -> bool:
+        """
+        determine output of method items(): if `True`, same as field_items(); else same as dict.items()
+        """
+        return False
+
+    def items(self) -> Iterable[Tuple[str, Any]]:
+        if self._iter_field_items_only:
+            return self.field_items()
+        return super().items()
+
+
```

### Comparing `flexible_dict-1.1.3/flexible_dict/script/class_builder.py` & `flexible_dict-1.1.4/flexible_dict/script/class_builder.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-1.1.3/flexible_dict.egg-info/PKG-INFO` & `flexible_dict-1.1.4/flexible_dict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible-dict
-Version: 1.1.3
+Version: 1.1.4
 Summary: A flexible way to access dict data instead of built-in dict.
 Home-page: https://github.com/darkpeath/flexible_dict
 Author: darkpeath
 Author-email: darkpeath@gmail.com
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `flexible_dict-1.1.3/setup.py` & `flexible_dict-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-1.1.3/tests/test_build_class.py` & `flexible_dict-1.1.4/tests/test_build_class.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-1.1.3/tests/test_json_object.py` & `flexible_dict-1.1.4/tests/test_json_object.py`

 * *Files identical despite different names*

