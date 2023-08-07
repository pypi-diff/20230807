# Comparing `tmp/arclet-alconna-tools-0.6.3.tar.gz` & `tmp/arclet-alconna-tools-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-tools-0.6.3.tar", last modified: Mon Jul  3 11:37:46 2023, max compression
+gzip compressed data, was "arclet-alconna-tools-0.6.4.tar", last modified: Mon Aug  7 10:52:27 2023, max compression
```

## Comparing `arclet-alconna-tools-0.6.3.tar` & `arclet-alconna-tools-0.6.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 arclet-alconna-tools-0.6.3/LICENSE
--rw-r--r--   0        0        0     1076 2023-07-03 11:26:40.570640 arclet-alconna-tools-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      749 2023-05-10 16:28:11.249182 arclet-alconna-tools-0.6.3/README.md
--rw-r--r--   0        0        0      387 2023-05-10 14:13:40.054086 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/__init__.py
--rw-r--r--   0        0        0     2355 2023-05-08 11:53:03.567259 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/actions.py
--rw-r--r--   0        0        0      866 2023-07-03 07:06:39.010899 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/checker.py
--rw-r--r--   0        0        0       96 2023-05-08 11:53:03.585160 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/config.py
--rw-r--r--   0        0        0    32583 2023-07-03 11:37:30.519633 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/construct.py
--rw-r--r--   0        0        0     3879 2023-05-07 05:15:13.335037 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/debug.py
--rw-r--r--   0        0        0    17620 2023-05-10 14:36:13.901208 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/formatter.py
--rw-r--r--   0        0        0       26 2023-05-08 11:44:10.335552 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/i18n/.config.json
--rw-r--r--   0        0        0      692 2023-05-08 16:08:05.985424 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/i18n/en-US.json
--rw-r--r--   0        0        0      661 2023-05-08 16:18:05.842731 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/i18n/zh-CN.json
--rw-r--r--   0        0        0     4453 2023-05-07 05:35:56.817434 arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/pattern.py
--rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 arclet-alconna-tools-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 arclet-alconna-tools-0.6.4/LICENSE
+-rw-r--r--   0        0        0     1082 2023-08-07 09:41:35.358501 arclet-alconna-tools-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      749 2023-05-10 16:28:11.249182 arclet-alconna-tools-0.6.4/README.md
+-rw-r--r--   0        0        0      387 2023-05-10 14:13:40.054086 arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/__init__.py
+-rw-r--r--   0        0        0     2355 2023-05-08 11:53:03.567259 arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/actions.py
+-rw-r--r--   0        0        0      866 2023-07-03 07:06:39.010899 arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/checker.py
+-rw-r--r--   0        0        0       96 2023-05-08 11:53:03.585160 arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/config.py
+-rw-r--r--   0        0        0    32257 2023-08-07 09:49:12.012837 arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/construct.py
+-rw-r--r--   0        0        0     3879 2023-05-07 05:15:13.335037 arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/debug.py
+-rw-r--r--   0        0        0    17620 2023-05-10 14:36:13.901208 arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/formatter.py
+-rw-r--r--   0        0        0       26 2023-05-08 11:44:10.335552 arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/i18n/.config.json
+-rw-r--r--   0        0        0      692 2023-05-08 16:08:05.985424 arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/i18n/en-US.json
+-rw-r--r--   0        0        0      661 2023-05-08 16:18:05.842731 arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/i18n/zh-CN.json
+-rw-r--r--   0        0        0     4453 2023-05-07 05:35:56.817434 arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/pattern.py
+-rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 arclet-alconna-tools-0.6.4/PKG-INFO
```

### Comparing `arclet-alconna-tools-0.6.3/LICENSE` & `arclet-alconna-tools-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.3/pyproject.toml` & `arclet-alconna-tools-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "arclet-alconna-tools"
-version = "0.6.3"
+version = "0.6.4"
 description = "Builtin Tools for Alconna"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nepattern<0.6.0, >=0.5.8",
-    "arclet-alconna>=1.7.10",
+    "arclet-alconna<2.0, >=1.7.14",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `arclet-alconna-tools-0.6.3/README.md` & `arclet-alconna-tools-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/actions.py` & `arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/actions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/checker.py` & `arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/checker.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/construct.py` & `arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/construct.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,15 +465,15 @@
                 Option(name, default=default, action=action)
             )
             return self
         parts = split(opt, (" ",))
         aliases = []
         index = 0
         for part in parts:
-            if not part.startswith("-"):
+            if part.startswith("<") or part.startswith("["):
                 break
             aliases.append(part)
             index += 1
         _args = Args()
         if parts[index:]:
             custom_types = getattr(inspect.getmodule(inspect.stack()[1][0]), "__dict__", {})
             _args = args_from_list(self.args_gen(" ".join(parts[index:])), custom_types.copy())
@@ -616,16 +616,14 @@
             main_args,
             *_options,
             help_text=config.get("description", main_help_text),
         )
 
 
 class FuncMounter(Alconna[TDC], Generic[T, TDC]):
-    target: Callable[..., T]
-
     def __init__(
         self, func: Callable[..., T], config: Optional[MountConfig] = None
     ):
         config = visit_config(func, config)
         func_name = func.__name__
         if func_name.startswith("_"):
             raise ValueError(lang.require("tools", "construct.func_name_error"))
@@ -639,28 +637,19 @@
             _args,
             meta=CommandMeta(
                 description=config.get("description", func.__doc__ or func_name),
                 raise_exception=config.get("raise_exception", True),
             ),
             namespace=config.get("namespace", None),
         )
-        self.target = func
         self.bind()(func)
 
-    def exec(self, message: TDC) -> Tuple[Arparma[TDC], Optional[T]]:
-        try:
-            arp = self._parse(message)
-        except NullMessage as e:
-            if self.meta.raise_exception:
-                raise e
-            return Arparma(self.path, message, False, error_info=e), None
-        if arp.matched:
-            arp = arp.execute(self.behaviors)
-            return arp, arp.call(self.target)
-        return arp, None
+    @property
+    def exec_result(self) -> dict[str, T]:
+        return {ext.target.__name__: res for ext, res in self._executors.items() if res is not None}
 
 class ModuleMounter(Alconna):
     def __init__(self, module: ModuleType, config: Optional[MountConfig] = None):
         self.mount_cls = module.__class__
         self.instance = module
         config = config or visit_config(module, config)
         _options = []
```

### Comparing `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/debug.py` & `arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/debug.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/formatter.py` & `arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/formatter.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/i18n/en-US.json` & `arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/i18n/zh-CN.json` & `arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.3/src/arclet/alconna/tools/pattern.py` & `arclet-alconna-tools-0.6.4/src/arclet/alconna/tools/pattern.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.3/PKG-INFO` & `arclet-alconna-tools-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-tools
-Version: 0.6.3
+Version: 0.6.4
 Summary: Builtin Tools for Alconna
 License: MIT
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Alconna Tools
```

