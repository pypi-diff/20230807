# Comparing `tmp/cmn-1.0.1.tar.gz` & `tmp/cmn-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmn-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cmn-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cmn-1.0.1.tar` & `cmn-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1005 2023-07-31 22:03:09.378237 cmn-1.0.1/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1124 2023-08-03 19:28:04.511400 cmn-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       82 2023-08-06 00:38:51.728449 cmn-1.0.1/.gitignore
--rw-r--r--   0        0        0     9229 2023-08-06 00:34:24.799239 cmn-1.0.1/LICENSE
--rw-r--r--   0        0        0     2649 2023-08-03 22:44:06.242819 cmn-1.0.1/README.md
--rw-r--r--   0        0        0       56 2023-08-06 01:33:42.687112 cmn-1.0.1/main.py
--rw-r--r--   0        0        0      502 2023-08-06 01:32:58.152292 cmn-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       15 2023-08-03 22:48:42.765195 cmn-1.0.1/requirements.txt
--rw-r--r--   0        0        0     1104 2023-08-06 01:09:25.634489 cmn-1.0.1/src/ColoredLogger/ColoredLogger.py
--rw-r--r--   0        0        0     2860 2023-08-06 01:09:25.666374 cmn-1.0.1/src/OutputFormatter/OutputFormatter.py
--rw-r--r--   0        0        0     2333 2023-08-06 00:57:16.241778 cmn-1.0.1/src/OutputFormatter/test_OutputFormatter.py
--rw-r--r--   0        0        0     6440 2023-08-06 01:37:57.207585 cmn-1.0.1/src/__init__.py
--rw-r--r--   0        0        0     4693 2023-08-06 01:37:57.207585 cmn-1.0.1/src/cmn/__init__.py
--rw-r--r--   0        0        0     7003 2023-08-06 01:23:48.559460 cmn-1.0.1/src/test_main.py
--rw-r--r--   0        0        0     2973 1970-01-01 00:00:00.000000 cmn-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1005 2023-07-31 22:03:09.378237 cmn-1.1.0/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1127 2023-08-07 18:53:04.536799 cmn-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       88 2023-08-07 19:14:41.930601 cmn-1.1.0/.gitignore
+-rw-r--r--   0        0        0     9229 2023-08-06 00:34:24.799239 cmn-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2649 2023-08-03 22:44:06.242819 cmn-1.1.0/README.md
+-rw-r--r--   0        0        0      502 2023-08-06 01:32:58.152292 cmn-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       15 2023-08-03 22:48:42.765195 cmn-1.1.0/requirements.txt
+-rw-r--r--   0        0        0     4726 2023-08-07 19:02:33.161717 cmn-1.1.0/src/ChangeMediaName/ChangeMediaName.py
+-rw-r--r--   0        0        0     1104 2023-08-06 01:09:25.634489 cmn-1.1.0/src/ColoredLogger/ColoredLogger.py
+-rw-r--r--   0        0        0     2860 2023-08-06 01:09:25.666374 cmn-1.1.0/src/OutputFormatter/OutputFormatter.py
+-rw-r--r--   0        0        0     2301 2023-08-07 19:01:17.007069 cmn-1.1.0/src/OutputFormatter/test_OutputFormatter.py
+-rw-r--r--   0        0        0     6480 2023-08-07 19:13:10.500439 cmn-1.1.0/src/cmn/__init__.py
+-rw-r--r--   0        0        0     7046 2023-08-07 19:12:00.845729 cmn-1.1.0/src/test_main.py
+-rw-r--r--   0        0        0     3048 1970-01-01 00:00:00.000000 cmn-1.1.0/PKG-INFO
```

### Comparing `cmn-1.0.1/.github/workflows/python-app.yml` & `cmn-1.1.0/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `cmn-1.0.1/.github/workflows/python-publish.yml` & `cmn-1.1.0/.github/workflows/python-publish.yml`

 * *Files 9% similar despite different names*

```diff
@@ -31,9 +31,9 @@
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
       with:
-        user: __token__
+        user: Henrique-190
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `cmn-1.0.1/LICENSE` & `cmn-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmn-1.0.1/README.md` & `cmn-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cmn-1.0.1/src/ColoredLogger/ColoredLogger.py` & `cmn-1.1.0/src/ColoredLogger/ColoredLogger.py`

 * *Files identical despite different names*

### Comparing `cmn-1.0.1/src/OutputFormatter/OutputFormatter.py` & `cmn-1.1.0/src/OutputFormatter/OutputFormatter.py`

 * *Files identical despite different names*

### Comparing `cmn-1.0.1/src/OutputFormatter/test_OutputFormatter.py` & `cmn-1.1.0/src/OutputFormatter/test_OutputFormatter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from src.OutputFormatter.OutputFormatter import ImageRegularformatter, VideoRegularformatter, AVIformatter
+from src import ImageRegularformatter, VideoRegularformatter, AVIformatter
 
 
 class OutputFormatterTest(unittest.TestCase):
     def test_getDateTime(self):
         samples = [
             {
                 "output": "Track Create Date               : 0000:00:00 00:00:00",
```

### Comparing `cmn-1.0.1/src/__init__.py` & `cmn-1.1.0/src/cmn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-__version__ = "1.0.1"
 """
 Main - Module responsible for the main program. Parses the arguments and calls the other modules.
 """
+__version__ = "1.1.0"
 
 import argparse
 import os
 import re
 
 from src.ColoredLogger.ColoredLogger import ColoredLogger
 
 from datetime import datetime
 
-from src.cmn import cmn
+from src.ChangeMediaName import ChangeMediaName
 
 logger = ColoredLogger()
 
 
 def nameFormatter(nf: str, aux: str) -> bool:
     global logger
     logger.debug(f"Parsing {aux}name format")
@@ -112,15 +112,15 @@
 
     if not nameFormatter(args.name_format, "") or not nameFormatter(args.name_folder_format, "folder "):
         return
 
     filetypes = getFiletypes(args.file_types, args.only_images, args.only_videos, args.not_file_types)
     files = getScanFiles(args.input_files, args.recursive, args.ignored_paths, args.not_ignore_subfolders, filetypes)
 
-    nChanged, nErrors = cmn(logger, files, args.create_new_folders, args.name_format, args.name_folder_format)
+    nChanged, nErrors = ChangeMediaName.cmn(logger, files, args.create_new_folders, args.name_format, args.name_folder_format)
     nProcessed = len(files)
     endTimer = datetime.now()
     logger.info(f"Processed {nProcessed} file{'s' if nProcessed != 1 else ''} in {endTimer - initialTimer}.")
     logger.info(f"Changed {nChanged} file{'s' if nChanged != 1 else ''}.")
     logger.info(f"Errors: {nErrors}.")
     logger.info("Program finished.")
```

### Comparing `cmn-1.0.1/src/cmn/__init__.py` & `cmn-1.1.0/src/ChangeMediaName/ChangeMediaName.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 __version__ = "1.0.1"
 import os
 import subprocess
 from datetime import datetime
 from shutil import which
 
-from src.ColoredLogger import ColoredLogger
+from src import ColoredLogger
 from src.OutputFormatter.OutputFormatter import ImageRegularformatter, VideoRegularformatter, AVIformatter
 
 NewNameFile = '{year}{month}{day}_{hour}{minute}{second}{filetype}'
 NewNameFolder = '{year}-{month}-{day}'
 
 nChanged = 0
 nErrors = 0
@@ -139,7 +139,10 @@
             changeFileName(oldpath, newpath, oldfile, nameFormat, date)
         except (Exception,):
             logger.error(f"{completed:.2f}% - Error getting new path of {file}.")
             nErrors += 1
             continue
 
     return nChanged, nErrors
+
+if __name__ == "__main__":
+    print("dont")
```

### Comparing `cmn-1.0.1/src/test_main.py` & `cmn-1.1.0/src/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from src import *
+from cmn import *
 
 
 class MainTest(unittest.TestCase):
     def test_nameFormatter(self):
         samples = [
             {
                 "nf": "%Y%m%d_%H%M%S",
@@ -38,46 +38,46 @@
             self.assertEqual(result, sample["expected"], f"Error in {sample['nf']}")
 
     def test_recursiveSearch(self):
         files = recursiveSearch("./src")
         newfiles = [x for x in files if "pycache" not in x and "pytest" not in x]
 
         self.assertSetEqual(set(newfiles),
-                            {'./src/test_main.py', './src/__init__.py', './src/cmn/__init__.py',
+                            {'./src/test_main.py', './src/cmn/__init__.py', './src/ChangeMediaName/ChangeMediaName.py',
                              './src/ColoredLogger/ColoredLogger.py', './src/OutputFormatter/test_OutputFormatter.py',
                              './src/OutputFormatter/OutputFormatter.py'},
                             "Error in recursiveSearch_test"
                             )
 
     def test_notRecursiveSearch(self):
         result = notRecursiveSearch("./src")
 
         self.assertSetEqual(set(result),
-                            {'./src/test_main.py', './src/__init__.py'},
+                            {'./src/test_main.py'},
                             "Error in notRecursiveSearch_test"
                             )
 
     def test_getFiles(self):
         samples = [
             {
                 "paths": ["./src"],
                 "recursive": True,
                 "expected": {
                     './src/test_main.py',
-                    './src/__init__.py',
                     './src/cmn/__init__.py',
+                    './src/ChangeMediaName/ChangeMediaName.py',
                     './src/ColoredLogger/ColoredLogger.py',
                     './src/OutputFormatter/test_OutputFormatter.py',
                     './src/OutputFormatter/OutputFormatter.py'
                 }
             },
             {
                 "paths": ["./src"],
                 "recursive": False,
-                "expected": {'./src/test_main.py', './src/__init__.py'}
+                "expected": {'./src/test_main.py'}
             }
         ]
 
         for sample in samples:
             files = getFiles(sample["paths"], sample["recursive"])
             newfiles = [x for x in files if "pycache" not in x and "pytest" not in x]
 
@@ -142,16 +142,16 @@
                 "recursive": True,
                 "ignored_paths": [],
                 "not_ignore_subfolders": False,
                 "filetypes": [".py"],
                 "expected":
                     {
                         './src/test_main.py',
-                        './src/__init__.py',
                         './src/cmn/__init__.py',
+                        './src/ChangeMediaName/ChangeMediaName.py',
                         './src/ColoredLogger/ColoredLogger.py',
                         './src/OutputFormatter/test_OutputFormatter.py',
                         './src/OutputFormatter/OutputFormatter.py'
                     }
             },
             {
                 "input_files": ["./src"],
@@ -160,20 +160,20 @@
                 "not_ignore_subfolders": False,
                 "filetypes": [],
                 "expected": set()
             },
             {
                 "input_files": ["./src"],
                 "recursive": True,
-                "ignored_paths": ["./src/cmn"],
+                "ignored_paths": ["./src/ChangeMediaName"],
                 "not_ignore_subfolders": True,
                 "filetypes": [".py"],
                 "expected": {
                     './src/test_main.py',
-                    './src/__init__.py',
+                    './src/cmn/__init__.py',
                     './src/ColoredLogger/ColoredLogger.py',
                     './src/OutputFormatter/test_OutputFormatter.py',
                     './src/OutputFormatter/OutputFormatter.py'
                 }
             },
             {
                 "input_files": ["./src"],
```

### Comparing `cmn-1.0.1/PKG-INFO` & `cmn-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cmn
-Version: 1.0.1
-Summary: CMN - Common functions
+Version: 1.1.0
+Summary: Main - Module responsible for the main program. Parses the arguments and calls the other modules.
 Author-email: Henrique Alvelos <henriquealvelos@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: colorama >= 0.4.6
 Project-URL: Home, https://github.com/Henrique-190/ChangeMediaName
```

