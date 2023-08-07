# Comparing `tmp/jcci-0.0.8.tar.gz` & `tmp/jcci-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcci-0.0.8.tar", last modified: Tue Jul 11 02:09:53 2023, max compression
+gzip compressed data, was "jcci-0.0.9.tar", last modified: Tue Jul 11 13:55:43 2023, max compression
```

## Comparing `jcci-0.0.8.tar` & `jcci-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 02:09:53.699941 jcci-0.0.8/
--rw-rw-rw-   0        0        0     1082 2023-06-30 07:21:11.000000 jcci-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3031 2023-07-11 02:09:53.698940 jcci-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2392 2023-07-04 11:32:51.000000 jcci-0.0.8/README.md
--rw-rw-rw-   0        0        0     1247 2023-07-10 09:21:41.000000 jcci-0.0.8/README.pypi.md
--rw-rw-rw-   0        0        0      710 2023-07-11 02:09:44.000000 jcci-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 02:09:53.699941 jcci-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-11 02:09:53.679939 jcci-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 02:09:53.690941 jcci-0.0.8/src/jcci/
--rw-rw-rw-   0        0        0        0 2023-06-30 07:21:11.000000 jcci-0.0.8/src/jcci/__init__.py
--rw-rw-rw-   0        0        0     2083 2023-06-30 07:21:11.000000 jcci-0.0.8/src/jcci/java_analyzer.py
--rw-rw-rw-   0        0        0    43818 2023-07-11 02:04:09.000000 jcci-0.0.8/src/jcci/jcci.py
-drwxrwxrwx   0        0        0        0 2023-07-11 02:09:53.696940 jcci-0.0.8/src/jcci.egg-info/
--rw-rw-rw-   0        0        0     3031 2023-07-11 02:09:53.000000 jcci-0.0.8/src/jcci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-07-11 02:09:53.000000 jcci-0.0.8/src/jcci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 02:09:53.000000 jcci-0.0.8/src/jcci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-11 02:09:53.000000 jcci-0.0.8/src/jcci.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-11 02:09:53.000000 jcci-0.0.8/src/jcci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 13:55:43.631126 jcci-0.0.9/
+-rw-rw-rw-   0        0        0     1082 2023-06-30 07:21:11.000000 jcci-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3031 2023-07-11 13:55:43.630126 jcci-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2392 2023-07-04 11:32:51.000000 jcci-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1247 2023-07-10 09:21:41.000000 jcci-0.0.9/README.pypi.md
+-rw-rw-rw-   0        0        0      710 2023-07-11 13:55:34.000000 jcci-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 13:55:43.631126 jcci-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 13:55:43.615131 jcci-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 13:55:43.624126 jcci-0.0.9/src/jcci/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:21:11.000000 jcci-0.0.9/src/jcci/__init__.py
+-rw-rw-rw-   0        0        0     2083 2023-06-30 07:21:11.000000 jcci-0.0.9/src/jcci/java_analyzer.py
+-rw-rw-rw-   0        0        0    44672 2023-07-11 13:52:41.000000 jcci-0.0.9/src/jcci/jcci.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:55:43.629125 jcci-0.0.9/src/jcci.egg-info/
+-rw-rw-rw-   0        0        0     3031 2023-07-11 13:55:43.000000 jcci-0.0.9/src/jcci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-07-11 13:55:43.000000 jcci-0.0.9/src/jcci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 13:55:43.000000 jcci-0.0.9/src/jcci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-11 13:55:43.000000 jcci-0.0.9/src/jcci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-11 13:55:43.000000 jcci-0.0.9/src/jcci.egg-info/top_level.txt
```

### Comparing `jcci-0.0.8/LICENSE` & `jcci-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jcci-0.0.8/PKG-INFO` & `jcci-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.0.8
+Version: 0.0.9
 Summary: Java code commit impact analyze in pure Python
 Author-email: Oliver Li <441640312@qq.com>
 License: MIT License
         
         Copyright (c) 2023 pipi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jcci-0.0.8/README.md` & `jcci-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `jcci-0.0.8/README.pypi.md` & `jcci-0.0.9/README.pypi.md`

 * *Files identical despite different names*

### Comparing `jcci-0.0.8/pyproject.toml` & `jcci-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jcci"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Oliver Li", email="441640312@qq.com" },
 ]
 description = "Java code commit impact analyze in pure Python"
 readme = "README.pypi.md"
 license = { file="LICENSE" }
 requires-python = ">=3.5"
```

### Comparing `jcci-0.0.8/src/jcci/java_analyzer.py` & `jcci-0.0.9/src/jcci/java_analyzer.py`

 * *Files identical despite different names*

### Comparing `jcci-0.0.8/src/jcci/jcci.py` & `jcci-0.0.9/src/jcci/jcci.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,17 +87,21 @@
                 if annotation.element is not None:
                     if 'value' in annotation.element.attrs:
                         base_request = annotation.element.value.replace('"', '')
                     elif 'values' in annotation.element.attrs:
                         # print(annotation.element.values)
                         base_request = ' || '.join([literal.value for literal in annotation.element.values])
             else:
-                base_request_list = [annotation_element.value.value.replace('"', '')
-                                     for annotation_element in annotation.element
-                                     if annotation_element.name == 'value' or annotation_element.name == 'path']
+                base_request_list = []
+                for annotation_element in annotation.element:
+                    if annotation_element.name == 'value' or annotation_element.name == 'path':
+                        if 'values' in annotation_element.value.attrs:
+                            base_request_list += _get_element_with_values(annotation_element.value)
+                        else:
+                            base_request_list = [annotation_element.value.value.replace('"', '')]
                 if len(base_request_list) > 0:
                     base_request = base_request_list[0]
     if is_controller and not base_request.endswith('/'):
         base_request += '/'
     class_path = package_name + '.' + class_name
     extends_name = types.extends.name \
         if 'extends' in types.attrs and types.extends is not None \
@@ -275,14 +279,28 @@
     file_analyze.imports = imports
     file_analyze.implements = implements_names_list
     file_analyze.declarators = fields_list
     file_analyze.methods = methods_list
     return file_analyze
 
 
+def _get_element_with_values(method_api_path_obj):
+    method_api_path = []
+    for method_api_value in method_api_path_obj.values:
+        if type(method_api_value).__name__ == "BinaryOperation":
+            operandl = method_api_value.operandl
+            operandr = method_api_value.operandr
+            operandl_str = _get_api_part_route(operandl)
+            operandr_str = _get_api_part_route(operandr)
+            method_api_path += [operandl_str.replace('"', '') + operandr_str.replace('"', '')]
+        else:
+            method_api_path += [method_api_value.value.replace('"', '')]
+    return method_api_path
+
+
 def _get_api_part_route(part):
     part_class = type(part).__name__
     if part_class == 'MemberReference':
         return part.member
     elif part_class == 'Literal':
         return part.value
```

### Comparing `jcci-0.0.8/src/jcci.egg-info/PKG-INFO` & `jcci-0.0.9/src/jcci.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.0.8
+Version: 0.0.9
 Summary: Java code commit impact analyze in pure Python
 Author-email: Oliver Li <441640312@qq.com>
 License: MIT License
         
         Copyright (c) 2023 pipi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

