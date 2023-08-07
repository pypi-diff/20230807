# Comparing `tmp/pyangbind-0.8.2.tar.gz` & `tmp/pyangbind-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyangbind-0.8.2.tar", last modified: Fri Jul 14 05:46:30 2023, max compression
+gzip compressed data, was "pyangbind-0.8.3.tar", last modified: Mon Aug  7 20:02:31 2023, max compression
```

## Comparing `pyangbind-0.8.2.tar` & `pyangbind-0.8.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-14 05:46:30.948363 pyangbind-0.8.2/
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     1381 2023-07-14 05:46:04.000000 pyangbind-0.8.2/CONTRIBUTING.md
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)      663 2023-07-09 09:56:01.000000 pyangbind-0.8.2/LICENSE
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       43 2023-07-09 09:56:01.000000 pyangbind-0.8.2/MANIFEST.in
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     4084 2023-07-14 05:46:30.949363 pyangbind-0.8.2/PKG-INFO
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    17961 2023-07-09 09:56:01.000000 pyangbind-0.8.2/README.md
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     2947 2023-07-09 09:56:01.000000 pyangbind-0.8.2/README.rst
-drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-14 05:46:30.928353 pyangbind-0.8.2/pyangbind/
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       22 2023-07-14 05:44:13.000000 pyangbind-0.8.2/pyangbind/__init__.py
-drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-14 05:46:30.939358 pyangbind-0.8.2/pyangbind/helpers/
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/helpers/__init__.py
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     5749 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/helpers/identity.py
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     1980 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/helpers/misc.py
-drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-14 05:46:30.944361 pyangbind-0.8.2/pyangbind/lib/
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/lib/__init__.py
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     4260 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/lib/base.py
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     6298 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/lib/pybindJSON.py
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    35984 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/lib/serialise.py
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    13400 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/lib/xpathhelper.py
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    51329 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/lib/yangtypes.py
-drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-14 05:46:30.946362 pyangbind-0.8.2/pyangbind/plugin/
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/plugin/__init__.py
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    74162 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/plugin/pybind.py
-drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-14 05:46:30.936357 pyangbind-0.8.2/pyangbind.egg-info/
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     4084 2023-07-14 05:46:30.000000 pyangbind-0.8.2/pyangbind.egg-info/PKG-INFO
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)      644 2023-07-14 05:46:30.000000 pyangbind-0.8.2/pyangbind.egg-info/SOURCES.txt
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        1 2023-07-14 05:46:30.000000 pyangbind-0.8.2/pyangbind.egg-info/dependency_links.txt
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        1 2023-07-09 12:06:51.000000 pyangbind-0.8.2/pyangbind.egg-info/not-zip-safe
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       37 2023-07-14 05:46:30.000000 pyangbind-0.8.2/pyangbind.egg-info/requires.txt
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       10 2023-07-14 05:46:30.000000 pyangbind-0.8.2/pyangbind.egg-info/top_level.txt
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       99 2023-07-14 05:46:04.000000 pyangbind-0.8.2/pyproject.toml
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)      114 2023-07-14 05:46:04.000000 pyangbind-0.8.2/requirements.DEVELOPER.txt
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       37 2023-07-09 09:56:01.000000 pyangbind-0.8.2/requirements.txt
--rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     1425 2023-07-14 05:46:30.950364 pyangbind-0.8.2/setup.cfg
+drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-08-07 20:02:31.477165 pyangbind-0.8.3/
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     1381 2023-07-19 04:21:04.000000 pyangbind-0.8.3/CONTRIBUTING.md
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)      663 2023-07-09 09:56:01.000000 pyangbind-0.8.3/LICENSE
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       43 2023-07-09 09:56:01.000000 pyangbind-0.8.3/MANIFEST.in
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     4086 2023-08-07 20:02:31.478165 pyangbind-0.8.3/PKG-INFO
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    17961 2023-07-09 09:56:01.000000 pyangbind-0.8.3/README.md
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     2947 2023-07-09 09:56:01.000000 pyangbind-0.8.3/README.rst
+drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-08-07 20:02:31.467165 pyangbind-0.8.3/pyangbind/
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       22 2023-08-07 04:27:39.000000 pyangbind-0.8.3/pyangbind/__init__.py
+drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-08-07 20:02:31.472165 pyangbind-0.8.3/pyangbind/helpers/
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-09 09:56:01.000000 pyangbind-0.8.3/pyangbind/helpers/__init__.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     5747 2023-07-24 18:10:12.000000 pyangbind-0.8.3/pyangbind/helpers/identity.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     2006 2023-08-07 04:27:50.000000 pyangbind-0.8.3/pyangbind/helpers/misc.py
+drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-08-07 20:02:31.475165 pyangbind-0.8.3/pyangbind/lib/
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-09 09:56:01.000000 pyangbind-0.8.3/pyangbind/lib/__init__.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     4257 2023-07-24 18:10:12.000000 pyangbind-0.8.3/pyangbind/lib/base.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     6297 2023-07-24 18:10:12.000000 pyangbind-0.8.3/pyangbind/lib/pybindJSON.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    36100 2023-08-07 04:26:45.000000 pyangbind-0.8.3/pyangbind/lib/serialise.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    13455 2023-07-24 18:10:12.000000 pyangbind-0.8.3/pyangbind/lib/xpathhelper.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    51681 2023-08-07 04:26:45.000000 pyangbind-0.8.3/pyangbind/lib/yangtypes.py
+drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-08-07 20:02:31.476165 pyangbind-0.8.3/pyangbind/plugin/
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-09 09:56:01.000000 pyangbind-0.8.3/pyangbind/plugin/__init__.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    74161 2023-08-07 04:27:50.000000 pyangbind-0.8.3/pyangbind/plugin/pybind.py
+drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-08-07 20:02:31.471165 pyangbind-0.8.3/pyangbind.egg-info/
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     4086 2023-08-07 20:02:31.000000 pyangbind-0.8.3/pyangbind.egg-info/PKG-INFO
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)      644 2023-08-07 20:02:31.000000 pyangbind-0.8.3/pyangbind.egg-info/SOURCES.txt
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        1 2023-08-07 20:02:31.000000 pyangbind-0.8.3/pyangbind.egg-info/dependency_links.txt
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        1 2023-07-09 12:06:51.000000 pyangbind-0.8.3/pyangbind.egg-info/not-zip-safe
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       28 2023-08-07 20:02:31.000000 pyangbind-0.8.3/pyangbind.egg-info/requires.txt
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       10 2023-08-07 20:02:31.000000 pyangbind-0.8.3/pyangbind.egg-info/top_level.txt
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       99 2023-07-19 04:21:04.000000 pyangbind-0.8.3/pyproject.toml
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       47 2023-07-24 18:10:12.000000 pyangbind-0.8.3/requirements.DEVELOPER.txt
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       28 2023-08-07 04:26:45.000000 pyangbind-0.8.3/requirements.txt
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     1427 2023-08-07 20:02:31.479165 pyangbind-0.8.3/setup.cfg
```

### Comparing `pyangbind-0.8.2/CONTRIBUTING.md` & `pyangbind-0.8.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyangbind-0.8.2/LICENSE` & `pyangbind-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyangbind-0.8.2/PKG-INFO` & `pyangbind-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pyangbind
-Version: 0.8.2
+Version: 0.8.3
 Summary: PyangBind is a plugin for pyang which converts YANG data models into a Python class hierarchy, such that Python can be used to manipulate data that conforms with a YANG model.
 Home-page: https://github.com/robshakir/pyangbind
 Author: Rob Shakir
 Author-email: rjs@rob.sh
 License: Apache License, Version 2.0
 Keywords: yang,pyang
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 PyangBind
```

### Comparing `pyangbind-0.8.2/README.md` & `pyangbind-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pyangbind-0.8.2/README.rst` & `pyangbind-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyangbind-0.8.2/pyangbind/helpers/identity.py` & `pyangbind-0.8.3/pyangbind/helpers/identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 """
 
 from pyang import util
 from .misc import module_import_prefixes
 
 
 class Identity(object):
-
     def __init__(self, name):
         self.name = name
         self.source_module = None
         self._imported_prefixes = []
         self.source_namespace = None
         self.base = None
         self.children = []
@@ -43,15 +42,14 @@
         return "%s:%s" % (self.source_module, self.name)
 
     def prefixes(self):
         return self._imported_prefixes
 
 
 class IdentityStore(object):
-
     def __init__(self):
         self._store = []
 
     def find_identity_by_source_name(self, s, n):
         for i in self._store:
             if i.source_module == s and i.name == n:
                 return i
```

### Comparing `pyangbind-0.8.2/pyangbind/helpers/misc.py` & `pyangbind-0.8.3/pyangbind/helpers/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import sys
-
+import copy
 
 def module_import_prefixes(ctx):
     mod_ref_prefixes = {}
-    for mod in ctx.modules:
+    for mod in copy.deepcopy(ctx.modules):
         m = ctx.search_module(0, mod[0])
         for importstmt in m.search("import"):
             if importstmt.arg not in mod_ref_prefixes:
                 mod_ref_prefixes[importstmt.arg] = []
             mod_ref_prefixes[importstmt.arg].append(importstmt.search_one("prefix").arg)
     return mod_ref_prefixes
```

### Comparing `pyangbind-0.8.2/pyangbind/lib/base.py` & `pyangbind-0.8.3/pyangbind/lib/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,25 +16,23 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 
 class PybindBase(object):
-
     __slots__ = ()
 
     def elements(self):
         return self._pyangbind_elements
 
     def __str__(self):
         return str(self.elements())
 
     def get(self, filter=False):
-
         def error():
             return NameError, "element does not exist"
 
         d = {}
         # for each YANG element within this container.
         for element_name in self._pyangbind_elements:
             element = getattr(self, element_name, error)
@@ -96,15 +94,14 @@
                     d[element_id] = element
                 else:
                     # changed = False, and filter = True
                     pass
         return d
 
     def __getitem__(self, k):
-
         def error():
             raise KeyError("Key %s does not exist" % k)
 
         element = getattr(self, k, error)
         return element()
 
     def __iter__(self):
```

### Comparing `pyangbind-0.8.2/pyangbind/lib/pybindJSON.py` & `pyangbind-0.8.3/pyangbind/lib/pybindJSON.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
         f = json.load(open(fn, "r"), object_pairs_hook=OrderedDict)
     except IOError as m:
         raise pybindJSONIOError("Could not open file to read: %s" % m)
     return loads_ietf(f, parent_pymod, yang_module, path_helper, extmethods=extmethods, overwrite=overwrite)
 
 
 def dumps(obj, indent=4, filter=True, skip_subtrees=[], select=False, mode="default", with_defaults=None):
-
     def lookup_subdict(dictionary, key):
         if not isinstance(key, list):
             raise AttributeError("keys should be a list")
         unresolved_dict = {}
         for k, v in six.iteritems(dictionary):
             if ":" in k:
                 k = k.split(":")[1]
```

### Comparing `pyangbind-0.8.2/pyangbind/lib/serialise.py` & `pyangbind-0.8.3/pyangbind/lib/serialise.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     to various data encodings. XML and/or JSON as the primary examples.
 """
 from __future__ import unicode_literals
 
 import json
 from collections import OrderedDict
 from decimal import Decimal
+import base64
 
 import six
 from enum import IntEnum
 from lxml import objectify, etree
 
 from pyangbind.lib.yangtypes import YANGBool, safe_name
 
@@ -54,14 +55,15 @@
 
 class pybindJSONDecodeError(Exception):
     pass
 
 
 class UnmappedItem(Exception):
     """Used to simulate an Optional value"""
+
     pass
 
 
 class SerialisedTypedList(list):
     pass
 
 
@@ -125,15 +127,15 @@
             except UnmappedItem:
                 pass
         elif orig_yangt in ["int8", "int16", "int32", "uint8", "uint16", "uint32"]:
             return self.yangt_int(obj)
         elif orig_yangt in ["string", "enumeration"]:
             return six.text_type(obj)
         elif orig_yangt in ["binary"]:
-            return obj.to01()
+            return six.text_type(base64.b64encode(obj), "ascii")
         elif orig_yangt in ["decimal64"]:
             return self.yangt_decimal(obj)
         elif orig_yangt in ["bool"]:
             return True if obj else False
         elif orig_yangt in ["empty"]:
             return self.yangt_empty(obj)
         elif orig_yangt in ["container"]:
@@ -175,16 +177,16 @@
             map_val = getattr(obj, "_restricted_class_base")[0]
 
         if map_val in ["pyangbind.lib.yangtypes.ReferencePathType", "ReferencePathType"]:
             return self.default(obj._get())
         elif map_val in ["pyangbind.lib.yangtypes.RestrictedPrecisionDecimal", "RestrictedPrecisionDecimal"]:
             # NOTE: this doesn't seem like it needs to be a special case?
             return self.yangt_decimal(obj)
-        elif map_val in ["bitarray.bitarray"]:
-            return obj.to01()
+        elif map_val in ["pyangbind.lib.yangtypes.YANGBinary", "YANGBinary"]:
+            return six.text_type(base64.b64encode(obj), "ascii")
         elif map_val in ["unicode"]:
             return six.text_type(obj)
         elif map_val in ["pyangbind.lib.yangtypes.YANGBool"]:
             if original_yang_type == "empty":
                 # NOTE: previously with IETF mode the code would fall-through if obj was falsey
                 return self.yangt_empty(obj)
             else:
@@ -262,31 +264,34 @@
 class _pybindJSONEncoderBase(json.JSONEncoder):
     """
     Pybind JSON encoder base class. Implements default `encode()` and `default()` methods
     to be used as an encoder class with the deault *json* module.
 
     Do not use directly, subclass and set the `serialiser_class` attribute appropriately
     """
+
     serialiser_class = None
 
     def encode(self, obj):
         return json.JSONEncoder.encode(self, self.serialiser_class().preprocess_element(obj))
 
     def default(self, obj):
         return self.serialiser_class().default(obj)
 
 
 class pybindJSONEncoder(_pybindJSONEncoderBase):
     """Default pybind JSON encoder"""
+
     serialiser_class = YangDataSerialiser
 
 
 class pybindIETFJSONEncoder(_pybindJSONEncoderBase):
     """IETF JSON encoder, we add a special method `generate_element()` that should be used
     to restructure the pybind object to fit IETF requirements prior to JSON encoding."""
+
     serialiser_class = IETFYangDataSerialiser
 
     @staticmethod
     def yname_ns_func(parent_namespace, element, yname):
         if not element._namespace == parent_namespace:
             # if the namespace is different, then precede with the module
             # name as per spec.
@@ -488,15 +493,14 @@
             # because we can't tell from the XML structure
             attr_get = getattr(obj, "_get_%s" % safe_name(ykey), None)
             if attr_get is None:
                 raise AttributeError("Invalid attribute specified (%s)" % ykey)
             chobj = attr_get()
 
             if chobj._yang_type == "container":
-
                 if hasattr(chobj, "_presence"):
                     if chobj._presence:
                         chobj._set_present()
 
                 pybindIETFXMLDecoder.load_xml(
                     child, None, None, obj=chobj, path_helper=path_helper, extmethods=extmethods
                 )
@@ -559,20 +563,18 @@
                         raise AttributeError("Invalid attribute specified in XML - %s" % (ykey))
                     set_method(val)
 
         return obj
 
 
 class pybindJSONDecoder(object):
-
     @staticmethod
     def load_json(
         d, parent, yang_base, obj=None, path_helper=None, extmethods=None, overwrite=False, skip_unknown=False
     ):
-
         if obj is None:
             # we need to find the class to create, as one has not been supplied.
             base_mod_cls = getattr(parent, safe_name(yang_base))
             tmp = base_mod_cls(path_helper=False)
 
             if path_helper is not None:
                 # check that this path doesn't already exist in the
```

### Comparing `pyangbind-0.8.2/pyangbind/lib/xpathhelper.py` & `pyangbind-0.8.3/pyangbind/lib/xpathhelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,57 +45,56 @@
 
 
 class PybindImplementationError(Exception):
     pass
 
 
 class PybindXpathHelper(object):
-
     def register(self, path, object_ptr, caller=False):
         """
-      A PybindXpathHelper class should supply a register() method that
-      takes two mandatory arguments, and one optional.
+        A PybindXpathHelper class should supply a register() method that
+        takes two mandatory arguments, and one optional.
 
-      * path - the path to which the object should be registered. This is
-        supplied as a list of the names of the elements of the path. For
-        example, /device/interfaces/interface[name='eth0'] is supplied as
-        a ["device", "interfaces", "interface[@name='eth0']"].
-
-      * object_ptr - a reference to the object that is to be stored at this
-        location in the tree.
-
-      * caller=False - this supplies the path of the object that is currently
-        trying to perform a register. In general, it will not be used, but it
-        is supplied to facilitate relative path lookups.
-    """
+        * path - the path to which the object should be registered. This is
+          supplied as a list of the names of the elements of the path. For
+          example, /device/interfaces/interface[name='eth0'] is supplied as
+          a ["device", "interfaces", "interface[@name='eth0']"].
+
+        * object_ptr - a reference to the object that is to be stored at this
+          location in the tree.
+
+        * caller=False - this supplies the path of the object that is currently
+          trying to perform a register. In general, it will not be used, but it
+          is supplied to facilitate relative path lookups.
+        """
         raise PybindImplementationError("The path helper class specified does " + "not implement register()")
 
     def unregister(self, path, caller=False):
         """
-      A PybindXpathHelper class should supply an unregister() method that
-      takes one mandatory argument, and one optional.
+        A PybindXpathHelper class should supply an unregister() method that
+        takes one mandatory argument, and one optional.
 
-      * path - the path of the object to be unregistered. Supplied as a list()
-        object of the elements of the path.
+        * path - the path of the object to be unregistered. Supplied as a list()
+          object of the elements of the path.
 
-      * caller=False - the absolute path of the object calling the unregister()
-        method.
-    """
+        * caller=False - the absolute path of the object calling the unregister()
+          method.
+        """
         raise PybindImplementationError("The path helper class specified does " + "not implement unregister()")
 
     def get(self, path, caller=False):
         """
-      A PybindXpathHelper class should supply a get() method that takes one
-      mandatory argument and one optional.
+        A PybindXpathHelper class should supply a get() method that takes one
+        mandatory argument and one optional.
 
-      * path - the path to the object to be retrieved. This may be specified as
-        a list of parts, or an XPATH expression.
+        * path - the path to the object to be retrieved. This may be specified as
+          a list of parts, or an XPATH expression.
 
-      * caller=False - the absolute path of the object calling the get method.
-    """
+        * caller=False - the absolute path of the object calling the get method.
+        """
         raise PybindImplementationError("The path helper class specified does " + "not implement get()")
 
 
 # A class which acts as "/" within the hierarchy - it acts as per any other
 # PyangBind element for the purposes of get() calls - allowing "/" to be
 # serialised to
 class FakeRoot(PybindBase):
```

### Comparing `pyangbind-0.8.2/pyangbind/lib/yangtypes.py` & `pyangbind-0.8.3/pyangbind/lib/yangtypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from __future__ import unicode_literals
 
+import base64
 import collections
 from collections import abc
 import copy
 import uuid
 from decimal import Decimal
 
 import regex
 import six
-from bitarray import bitarray
 
 # Words that could turn up in YANG definition files that are actually
 # reserved names in Python, such as being builtin types. This list is
 # not complete, but will probably continue to grow.
 reserved_name = [
     "list",
     "str",
@@ -81,14 +81,15 @@
     "or",
     "and",
     "not",
     "yield",
     "property",
     "min",
     "max",
+    "async",
 ]
 
 
 def is_yang_list(arg):
     if isinstance(arg, list):
         return True
     elif hasattr(arg, "_pybind_generated_by"):
@@ -116,45 +117,46 @@
             new_path.append(i)
     return new_path
 
 
 def safe_name(arg):
     """
     Make a leaf or container name safe for use in Python.
-  """
+    """
     arg = arg.replace("-", "_")
     arg = arg.replace(".", "_")
     if arg in reserved_name:
         arg += "_"
     # store the unsafe->original version mapping
     # so that we can retrieve it when get() is called.
     return arg
 
 
 def RestrictedPrecisionDecimalType(*args, **kwargs):
     """
     Function to return a new type that is based on decimal.Decimal with
     an arbitrary restricted precision.
-  """
+    """
     precision = kwargs.pop("precision", False)
 
     class RestrictedPrecisionDecimal(Decimal):
         """
-      Class extending decimal.Decimal to restrict the precision that is
-      stored, supporting the fraction-digits argument of the YANG decimal64
-      type.
-    """
+        Class extending decimal.Decimal to restrict the precision that is
+        stored, supporting the fraction-digits argument of the YANG decimal64
+        type.
+        """
+
         _precision = 10.0 ** (-1.0 * int(precision))
         _pybind_generated_by = "RestrictedPrecisionDecimal"
 
         def __new__(self, *args, **kwargs):
             """
-        Overloads the decimal __new__ function in order to round the input
-        value to the new value.
-      """
+            Overloads the decimal __new__ function in order to round the input
+            value to the new value.
+            """
             if self._precision is not None:
                 if len(args):
                     value = Decimal(args[0]).quantize(Decimal(str(self._precision)))
                 else:
                     value = Decimal(0)
             elif len(args):
                 value = Decimal(args[0])
@@ -168,15 +170,15 @@
 
 def RestrictedClassType(*args, **kwargs):
     """
     Function to return a new type that restricts an arbitrary base_type with
     a specified restriction. The restriction_type specified determines the
     type of restriction placed on the class, and the restriction_arg gives
     any input data that this function needs.
-  """
+    """
     base_type = kwargs.pop("base_type", six.text_type)
     restriction_type = kwargs.pop("restriction_type", None)
     restriction_arg = kwargs.pop("restriction_arg", None)
     restriction_dict = kwargs.pop("restriction_dict", None)
     int_size = kwargs.pop("int_size", None)
 
     # this gives deserialisers some hints as to how to encode/decode this value
@@ -187,29 +189,30 @@
         restricted_class_hint = getattr(base_type, "_restricted_class_base")
         restricted_class_hint.append(current_restricted_class_type)
     else:
         restricted_class_hint = [current_restricted_class_type]
 
     class RestrictedClass(base_type):
         """
-      A class that restricts the base_type class with a new function that the
-      input value is validated against before being applied. The function is
-      a static method which is assigned to _restricted_test.
-    """
+        A class that restricts the base_type class with a new function that the
+        input value is validated against before being applied. The function is
+        a static method which is assigned to _restricted_test.
+        """
+
         _pybind_generated_by = "RestrictedClassType"
 
         _restricted_class_base = restricted_class_hint
         _restricted_int_size = int_size
 
         def __init__(self, *args, **kwargs):
             """
-        Overloads the base_class __init__ method to check the input argument
-        against the validation function - returns on instance of the base_type
-        class, which can be manipulated as per a usual Python object.
-      """
+            Overloads the base_class __init__ method to check the input argument
+            against the validation function - returns on instance of the base_type
+            class, which can be manipulated as per a usual Python object.
+            """
             try:
                 self.__check(args[0])
             except IndexError:
                 pass
             try:
                 super(RestrictedClass, self).__init__(*args, **kwargs)
             except TypeError:
@@ -224,15 +227,14 @@
         _restriction_test method so that it can be called by other functions.
       """
 
             range_regex = regex.compile("(?P<low>\-?[0-9\.]+|min)([ ]+)?\.\.([ ]+)?" + "(?P<high>(\-?[0-9\.]+|max))")
             range_single_value_regex = regex.compile("(?P<value>\-?[0-9\.]+)")
 
             def convert_regexp(pattern):
-
                 # Some patterns include a $ character in them in some IANA modules, this
                 # is not escaped. Do some logic to escape them, whilst leaving one at the
                 # end of the string if it's there.
                 trimmed = False
                 if pattern[-1] == "$":
                     tmp_pattern = pattern[:-1]
                     trimmed = True
@@ -267,19 +269,16 @@
                     else:
                         eqval = int(eqval) * multiplier
                     return (eqval,)
                 else:
                     raise ValueError("Invalid range or length argument specified")
 
             def in_range_check(low_high_tuples, length=False):
-
                 def range_check(value):
-                    if length and isinstance(value, bitarray):
-                        value = value.length()
-                    elif length:
+                    if length:
                         value = len(value)
                     range_results = []
                     for check_tuple in low_high_tuples:
                         chk = True
                         if len(check_tuple) == 2:
                             if check_tuple[0] is not None and value < check_tuple[0]:
                                 chk = False
@@ -292,15 +291,14 @@
                             raise AttributeError("Invalid check tuple length specified")
                         range_results.append(chk)
                     return True in range_results
 
                 return range_check
 
             def match_pattern_check(regexp):
-
                 def mp_check(value):
                     if not isinstance(value, six.string_types + (six.text_type,)):
                         return False
                     if regex.match(convert_regexp(regexp), value):
                         return True
                     return False
 
@@ -330,20 +328,15 @@
                     self._restriction_tests.append(in_range_check(ranges))
                     if val:
                         try:
                             val = base_type(val)
                         except Exception:
                             raise TypeError("must specify a numeric type for a range " + "argument")
                 elif rtype == "length":
-                    # When the type is a binary then the length is specified in
-                    # octets rather than bits, so we must specify the length to
-                    # be multiplied by 8.
                     multiplier = 1
-                    if base_type == bitarray:
-                        multiplier = 8
                     lengths = []
                     for range_spec in rarg:
                         lengths.append(build_length_range_tuples(range_spec, length=True, multiplier=multiplier))
                     self._restriction_tests.append(in_range_check(lengths, length=True))
                 elif rtype == "dict_key":
                     new_rarg = copy.deepcopy(rarg)
                     for k in rarg:
@@ -379,43 +372,43 @@
                 obj = base_type.__new__(self, *args, **kwargs)
             except TypeError:
                 obj = base_type.__new__(self)
             return obj
 
         def __check(self, v):
             """
-        Run the _restriction_test static method against the argument v,
-        returning an error if the value does not validate.
-      """
+            Run the _restriction_test static method against the argument v,
+            returning an error if the value does not validate.
+            """
             v = base_type(v)
             for chkfn in self._restriction_tests:
                 if not chkfn(v):
                     raise ValueError("did not match restricted type")
             return True
 
         def getValue(self, *args, **kwargs):
             """
-        For types where there is a dict_key restriction (such as YANG
-        enumeration), return the value of the dictionary key.
-      """
+            For types where there is a dict_key restriction (such as YANG
+            enumeration), return the value of the dictionary key.
+            """
             if "dict_key" in self._restriction_dict:
                 value = kwargs.pop("mapped", False)
                 if value:
                     return self._enumeration_dict[self.__str__()]["value"]
             return self
 
     return type(RestrictedClass(*args, **kwargs))
 
 
 def TypedListType(*args, **kwargs):
     """
     Return a type that consists of a list object where only
     certain types (specified by allowed_type kwarg to the function)
     can be added to the list.
-  """
+    """
     allowed_type = kwargs.pop("allowed_type", six.text_type)
     if not isinstance(allowed_type, list):
         allowed_type = [allowed_type]
 
     class TypedList(abc.MutableSequence):
         _pybind_generated_by = "TypedListType"
         _list = list()
@@ -534,15 +527,15 @@
 
     .add(key) - initialises a new member of the list
     .delete(key) - removes it.
 
     Where a list exists that does not have a key - which can be the
     case for 'config false' lists - a uuid is generated and used
     as the key for the list.
-  """
+    """
     try:
         keyname = args[0]
         listclass = args[1]
     except Exception:
         raise TypeError("A YANGList must be specified with a key value and a " + "contained class")
     is_container = kwargs.pop("is_container", False)
     parent = kwargs.pop("parent", False)
@@ -884,15 +877,15 @@
     """
     A custom boolean class for using in YANG. Since bool has specific
     logic in python, it is not possible to extend the existing bool
     objects.
 
     This bool also accepts input matching strings to handle the
     forms that might be used in YANG modules.
-  """
+    """
 
     def __new__(self, *args, **kwargs):
         false_args = ["false", "False", False, 0, "0"]
         true_args = ["true", "True", True, 1, "1"]
         if len(args):
             if not args[0] in false_args + true_args:
                 raise ValueError("%s is an invalid value for a YANGBool" % args[0])
@@ -931,15 +924,15 @@
                                 the path.
       - extensions:  The list of extensions that should be stored
                      with the type.
       - is_config:   Whether this is a configuration (editable)
                      node.
       - presence:    Whether the YANG container that is being
                      represented has the presence keyword
-  """
+    """
     base_type = kwargs.pop("base", False)
     default = kwargs.pop("default", False)
     yang_name = kwargs.pop("yang_name", False)
     parent_instance = kwargs.pop("parent", False)
     choice_member = kwargs.pop("choice", False)
     is_container = kwargs.pop("is_container", False)
     is_leaf = kwargs.pop("is_leaf", False)
@@ -1194,15 +1187,14 @@
                 return self._supplied_register_path
             if self._parent is not None:
                 return self._parent._path() + [self._yang_name]
             else:
                 return []
 
         def __generate_extmethod(self, methodfn):
-
             def extmethodfn(*args, **kwargs):
                 kwargs["caller"] = self._register_path()
                 kwargs["path_helper"] = self._path_helper
                 return methodfn(*args, **kwargs)
 
             return extmethodfn
 
@@ -1228,22 +1220,21 @@
 def ReferenceType(*args, **kwargs):
     """
     A type which based on a path provided acts as a leafref.
     The caller argument is used to allow the path that is provided
     to be a relative (rather than absolute) path. The require_instance
     argument specifies whether errors should be thrown in the case
     that the referenced instance does not exist.
-  """
+    """
     ref_path = kwargs.pop("referenced_path", False)
     path_helper = kwargs.pop("path_helper", None)
     caller = kwargs.pop("caller", False)
     require_instance = kwargs.pop("require_instance", False)
 
     class ReferencePathType(object):
-
         __slots__ = (
             "_referenced_path",
             "_path_helper",
             "_caller",
             "_referenced_object",
             "_ptr",
             "_require_instance",
@@ -1350,7 +1341,32 @@
 
         def __str__(self):
             if not self._ptr:
                 return str(self._referenced_object)
             return str(self._get_ptr())
 
     return type(ReferencePathType(*args, **kwargs))
+
+
+class YANGBinary(bytes):
+    """
+    A custom binary class for using in YANG.
+    """
+
+    def __new__(self, *args, **kwargs):
+        value = b""
+        if args:
+            value = args[0]
+            if isinstance(value, str):
+                value = base64.b64decode(value)
+            elif isinstance(value, bytes):
+                value = value
+            else:
+                raise ValueError(f"invalid type for {value}: {type(value)}")
+
+        return bytes.__new__(self, value)
+
+    def __repr__(self):
+        return str(self)
+
+    def __str__(self, encoding="ascii", errors="replace"):
+        return str(self, encoding=encoding, errors=errors)
```

### Comparing `pyangbind-0.8.2/pyangbind/plugin/pybind.py` & `pyangbind-0.8.3/pyangbind/plugin/pybind.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,20 +26,19 @@
 import decimal
 import optparse
 import os
 import sys
 from collections import OrderedDict
 
 import six
-from bitarray import bitarray
 from pyang import plugin, statements, util
 
 import pyangbind.helpers.misc as misc_help
 from pyangbind.helpers.identity import IdentityStore
-from pyangbind.lib.yangtypes import RestrictedClassType, YANGBool, safe_name
+from pyangbind.lib.yangtypes import RestrictedClassType, YANGBool, safe_name, YANGBinary
 
 # Python3 support
 if six.PY3:
     long = int
 else:
     import codecs
 
@@ -96,15 +95,15 @@
     "boolean": {
         "native_type": "YANGBool",
         "map": class_bool_map,
         "base_type": True,
         "quote_arg": True,
         "pytype": YANGBool,
     },
-    "binary": {"native_type": "bitarray", "base_type": True, "quote_arg": True, "pytype": bitarray},
+    "binary": {"native_type": "YANGBinary", "base_type": True, "quote_arg": True, "pytype": YANGBinary},
     "uint8": {
         "native_type": ("RestrictedClassType(base_type=int," + " restriction_dict={'range': ['0..255']}, int_size=8)"),
         "base_type": True,
         "pytype": RestrictedClassType(base_type=int, restriction_dict={"range": ["0..255"]}, int_size=8),
     },
     "uint16": {
         "native_type": (
@@ -188,15 +187,14 @@
 
 # Base machinery to support operation as a plugin to pyang.
 def pyang_plugin_init():
     plugin.register_plugin(PyangBindClass())
 
 
 class PyangBindClass(plugin.PyangPlugin):
-
     def add_output_format(self, fmts):
         # Add the 'pybind' output format to pyang.
         self.multiple_modules = True
         fmts["pybind"] = self
 
     def emit(self, ctx, modules, fd):
         # When called, call the build_pyangbind function.
@@ -314,21 +312,21 @@
         "RestrictedPrecisionDecimalType",
         "RestrictedClassType",
         "TypedListType",
         "YANGBool",
         "YANGListType",
         "YANGDynClass",
         "ReferenceType",
+        "YANGBinary",
     ]
     for library in yangtypes_imports:
         ctx.pybind_common_hdr += "from pyangbind.lib.yangtypes import {}\n".format(library)
     ctx.pybind_common_hdr += "from pyangbind.lib.base import PybindBase\n"
     ctx.pybind_common_hdr += "from collections import OrderedDict\n"
     ctx.pybind_common_hdr += "from decimal import Decimal\n"
-    ctx.pybind_common_hdr += "from bitarray import bitarray\n"
     ctx.pybind_common_hdr += "import six\n"
 
     # Python3 support
     ctx.pybind_common_hdr += """
 # PY3 support of some PY2 keywords (needs improved)
 if six.PY3:
   import builtins as __builtin__
@@ -615,15 +613,14 @@
             # Handle a typedef that is a union - extended the class_map arguments
             # to be a list that is parsed by the relevant dynamic type generation
             # function.
             native_type = []
             parent_type = []
             default = False if default_stmt is None else default_stmt.arg
             for i in elemtype:
-
                 if isinstance(i[1]["native_type"], list):
                     native_type.extend(i[1]["native_type"])
                 else:
                     native_type.append(i[1]["native_type"])
 
                 if i[1]["yang_type"] in known_types:
                     parent_type.append(i[1]["yang_type"])
@@ -644,15 +641,14 @@
                 class_map[type_name]["default"] = default[0]
                 class_map[type_name]["quote_default"] = default[1]
 
         class_map[type_name.split(":")[1]] = class_map[type_name]
 
 
 def get_children(ctx, fd, i_children, module, parent, path=str(), parent_cfg=True, choice=False, register_paths=True):
-
     # Iterative function that is called for all elements that have childen
     # data nodes in the tree. This function resolves those nodes into the
     # relevant leaf, or container/list configuration and outputs the python
     # code that corresponds to it to the relevant file. parent_cfg is used to
     # ensure that where a parent container was set to config false, this is
     # inherited by all elements below it; and choice is used to store whether
     # these leaves are within a choice or not.
@@ -1512,17 +1508,18 @@
                 elemdict["user_ordered"] = (
                     True if user_ordered is not None and user_ordered.arg.upper() == "USER" else False
                 )
             this_object.append(elemdict)
             has_children = True
 
     # Deal with the cases that the attribute does not have children.
-    if not has_children:
+    if not has_children: # and element.search_one("type"):
         if element.keyword in ["leaf-list"]:
             create_list = True
+        print(element)
         cls, elemtype = copy.deepcopy(build_elemtype(ctx, element.search_one("type")))
 
         # Determine what the default for the leaf should be where there are
         # multiple available.
         # Algorithm:
         #   - build a tree that is rooted on this class.
         #   - perform a breadth-first search - the first node found
```

### Comparing `pyangbind-0.8.2/pyangbind.egg-info/PKG-INFO` & `pyangbind-0.8.3/pyangbind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pyangbind
-Version: 0.8.2
+Version: 0.8.3
 Summary: PyangBind is a plugin for pyang which converts YANG data models into a Python class hierarchy, such that Python can be used to manipulate data that conforms with a YANG model.
 Home-page: https://github.com/robshakir/pyangbind
 Author: Rob Shakir
 Author-email: rjs@rob.sh
 License: Apache License, Version 2.0
 Keywords: yang,pyang
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 PyangBind
```

### Comparing `pyangbind-0.8.2/pyangbind.egg-info/SOURCES.txt` & `pyangbind-0.8.3/pyangbind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyangbind-0.8.2/setup.cfg` & `pyangbind-0.8.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 	pyang
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Telecommunications Industry
 	Intended Audience :: Developers
 	Topic :: Software Development :: Code Generators
 	License :: OSI Approved :: Apache Software License
-	Programming Language :: Python :: 2.7
-	Programming Language :: Python :: 3.4
-	Programming Language :: Python :: 3.5
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 python_requires = >=3.7
 install_requires = file: requirements.txt
 packages = find:
```

