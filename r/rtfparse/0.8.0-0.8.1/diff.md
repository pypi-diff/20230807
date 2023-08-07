# Comparing `tmp/rtfparse-0.8.0.tar.gz` & `tmp/rtfparse-0.8.1.tar.gz`

## Comparing `rtfparse-0.8.0.tar` & `rtfparse-0.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 rtfparse-0.8.0/CHANGELOG.md
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 rtfparse-0.8.0/release.cmd
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 rtfparse-0.8.0/requirements.txt
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 rtfparse-0.8.0/changelog.d/changelog_template.jinja
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/__about__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/__init__.py
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/cli.py
--rw-r--r--   0        0        0     8702 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/entities.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/enums.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/logging_conf.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/minimal.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/parser.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/re_patterns.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/utils.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/renderers/__init__.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 rtfparse-0.8.0/src/rtfparse/renderers/de_encapsulate_html.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 rtfparse-0.8.0/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 rtfparse-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 rtfparse-0.8.0/README.md
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 rtfparse-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 rtfparse-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 rtfparse-0.8.1/CHANGELOG.md
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 rtfparse-0.8.1/release.cmd
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 rtfparse-0.8.1/requirements.txt
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 rtfparse-0.8.1/changelog.d/changelog_template.jinja
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 rtfparse-0.8.1/src/rtfparse/__about__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 rtfparse-0.8.1/src/rtfparse/__init__.py
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 rtfparse-0.8.1/src/rtfparse/cli.py
+-rw-r--r--   0        0        0     8846 2020-02-02 00:00:00.000000 rtfparse-0.8.1/src/rtfparse/entities.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rtfparse-0.8.1/src/rtfparse/enums.py
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 rtfparse-0.8.1/src/rtfparse/logging_conf.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 rtfparse-0.8.1/src/rtfparse/minimal.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 rtfparse-0.8.1/src/rtfparse/parser.py
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 rtfparse-0.8.1/src/rtfparse/re_patterns.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 rtfparse-0.8.1/src/rtfparse/utils.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 rtfparse-0.8.1/src/rtfparse/renderers/__init__.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 rtfparse-0.8.1/src/rtfparse/renderers/de_encapsulate_html.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 rtfparse-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 rtfparse-0.8.1/LICENSE.txt
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 rtfparse-0.8.1/README.md
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 rtfparse-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 rtfparse-0.8.1/PKG-INFO
```

### Comparing `rtfparse-0.8.0/src/rtfparse/cli.py` & `rtfparse-0.8.1/src/rtfparse/cli.py`

 * *Files identical despite different names*

### Comparing `rtfparse-0.8.0/src/rtfparse/entities.py` & `rtfparse-0.8.1/src/rtfparse/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,24 +16,30 @@
 # Constants, number of bytes to read when creating entities
 CHARACTER = BACKSLASH = DELIMITER = MINUS = GROUP_END = len(b"\\")
 SYMBOL = IGNORABLE = BACKSLASH + CHARACTER
 GROUP_START = BACKSLASH + IGNORABLE
 MAX_CW_LETTERS = 32  # As specified in RTF Spec
 INTEGER_MAGNITUDE = 32  # As specified in RTF Spec
 PLAIN_TEXT = CONTROL_WORD = (
-    BACKSLASH + MAX_CW_LETTERS + MINUS + len(str((1 << INTEGER_MAGNITUDE) // 2)) + DELIMITER
+    BACKSLASH
+    + MAX_CW_LETTERS
+    + MINUS
+    + len(str((1 << INTEGER_MAGNITUDE) // 2))
+    + DELIMITER
 )
 
 
 class Entity:
     def __init__(self) -> None:
         self.text = ""
 
     @classmethod
-    def probe(cls, pattern: re_patterns.Bytes_Regex, file: io.BufferedReader) -> Bytestring_Type:
+    def probe(
+        cls, pattern: re_patterns.Bytes_Regex, file: io.BufferedReader
+    ) -> Bytestring_Type:
         logger.debug(f"Probing file at position {file.tell()}")
         original_position = file.tell()
         while True:
             probed = file.read(len(re_patterns.probe_pattern))
             logger.debug(f"{probed = }")
             file.seek(original_position)
             logger.debug(f"Probe returned to position {file.tell()}")
@@ -44,15 +50,17 @@
             elif match := re_patterns.control_word.match(probed):
                 result = Bytestring_Type.CONTROL_WORD
             elif match := re_patterns.control_symbol.match(probed):
                 result = Bytestring_Type.CONTROL_SYMBOL
             elif match := re_patterns.plain_text.match(probed):
                 result = Bytestring_Type.PLAIN_TEXT
             else:
-                logger.debug(f"This does not match anything, it's probably a newline, moving on")
+                logger.debug(
+                    f"This does not match anything, it's probably a newline, moving on"
+                )
                 original_position += 1
                 file.seek(original_position)
                 logger.debug(f"Probe moved to position {file.tell()}")
                 if not probed:
                     logger.debug(f"Reached unexpected end of file.")
                     result = Bytestring_Type.GROUP_END
                     break
@@ -88,15 +96,17 @@
                 logger.debug(
                     f"Delimiter is {match.group('other').decode(self.encoding)}, len: {len(match.group('delimiter'))}"
                 )
                 target_position -= len(match.group("delimiter"))
             file.seek(target_position)
             # handle \binN:
             if self.control_name == "bin":
-                self.bindata = file.read(utils.twos_complement(self.parameter, INTEGER_MAGNITUDE))
+                self.bindata = file.read(
+                    utils.twos_complement(self.parameter, INTEGER_MAGNITUDE)
+                )
         else:
             logger.warning(f"Missing Control Word")
             file.seek(self.start_position)
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}: {self.control_name}{self.parameter}>"
 
@@ -174,15 +184,17 @@
             self.known = bool(match.group("group_start"))
             self.ignorable = bool(match.group("ignorable"))
             if not self.ignorable:
                 file.seek(self.start_position + GROUP_START - IGNORABLE)
                 logger.debug(f"Returned to position {file.tell()}")
         else:
             logger.warning(
-                utils.warn(f"Expected a group but found no group start. Creating unknown group")
+                utils.warn(
+                    f"Expected a group but found no group start. Creating unknown group"
+                )
             )
             file.seek(self.start_position)
         while True:
             probed = self.probe(re_patterns.probe, file)
             if probed is Bytestring_Type.CONTROL_WORD:
                 self.structure.append(Control_Word(self.encoding, file))
             elif probed is Bytestring_Type.GROUP_END:
```

### Comparing `rtfparse-0.8.0/src/rtfparse/logging_conf.py` & `rtfparse-0.8.1/src/rtfparse/logging_conf.py`

 * *Files identical despite different names*

### Comparing `rtfparse-0.8.0/src/rtfparse/minimal.py` & `rtfparse-0.8.1/src/rtfparse/minimal.py`

 * *Files identical despite different names*

### Comparing `rtfparse-0.8.0/src/rtfparse/parser.py` & `rtfparse-0.8.1/src/rtfparse/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 
 
 import io
 import logging
 import pathlib
 import re
+from argparse import Namespace
 
 # Typing
 from typing import Optional, Union
 
 # Own modules
 from rtfparse import entities, re_patterns, utils
 
@@ -22,15 +23,17 @@
         rtf_path: Optional[pathlib.Path] = None,
         rtf_file: Optional[Union[io.BufferedReader, io.BytesIO]] = None,
     ) -> None:
         self.rtf_path = rtf_path
         self.rtf_file = rtf_file
         if not (self.rtf_path or self.rtf_file):
             raise ValueError("Need `rtf_path` or `rtf_file` argument")
-        self.ENCODING_PROBE = 48  # look for encoding information in the first 48 bytes of the file
+        self.ENCODING_PROBE = (
+            48  # look for encoding information in the first 48 bytes of the file
+        )
 
     def read_encoding(self, file: Union[io.BufferedReader, io.BytesIO]) -> str:
         probed = file.read(self.ENCODING_PROBE)
         group = entities.Group("cp1252", io.BytesIO(probed))
         recognized_encodings = (
             "ansi",
             "ansicpg",
@@ -48,25 +51,30 @@
         )
         # Check if the ANSI code page is set as a parameter of any of the control words:
         cp = None
         for item in names:
             # if any item is a Control_Word which has a parameter, we assume that this is the parameter of \ansicpg, and that corresponds to the codepage we are looking for
             if item.parameter:
                 param = item.parameter
+            else:
+                param = None
         if param:
             if param == 65001:
                 logger.warning(
-                    "Found encoding 65001, but often this is actually cp1252, so I'm overriding it"
+                    "Found encoding '65001', but often this is actually 'cp1252', so I'm taking that"
                 )
                 encoding = "cp1252"
             else:
                 encoding = f"cp{param}"
         else:
             if names[0].control_name == "ansi":
-                encoding = "ansi"
+                logger.warning(
+                    "Found encoding 'ansi', but often this is actually 'cp1252', so I'm taking that"
+                )
+                encoding = "cp1252"
             elif names[0].control_name == "mac":
                 encoding = "mac_roman"
             elif names[0].control_name == "pc":
                 encoding = "cp437"
             elif names[0].control_name == "pca":
                 encoding = "cp850"
         file.seek(0)
@@ -83,14 +91,16 @@
         parsed_object = utils.what_is_being_parsed(file)
         logger.info(f"Parsing the structure of {parsed_object}")
         try:
             encoding = self.read_encoding(file)
             self.parsed = entities.Group(encoding, file)
         except Exception as err:
             logger.exception(err)
+            self.parsed == Namespace()
+            self.parsed.structure = list()
         finally:
             if self.rtf_path is not None:
                 logger.debug(f"Closing {parsed_object}")
                 file.close()
             logger.info(f"Structure of {parsed_object} parsed")
             return self.parsed
```

### Comparing `rtfparse-0.8.0/src/rtfparse/re_patterns.py` & `rtfparse-0.8.1/src/rtfparse/re_patterns.py`

 * *Files identical despite different names*

### Comparing `rtfparse-0.8.0/src/rtfparse/utils.py` & `rtfparse-0.8.1/src/rtfparse/utils.py`

 * *Files identical despite different names*

### Comparing `rtfparse-0.8.0/src/rtfparse/renderers/de_encapsulate_html.py` & `rtfparse-0.8.1/src/rtfparse/renderers/de_encapsulate_html.py`

 * *Files identical despite different names*

### Comparing `rtfparse-0.8.0/.gitignore` & `rtfparse-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rtfparse-0.8.0/LICENSE.txt` & `rtfparse-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rtfparse-0.8.0/README.md` & `rtfparse-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `rtfparse-0.8.0/pyproject.toml` & `rtfparse-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rtfparse-0.8.0/PKG-INFO` & `rtfparse-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtfparse
-Version: 0.8.0
+Version: 0.8.1
 Summary: Tool to parse Microsoft Rich Text Format (RTF)
 Project-URL: Documentation, https://github.com/fleetingbytes/rtfparse#readme
 Project-URL: Issues, https://github.com/fleetingbytes/rtfparse/issues
 Project-URL: Source, https://github.com/fleetingbytes/rtfparse
 Author-email: Sven Siegmund <sven.siegmund@iav.de>
 License: Copyright (c) 2023 Sven Siegmud
```

