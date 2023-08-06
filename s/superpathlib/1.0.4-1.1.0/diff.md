# Comparing `tmp/superpathlib-1.0.4.tar.gz` & `tmp/superpathlib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpathlib-1.0.4.tar", last modified: Tue Jul 25 23:51:01 2023, max compression
+gzip compressed data, was "superpathlib-1.1.0.tar", last modified: Sun Aug  6 22:03:44 2023, max compression
```

## Comparing `superpathlib-1.0.4.tar` & `superpathlib-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:51:01.340200 superpathlib-1.0.4/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-07-25 23:50:13.000000 superpathlib-1.0.4/LICENSE
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2975 2023-07-25 23:51:01.340200 superpathlib-1.0.4/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2630 2023-07-25 23:50:13.000000 superpathlib-1.0.4/README.md
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:51:01.336200 superpathlib-1.0.4/plib/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       23 2023-07-25 23:50:13.000000 superpathlib-1.0.4/plib/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)    15444 2023-07-25 23:50:13.000000 superpathlib-1.0.4/plib/plib.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1152 2023-07-25 23:50:13.000000 superpathlib-1.0.4/plib/tags.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      857 2023-07-25 23:50:13.000000 superpathlib-1.0.4/plib/utils.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      722 2023-07-25 23:50:25.000000 superpathlib-1.0.4/pyproject.toml
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       38 2023-07-25 23:51:01.340200 superpathlib-1.0.4/setup.cfg
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:51:01.340200 superpathlib-1.0.4/superpathlib.egg-info/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2975 2023-07-25 23:51:01.000000 superpathlib-1.0.4/superpathlib.egg-info/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      373 2023-07-25 23:51:01.000000 superpathlib-1.0.4/superpathlib.egg-info/SOURCES.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-07-25 23:51:01.000000 superpathlib-1.0.4/superpathlib.egg-info/dependency_links.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       69 2023-07-25 23:51:01.000000 superpathlib-1.0.4/superpathlib.egg-info/requires.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        5 2023-07-25 23:51:01.000000 superpathlib-1.0.4/superpathlib.egg-info/top_level.txt
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:51:01.340200 superpathlib-1.0.4/tests/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1649 2023-07-25 23:50:13.000000 superpathlib-1.0.4/tests/test_content.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1678 2023-07-25 23:50:13.000000 superpathlib-1.0.4/tests/test_encrypted_content.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2045 2023-07-25 23:50:13.000000 superpathlib-1.0.4/tests/test_functionality.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      937 2023-07-25 23:50:13.000000 superpathlib-1.0.4/tests/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:03:44.415068 superpathlib-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-06 22:03:33.000000 superpathlib-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-08-06 22:03:44.415068 superpathlib-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-08-06 22:03:33.000000 superpathlib-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:03:44.415068 superpathlib-1.1.0/plib/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-06 22:03:33.000000 superpathlib-1.1.0/plib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-06 22:03:33.000000 superpathlib-1.1.0/plib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-06 22:03:33.000000 superpathlib-1.1.0/plib/common_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-06 22:03:33.000000 superpathlib-1.1.0/plib/content_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-06 22:03:33.000000 superpathlib-1.1.0/plib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-08-06 22:03:33.000000 superpathlib-1.1.0/plib/extra_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-06 22:03:33.000000 superpathlib-1.1.0/plib/metadata_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-06 22:03:33.000000 superpathlib-1.1.0/plib/override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-06 22:03:33.000000 superpathlib-1.1.0/plib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-06 22:03:33.000000 superpathlib-1.1.0/plib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-06 22:03:33.000000 superpathlib-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 22:03:44.415068 superpathlib-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:03:44.415068 superpathlib-1.1.0/superpathlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-08-06 22:03:44.000000 superpathlib-1.1.0/superpathlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-06 22:03:44.000000 superpathlib-1.1.0/superpathlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 22:03:44.000000 superpathlib-1.1.0/superpathlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-06 22:03:44.000000 superpathlib-1.1.0/superpathlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-06 22:03:44.000000 superpathlib-1.1.0/superpathlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:03:44.415068 superpathlib-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-06 22:03:33.000000 superpathlib-1.1.0/tests/test_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-06 22:03:33.000000 superpathlib-1.1.0/tests/test_encrypted_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-06 22:03:33.000000 superpathlib-1.1.0/tests/test_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-06 22:03:33.000000 superpathlib-1.1.0/tests/test_metadata.py
```

### Comparing `superpathlib-1.0.4/LICENSE` & `superpathlib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.4/PKG-INFO` & `superpathlib-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpathlib
-Version: 1.0.4
+Version: 1.1.0
 Summary: Extended Pathlib
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/superpathlib
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -72,14 +72,15 @@
 * find(): recursively find all paths under a root that match a condition (extra options available for performance optimization)
 * rmtree(): remove directory recursively
 * copy_to(dest): copy content to dest
 * copy_properties_to(dest): recursively copy path properties (mtime, tag) to all n-level children of dest
 * tempfile(): create temporary file that can be used as context manager
 * unpack(): extract archive(zip, tar, ..) file to desired folder
 * pop_parent(): remove first parent from path in filesystem
+* from_uri(): create path object from uri string
 
 examples: 
 
 ```shell
 with Path.tempfile() as tmp:
     do_work(logfile=tmp)
     log = tmp.text
@@ -94,22 +95,22 @@
 * Return default values when path does not exist (e.g. size = 0, lines=[])
 
 ### 6) Inherit from Path to define your own additional functionality:
 
 example: 
 
 ```shell
-from plib import Path as BasePath
+import plib
 
-class Path(BasePath):
+class Path(plib.Path):
     def count_children(self):
         return sum(1 for _ in self.iterdir())
 ```
 
-This only works if you inherit from plib and not from the builtin pathlib
+This only works if you inherit from plib Path, not the standard library pathlib Path
 
 
 ## Installation
 
 ```shell
 pip install superpathlib
 ```
```

### Comparing `superpathlib-1.0.4/README.md` & `superpathlib-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 * find(): recursively find all paths under a root that match a condition (extra options available for performance optimization)
 * rmtree(): remove directory recursively
 * copy_to(dest): copy content to dest
 * copy_properties_to(dest): recursively copy path properties (mtime, tag) to all n-level children of dest
 * tempfile(): create temporary file that can be used as context manager
 * unpack(): extract archive(zip, tar, ..) file to desired folder
 * pop_parent(): remove first parent from path in filesystem
+* from_uri(): create path object from uri string
 
 examples: 
 
 ```shell
 with Path.tempfile() as tmp:
     do_work(logfile=tmp)
     log = tmp.text
@@ -81,22 +82,22 @@
 * Return default values when path does not exist (e.g. size = 0, lines=[])
 
 ### 6) Inherit from Path to define your own additional functionality:
 
 example: 
 
 ```shell
-from plib import Path as BasePath
+import plib
 
-class Path(BasePath):
+class Path(plib.Path):
     def count_children(self):
         return sum(1 for _ in self.iterdir())
 ```
 
-This only works if you inherit from plib and not from the builtin pathlib
+This only works if you inherit from plib Path, not the standard library pathlib Path
 
 
 ## Installation
 
 ```shell
 pip install superpathlib
 ```
```

### Comparing `superpathlib-1.0.4/plib/tags.py` & `superpathlib-1.1.0/plib/tags.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 try:
-    import xattr
+    import xattr  # noqa
 
-except:
+
+except ModuleNotFoundError:
     xattr = None  # Don't fail if xattr not supported (Windows)
 
 delim = ","
 default_tag_name = "user.xdg.tags"
 
-"""
-More user-friendly way to interact with tags.
-- Work with strings and integers instead of bytes
-- Use xdg tags by default -> useful for filemanager that can order according to this tag
-"""
-
 
 class XDGTags:
+    """More user-friendly way to interact with tags.
+
+    - Work with strings and integers instead of bytes
+    - Use xdg tags by default ->
+        useful for filemanager that can order according to this tag
+    """
+
     def __init__(self, path, name=default_tag_name):
         self.tags = xattr.xattr(path) if xattr is not None else None
         self.name = name
 
     def get(self):
         tags = set({})
         if self.tags and self.tags.has_key(self.name):
             tags = self.tags[self.name].decode().strip().split(delim)
         return tags
 
-    def set(self, *values, name=default_tag_name):
+    def set(self, *values):
         """
         :param values: tag values to set
         """
         if self.tags is not None:
             values = {str(v).zfill(4) if isinstance(v, int) else str(v) for v in values}
             values = delim.join(values).encode()
             self.tags.set(self.name, values)
```

### Comparing `superpathlib-1.0.4/plib/utils.py` & `superpathlib-1.1.0/plib/utils.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.4/pyproject.toml` & `superpathlib-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "superpathlib"
-version = "1.0.4"
+version = "1.1.0"
 description = "Extended Pathlib"
 authors = [{name = "Quinten Roets", email = "qdr2104@columbia.edu"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = []
 
@@ -33,7 +33,10 @@
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
     "UP",  # pyupgrade
 ]
 fix = true
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]
```

### Comparing `superpathlib-1.0.4/superpathlib.egg-info/PKG-INFO` & `superpathlib-1.1.0/superpathlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpathlib
-Version: 1.0.4
+Version: 1.1.0
 Summary: Extended Pathlib
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/superpathlib
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -72,14 +72,15 @@
 * find(): recursively find all paths under a root that match a condition (extra options available for performance optimization)
 * rmtree(): remove directory recursively
 * copy_to(dest): copy content to dest
 * copy_properties_to(dest): recursively copy path properties (mtime, tag) to all n-level children of dest
 * tempfile(): create temporary file that can be used as context manager
 * unpack(): extract archive(zip, tar, ..) file to desired folder
 * pop_parent(): remove first parent from path in filesystem
+* from_uri(): create path object from uri string
 
 examples: 
 
 ```shell
 with Path.tempfile() as tmp:
     do_work(logfile=tmp)
     log = tmp.text
@@ -94,22 +95,22 @@
 * Return default values when path does not exist (e.g. size = 0, lines=[])
 
 ### 6) Inherit from Path to define your own additional functionality:
 
 example: 
 
 ```shell
-from plib import Path as BasePath
+import plib
 
-class Path(BasePath):
+class Path(plib.Path):
     def count_children(self):
         return sum(1 for _ in self.iterdir())
 ```
 
-This only works if you inherit from plib and not from the builtin pathlib
+This only works if you inherit from plib Path, not the standard library pathlib Path
 
 
 ## Installation
 
 ```shell
 pip install superpathlib
 ```
```

### Comparing `superpathlib-1.0.4/tests/test_encrypted_content.py` & `superpathlib-1.1.0/tests/test_encrypted_content.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.4/tests/test_functionality.py` & `superpathlib-1.1.0/tests/test_functionality.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,19 @@
     non_archive_assets = Path(__file__).parent / "assets" / "non_archives"
     assert not non_archive_assets.is_empty()
     for path in non_archive_assets.iterdir():
         path.unpack_if_archive(folder)
         assert folder.is_empty()
 
 
+def test_uri(path: Path):
+    uri = path.as_uri()
+    assert Path.from_uri(uri) == path
+
+
 @ignore_fixture_warning
 @byte_content
 def test_copy(path: Path, path2: Path, content: bytes):
     path.byte_content = content
     path.copy_to(path2)
     assert path2.byte_content == content
```

### Comparing `superpathlib-1.0.4/tests/test_metadata.py` & `superpathlib-1.1.0/tests/test_metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,28 +7,31 @@
 
 from plib import Path
 
 
 @ignore_fixture_warning
 @given(mtime=strategies.floats(min_value=0, max_value=time.time()))
 def test_mtime(path: Path, mtime: float):
+    assert isinstance(Path.mtime, property)
     path.mtime = mtime
     assert math.isclose(path.mtime, mtime, abs_tol=1e-3)
 
 
 @ignore_fixture_warning
 @given(content=text_strategy(blacklist_characters=","))
 def test_tag(path: Path, content: str):
+    assert isinstance(Path.tag, property)
     path.tag = content
     assert path.tag == content
 
 
 @ignore_fixture_warning
 @byte_content
 def test_size(path, content):
+    assert isinstance(Path.size, property)
     path.byte_content = content
     assert path.size == len(content)
 
 
 def test_filetypes(path):
     filetype_mappings = {"text": "txt", "video": "mp4", "image": "jpg"}
     for filetype, extension in filetype_mappings.items():
```

