# Comparing `tmp/oapi-1.59.5.tar.gz` & `tmp/oapi-1.60.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oapi-1.59.5.tar", last modified: Thu Jun 29 17:30:14 2023, max compression
+gzip compressed data, was "oapi-1.60.0.tar", last modified: Mon Aug  7 16:59:52 2023, max compression
```

## Comparing `oapi-1.59.5.tar` & `oapi-1.60.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:30:14.015496 oapi-1.59.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-29 17:29:18.000000 oapi-1.59.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-29 17:30:14.015496 oapi-1.59.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-29 17:29:18.000000 oapi-1.59.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:30:14.011496 oapi-1.59.5/oapi/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/_multipart_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)   126802 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    61478 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:30:14.011496 oapi-1.59.5/oapi/oas/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/oas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125708 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/oas/model.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/oas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/oas/references.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:18.000000 oapi-1.59.5/oapi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:30:14.011496 oapi-1.59.5/oapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-29 17:30:13.000000 oapi-1.59.5/oapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-29 17:30:13.000000 oapi-1.59.5/oapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:30:13.000000 oapi-1.59.5/oapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-29 17:30:13.000000 oapi-1.59.5/oapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 17:30:13.000000 oapi-1.59.5/oapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-29 17:29:18.000000 oapi-1.59.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-29 17:30:14.015496 oapi-1.59.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-29 17:29:18.000000 oapi-1.59.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:30:14.011496 oapi-1.59.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-29 17:29:18.000000 oapi-1.59.5/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-29 17:29:18.000000 oapi-1.59.5/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:59:52.925197 oapi-1.60.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-07 16:59:21.000000 oapi-1.60.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-08-07 16:59:52.925197 oapi-1.60.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-08-07 16:59:21.000000 oapi-1.60.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:59:52.921197 oapi-1.60.0/oapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-07 16:59:21.000000 oapi-1.60.0/oapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 16:59:21.000000 oapi-1.60.0/oapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-08-07 16:59:21.000000 oapi-1.60.0/oapi/_multipart_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-08-07 16:59:21.000000 oapi-1.60.0/oapi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127659 2023-08-07 16:59:21.000000 oapi-1.60.0/oapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-07 16:59:21.000000 oapi-1.60.0/oapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61478 2023-08-07 16:59:21.000000 oapi-1.60.0/oapi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:59:52.921197 oapi-1.60.0/oapi/oas/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-07 16:59:21.000000 oapi-1.60.0/oapi/oas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125708 2023-08-07 16:59:21.000000 oapi-1.60.0/oapi/oas/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 16:59:21.000000 oapi-1.60.0/oapi/oas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-08-07 16:59:21.000000 oapi-1.60.0/oapi/oas/references.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 16:59:21.000000 oapi-1.60.0/oapi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:59:52.921197 oapi-1.60.0/oapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-08-07 16:59:52.000000 oapi-1.60.0/oapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-07 16:59:52.000000 oapi-1.60.0/oapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:59:52.000000 oapi-1.60.0/oapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-07 16:59:52.000000 oapi-1.60.0/oapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 16:59:52.000000 oapi-1.60.0/oapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-07 16:59:21.000000 oapi-1.60.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-07 16:59:52.925197 oapi-1.60.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-07 16:59:21.000000 oapi-1.60.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:59:52.925197 oapi-1.60.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-07 16:59:21.000000 oapi-1.60.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-08-07 16:59:21.000000 oapi-1.60.0/tests/test_model.py
```

### Comparing `oapi-1.59.5/LICENSE` & `oapi-1.60.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oapi-1.59.5/PKG-INFO` & `oapi-1.60.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oapi
-Version: 1.59.5
+Version: 1.60.0
 Summary: An SDK for parsing OpenAPI (Swagger) 2.0 - 3.0 specifications
 Home-page: https://github.com/enorganic/oapi
 Author-email: david@belais.me
 License: MIT
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oapi-1.59.5/README.md` & `oapi-1.60.0/README.md`

 * *Files identical despite different names*

### Comparing `oapi-1.59.5/oapi/_multipart_request.py` & `oapi-1.60.0/oapi/_multipart_request.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.5/oapi/_utilities.py` & `oapi-1.60.0/oapi/_utilities.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.5/oapi/client.py` & `oapi-1.60.0/oapi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1907,14 +1907,27 @@
         yield "            },"
 
 
 def _strip_def_decorators(source: str) -> str:
     return re.sub(r"^(\s*)@(?:.|\n)*?(\bdef )", r"\1\2", source)
 
 
+def get_default_method_name_from_path_method_operation(
+    path: str, method: str, operation_id: Optional[str]
+) -> str:
+    method_name: str
+    if operation_id:
+        method_name = sob.utilities.string.property_name(operation_id)
+    else:
+        method_name = (
+            f"{method.lower()}_" f"{sob.utilities.string.property_name(path)}"
+        )
+    return method_name.rstrip("_")
+
+
 class Module:
     """
     This class parses an Open API document and outputs a module defining
     a client class for interfacing with the API described by an OpenAPI
     document.
 
     Initialization Parameters:
@@ -1967,14 +1980,18 @@
         add_init_parameter_docs: Union[str, Tuple[str, ...]] = (),
         init_parameter_defaults: Union[
             Mapping[str, Any], Sequence[Tuple[str, Any]]
         ] = (),
         init_parameter_defaults_source: Union[
             Mapping[str, Any], Sequence[Tuple[str, Any]]
         ] = (),
+        get_method_name_from_path_method_operation: Callable[
+            [str, str, Optional[str]], str
+        ] = get_default_method_name_from_path_method_operation,
+        use_operation_id: bool = False,
     ) -> None:
         # Ensure a valid model path has been provided
         assert os.path.exists(model_path)
         # Get an OpenAPI document
         if isinstance(open_api, str):
             if os.path.exists(open_api):
                 open_api = _get_path_open_api(open_api)
@@ -2042,14 +2059,18 @@
                         "import oapi",
                         "from logging import Logger",
                     )
                     + ((imports,) if isinstance(imports, str) else imports)
                 ),
             )
         )
+        self.get_method_name_from_path_method_operation = (
+            get_method_name_from_path_method_operation
+        )
+        self.use_operation_id = use_operation_id
 
     def _get_open_api_major_version(self) -> int:
         return int(
             (self.open_api.swagger or self.open_api.openapi or "0")
             .split(".")[0]
             .strip()
         )
@@ -3158,17 +3179,19 @@
         method: str,
         operation: Operation,
         path_item: PathItem,
         parameter_locations: _ParameterLocations,
     ) -> Iterable[str]:
         parameter: Parameter
         previous_parameter_required: bool = True
-        method_name: str = (
-            f"{method}_{sob.utilities.string.property_name(path)}"
-        ).rstrip("_")
+        method_name: str = self.get_method_name_from_path_method_operation(
+            path,
+            method,
+            (operation.operation_id if self.use_operation_id else None),
+        )
         yield f"    def {method_name}("
         yield "        self,"
         # Request Body
         request_body: Optional[RequestBody] = None
         parameter_names: Set[str] = set(
             map(
                 sob.utilities.string.property_name,
```

### Comparing `oapi-1.59.5/oapi/model.py` & `oapi-1.60.0/oapi/model.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.5/oapi/oas/model.py` & `oapi-1.60.0/oapi/oas/model.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.5/oapi/oas/references.py` & `oapi-1.60.0/oapi/oas/references.py`

 * *Files identical despite different names*

### Comparing `oapi-1.59.5/oapi.egg-info/PKG-INFO` & `oapi-1.60.0/oapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oapi
-Version: 1.59.5
+Version: 1.60.0
 Summary: An SDK for parsing OpenAPI (Swagger) 2.0 - 3.0 specifications
 Home-page: https://github.com/enorganic/oapi
 Author-email: david@belais.me
 License: MIT
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oapi-1.59.5/setup.cfg` & `oapi-1.60.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oapi
-version = 1.59.5
+version = 1.60.0
 author_email = david@belais.me
 description = An SDK for parsing OpenAPI (Swagger) 2.0 - 3.0 specifications
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 url = https://github.com/enorganic/oapi
```

### Comparing `oapi-1.59.5/tests/test_model.py` & `oapi-1.60.0/tests/test_model.py`

 * *Files identical despite different names*

