# Comparing `tmp/formkit_ninja-0.4.0a0.tar.gz` & `tmp/formkit_ninja-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formkit_ninja-0.4.0a0.tar", max compression
+gzip compressed data, was "formkit_ninja-0.4.0a1.tar", max compression
```

## Comparing `formkit_ninja-0.4.0a0.tar` & `formkit_ninja-0.4.0a1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      813 2023-08-02 03:08:55.535863 formkit_ninja-0.4.0a0/README.md
--rw-r--r--   0        0        0        0 2023-08-02 03:08:55.547864 formkit_ninja-0.4.0a0/formkit_ninja/__init__.py
--rw-r--r--   0        0        0        0 2023-08-02 03:08:55.535863 formkit_ninja-0.4.0a0/formkit_ninja/__main__.py
--rw-r--r--   0        0        0    14803 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a0/formkit_ninja/admin.py
--rw-r--r--   0        0        0     2568 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a0/formkit_ninja/api.py
--rw-r--r--   0        0        0     4333 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a0/formkit_ninja/fields.py
--rw-r--r--   0        0        0    14920 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/formkit_schema.py
--rw-r--r--   0        0        0        0 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a0/formkit_ninja/management/__init__.py
--rw-r--r--   0        0        0        0 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a0/formkit_ninja/management/commands/__init__.py
--rw-r--r--   0        0        0     3807 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/management/commands/common_nodes.py
--rw-r--r--   0        0        0    19033 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/management/commands/create_sf11_form.py
--rw-r--r--   0        0        0     3190 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/management/commands/create_sf12_form.py
--rw-r--r--   0        0        0     1359 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/management/commands/create_sf13_form.py
--rw-r--r--   0        0        0    15058 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/migrations/0001_initial.py
--rw-r--r--   0        0        0      605 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py
--rw-r--r--   0        0        0      338 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/migrations/0003_delete_translatable.py
--rw-r--r--   0        0        0        0 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a0/formkit_ninja/migrations/__init__.py
--rw-r--r--   0        0        0     9571 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/models.py
--rw-r--r--   0        0        0        0 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a0/formkit_ninja/parser/__init__.py
--rw-r--r--   0        0        0     1674 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/parser/get_tables.py
--rw-r--r--   0        0        0       72 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/parser/logger.py
--rw-r--r--   0        0        0    16186 2023-08-04 07:51:08.403190 formkit_ninja-0.4.0a0/formkit_ninja/parser/type_convert.py
--rw-r--r--   0        0        0      101 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/urls.py
--rw-r--r--   0        0        0     1208 2023-08-04 07:51:40.578409 formkit_ninja-0.4.0a0/pyproject.toml
--rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 formkit_ninja-0.4.0a0/PKG-INFO
+-rw-r--r--   0        0        0      813 2023-08-02 03:08:55.535863 formkit_ninja-0.4.0a1/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 03:08:55.547864 formkit_ninja-0.4.0a1/formkit_ninja/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 03:08:55.535863 formkit_ninja-0.4.0a1/formkit_ninja/__main__.py
+-rw-r--r--   0        0        0    14803 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a1/formkit_ninja/admin.py
+-rw-r--r--   0        0        0     2568 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a1/formkit_ninja/api.py
+-rw-r--r--   0        0        0     4333 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a1/formkit_ninja/fields.py
+-rw-r--r--   0        0        0    14920 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a1/formkit_ninja/formkit_schema.py
+-rw-r--r--   0        0        0        0 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a1/formkit_ninja/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a1/formkit_ninja/management/commands/__init__.py
+-rw-r--r--   0        0        0     3807 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a1/formkit_ninja/management/commands/common_nodes.py
+-rw-r--r--   0        0        0    19033 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a1/formkit_ninja/management/commands/create_sf11_form.py
+-rw-r--r--   0        0        0     3190 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a1/formkit_ninja/management/commands/create_sf12_form.py
+-rw-r--r--   0        0        0     1359 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a1/formkit_ninja/management/commands/create_sf13_form.py
+-rw-r--r--   0        0        0    15058 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a1/formkit_ninja/migrations/0001_initial.py
+-rw-r--r--   0        0        0      605 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a1/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py
+-rw-r--r--   0        0        0      338 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a1/formkit_ninja/migrations/0003_delete_translatable.py
+-rw-r--r--   0        0        0        0 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a1/formkit_ninja/migrations/__init__.py
+-rw-r--r--   0        0        0     9571 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a1/formkit_ninja/models.py
+-rw-r--r--   0        0        0        0 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a1/formkit_ninja/parser/__init__.py
+-rw-r--r--   0        0        0     1674 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a1/formkit_ninja/parser/get_tables.py
+-rw-r--r--   0        0        0       72 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a1/formkit_ninja/parser/logger.py
+-rw-r--r--   0        0        0    16171 2023-08-07 01:35:31.690858 formkit_ninja-0.4.0a1/formkit_ninja/parser/type_convert.py
+-rw-r--r--   0        0        0      101 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a1/formkit_ninja/urls.py
+-rw-r--r--   0        0        0     1208 2023-08-07 01:36:19.791587 formkit_ninja-0.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 formkit_ninja-0.4.0a1/PKG-INFO
```

### Comparing `formkit_ninja-0.4.0a0/README.md` & `formkit_ninja-0.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.4.0a0/formkit_ninja/admin.py` & `formkit_ninja-0.4.0a1/formkit_ninja/admin.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.4.0a0/formkit_ninja/api.py` & `formkit_ninja-0.4.0a1/formkit_ninja/api.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.4.0a0/formkit_ninja/fields.py` & `formkit_ninja-0.4.0a1/formkit_ninja/fields.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.4.0a0/formkit_ninja/formkit_schema.py` & `formkit_ninja-0.4.0a1/formkit_ninja/formkit_schema.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.4.0a0/formkit_ninja/management/commands/common_nodes.py` & `formkit_ninja-0.4.0a1/formkit_ninja/management/commands/common_nodes.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.4.0a0/formkit_ninja/management/commands/create_sf11_form.py` & `formkit_ninja-0.4.0a1/formkit_ninja/management/commands/create_sf11_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.4.0a0/formkit_ninja/management/commands/create_sf12_form.py` & `formkit_ninja-0.4.0a1/formkit_ninja/management/commands/create_sf12_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.4.0a0/formkit_ninja/management/commands/create_sf13_form.py` & `formkit_ninja-0.4.0a1/formkit_ninja/management/commands/create_sf13_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.4.0a0/formkit_ninja/migrations/0001_initial.py` & `formkit_ninja-0.4.0a1/formkit_ninja/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.4.0a0/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py` & `formkit_ninja-0.4.0a1/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.4.0a0/formkit_ninja/models.py` & `formkit_ninja-0.4.0a1/formkit_ninja/models.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.4.0a0/formkit_ninja/parser/get_tables.py` & `formkit_ninja-0.4.0a1/formkit_ninja/parser/get_tables.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.4.0a0/formkit_ninja/parser/type_convert.py` & `formkit_ninja-0.4.0a1/formkit_ninja/parser/type_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from keyword import iskeyword
-from typing import Any, Iterable, Literal
+from typing import Iterable, Literal
 
 from formkit_ninja.formkit_schema import FormKitSchemaFormKit, FormKitSchemaProps, GroupNode, RepeaterNode
 from formkit_ninja.parser.logger import log
 
 
 class NodePath:
     """
@@ -113,14 +113,18 @@
         else:
             return None
 
     @property
     def is_child(self):
         return self.parent is not None
 
+    @property
+    def depth(self):
+        return len(self.nodes)
+
     def tail(self):
         return NodePath(self.node)
 
     def __str__(self):
         return f"NodePath {len(self.nodes)}: {self.node}"
 
 
@@ -282,15 +286,15 @@
         # if a Repeater node, we want to preserve insertion order
         if self.nodes.is_repeater:
             has_attributes = True
             parent_class_name = (self.nodes / "..").suggest_class_name()
             related_name = (
                 self.nodes.node.name
             )  # This is the property name in JSON. It's important to have for importers to know where to put nested data.
-            yield f"    # This class is a Repeater: Parent and ordinality fields have been added"
+            yield "    # This class is a Repeater: Parent and ordinality fields have been added"
             yield f'    parent = models.ForeignKey("{parent_class_name}", on_delete=models.CASCADE, related_name="{related_name}")'
             yield "    ordinality = models.IntegerField()"
 
         if self.extra_attribs:
             has_attributes = True
             for e_a in self.extra_attribs:
                 if isinstance(e_a, str):
@@ -337,14 +341,17 @@
         klassname="BaseModel",  # Allows us to use a Django-Ninja schema or a subclass of models.Model
     ):
         self.nodes = nodes
         self.extra_attribs = extra_attribs
         self.config = config or ParserConfig
         self.klassname = klassname
 
+    def get_extra_attribs(self):
+        return self.extra_attribs
+
     def __iter__(self) -> Iterable[str]:
         """
         Returns a string generator to generate a complete
         set of Pydantic classes
         """
         # Recursively write dependencies
         for n in self.nodes.repeaters:
@@ -471,9 +478,7 @@
         yield "class ReadOnlyInline(admin.TabularInline):\n"
         yield "    def has_change_permission(self, request, obj=None):\n"
         yield "        return False\n"
         yield "    def has_add_permission(self, request, obj=None):\n"
         yield "        return False\n"
         yield "    def has_delete_permission(self, request, obj=None):\n"
         yield "        return False\n"
-        yield "    def get_readonly_fields(self, request, obj=None):\n"
-        yield "        return list(super().get_fields(request, obj))\n"
```

### Comparing `formkit_ninja-0.4.0a0/pyproject.toml` & `formkit_ninja-0.4.0a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "formkit-ninja"
-version = "0.4.0a0"
+version = "0.4.0a1"
 description = "A Django-Ninja backend to specify FormKit schemas"
 authors = ["Josh Brooks <josh@catalpa.io>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/catalpainternational/formkit-ninja"
 repository = "https://github.com/catalpainternational/formkit-ninja"
 packages = [{include = "formkit_ninja"}]
```

### Comparing `formkit_ninja-0.4.0a0/PKG-INFO` & `formkit_ninja-0.4.0a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formkit-ninja
-Version: 0.4.0a0
+Version: 0.4.0a1
 Summary: A Django-Ninja backend to specify FormKit schemas
 Home-page: https://github.com/catalpainternational/formkit-ninja
 License: GPLv3
 Author: Josh Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

