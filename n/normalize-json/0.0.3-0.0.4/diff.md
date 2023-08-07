# Comparing `tmp/normalize_json-0.0.3.tar.gz` & `tmp/normalize_json-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "normalize_json-0.0.3.tar", last modified: Mon Aug  7 03:51:49 2023, max compression
+gzip compressed data, was "normalize_json-0.0.4.tar", last modified: Mon Aug  7 19:50:11 2023, max compression
```

## Comparing `normalize_json-0.0.3.tar` & `normalize_json-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 03:51:49.489013 normalize_json-0.0.3/
--rw-r--r--   0 mega      (1000) mega      (1000)     1083 2023-08-04 22:32:02.000000 normalize_json-0.0.3/LICENSE
--rw-r--r--   0 mega      (1000) mega      (1000)     4547 2023-08-07 03:51:49.489013 normalize_json-0.0.3/PKG-INFO
--rw-r--r--   0 mega      (1000) mega      (1000)     4114 2023-08-07 01:23:20.000000 normalize_json-0.0.3/README.md
--rw-r--r--   0 mega      (1000) mega      (1000)      506 2023-08-07 03:51:32.000000 normalize_json-0.0.3/pyproject.toml
--rw-r--r--   0 mega      (1000) mega      (1000)       38 2023-08-07 03:51:49.489013 normalize_json-0.0.3/setup.cfg
-drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 03:51:49.489013 normalize_json-0.0.3/src/
-drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 03:51:49.489013 normalize_json-0.0.3/src/normalize_json/
--rw-r--r--   0 mega      (1000) mega      (1000)       25 2023-08-04 23:11:44.000000 normalize_json-0.0.3/src/normalize_json/__init__.py
--rw-r--r--   0 mega      (1000) mega      (1000)     1410 2023-08-05 00:11:28.000000 normalize_json-0.0.3/src/normalize_json/cli.py
--rw-r--r--   0 mega      (1000) mega      (1000)     6698 2023-08-07 03:25:13.000000 normalize_json-0.0.3/src/normalize_json/normalize.py
-drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 03:51:49.489013 normalize_json-0.0.3/src/normalize_json.egg-info/
--rw-r--r--   0 mega      (1000) mega      (1000)     4547 2023-08-07 03:51:49.000000 normalize_json-0.0.3/src/normalize_json.egg-info/PKG-INFO
--rw-r--r--   0 mega      (1000) mega      (1000)      289 2023-08-07 03:51:49.000000 normalize_json-0.0.3/src/normalize_json.egg-info/SOURCES.txt
--rw-r--r--   0 mega      (1000) mega      (1000)        1 2023-08-07 03:51:49.000000 normalize_json-0.0.3/src/normalize_json.egg-info/dependency_links.txt
--rw-r--r--   0 mega      (1000) mega      (1000)       15 2023-08-07 03:51:49.000000 normalize_json-0.0.3/src/normalize_json.egg-info/top_level.txt
+drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 19:50:11.711550 normalize_json-0.0.4/
+-rw-r--r--   0 mega      (1000) mega      (1000)     1083 2023-08-04 22:32:02.000000 normalize_json-0.0.4/LICENSE
+-rw-r--r--   0 mega      (1000) mega      (1000)     4593 2023-08-07 19:50:11.711550 normalize_json-0.0.4/PKG-INFO
+-rw-r--r--   0 mega      (1000) mega      (1000)     4160 2023-08-07 04:06:44.000000 normalize_json-0.0.4/README.md
+-rw-r--r--   0 mega      (1000) mega      (1000)      506 2023-08-07 19:48:44.000000 normalize_json-0.0.4/pyproject.toml
+-rw-r--r--   0 mega      (1000) mega      (1000)       38 2023-08-07 19:50:11.711550 normalize_json-0.0.4/setup.cfg
+drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 19:50:11.711550 normalize_json-0.0.4/src/
+drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 19:50:11.711550 normalize_json-0.0.4/src/normalize_json/
+-rw-r--r--   0 mega      (1000) mega      (1000)       25 2023-08-04 23:11:44.000000 normalize_json-0.0.4/src/normalize_json/__init__.py
+-rw-r--r--   0 mega      (1000) mega      (1000)     1410 2023-08-05 00:11:28.000000 normalize_json-0.0.4/src/normalize_json/cli.py
+-rw-r--r--   0 mega      (1000) mega      (1000)     6845 2023-08-07 19:48:26.000000 normalize_json-0.0.4/src/normalize_json/normalize.py
+drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 19:50:11.711550 normalize_json-0.0.4/src/normalize_json.egg-info/
+-rw-r--r--   0 mega      (1000) mega      (1000)     4593 2023-08-07 19:50:11.000000 normalize_json-0.0.4/src/normalize_json.egg-info/PKG-INFO
+-rw-r--r--   0 mega      (1000) mega      (1000)      289 2023-08-07 19:50:11.000000 normalize_json-0.0.4/src/normalize_json.egg-info/SOURCES.txt
+-rw-r--r--   0 mega      (1000) mega      (1000)        1 2023-08-07 19:50:11.000000 normalize_json-0.0.4/src/normalize_json.egg-info/dependency_links.txt
+-rw-r--r--   0 mega      (1000) mega      (1000)       15 2023-08-07 19:50:11.000000 normalize_json-0.0.4/src/normalize_json.egg-info/top_level.txt
```

### Comparing `normalize_json-0.0.3/LICENSE` & `normalize_json-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `normalize_json-0.0.3/PKG-INFO` & `normalize_json-0.0.4/src/normalize_json.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: normalize_json
-Version: 0.0.3
+Name: normalize-json
+Version: 0.0.4
 Summary: todo
 Author-email: João Gabriel Santos <joaosan177@gmail.com>
 Project-URL: Homepage, https://github.com/capsulbrasil/normalize-json
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -194,14 +194,15 @@
 - `enforce`: cast values to expected type instead of raising a TypeError
 
 ### Attributes
 
 - `array`: whether the expected value is an array or not
 - `trim_start`: trim `n` characters from the beginning of the string
 - `trim_end`: trim `n` characters from the end of the string
+- `pick_until`: same as `value.split(str)[0]`
 
 ## Support and contributing
 
 You can obtain suport if you're using this library on production. Just email the author at joaosan177[at]gmail.com. You may also send PRs, just make sure to include tests and follow PEP guidelines.
 
 ### Run typechecking
```

### Comparing `normalize_json-0.0.3/README.md` & `normalize_json-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,15 @@
 - `enforce`: cast values to expected type instead of raising a TypeError
 
 ### Attributes
 
 - `array`: whether the expected value is an array or not
 - `trim_start`: trim `n` characters from the beginning of the string
 - `trim_end`: trim `n` characters from the end of the string
+- `pick_until`: same as `value.split(str)[0]`
 
 ## Support and contributing
 
 You can obtain suport if you're using this library on production. Just email the author at joaosan177[at]gmail.com. You may also send PRs, just make sure to include tests and follow PEP guidelines.
 
 ### Run typechecking
```

### Comparing `normalize_json-0.0.3/src/normalize_json/cli.py` & `normalize_json-0.0.4/src/normalize_json/cli.py`

 * *Files identical despite different names*

### Comparing `normalize_json-0.0.3/src/normalize_json/normalize.py` & `normalize_json-0.0.4/src/normalize_json/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     'map': typing.NotRequired[str | list[str]],
     'type': AcceptedType,
     'array': typing.NotRequired[bool],
     'default': typing.NotRequired[typing.Any],
     'modifiers': typing.NotRequired[list[Modifier]],
     'trim_start': typing.NotRequired[int],
     'trim_end': typing.NotRequired[int],
+    'pick_until': typing.NotRequired[str],
     '__fields': typing.NotRequired[dict[str, 'Node']]
 })
 
 Mapping = typing.TypedDict('Mapping', {
     'modifiers': typing.NotRequired[list[Modifier]],
     '__fields': typing.NotRequired[dict[str, 'Node']]
 })
@@ -57,15 +58,16 @@
 
 RawObject = dict[str, typing.Any]
 
 def unserialize(raw: RawObject | str | bytes, mime: AcceptedMime = 'application/json'):
     match mime:
         case 'application/json':
             if isinstance(raw, dict): return raw
-            if isinstance(raw, bytes): return json.loads(raw)
+            if isinstance(raw, str): return raw
+            else: return json.loads(raw)
 
     raise TypeError('invalid mime')
 
 def flatten(target: RawObject, separator: str = '.', preserve_arrays: bool = False):
     ret: RawObject = {}
 
     def internal_flatten(obj: typing.Any, parent: str = '') -> typing.Any:
@@ -112,14 +114,17 @@
 
     if trim := node.get('trim_start'):
         value = value[trim:]
 
     if trim := node.get('trim_end'):
         value = value[:trim]
 
+    if pick := node.get('pick_until'):
+        value = value.split(pick)[0]
+
     if 'enforce' in modifiers:
         match node['type']:
             case 'number': value = float(value)
             case 'integer': value = int(value)
             case 'string': value = str(value)
             case 'datetime': value = dateparser.parse(value)
             case _: ...
```

### Comparing `normalize_json-0.0.3/src/normalize_json.egg-info/PKG-INFO` & `normalize_json-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: normalize-json
-Version: 0.0.3
+Name: normalize_json
+Version: 0.0.4
 Summary: todo
 Author-email: João Gabriel Santos <joaosan177@gmail.com>
 Project-URL: Homepage, https://github.com/capsulbrasil/normalize-json
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -194,14 +194,15 @@
 - `enforce`: cast values to expected type instead of raising a TypeError
 
 ### Attributes
 
 - `array`: whether the expected value is an array or not
 - `trim_start`: trim `n` characters from the beginning of the string
 - `trim_end`: trim `n` characters from the end of the string
+- `pick_until`: same as `value.split(str)[0]`
 
 ## Support and contributing
 
 You can obtain suport if you're using this library on production. Just email the author at joaosan177[at]gmail.com. You may also send PRs, just make sure to include tests and follow PEP guidelines.
 
 ### Run typechecking
```

