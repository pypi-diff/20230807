# Comparing `tmp/typerconf-2.3.tar.gz` & `tmp/typerconf-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typerconf-2.3.tar", max compression
+gzip compressed data, was "typerconf-2.4.tar", max compression
```

## Comparing `typerconf-2.3.tar` & `typerconf-2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-2.3/LICENSE
--rw-r--r--   0        0        0     2907 2023-06-30 12:44:28.813745 typerconf-2.3/README.md
--rw-r--r--   0        0        0      934 2023-08-06 06:05:45.566209 typerconf-2.3/pyproject.toml
--rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-2.3/src/typerconf/.gitignore
--rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-2.3/src/typerconf/Makefile
--rw-r--r--   0        0        0    11100 2023-08-06 06:05:50.260873 typerconf-2.3/src/typerconf/__init__.py
--rw-r--r--   0        0        0    33580 2023-08-06 06:04:55.620408 typerconf-2.3/src/typerconf/init.nw
--rw-r--r--   0        0        0     4052 1970-01-01 00:00:00.000000 typerconf-2.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-2.4/LICENSE
+-rw-r--r--   0        0        0     2907 2023-06-30 12:44:28.813745 typerconf-2.4/README.md
+-rw-r--r--   0        0        0      934 2023-08-07 11:18:36.173295 typerconf-2.4/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-2.4/src/typerconf/.gitignore
+-rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-2.4/src/typerconf/Makefile
+-rw-r--r--   0        0        0    11340 2023-08-07 11:20:40.102338 typerconf-2.4/src/typerconf/__init__.py
+-rw-r--r--   0        0        0    33830 2023-08-07 11:18:36.173295 typerconf-2.4/src/typerconf/init.nw
+-rw-r--r--   0        0        0     4053 1970-01-01 00:00:00.000000 typerconf-2.4/PKG-INFO
```

### Comparing `typerconf-2.3/LICENSE` & `typerconf-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `typerconf-2.3/README.md` & `typerconf-2.4/README.md`

 * *Files identical despite different names*

### Comparing `typerconf-2.3/pyproject.toml` & `typerconf-2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typerconf"
-version = "2.3"
+version = "2.4"
 description = "Library to read and write configs using API and CLI with Typer"
 authors = ["Daniel Bosk <daniel@bosk.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbosk/typerconf"
 keywords = ["typer", "conf", "config", "git-like", "config lib", "write conf"]
 classifiers = [
@@ -19,15 +19,15 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/dbosk/typerconf/issues"
 "Releases" = "https://github.com/dbosk/typerconf/releases"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 appdirs = "^1.4.4"
-typer = "^0.7.0"
+typer = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `typerconf-2.3/src/typerconf/__init__.py` & `typerconf-2.4/src/typerconf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """The typerconf module and config subcommand"""
 
 import appdirs
 import io
 import json
 import logging
 import os
+import pathlib
 import sys
 import typer
 import typing
+from typing_extensions import Annotated
 
 normalized_path = os.path.normpath(sys.argv[0])
 basename = os.path.basename(normalized_path)
 dirs = appdirs.AppDirs(basename)
 
 class Config:
   """Navigates nested JSON structures by dot-separated addressing."""
 
-  def __init__(self, json_data=None,
+  def __init__(self, json_data: dict = None,
                      conf_file=None):
     """
     Constructs a config object to navigate from JSON data `json_data`.
 
     `conf_file` takes a path to a file which will be used as a config file. If this 
     argument is supplied, the data will be read from the file.
 
@@ -122,15 +124,15 @@
         del structure[part]
       except KeyError:
         pass
     else:
       structure[part] = value
     if self.__conf_file:
       self.write_config(self.__conf_file)
-  def paths(self, from_root=""):
+  def paths(self, from_root: str = ""):
     """
     Returns all existing paths.
 
     The optional argument `from_root` is a path and the method return all 
     subpaths rooted at that point.
     """
     paths = []
@@ -145,16 +147,18 @@
 
         paths.append(path)
         paths += self.paths(from_root=path)
     elif isinstance(root, list):
       paths += [f"{from_root}.{x}" for x in range(len(root))]
 
     return paths
-  def read_config(self, conf_file=f"{dirs.user_config_dir}/config.json",
-                        writeback=False):
+  def read_config(self,
+                  conf_file: pathlib.Path =
+                    f"{dirs.user_config_dir}/config.json",
+                  writeback=False):
     """
     Reads the config data structure (JSON) into the Config object.
 
     `conf_file` is an optional argument providing one of the following:
     - an already opened file object (anything derived from `io.IOBase`);
     - anything that `open` can handle, for instance:
       - a string, which is the path to the config file;
@@ -202,15 +206,17 @@
         try:
           self.__conf_file = conf_file.name
         except AttributeError:
           raise ValueError(f"can't enable writeback when `conf_file` is "
                            f"a file-like object without a name: {conf_file}")
       else:
         self.__conf_file = conf_file
-  def write_config(self, conf_file=f"{dirs.user_config_dir}/config.json"):
+  def write_config(self,
+                   conf_file: pathlib.Path =
+                    f"{dirs.user_config_dir}/config.json"):
     """
     Stores the config data (as JSON) in the config file.
     `conf_file` is an optional argument providing one of the following:
     - an already opened file object (anything derived from `io.IOBase`);
     - anything that `open` can handle, for instance:
       - a string, which is the path to the config file;
       - an integer, which is a file descriptor (see `os.open`).
@@ -235,59 +241,59 @@
     if conf_path:
       conf.read_config(conf_path)
     else:
       conf.read_config()
   except ValueError:
     pass
 
-  path_arg = typer.Argument("",
-                            help="Path in config, e.g. 'courses.datintro22'. "
+  path_arg = typer.Argument(help="Path in config, e.g. 'courses.datintro22'. "
                                  "Empty string is root of config. Defaults to "
                                  "the empty string.",
                             autocompletion=complete_path_callback)
-  value_arg = typer.Option([], "-s", "--set",
+  value_arg = typer.Option("-s", "--set",
                            help="Values to store. "
                                 "More than one value makes a list. "
                                 "Values are treated as JSON if possible.")
 
   @cli.command(name="config")
-  def config_cmd(path: str = path_arg,
-                 values: typing.List[str] = value_arg):
+  def config_cmd(path: Annotated[str, path_arg] = "",
+                 values: Annotated[typing.List[str], value_arg] = []):
     """
     Reads values from or writes values to the config.
     """
     if values:
       if len(values) == 1:
         values = values[0]
       if values == "":
         values = None
       conf.set(path, values)
     else:
       print_config(conf.get(path), path)
-def merge_dictionaries(dir1, dir2):
+def merge_dictionaries(dict1: dict, dict2: dict):
   """
   Returns a copy of dir1 with values in dir1 updated from dir2 for keys that 
   exist. Keys that exist in dir2 are created in dir, with the proper values.
 
   The merge recurses through values that are dictionaries, which makes this 
   different from `dir1 | dir2` and `{**dir1, **dir2}`. Using those would replace 
   entire subdictionaries instead of merging them.
   """
-  dir = dir1.copy()
+  new_dict = dict1.copy()
 
-  for key, value in dir2.items():
+  for key, value in dict2.items():
     try:
-      if isinstance(value, dict) and isinstance(current_value := dir[key], dict):
-        dir[key] = merge_dictionaries(current_value, value)
+      if isinstance(value, dict) and \
+          isinstance(current_value := new_dict[key], dict):
+        new_dict[key] = merge_dictionaries(current_value, value)
       else:
-        dir[key] = value
+        new_dict[key] = value
     except KeyError:
-      dir[key] = value
+      new_dict[key] = value
 
-  return dir
+  return new_dict
 def get(path: str = "") -> typing.Any:
   """
   Returns the value stored at `path` in the config.
 
   By default, `path = ""`, which returns the entire configuration as a Config 
   object.
   """
@@ -315,15 +321,15 @@
   if not conf:
     conf = Config(get())
 
   return filter(lambda x: x.startswith(initial_path),
                 conf.paths())
 def complete_path_callback(initial_path: str):
   return complete_path(initial_path)
-def print_config(conf, path=""):
+def print_config(conf: Config, path: str = ""):
   """
   Prints the config tree contained in `conf` to stdout.
   Optional `path` is prepended.
   """
   try:
     for key in conf.keys():
       if path:
```

### Comparing `typerconf-2.3/src/typerconf/init.nw` & `typerconf-2.4/src/typerconf/init.nw`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 """The typerconf module and config subcommand"""
 
 import appdirs
 import io
 import json
 import logging
 import os
+import pathlib
 import sys
 import typer
 import typing
+from typing_extensions import Annotated
 
 <<set up appdirs dirs>>
 
 <<classes>>
 <<helper functions>>
 
 def main():
@@ -119,15 +121,15 @@
 This class has two methods that are central:
 The first gets a value out, the other sets a value in.
 Both work with these dot-separated addresses.
 <<classes>>=
 class Config:
   """Navigates nested JSON structures by dot-separated addressing."""
 
-  def __init__(self, json_data=None,
+  def __init__(self, json_data: dict = None,
                      <<Config constructor args>>):
     """
     Constructs a config object to navigate from JSON data `json_data`.
 
     <<Config constructor args doc>>
     """
     if not json_data:
@@ -386,15 +388,15 @@
 @
 
 \subsection{Listing all existing paths}
 
 Lastly, what we want to do is to create a list containing all paths in the 
 config.
 <<Config methods for available paths>>=
-def paths(self, from_root=""):
+def paths(self, from_root: str = ""):
   """
   Returns all existing paths.
 
   The optional argument `from_root` is a path and the method return all 
   subpaths rooted at that point.
   """
   <<return list of all paths>>
@@ -453,16 +455,18 @@
 
 \subsubsection{Reading the config}
 
 Let's start with reading.
 Anything that is derived from [[io.IOBase]] is already opened.
 Anything else, we pass to [[open]] to handle.
 <<Config methods for reading from and writing to file>>=
-def read_config(self, conf_file=f"{dirs.user_config_dir}/config.json",
-                      <<additional [[read_config]] args>>):
+def read_config(self,
+                conf_file: pathlib.Path =
+                  f"{dirs.user_config_dir}/config.json",
+                <<additional [[read_config]] args>>):
   """
   Reads the config data structure (JSON) into the Config object.
 
   <<[[conf_file]] argument doc>>
 
   <<additional [[read_config]] args doc>>
 
@@ -528,43 +532,44 @@
 Returns a copy of dir1 with values in dir1 updated from dir2 for keys that 
 exist. Keys that exist in dir2 are created in dir, with the proper values.
 
 The merge recurses through values that are dictionaries, which makes this 
 different from `dir1 | dir2` and `{**dir1, **dir2}`. Using those would replace 
 entire subdictionaries instead of merging them.
 <<helper functions>>=
-def merge_dictionaries(dir1, dir2):
+def merge_dictionaries(dict1: dict, dict2: dict):
   """
   <<merge dir doc>>
   """
-  dir = dir1.copy()
+  new_dict = dict1.copy()
 
-  for key, value in dir2.items():
-    <<update [[dir[key]]] with value>>
+  for key, value in dict2.items():
+    <<update [[new_dict[key]]] with value>>
 
-  return dir
+  return new_dict
 @
 
 To do the update, we need to check if [[value]] is a (sub)dictionary.
-However, we also need to check if [[dir[key]]] is a dictionary.
+However, we also need to check if [[new_dict[key]]] is a dictionary.
 If both are dictionaries, we should merge.
 Otherwise, we simply replace.
 
-To not have to read out [[dir[key]]] too many times, we use the walrus operator 
+To not have to read out [[new_dict[key]]] too many times, we use the walrus operator 
 to store its value in [[current_value]].
 And since we place it after the [[and]] in the conditional, we only read it 
 when absolutely necessary.
-<<update [[dir[key]]] with value>>=
+<<update [[new_dict[key]]] with value>>=
 try:
-  if isinstance(value, dict) and isinstance(current_value := dir[key], dict):
-    dir[key] = merge_dictionaries(current_value, value)
+  if isinstance(value, dict) and \
+      isinstance(current_value := new_dict[key], dict):
+    new_dict[key] = merge_dictionaries(current_value, value)
   else:
-    dir[key] = value
+    new_dict[key] = value
 except KeyError:
-  dir[key] = value
+  new_dict[key] = value
 @
 
 Let's test this.
 <<test functions>>=
 def test_merge_dictionaries():
   a = {"a": 1, "b": {"c": 3}}
   b = {"a": 2, "b": {"d": 4}}
@@ -660,15 +665,17 @@
 @
 
 \subsubsection{Writing the config}
 
 Conversely, we want to write the data to the config file as well.
 We do the same things as above, but open for writing instead.
 <<Config methods for reading from and writing to file>>=
-def write_config(self, conf_file=f"{dirs.user_config_dir}/config.json"):
+def write_config(self,
+                 conf_file: pathlib.Path =
+                  f"{dirs.user_config_dir}/config.json"):
   """
   Stores the config data (as JSON) in the config file.
   <<[[conf_file]] argument doc>>
   """
   if isinstance(conf_file, io.IOBase):
     <<write the data from [[self.__data]]>>
   else:
@@ -923,16 +930,16 @@
     conf.read_config()
 except ValueError:
   pass
 
 <<default values for [[config_cmd]]>>
 
 @cli.command(name="config")
-def config_cmd(path: str = path_arg,
-               values: typing.List[str] = value_arg):
+def config_cmd(path: Annotated[str, path_arg] = "",
+               values: Annotated[typing.List[str], value_arg] = []):
   """
   Reads values from or writes values to the config.
   """
   if values:
     <<change [[values]] to non-list if one-element list>>
     <<if [[values]] is empty string, replace it with [[None]]>>
     conf.set(path, values)
@@ -941,20 +948,19 @@
 @
 
 The default values are the special Typer objects that specify how the command 
 arguments and options should behave.
 We can autocomplete the path since we can predict the possible values.
 The same cannot be said of the value to store, that can be arbitrary.
 <<default values for [[config_cmd]]>>=
-path_arg = typer.Argument("",
-                          help="Path in config, e.g. 'courses.datintro22'. "
+path_arg = typer.Argument(help="Path in config, e.g. 'courses.datintro22'. "
                                "Empty string is root of config. Defaults to "
                                "the empty string.",
                           autocompletion=complete_path_callback)
-value_arg = typer.Option([], "-s", "--set",
+value_arg = typer.Option("-s", "--set",
                          help="Values to store. "
                               "More than one value makes a list. "
                               "Values are treated as JSON if possible.")
 @
 
 If the user supplies only one argument on the command line, we don't want it to 
 be interpreted as a one-element list, but rather as a value that is not a list.
@@ -1096,15 +1102,15 @@
 [[courses.datintro22.url = https://...]].
 This function will do a depth-first traversal through the config to print all 
 values.
 The idea is that the config path will move from the dictionary representation 
 in [[conf]] to the string representation in [[path]].
 When at the leaf, [[conf]] will contain the value and [[path]] the entire path.
 <<helper functions>>=
-def print_config(conf, path=""):
+def print_config(conf: Config, path: str = ""):
   """
   Prints the config tree contained in `conf` to stdout.
   Optional `path` is prepended.
   """
   try:
     for key in conf.keys():
       <<recurse deeper into the config tree>>
```

### Comparing `typerconf-2.3/PKG-INFO` & `typerconf-2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typerconf
-Version: 2.3
+Version: 2.4
 Summary: Library to read and write configs using API and CLI with Typer
 Home-page: https://github.com/dbosk/typerconf
 License: MIT
 Keywords: typer,conf,config,git-like,config lib,write conf
 Author: Daniel Bosk
 Author-email: daniel@bosk.se
 Requires-Python: >=3.7,<4.0
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/dbosk/typerconf/issues
 Project-URL: Repository, https://github.com/dbosk/typerconf
 Project-URL: Releases, https://github.com/dbosk/typerconf/releases
 Description-Content-Type: text/markdown
 
 The configuration is a JSON structure. We'll use the following for the
 coming examples.
```

