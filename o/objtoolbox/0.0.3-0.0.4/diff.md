# Comparing `tmp/objtoolbox-0.0.3.tar.gz` & `tmp/objtoolbox-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objtoolbox-0.0.3.tar", last modified: Tue Jul 11 18:59:23 2023, max compression
+gzip compressed data, was "objtoolbox-0.0.4.tar", last modified: Mon Aug  7 08:34:51 2023, max compression
```

## Comparing `objtoolbox-0.0.3.tar` & `objtoolbox-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-11 18:59:23.867648 objtoolbox-0.0.3/
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1496 2023-03-31 07:55:26.000000 objtoolbox-0.0.3/LICENSE
--rw-r--r--   0 ruof      (1000) ruof      (1000)      632 2023-07-11 18:59:23.867648 objtoolbox-0.0.3/PKG-INFO
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      212 2023-07-03 08:00:36.000000 objtoolbox-0.0.3/README.md
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      562 2023-07-11 18:57:33.000000 objtoolbox-0.0.3/pyproject.toml
--rw-r--r--   0 ruof      (1000) ruof      (1000)       38 2023-07-11 18:59:23.867648 objtoolbox-0.0.3/setup.cfg
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-11 18:59:23.867648 objtoolbox-0.0.3/src/
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-11 18:59:23.867648 objtoolbox-0.0.3/src/objtoolbox/
--rw-r--r--   0 ruof      (1000) ruof      (1000)      128 2023-07-03 08:22:06.000000 objtoolbox-0.0.3/src/objtoolbox/__init__.py
--rw-r--r--   0 ruof      (1000) ruof      (1000)     1787 2023-07-10 09:52:01.000000 objtoolbox-0.0.3/src/objtoolbox/merge.py
--rw-r--r--   0 ruof      (1000) ruof      (1000)    12320 2023-07-07 13:36:04.000000 objtoolbox-0.0.3/src/objtoolbox/storage.py
--rw-r--r--   0 ruof      (1000) ruof      (1000)     2434 2023-07-11 18:58:26.000000 objtoolbox-0.0.3/src/objtoolbox/utils.py
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-11 18:59:23.867648 objtoolbox-0.0.3/src/objtoolbox.egg-info/
--rw-r--r--   0 ruof      (1000) ruof      (1000)      632 2023-07-11 18:59:23.000000 objtoolbox-0.0.3/src/objtoolbox.egg-info/PKG-INFO
--rw-r--r--   0 ruof      (1000) ruof      (1000)      322 2023-07-11 18:59:23.000000 objtoolbox-0.0.3/src/objtoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 ruof      (1000) ruof      (1000)        1 2023-07-11 18:59:23.000000 objtoolbox-0.0.3/src/objtoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 ruof      (1000) ruof      (1000)       25 2023-07-11 18:59:23.000000 objtoolbox-0.0.3/src/objtoolbox.egg-info/requires.txt
--rw-r--r--   0 ruof      (1000) ruof      (1000)       11 2023-07-11 18:59:23.000000 objtoolbox-0.0.3/src/objtoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-07 08:34:51.204189 objtoolbox-0.0.4/
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1496 2023-03-31 07:55:26.000000 objtoolbox-0.0.4/LICENSE
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      632 2023-08-07 08:34:51.204189 objtoolbox-0.0.4/PKG-INFO
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      212 2023-07-03 08:00:36.000000 objtoolbox-0.0.4/README.md
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      562 2023-08-07 08:34:08.000000 objtoolbox-0.0.4/pyproject.toml
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       38 2023-08-07 08:34:51.204189 objtoolbox-0.0.4/setup.cfg
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-07 08:34:51.204189 objtoolbox-0.0.4/src/
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-07 08:34:51.204189 objtoolbox-0.0.4/src/objtoolbox/
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      142 2023-08-07 08:34:08.000000 objtoolbox-0.0.4/src/objtoolbox/__init__.py
+-rw-r--r--   0 ruof      (1000) ruof      (1000)     1787 2023-07-10 09:52:01.000000 objtoolbox-0.0.4/src/objtoolbox/merge.py
+-rw-r--r--   0 ruof      (1000) ruof      (1000)    12796 2023-08-07 08:34:08.000000 objtoolbox-0.0.4/src/objtoolbox/storage.py
+-rw-r--r--   0 ruof      (1000) ruof      (1000)     2434 2023-07-11 18:58:26.000000 objtoolbox-0.0.4/src/objtoolbox/utils.py
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-07 08:34:51.204189 objtoolbox-0.0.4/src/objtoolbox.egg-info/
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      632 2023-08-07 08:34:51.000000 objtoolbox-0.0.4/src/objtoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      322 2023-08-07 08:34:51.000000 objtoolbox-0.0.4/src/objtoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)        1 2023-08-07 08:34:51.000000 objtoolbox-0.0.4/src/objtoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       25 2023-08-07 08:34:51.000000 objtoolbox-0.0.4/src/objtoolbox.egg-info/requires.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       11 2023-08-07 08:34:51.000000 objtoolbox-0.0.4/src/objtoolbox.egg-info/top_level.txt
```

### Comparing `objtoolbox-0.0.3/LICENSE` & `objtoolbox-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `objtoolbox-0.0.3/PKG-INFO` & `objtoolbox-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objtoolbox
-Version: 0.0.3
+Version: 0.0.4
 Summary: Advanced utility functions for python objects
 Author-email: Jona Ruof <jona.ruof@uni-ulm.de>
 Project-URL: Homepage, https://github.com/joruof/objtoolbox
 Project-URL: Bug Tracker, https://github.com/joruof/objtoolbox/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `objtoolbox-0.0.3/pyproject.toml` & `objtoolbox-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "objtoolbox"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jona Ruof", email="jona.ruof@uni-ulm.de" },
 ]
 description = "Advanced utility functions for python objects"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `objtoolbox-0.0.3/src/objtoolbox/merge.py` & `objtoolbox-0.0.4/src/objtoolbox/merge.py`

 * *Files identical despite different names*

### Comparing `objtoolbox-0.0.3/src/objtoolbox/storage.py` & `objtoolbox-0.0.4/src/objtoolbox/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # i still like this
 from pydoc import locate
 
 import zarr
 import numpy as np
 
-from objtoolbox import ext_setattr, fqn_type_name
+from objtoolbox import ext_setattr, get_obj_dict, fqn_type_name
 
 
 def patch_zarr_indexing():
     """
     Evil, dark-magic, monkey-patching to make zarr array indexing
     behave even more like numpy indexing.
     Will hopefully become unnecessary in future zarr versions.
@@ -82,23 +82,29 @@
 
 class Serializer:
     """
     Converts an object tree into a json serializeable object tree.
     Large numpy arrays are automatically referenced and stored externally.
     """
 
-    def __init__(self, path, hide_private=True, compressor=None):
+    def __init__(self,
+                 path,
+                 hide_private=True,
+                 compressor=None,
+                 externalize=True):
 
         self.hide_private = hide_private
         self.compressor = compressor
+        self.externalize = externalize
 
-        self.ext_path = os.path.join(path, "extern")
-        self.array_store = zarr.open(get_chunk_store(self.ext_path))
+        if self.externalize:
+            self.ext_path = os.path.join(path, "extern")
+            self.array_store = zarr.open(get_chunk_store(self.ext_path))
 
-        self.saved_arrays = set()
+        self.used_arrays = set()
 
         self.obj_path = []
 
     def serialize(self, obj, key="", parent=None):
 
         if type(key) == str:
             if self.hide_private and len(key) > 0 and key[0] == "_":
@@ -108,66 +114,73 @@
         if (isinstance(obj, types.FunctionType)
                 or isinstance(obj, types.MethodType)
                 or isinstance(obj, types.LambdaType)):
             return Skip
 
         # special treatment for numpy arrays
         if type(obj) == np.ndarray:
-            if obj.size > 25:
+            if obj.size > 25 and self.externalize:
 
                 path = ".".join([str(p) for p in self.obj_path])
                 obj = self.array_store.array(
                         path,
                         obj,
                         chunks=False,
                         compressor=self.compressor,
                         overwrite=True)
 
                 if type(key) == str:
                     ext_setattr(parent, key, obj)
                 elif type(key) == int:
                     parent[key] = obj
 
-                self.saved_arrays.add(path)
+                self.used_arrays.add(path)
                 return {
                     "__class__": "__extern__",
                     "path": path
                 }
             else:
                 return {
                     "__class__": fqn_type_name(obj),
                     "dtype": obj.dtype.name,
                     "data": obj.tolist()
                 }
 
         # already saved arrays
         if type(obj) == zarr.core.Array:
+            if self.externalize:
+                path = ".".join([str(p) for p in self.obj_path])
 
-            path = ".".join([str(p) for p in self.obj_path])
+                if (self.array_store.store.path != obj.store.path
+                        or obj.path != path):
 
-            if (self.array_store.store.path != obj.store.path
-                    or obj.path != path):
+                    obj = self.array_store.array(
+                            path,
+                            obj,
+                            chunks=False,
+                            compressor=self.compressor,
+                            overwrite=True)
+
+                    if type(key) == str:
+                        ext_setattr(parent, key, obj)
+                    elif type(key) == int:
+                        parent[key] = obj
 
-                obj = self.array_store.array(
-                        path,
-                        obj,
-                        chunks=False,
-                        compressor=self.compressor,
-                        overwrite=True)
-
-                if type(key) == str:
-                    ext_setattr(parent, key, obj)
-                elif type(key) == int:
-                    parent[key] = obj
-
-            self.saved_arrays.add(obj.path)
-            return {
-                "__class__": "__extern__",
-                "path": obj.path
-            }
+                self.used_arrays.add(obj.path)
+                return {
+                    "__class__": "__extern__",
+                    "path": obj.path
+                }
+            else:
+                np_obj = np.array(obj)
+                return {
+                    "__class__": fqn_type_name(np_obj),
+                    "dtype": np_obj.dtype.name,
+                    "data": np_obj.tolist()
+                }
 
         if type(obj) == list or type(obj) == tuple:
             jvs = []
             for i, v in enumerate(obj):
                 self.obj_path.append(i)
                 jv = self.serialize(v, i, parent=obj)
                 self.obj_path.pop()
@@ -221,21 +234,21 @@
     """
     Loads an object tree from a json file.
     External numpy arrays are automatically dereferenced and mem-mapped.
     """
 
     def __init__(self, path, map_arrays=True):
 
-        self.ext_path = os.path.join(path, "extern")
-
         self.map_arrays = map_arrays
 
-        self.array_store = zarr.open(get_chunk_store(self.ext_path))
+        self.ext_path = os.path.join(path, "extern")
+        if os.path.exists(self.ext_path):
+            self.array_store = zarr.open(get_chunk_store(self.ext_path))
 
-        self.loaded_arrays = set()
+        self.used_arrays = set()
 
     def load(self, obj, json_obj):
 
         t = type(obj)
         jt = type(json_obj)
 
         # before we do anything else we check if we
@@ -250,32 +263,25 @@
                 try:
                     json_obj = self.array_store[path]
                 except KeyError:
                     return obj
                 if not self.map_arrays:
                     json_obj = np.array(json_obj)
 
-                self.loaded_arrays.add(path)
+                self.used_arrays.add(path)
                 # we are lying about this one (actually zarr.core.Array)
                 # in practice it should behave (mostly) like ndarray
                 jt = np.ndarray
             elif cls == "numpy.ndarray":
                 json_obj = np.array(json_obj["data"], dtype=json_obj["dtype"])
                 jt = np.ndarray
 
         # try to get a dict representation of the object
 
-        attrs = None
-
-        if hasattr(obj, "__dict__"):
-            attrs = obj.__dict__
-        elif hasattr(obj, "__slots__"):
-            attrs = {n: getattr(obj, n) for n in obj.__slots__}
-        elif isinstance(obj, dict):
-            attrs = obj
+        attrs = get_obj_dict(obj)
 
         # now check how we should continue
 
         if attrs is not None and jt == dict:
 
             # handles general objects and dicts
 
@@ -349,16 +355,14 @@
 
 def save(obj, directory, compressor=None):
     """
     Stores obj under a given directory.
     The directory will be created if it not already exists.
     """
 
-    # write to json
-
     os.makedirs(directory, exist_ok=True)
 
     ser = Serializer(directory, compressor=compressor)
     rep = ser.serialize(obj)
 
     if rep is Skip:
         return
@@ -368,26 +372,26 @@
     with open(unfinished_path, "w+") as fd:
         json.dump(rep, fd, indent=2)
 
     state_path = os.path.join(directory, "state.json")
 
     os.rename(unfinished_path, state_path)
 
-    # remove unused external numpy arrays
+    clean_zarr_store(ser)
 
-    on_disk = set(ser.array_store.keys())
-    unused = on_disk - ser.saved_arrays
 
-    for k in unused:
-        del ser.array_store[k]
+def saves(obj):
+    """
+    Serializes obj to a string represenation.
+    """
 
-        # because zarr does not clean up emtpy folders
-        arr_path = os.path.join(ser.ext_path, k)
-        if os.path.isdir(arr_path):
-            shutil.rmtree(arr_path)
+    ser = Serializer("", externalize=False)
+    rep = ser.serialize(obj)
+
+    return json.dumps(rep)
 
 
 def load(obj, path, map_arrays=True):
     """
     Updates obj with data stored at the given path.
     """
 
@@ -398,19 +402,36 @@
 
     with open(state_path, "r") as fd:
         json_state = json.load(fd)
 
     lod = Loader(path, map_arrays)
     lod.load(obj, json_state)
 
-    # remove unused external numpy arrays
+    clean_zarr_store(lod)
+
+
+def loads(obj, string):
+    """
+    Updates obj with data store in the given string.
+    """
+
+    json_state = json.loads(string)
+
+    lod = Loader("", map_arrays=False)
+    lod.load(obj, json_state)
+
+
+def clean_zarr_store(o):
+    """
+    Removes unused external zarr arrays form the zarr store.
+    """
 
-    on_disk = set(lod.array_store.keys())
-    unused = on_disk - lod.loaded_arrays
+    on_disk = set(o.array_store.keys())
+    unused = on_disk - o.used_arrays
 
     for k in unused:
-        del lod.array_store[k]
+        del o.array_store[k]
 
-        # because zarr does not clean up emtpy folders
-        arr_path = os.path.join(lod.ext_path, k)
+        # because zarr does not clean up empy folders
+        arr_path = os.path.join(o.ext_path, k)
         if os.path.isdir(arr_path):
             shutil.rmtree(arr_path)
```

### Comparing `objtoolbox-0.0.3/src/objtoolbox/utils.py` & `objtoolbox-0.0.4/src/objtoolbox/utils.py`

 * *Files identical despite different names*

### Comparing `objtoolbox-0.0.3/src/objtoolbox.egg-info/PKG-INFO` & `objtoolbox-0.0.4/src/objtoolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objtoolbox
-Version: 0.0.3
+Version: 0.0.4
 Summary: Advanced utility functions for python objects
 Author-email: Jona Ruof <jona.ruof@uni-ulm.de>
 Project-URL: Homepage, https://github.com/joruof/objtoolbox
 Project-URL: Bug Tracker, https://github.com/joruof/objtoolbox/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

