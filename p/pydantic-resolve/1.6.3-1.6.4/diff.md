# Comparing `tmp/pydantic_resolve-1.6.3.tar.gz` & `tmp/pydantic_resolve-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.6.3.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.6.4.tar", max compression
```

## Comparing `pydantic_resolve-1.6.3.tar` & `pydantic_resolve-1.6.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.6.3/LICENSE
--rw-r--r--   0        0        0      593 2023-07-12 08:04:20.448957 pydantic_resolve-1.6.3/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0      362 2023-07-19 12:50:41.795062 pydantic_resolve-1.6.3/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     2094 2023-07-19 09:08:47.652925 pydantic_resolve-1.6.3/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.6.3/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     8700 2023-07-20 15:32:02.047585 pydantic_resolve-1.6.3/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     8446 2023-07-20 15:40:08.283768 pydantic_resolve-1.6.3/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-07-20 15:41:19.280695 pydantic_resolve-1.6.3/pyproject.toml
--rw-r--r--   0        0        0    11394 2023-07-15 15:05:51.080033 pydantic_resolve-1.6.3/README.md
--rw-r--r--   0        0        0    11791 1970-01-01 00:00:00.000000 pydantic_resolve-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.6.4/LICENSE
+-rw-r--r--   0        0        0      593 2023-07-12 08:04:20.448957 pydantic_resolve-1.6.4/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0      362 2023-07-19 12:50:41.795062 pydantic_resolve-1.6.4/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     2094 2023-07-19 09:08:47.652925 pydantic_resolve-1.6.4/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.6.4/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     8278 2023-08-07 12:13:15.949926 pydantic_resolve-1.6.4/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     8446 2023-07-27 14:20:52.399501 pydantic_resolve-1.6.4/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      795 2023-08-07 13:15:39.878737 pydantic_resolve-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0    11394 2023-07-15 15:05:51.080033 pydantic_resolve-1.6.4/README.md
+-rw-r--r--   0        0        0    11772 1970-01-01 00:00:00.000000 pydantic_resolve-1.6.4/PKG-INFO
```

### Comparing `pydantic_resolve-1.6.3/LICENSE` & `pydantic_resolve-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.6.3/pydantic_resolve/__init__.py` & `pydantic_resolve-1.6.4/pydantic_resolve/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.6.3/pydantic_resolve/core.py` & `pydantic_resolve-1.6.4/pydantic_resolve/core.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.6.3/pydantic_resolve/resolver.py` & `pydantic_resolve-1.6.4/pydantic_resolve/resolver.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,18 +37,18 @@
             self, 
             loader_filters: Optional[Dict[Any, Dict[str, Any]]] = None, 
             loader_instances: Optional[Dict[Any, Any]] = None,
             annotation_class: Optional[Type] = None,
             ensure_type=False,
             context: Optional[Dict[str, Any]] = None
             ):
-        self.ctx = contextvars.ContextVar('pydantic_resolve_internal_context', default={})
+        self.ctx = {}
 
         # for dataloader which has class attributes, you can assign the value at here
-        self.loader_filters_ctx = contextvars.ContextVar('pydantic_resolve_internal_filter', default=loader_filters or {})
+        self.loader_filters = loader_filters or {}
 
         # now you can pass your loader instance, Resolver will check isinstance
         if loader_instances and self.validate_instance(loader_instances):
             self.loader_instances = loader_instances
         else:
             self.loader_instances = None
 
@@ -84,56 +84,52 @@
 
         # manage the creation of loader instances
         for k, v in signature.parameters.items():
 
             # >>> 2
             if isinstance(v.default, Depends):
                 # Base: DataLoader or batch_load_fn
-                Base = v.default.dependency
+                Loader = v.default.dependency
 
                 # check loader_instance first, if has predefined loader instance, just use it.
-                if self.loader_instances and self.loader_instances.get(Base):
-                    loader = self.loader_instances.get(Base)
+                if self.loader_instances and self.loader_instances.get(Loader):
+                    loader = self.loader_instances.get(Loader)
                     params[k] = loader
                     continue
 
                 # module.kls to avoid same kls name from different module
                 cache_key = f'{v.default.dependency.__module__}.{v.default.dependency.__name__}'
-                cache_provider = self.ctx.get()
-                hit = cache_provider.get(cache_key, None)
+                hit = self.ctx.get(cache_key)
                 if hit:
                     loader = hit
                 else:
                     # >>> 2.1
                     # create loader instance 
-                    if isclass(Base):
+                    if isclass(Loader):
                         # if extra transform provides
-                        loader = Base()
+                        loader = Loader()
 
-                        # and pick config from 'loader_filters' param, only for DataClass
-                        filter_config_provider = self.loader_filters_ctx.get()
-                        filter_config = filter_config_provider.get(Base, {})
+                        filter_config = self.loader_filters.get(Loader, {})
 
+                        for field in util.get_class_field_annotations(Loader):
                         # >>> 2.1.1
                         # class ExampleLoader(DataLoader):
                         #     filtar_x: bool  <--------------- set this field
-                        for field in util.get_class_field_annotations(Base):
                             try:
                                 value = filter_config[field]
                                 setattr(loader, field, value)
                             except KeyError:
                                 raise LoaderFieldNotProvidedError(f'{cache_key}.{field} not found in Resolver()')
 
                     # >>> 2.2
                     # build loader from batch_load_fn, filters config is impossible
                     else:
-                        loader = DataLoader(batch_load_fn=Base) # type:ignore
+                        loader = DataLoader(batch_load_fn=Loader) # type:ignore
 
-                    cache_provider[cache_key] = loader
-                    self.ctx.set(cache_provider)
+                    self.ctx[cache_key] = loader
                 params[k] = loader
         return method(**params)
 
 
     async def _resolve_obj_field(self, target, field, attr):
         """
         resolve object fields
@@ -161,15 +157,15 @@
         # >>> 3
         if not getattr(attr, const.HAS_MAPPER_FUNCTION, False):  # defined in util.mapper
             val = util.try_parse_data_to_target_field_type(target, target_attr_name, val)
 
         val = await self._resolve(val)
 
         # >>> 4
-        target.__setattr__(target_attr_name, val)
+        setattr(target, target_attr_name, val)
 
 
     async def _resolve(self, target: T) -> T:
         """ 
         resolve dataclass object or pydantic object / or list in place 
 
         1. iterate over elements if target is list
@@ -197,15 +193,15 @@
             for post_key in core.iter_over_object_post_methods(target):
                 post_attr_name = post_key.replace(const.POST_PREFIX, '')
                 if not hasattr(target, post_attr_name):
                     raise ResolverTargetAttrNotFound(f"fail to run {post_key}(), attribute {post_attr_name} not found")
 
                 post_method = target.__getattribute__(post_key)
                 calc_result = post_method()
-                target.__setattr__(post_attr_name, calc_result)
+                setattr(target, post_attr_name, calc_result)
             
             # hidden entry for performance. run at last
             default_post_method = getattr(target, const.POST_DEFAULT_HANDLER, None)
             if default_post_method:
                 default_post_method()
 
         return target
```

### Comparing `pydantic_resolve-1.6.3/pydantic_resolve/util.py` & `pydantic_resolve-1.6.4/pydantic_resolve/util.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.6.3/pyproject.toml` & `pydantic_resolve-1.6.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.6.3"
-description = "Make pydantic have a GraphQL-like assembly experience."
+version = "1.6.4"
+description = "create nested data structure easily"
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-1.6.3/README.md` & `pydantic_resolve-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.6.3/PKG-INFO` & `pydantic_resolve-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 1.6.3
-Summary: Make pydantic have a GraphQL-like assembly experience.
+Version: 1.6.4
+Summary: create nested data structure easily
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

