# Comparing `tmp/tko-0.0.3.tar.gz` & `tmp/tko-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tko-0.0.3.tar", last modified: Sat Aug  5 18:54:53 2023, max compression
+gzip compressed data, was "tko-0.0.4.tar", last modified: Sun Aug  6 17:42:57 2023, max compression
```

## Comparing `tko-0.0.3.tar` & `tko-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-05 18:54:53.059576 tko-0.0.3/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.0.3/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.0.3/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     1137 2023-08-05 18:54:53.059576 tko-0.0.3/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      422 2023-08-05 18:49:31.000000 tko-0.0.3/README.md
--rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.0.3/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2023-08-05 18:54:53.059576 tko-0.0.3/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3982 2023-08-05 15:02:11.000000 tko-0.0.3/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-05 18:54:53.046242 tko-0.0.3/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-05 18:54:53.052909 tko-0.0.3/src/tko/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2023-08-05 18:54:13.000000 tko-0.0.3/src/tko/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     6596 2023-08-05 18:09:28.000000 tko-0.0.3/src/tko/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3330 2023-08-05 18:23:50.000000 tko-0.0.3/src/tko/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3569 2023-08-05 17:47:30.000000 tko-0.0.3/src/tko/basic.py
--rw-r--r--   0 lion      (1000) lion      (1000)     6767 2023-08-05 17:57:03.000000 tko-0.0.3/src/tko/diff.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5186 2023-08-05 17:51:49.000000 tko-0.0.3/src/tko/down.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4684 2023-08-05 16:55:34.000000 tko-0.0.3/src/tko/format.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8151 2023-08-05 18:09:28.000000 tko-0.0.3/src/tko/loader.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.0.3/src/tko/pattern.py
--rw-r--r--   0 lion      (1000) lion      (1000)      594 2023-08-05 17:03:33.000000 tko-0.0.3/src/tko/runner.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1222 2023-08-05 16:47:30.000000 tko-0.0.3/src/tko/settings.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5223 2023-08-05 17:49:27.000000 tko-0.0.3/src/tko/solver.py
--rw-r--r--   0 lion      (1000) lion      (1000)     6480 2023-08-05 17:50:47.000000 tko-0.0.3/src/tko/wdir.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3174 2023-08-05 18:09:28.000000 tko-0.0.3/src/tko/writer.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-05 18:54:53.056242 tko-0.0.3/src/tko.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     1137 2023-08-05 18:54:53.000000 tko-0.0.3/src/tko.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      506 2023-08-05 18:54:53.000000 tko-0.0.3/src/tko.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2023-08-05 18:54:53.000000 tko-0.0.3/src/tko.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       47 2023-08-05 18:54:53.000000 tko-0.0.3/src/tko.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       59 2023-08-05 18:54:53.000000 tko-0.0.3/src/tko.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        4 2023-08-05 18:54:53.000000 tko-0.0.3/src/tko.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-06 17:42:57.477199 tko-0.0.4/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.0.4/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.0.4/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     1137 2023-08-06 17:42:57.477199 tko-0.0.4/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      422 2023-08-05 18:49:31.000000 tko-0.0.4/README.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.0.4/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2023-08-06 17:42:57.480532 tko-0.0.4/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3982 2023-08-05 15:02:11.000000 tko-0.0.4/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-06 17:42:57.447198 tko-0.0.4/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-06 17:42:57.470532 tko-0.0.4/src/tko/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2023-08-06 17:42:17.000000 tko-0.0.4/src/tko/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     6592 2023-08-06 17:36:37.000000 tko-0.0.4/src/tko/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3329 2023-08-06 15:03:29.000000 tko-0.0.4/src/tko/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3572 2023-08-06 15:04:48.000000 tko-0.0.4/src/tko/basic.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     6768 2023-08-06 15:04:48.000000 tko-0.0.4/src/tko/diff.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5207 2023-08-06 16:57:34.000000 tko-0.0.4/src/tko/down.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4777 2023-08-06 17:37:09.000000 tko-0.0.4/src/tko/format.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8151 2023-08-05 18:09:28.000000 tko-0.0.4/src/tko/loader.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.0.4/src/tko/pattern.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      594 2023-08-05 17:03:33.000000 tko-0.0.4/src/tko/runner.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2024 2023-08-06 17:33:48.000000 tko-0.0.4/src/tko/settings.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5215 2023-08-06 15:10:51.000000 tko-0.0.4/src/tko/solver.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     6530 2023-08-06 15:10:51.000000 tko-0.0.4/src/tko/wdir.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3174 2023-08-05 18:09:28.000000 tko-0.0.4/src/tko/writer.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-06 17:42:57.477199 tko-0.0.4/src/tko.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1137 2023-08-06 17:42:57.000000 tko-0.0.4/src/tko.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      506 2023-08-06 17:42:57.000000 tko-0.0.4/src/tko.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2023-08-06 17:42:57.000000 tko-0.0.4/src/tko.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       47 2023-08-06 17:42:57.000000 tko-0.0.4/src/tko.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       59 2023-08-06 17:42:57.000000 tko-0.0.4/src/tko.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        4 2023-08-06 17:42:57.000000 tko-0.0.4/src/tko.egg-info/top_level.txt
```

### Comparing `tko-0.0.3/LICENSE` & `tko-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tko-0.0.3/PKG-INFO` & `tko-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tko
-Version: 0.0.3
+Version: 0.0.4
 Summary: tko: Test Engine for Judge Operations
 Home-page: https://github.com/senapk/tko
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/tko/issues
 Project-URL: Source, https://github.com/senapk/tko/
 Keywords: programming,learning
```

### Comparing `tko-0.0.3/setup.py` & `tko-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `tko-0.0.3/src/tko/__main__.py` & `tko-0.0.4/src/tko/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# Console scripts
+from __future__ import annotations
 
 import argparse
 import sys
 
+
 from .actions import Actions
 from .basic import Param
 from .pattern import PatternLoader
 from .basic import DiffMode
 from .format import Report
 from .down import Down
 from .settings import SettingsParser
+from .__init__ import __version__
 
 
 class Main:
     @staticmethod
     def execute(args):
         Actions.exec(args.target_list)
 
@@ -44,14 +46,17 @@
         PatternLoader.pattern = args.pattern
         manip = Param.Manip().set_unlabel(args.unlabel).set_to_sort(args.sort).set_to_number(args.number)
         Actions.build(args.target, args.target_list, manip, args.force)
     
     @staticmethod
     def settings(args):
         print("settings file at " + SettingsParser().get_settings_file())
+        if (args.ascii):
+            SettingsParser().toggle_ascii()
+            print("Initializing symbols... in " + ("ASCII" if SettingsParser().get_ascii() else "UTF-8"))
 
     # @staticmethod
     # def rebuild(args):
     #     if args.width is not None:
     #         Report.set_terminal_size(args.width)
     #     PatternLoader.pattern = args.pattern
     #     manip = Param.Manip().set_unlabel(args.unlabel).set_to_sort(args.sort).set_to_number(args.number)
@@ -66,29 +71,30 @@
     def down(args):
         destiny = Down.create_problem_folder(args.disc, args.index, args.extension)
         Down.entry_unpack(destiny, args.disc, args.index, args.extension)
 
     @staticmethod
     def main():
         parent_basic = argparse.ArgumentParser(add_help=False)
-        # parent_basic.add_argument('--version', '-v', action='version', help='show version.')
         parent_basic.add_argument('--width', '-w', type=int, help="term width")
         parent_basic.add_argument('--index', '-i', metavar="I", type=int, help='run a specific index.')
         parent_basic.add_argument('--pattern', '-p', metavar="P", type=str, default='@.in @.sol',
                                   help='pattern load/save a folder, default: "@.in @.sol"')
 
         parent_manip = argparse.ArgumentParser(add_help=False)
         parent_manip.add_argument('--width', '-w', type=int, help="term width.")
         parent_manip.add_argument('--unlabel', '-u', action='store_true', help='remove all labels.')
         parent_manip.add_argument('--number', '-n', action='store_true', help='number labels.')
         parent_manip.add_argument('--sort', '-s', action='store_true', help="sort test cases by input size.")
         parent_manip.add_argument('--pattern', '-p', metavar="@.in @.out", type=str, default='@.in @.sol',
                                   help='pattern load/save a folder, default: "@.in @.sol"')
 
         parser = argparse.ArgumentParser(prog='tko', description='A tool for competitive programming.')
+        parser.add_argument('--version', '-v', action='store_true', help='show version.')
+        
         subparsers = parser.add_subparsers(title='subcommands', help='help for subcommand.')
 
         # list
         parser_l = subparsers.add_parser('list', parents=[parent_basic], help='show case packs or folders.')
         parser_l.add_argument('target_list', metavar='T', type=str, nargs='*', help='targets.')
         parser_l.set_defaults(func=Main.list)
 
@@ -107,38 +113,35 @@
         # build
         parser_b = subparsers.add_parser('build', parents=[parent_manip], help='build a test target.')
         parser_b.add_argument('target', metavar='T_OUT', type=str, help='target to be build.')
         parser_b.add_argument('target_list', metavar='T', type=str, nargs='+', help='input test targets.')
         parser_b.add_argument('--force', '-f', action='store_true', help='enable overwrite.')
         parser_b.set_defaults(func=Main.build)
 
-        # # rebuild
-        # parser_rb = subparsers.add_parser('rebuild', parents=[parent_manip], help='rebuild a test target.')
-        # parser_rb.add_argument('target_list', metavar='T', type=str, nargs='+', help='input test targets.')
-        # parser_rb.add_argument('--cmd', '-c', type=str, help="solver file or command to update outputs.")
-        # parser_rb.set_defaults(func=Main.rebuild)
-
         # down
         parser_d = subparsers.add_parser('down', help='download test from remote repository.')
         parser_d.add_argument('disc', type=str, help=" [ fup | ed | poo ]")
         parser_d.add_argument('index', type=str, help="3 digits label like 021")
-        parser_d.add_argument('extension', type=str, nargs = '?', default = "-", help="[ c | cpp | js | ts | py | java ]")
+        parser_d.add_argument('extension', type=str, nargs='?', default="-", help="[ c | cpp | js | ts | py | java ]")
         parser_d.set_defaults(func=Main.down)
 
         # update
         parser_u = subparsers.add_parser('update', help='update problem from repository.')
         parser_u.set_defaults(func=Main.update)
 
         # settings
         parser_s = subparsers.add_parser('settings', help='show settings.')
+        parser_s.add_argument('--ascii', '-a', action='store_true', help='toggle ascii mode.')
         parser_s.set_defaults(func=Main.settings)
 
         args = parser.parse_args()
         if len(sys.argv) == 1:
             print("You must call a subcommand. Use --help for more information.")
+        elif args.version:
+            print("tko version " + __version__)
         else:
             try:
                 args.func(args)
             except ValueError as e:
                 print(str(e))
```

### Comparing `tko-0.0.3/src/tko/actions.py` & `tko-0.0.4/src/tko/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from .diff import Diff
 from .format import Symbol, Colored, Color, Report
 from .writer import Writer
 from .solver import Solver
 from .runner import Runner
 
 
-
 class Execution:
 
     def __init__(self):
         pass
 
     # run a unit using a solver and return if the result is correct
     @staticmethod
```

### Comparing `tko-0.0.3/src/tko/basic.py` & `tko-0.0.4/src/tko/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 from typing import Optional
 
 import os
 
 
 from .format import Symbol
 
+
 class ExecutionResult(Enum):
     UNTESTED = Symbol.neutral
     SUCCESS = Symbol.success
     WRONG_OUTPUT = Symbol.failure
     COMPILATION_ERROR = Symbol.compilation
     EXECUTION_ERROR = Symbol.execution
 
     def __str__(self):
         return self.value
 
+
 class CompilerError(Exception):
     pass
 
 
 class DiffMode(Enum):
     FIRST = "MODE: SHOW FIRST FAILURE ONLY"
     QUIET = "MODE: SHOW NONE FAILURES"
@@ -57,15 +59,15 @@
         self.source_pad = 0  # stores the pad to justify the source file
         self.case = case  # name
         self.case_pad = 0  # stores the pad to justify the case name
         self.input = inp  # input
         self.output = outp  # expected output
         self.user: Optional[str] = None  # solver generated answer
         self.grade: Optional[int] = grade  # None represents proportional gr, 100 represents all
-        self.grade_reduction: int = 0 # if grade is None, this atribute should be filled with the right grade reduction
+        self.grade_reduction: int = 0  # if grade is None, this atribute should be filled with the right grade reduction
         self.index = 0
         self.repeated: Optional[int] = None
 
         self.result: ExecutionResult = ExecutionResult.UNTESTED
 
     def __str__(self):
         index = str(self.index).zfill(2)
```

### Comparing `tko-0.0.3/src/tko/diff.py` & `tko-0.0.4/src/tko/diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, Optional, Tuple
 import io
 
 from .format import Symbol, Colored, Color, Report
 from .basic import Unit
 
+
 class Diff:
 
     @staticmethod
     def render_white(text: Optional[str], color: Optional[Color] = None) -> Optional[str]:
         if text is None:
             return None
         if color is None:
```

### Comparing `tko-0.0.3/src/tko/down.py` & `tko-0.0.4/src/tko/down.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import urllib.request
 import urllib.error
 import json
 
 from .settings import SettingsParser
 
+
 class Down:
 
     @staticmethod
     def update():
         if os.path.isfile(".info"):
             data = open(".info", "r").read().split("\n")[0]
             data = data.split(" ")
@@ -36,15 +37,14 @@
         for entry in loaded["keep"]:
             Down.compare_and_save(entry["contents"], os.path.join(destiny, entry["name"]))
 
         for entry in loaded["required"]:
             path = os.path.join(destiny, entry["name"])
             Down.compare_and_save(entry["contents"], path)
 
-
     @staticmethod
     def compare_and_save(content, path):
         if not os.path.exists(path):
             with open(path, "w") as f:
                 f.write(content)
             print(path + " (New)")
         else:
@@ -68,15 +68,15 @@
         return readme, mapi
 
     @staticmethod
     def create_problem_folder(disc, index, ext):
         # create dir
         destiny = disc + "@" + index
         if not os.path.exists(destiny):
-            os.mkdir(destiny)
+            os.makedirs(destiny, exist_ok=True)
         else:
             print("problem folder", destiny, "found, merging content.")
 
         # saving problem info on folder
         info_file = os.path.join(destiny, ".info")
         with open(info_file, "w") as f:
             f.write(disc + " " + index + " " + ext + "\n")
@@ -90,37 +90,37 @@
             return
         
         index_url = discp_url + index + "/"
         cache_url = index_url + ".cache/"
         
         # downloading Readme
         try:
-            [readme_path, mapi_path] = Down.down_problem_def(destiny, cache_url)
+            [_readme_path, mapi_path] = Down.down_problem_def(destiny, cache_url)
         except urllib.error.HTTPError:
             print("Problem not found")
             return
 
         with open(mapi_path) as f:
             loaded_json = json.load(f)
         os.remove(mapi_path)
         Down.unpack_json(loaded_json, destiny)
 
-        if len(loaded_json["required"]) == 1: # you already have the students file
+        if len(loaded_json["required"]) == 1:  # you already have the students file
             return
 
         # creating source file for student
-        # search if exists a draft file for the extension choosed
+        # search if exists a draft file for the extension choosen
         if ext == "-":
             return
 
         try:
             draft_path = os.path.join(destiny, "draft." + ext)
             urllib.request.urlretrieve(cache_url + "draft." + ext, draft_path)
             print(draft_path + " (Draft) Rename before modify.")
-        except urllib.error.HTTPError: # draft not found
+        except urllib.error.HTTPError:  # draft not found
             filename = "Solver." if ext == "java" else "solver."
             draft_path = os.path.join(destiny, filename + ext)
             if not os.path.exists(draft_path):
                 with open(draft_path, "w") as f:
                     f.write("")
                 print(draft_path, "(Empty)")
```

### Comparing `tko-0.0.3/src/tko/format.py` & `tko-0.0.4/src/tko/format.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from typing import Optional
 import shutil
 
 from enum import Enum
 from typing import Optional
-
-asc2only: bool = False
+from .settings import SettingsParser
 
 class Color(Enum):
     RED = 1
     GREEN = 2
     YELLOW = 3
     BLUE = 4
     MAGENTA = 5
     CYAN = 6
     WHITE = 7
     RESET = 8
     BOLD = 9
     ULINE = 10
 
+
 class Colored:
     __map = {
-        Color.RED     : '\u001b[31m',
-        Color.GREEN   : '\u001b[32m',
-        Color.YELLOW  : '\u001b[33m',
-        Color.BLUE    : '\u001b[34m',
-        Color.MAGENTA : '\u001b[35m',
-        Color.CYAN    : '\u001b[36m',
-        Color.WHITE   : '\u001b[37m',
-        Color.RESET   : '\u001b[0m',
-        Color.BOLD    : '\u001b[1m',
-        Color.ULINE   : '\u001b[4m'
+        Color.RED: '\u001b[31m',
+        Color.GREEN: '\u001b[32m',
+        Color.YELLOW: '\u001b[33m',
+        Color.BLUE: '\u001b[34m',
+        Color.MAGENTA: '\u001b[35m',
+        Color.CYAN: '\u001b[36m',
+        Color.WHITE: '\u001b[37m',
+        Color.RESET: '\u001b[0m',
+        Color.BOLD: '\u001b[1m',
+        Color.ULINE: '\u001b[4m'
     }
 
     @staticmethod
     def paint(text: str, color: Color, color2: Optional[Color] = None) -> str:
-        return Colored.__map[color] + ("" if color2 is None else Colored.__map[color2]) + text + Colored.__map[Color.RESET]
+        return (Colored.__map[color] + ("" if color2 is None else Colored.__map[color2])
+                + text + Colored.__map[Color.RESET])
 
     @staticmethod
     def green(text: str) -> str:
         return Colored.paint(text, Color.GREEN)
     
     @staticmethod
     def red(text: str) -> str:
@@ -57,72 +57,74 @@
         return Colored.paint(text, Color.BLUE)
 
     @staticmethod
     def ljust(text: str, width: int) -> str:
         return text + ' ' * (width - Colored.len(text))
 
     @staticmethod
-    def center(text: str, width: int, filler) -> str:
+    def center(text: str, width: int, filler: str) -> str:
         return filler * ((width - Colored.len(text)) // 2) + text + filler * ((width - Colored.len(text) + 1) // 2)
 
     @staticmethod
     def remove_colors(text: str) -> str:
         for color in Colored.__map.values():
             text = text.replace(color, '')
         return text
 
     @staticmethod
     def len(text):
         return len(Colored.remove_colors(text))
 
+
 class Symbol:
     opening = "=>"
     neutral = ""
     success = ""
     failure = ""
     wrong = ""
     compilation = ""
     execution = ""
     unequal = ""
-    equalbar= ""
+    equalbar = ""
     hbar = "─"
     vbar = "│"
     whitespace = "\u2E31"  # interpunct
     newline = "\u21B5"  # carriage return
     cfill = "_"
     tab = "    "
 
     def __init__(self):
         pass
 
     @staticmethod
-    def initialize(asc2only: bool):
-        Symbol.neutral = "." if asc2only else "»"  # u"\u2610"  # ☐
-        Symbol.success = "S" if asc2only else "✓"
-        Symbol.failure = "X" if asc2only else "✗"
-        Symbol.wrong = "W" if asc2only else "ω"
-        Symbol.compilation = "C" if asc2only else "ϲ"
-        Symbol.execution = "E" if asc2only else "ϵ"
-        Symbol.unequal = "#" if asc2only else "≠"
-        Symbol.equalbar = "|" if asc2only else "│"
+    def initialize(_asc2only: bool):
+        # print("Initializing symbols... in " + ("ASCII" if _asc2only else "UTF-8"))
+        Symbol.neutral = "." if _asc2only else "»"  # u"\u2610"  # ☐
+        Symbol.success = "S" if _asc2only else "✓"
+        Symbol.failure = "X" if _asc2only else "✗"
+        Symbol.wrong = "W" if _asc2only else "ω"
+        Symbol.compilation = "C" if _asc2only else "ϲ"
+        Symbol.execution = "E" if _asc2only else "ϵ"
+        Symbol.unequal = "#" if _asc2only else "≠"
+        Symbol.equalbar = "|" if _asc2only else "│"
 
         Symbol.opening = Colored.paint(Symbol.opening, Color.BLUE)
         Symbol.neutral = Colored.paint(Symbol.neutral, Color.BLUE)
 
         Symbol.success = Colored.paint(Symbol.success, Color.GREEN)
         Symbol.failure = Colored.paint(Symbol.failure, Color.RED)
         
         # Symbol.wrong       = Colored.paint(Symbol.wrong,       Color.RED)
         Symbol.compilation = Colored.paint(Symbol.compilation, Color.YELLOW)
         Symbol.execution = Colored.paint(Symbol.execution,   Color.YELLOW)
         Symbol.unequal = Colored.paint(Symbol.unequal,     Color.RED)
         Symbol.equalbar = Colored.paint(Symbol.equalbar,    Color.GREEN)
 
 
-Symbol.initialize(asc2only)  # inicalizacao estatica
+Symbol.initialize(SettingsParser().get_ascii())  # inicalizacao estatica
 
 
 class Report:
     __term_width: Optional[int] = None
 
     def __init__(self):
         pass
```

### Comparing `tko-0.0.3/src/tko/loader.py` & `tko-0.0.4/src/tko/loader.py`

 * *Files identical despite different names*

### Comparing `tko-0.0.3/src/tko/pattern.py` & `tko-0.0.4/src/tko/pattern.py`

 * *Files identical despite different names*

### Comparing `tko-0.0.3/src/tko/runner.py` & `tko-0.0.4/src/tko/runner.py`

 * *Files identical despite different names*

### Comparing `tko-0.0.3/src/tko/settings.py` & `tko-0.0.4/src/tko/settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import os
 import configparser
 from appdirs import user_data_dir
 
+
 class SettingsParser:
 
     default_cfg_content = """[REP]
 fup = https://raw.githubusercontent.com/qxcodefup/arcade/master/base/
 ed = https://raw.githubusercontent.com/qxcodeed/arcade/master/base/
 poo = https://raw.githubusercontent.com/qxcodepoo/arcade/master/base/
+
+[VISUAL]
+ascii = False
 """
 
     def __init__(self):
         self.package_name = "tko"
         self.filename = "settings.cfg"
         self.settings_dir = user_data_dir(self.package_name)
         self.settings_file = os.path.join(self.settings_dir, self.filename)
@@ -21,15 +25,36 @@
             self.create_default_settings_file()
         parser = configparser.ConfigParser()
         parser.read(self.settings_file)
         return parser["REP"][disc]
 
     def create_default_settings_file(self):
         if not os.path.isdir(self.settings_dir):
-            os.mkdir(self.settings_dir)
+            os.makedirs(self.settings_dir, exist_ok=True)
         with open(self.settings_file, "w") as f:
             f.write(self.default_cfg_content)
 
-    def get_settings_file(self):
+    def check_settings_file(self):
         if not os.path.isfile(self.settings_file):
             self.create_default_settings_file()
+        parser = configparser.ConfigParser()
+        parser.read(self.settings_file)
+        if "VISUAL" not in parser or "REP" not in parser:
+            self.create_default_settings_file()
+
+    def get_settings_file(self):
+        self.check_settings_file()
         return self.settings_file
+
+    def get_ascii(self) -> bool:
+        self.check_settings_file()
+        parser = configparser.ConfigParser()
+        parser.read(self.settings_file)
+        return parser["VISUAL"]["ascii"] == "True"
+    
+    def toggle_ascii(self):
+        self.check_settings_file()
+        parser = configparser.ConfigParser()
+        parser.read(self.settings_file)
+        parser["VISUAL"]["ascii"] = str(not self.get_ascii())
+        with open(self.settings_file, "w") as f:
+            parser.write(f)
```

### Comparing `tko-0.0.3/src/tko/solver.py` & `tko-0.0.4/src/tko/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .runner import Runner
 
 
 def check_tool(name):
     if which(name) is None:
         raise CompilerError("fail: " + name + " executable not found")
 
+
 class Solver:
     def __init__(self, solver_list: List[str]):
         self.path_list: List[str] = [Solver.__add_dot_bar(path) for path in solver_list]
         
         self.temp_dir = tempfile.mkdtemp()
         # print("Tempdir for execution: " + self.temp_dir)
         # copia para tempdir e atualiza os paths
@@ -56,15 +57,14 @@
 
     def __prepare_java(self):
         check_tool("javac")
 
         solver = self.path_list[0]
         filename = os.path.basename(solver)
         # tempdir = os.path.dirname(self.path_list[0])
-        
 
         cmd = ["javac"] + self.path_list + ['-d', self.temp_dir]
         return_code, stdout, stderr = Runner.subprocess_run(cmd)
         print(stdout)
         print(stderr)
         if return_code != 0:
             raise CompilerError(stdout + stderr)
```

### Comparing `tko-0.0.3/src/tko/wdir.py` & `tko-0.0.4/src/tko/wdir.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from .basic import IdentifierType, Identifier, Unit, Param
 from .loader import Loader
 from .solver import Solver
 from .format import Symbol, Colored, Color
 
 # generate label for cases
+
+
 class LabelFactory:
     def __init__(self):
         self._label = ""
         self._index = -1
 
     def index(self, value: int):
         try:
@@ -47,14 +49,15 @@
         if len(split_label) > 0:
             try:
                 int(split_label[0])
                 return " ".join(split_label[1:])
             except ValueError:
                 return label
 
+
 class Wdir:
     def __init__(self):
         self.solver: Optional[Solver] = None
         self.source_list: List[str] = []
         self.pack_list: List[List[Unit]] = []
         self.unit_list: List[Unit] = []
 
@@ -169,13 +172,15 @@
             for i in range(len(self.pack_list)):
                 nome: str = self.source_list[i].split(os.sep)[-1]
                 out.append(nome + "(" + str(len(self.pack_list[i])).zfill(2) + ")")
             return Colored.paint("sources:", Color.GREEN) + "[" + ", ".join(out) + "]"
 
         def solvers() -> str:
             path_list = [] if self.solver is None else self.solver.path_list
-            return Colored.paint("solvers:", Color.GREEN) + "[" + ", ".join([os.path.basename(path) for path in path_list]) + "]"
+            return (Colored.paint("solvers:", Color.GREEN) +
+                    "[" + ", ".join([os.path.basename(path) for path in path_list]) + "]")
 
         folder = os.getcwd().split(os.sep)[-1]
-        tests_count = Colored.paint("tests:", Color.GREEN) + str(len([x for x in self.unit_list if x.repeated is None])).zfill(2)
+        tests_count = (Colored.paint("tests:", Color.GREEN) +
+                       str(len([x for x in self.unit_list if x.repeated is None])).zfill(2))
 
         return Symbol.opening + folder + " " + tests_count + " " + sources() + " " + solvers()
```

### Comparing `tko-0.0.3/src/tko/writer.py` & `tko-0.0.4/src/tko/writer.py`

 * *Files identical despite different names*

### Comparing `tko-0.0.3/src/tko.egg-info/PKG-INFO` & `tko-0.0.4/src/tko.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tko
-Version: 0.0.3
+Version: 0.0.4
 Summary: tko: Test Engine for Judge Operations
 Home-page: https://github.com/senapk/tko
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/tko/issues
 Project-URL: Source, https://github.com/senapk/tko/
 Keywords: programming,learning
```

