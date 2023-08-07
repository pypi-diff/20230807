# Comparing `tmp/swaggerspect-0.0.4.tar.gz` & `tmp/swaggerspect-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swaggerspect-0.0.4.tar", last modified: Thu Jun 22 10:57:23 2023, max compression
+gzip compressed data, was "dist/swaggerspect-0.0.7.tar", last modified: Mon Aug  7 07:22:05 2023, max compression
```

## Comparing `swaggerspect-0.0.4.tar` & `swaggerspect-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      513 2023-06-22 10:56:43.000000 swaggerspect-0.0.4/setup.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1077 2023-06-07 16:00:04.000000 swaggerspect-0.0.4/LICENSE
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/setup.cfg
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/swaggerspect/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)    11895 2023-06-22 10:56:14.000000 swaggerspect-0.0.4/swaggerspect/__init__.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-06-15 12:42:58.000000 swaggerspect-0.0.4/swaggerspect/test.py
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/swaggerspect.egg-info/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/swaggerspect.egg-info/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/swaggerspect.egg-info/dependency_links.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       13 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/swaggerspect.egg-info/top_level.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        9 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/swaggerspect.egg-info/requires.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      251 2023-06-22 10:57:23.000000 swaggerspect-0.0.4/swaggerspect.egg-info/SOURCES.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     2037 2023-06-16 07:24:49.000000 swaggerspect-0.0.4/README.md
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-08-07 07:22:05.000000 swaggerspect-0.0.7/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      534 2023-08-07 07:21:08.000000 swaggerspect-0.0.7/setup.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-08-07 07:22:05.000000 swaggerspect-0.0.7/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1077 2023-06-07 16:00:04.000000 swaggerspect-0.0.7/LICENSE
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2023-08-07 07:22:05.000000 swaggerspect-0.0.7/setup.cfg
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-08-07 07:22:05.000000 swaggerspect-0.0.7/swaggerspect/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)    14034 2023-07-04 15:07:50.000000 swaggerspect-0.0.7/swaggerspect/__init__.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      877 2023-06-28 09:14:49.000000 swaggerspect-0.0.7/swaggerspect/validate.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-06-15 12:42:58.000000 swaggerspect-0.0.7/swaggerspect/test.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-08-07 07:22:05.000000 swaggerspect-0.0.7/swaggerspect.egg-info/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      364 2023-08-07 07:22:05.000000 swaggerspect-0.0.7/swaggerspect.egg-info/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2023-08-07 07:22:05.000000 swaggerspect-0.0.7/swaggerspect.egg-info/dependency_links.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       13 2023-08-07 07:22:05.000000 swaggerspect-0.0.7/swaggerspect.egg-info/top_level.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       20 2023-08-07 07:22:05.000000 swaggerspect-0.0.7/swaggerspect.egg-info/requires.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      276 2023-08-07 07:22:05.000000 swaggerspect-0.0.7/swaggerspect.egg-info/SOURCES.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     2231 2023-06-27 14:46:39.000000 swaggerspect-0.0.7/README.md
```

### Comparing `swaggerspect-0.0.4/setup.py` & `swaggerspect-0.0.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python
 
 import setuptools
 
 setuptools.setup(
     name='swaggerspect',
-    version='0.0.4',
+    version='0.0.7',
     description='',
     long_description="""Introspects python classes and functions and generates swagger style documentation objects.""",
     long_description_content_type="text/markdown",
     author='Egil Moeller',
     author_email='em@emrld.no',
     url='https://github.com/emerald-geomodelling/swaggerspect',
     packages=setuptools.find_packages(),
     install_requires=[
         "numpydoc",
+        "jsonschema"
     ],
 )
```

### Comparing `swaggerspect-0.0.4/LICENSE` & `swaggerspect-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `swaggerspect-0.0.4/swaggerspect/__init__.py` & `swaggerspect-0.0.7/swaggerspect/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import inspect
 import numpydoc.docscrape
 import ast
 import typing
 import types
 import importlib.metadata
+import copy
 
 def _get_name(obj):
     if obj is None: return None
     if obj is typing.Any: return 'typing.Any'
     return obj.__module__ + "." + obj.__name__
 
 typemap = {
@@ -29,15 +30,15 @@
 }
 
 def typeof(v):
     if v is None: return None
     if v is inspect._empty: return None
     return type(v)
 
-def make_type_schema(*typenames, hasdefault=False):
+def make_type_schema(*typenames, hasdefault=None):
     for typename in typenames:
         if typename is inspect._empty:
             continue
         if typename is None:
             continue
 
         orig = repr(typename)
@@ -72,20 +73,27 @@
             if schema["type"] == "array" and args:
                 schema["items"] = make_type_schema(args[0])
             elif schema["type"] == "object" and args:
                 schema["propertyNames"] = make_type_schema(args[0])
                 schema["patternProperties"] = make_type_schema(args[1])
 
         if metadatas:
-           for metadata in metadatas:
-               schema.update({key[len("swaggerspect_"):]: getattr(metadata, key)
-                              for key in dir(metadata) if key.startswith("swaggerspect_")})
-               if hasattr(metadata, "json_schema"):
-                   schema.update(metadata.json_schema)
-            
+            for metadata in metadatas:
+                if isinstance(metadata, dict):
+                    schema.update({key[len("swaggerspect_"):]: value
+                                   for key, value in metadata.items()
+                                   if key.startswith("swaggerspect_")})
+                    if "json_schema" in metadata:
+                        schema.update(metadata["json_schema"])
+                else:
+                    schema.update({key[len("swaggerspect_"):]: getattr(metadata, key)
+                                   for key in dir(metadata)
+                                   if key.startswith("swaggerspect_")})
+                    if hasattr(metadata, "json_schema"):
+                        schema.update(metadata.json_schema)
         return schema
     return {}
 
 def make_value_schema(*values):
     for value in values:
         if value is inspect._empty:
             continue
@@ -282,18 +290,67 @@
                           if not name.startswith("__")},
                          local_names=True)
     docs["info"] = {"title": _get_name(cls),
                     "version": "1.0",
                     "description": inspect.getdoc(cls) or cls.__name__}
     return docs
 
-def get_apis(objs):
-    """Generates a swagger specification for module or entry point group."""
-    return merge(merge(get_apis_module(objs), get_apis_entrypoints(objs)), get_apis_class(objs))
+def _group_parameters(parameters):
+    grouped = []
+    grouped_by_name = {}
+    for param in parameters:
+        if "__" not in param["name"]:
+            grouped.append(param)
+            grouped_by_name[param["name"]] = param
+        else:
+            param = dict(param)
+            path = param["name"].split("__")
+            if path[0] not in grouped_by_name:
+                grouped_by_name[path[0]] = {
+                    "in": param["in"],
+                    "name": path[0],
+                    "schema": {
+                        "type": "object",
+                        "properties": {},
+                        "x-python-type": None
+                    }
+                }
+                grouped.append(grouped_by_name[path[0]])
+            
+            g = grouped_by_name[path[0]]["schema"]
+            for item in path[1:-1]:
+                if item not in g["properties"]:
+                    g["properties"][item] = {
+                        "type": "object",
+                        "properties": {},
+                        "x-python-type": None
+                    }
+                g = g["properties"][item]
+            
+            g["properties"][path[-1]] = param["schema"]
+    return grouped
 
+def group_apis_parameters(apis):
+    apis = copy.deepcopy(apis)
+    for path, methods in apis["paths"].items():
+        for method, api in methods.items():
+            api["parameters"] = _group_parameters(api["parameters"])
+    return apis
+
+
+def get_apis(objs, group_parameters = False):
+    """Generates a swagger specification for module or entry point group.
+    If group_parameters is True, then parameter names are treated as
+    "__" separated paths in a tree of dictionaries.
+    """
+    res = merge(merge(get_apis_module(objs), get_apis_entrypoints(objs)), get_apis_class(objs))
+    if merge:
+        res = group_apis_parameters(res)
+    return res
+    
 def swagger_to_json_schema(api, multi = True):
     """Converts a swagger specification into a JSON schema for either
     a single function call serialized as
 
     {"function.name": {"argname1": "value1", ... "argnameN": "valueN"}}
 
     or if multi is True (the default), a list of function calls each
```

### Comparing `swaggerspect-0.0.4/README.md` & `swaggerspect-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,10 +25,17 @@
 The same, but as a JSON schema for a single finction call, or a list of calls (`multi=True`):
 ```
 print(yaml.dump(swaggerspect.swagger_to_json_schema(swaggerspect.get_apis("my.entrypoint.group"), multi=False)))
 ```
 
 # Notes and caveats:
 
-* The API parameters for a class, are its properties, not the parameters to `__init__()`.
-* Parameters of unknown types / types with no equivalent in JSON, that have default values, are hidden/ignored.
-* A more elaborate schema for a parameter can be specified using typing.Annotated with an annotation that has a property `json_schema` containing a literal JSON Schema fragment.
+* The API parameters for a class, are its properties, not the
+  parameters to `__init__()`.
+* Parameters of unknown types / types with no equivalent in JSON, that
+  have default values, are hidden/ignored.
+* A more elaborate schema for a parameter can be specified using
+  typing.Annotated with an annotation that has a property
+  `json_schema` containing a literal JSON Schema fragment.
+* Parameters of a class can be grouped into dictionaries in the
+  schema, by sharing a common prefix (separated by `__`), and seting
+  `group_parameters=True` in the call to `get_apis`.
```

