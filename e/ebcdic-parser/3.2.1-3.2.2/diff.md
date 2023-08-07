# Comparing `tmp/ebcdic_parser-3.2.1.tar.gz` & `tmp/ebcdic_parser-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Projects\ebcdic-parser\dist\.tmp-3zgl4xxa\ebcdic_parser-3.2.1.tar", last modified: Sun Aug  6 03:04:08 2023, max compression
+gzip compressed data, was "D:\Projects\ebcdic-parser\dist\.tmp-7cbtzxka\ebcdic_parser-3.2.2.tar", last modified: Mon Aug  7 15:08:55 2023, max compression
```

## Comparing `ebcdic_parser-3.2.1.tar` & `ebcdic_parser-3.2.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 03:04:08.000000 ebcdic_parser-3.2.1/
--rw-rw-rw-   0        0        0       16 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.1/AUTHORS
--rw-rw-rw-   0        0        0     1066 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.1/LICENSE
--rw-rw-rw-   0        0        0     7061 2023-08-06 03:04:08.000000 ebcdic_parser-3.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    11905 2023-08-05 03:48:43.000000 ebcdic_parser-3.2.1/README.md
--rw-rw-rw-   0        0        0     6248 2023-08-06 03:02:40.000000 ebcdic_parser-3.2.1/READMEPYPI.md
--rw-rw-rw-   0        0        0       86 2023-07-18 03:12:01.000000 ebcdic_parser-3.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      787 2023-08-06 03:04:08.000000 ebcdic_parser-3.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-06 03:04:08.000000 ebcdic_parser-3.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 03:04:08.000000 ebcdic_parser-3.2.1/src/ebcdic_parser/
--rw-rw-rw-   0        0        0        0 2023-07-18 02:52:18.000000 ebcdic_parser-3.2.1/src/ebcdic_parser/__init__.py
--rw-rw-rw-   0        0        0       67 2023-08-03 03:22:06.000000 ebcdic_parser-3.2.1/src/ebcdic_parser/__main__.py
--rw-rw-rw-   0        0        0    59935 2023-08-06 03:03:28.000000 ebcdic_parser-3.2.1/src/ebcdic_parser/convert.py
-drwxrwxrwx   0        0        0        0 2023-08-06 03:04:08.000000 ebcdic_parser-3.2.1/src/ebcdic_parser.egg-info/
--rw-rw-rw-   0        0        0     7061 2023-08-06 03:04:08.000000 ebcdic_parser-3.2.1/src/ebcdic_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-08-06 03:04:08.000000 ebcdic_parser-3.2.1/src/ebcdic_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 03:04:08.000000 ebcdic_parser-3.2.1/src/ebcdic_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-08-06 03:04:08.000000 ebcdic_parser-3.2.1/src/ebcdic_parser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-06 03:04:08.000000 ebcdic_parser-3.2.1/tests/
--rw-rw-rw-   0        0        0    17737 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.1/tests/test_functional.py
--rw-rw-rw-   0        0        0     6168 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.1/tests/test_system_311_calls_for_service_requests_all_strings.py
--rw-rw-rw-   0        0        0     5949 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.1/tests/test_system_common.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:08:55.000000 ebcdic_parser-3.2.2/
+-rw-rw-rw-   0        0        0       16 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.2/AUTHORS
+-rw-rw-rw-   0        0        0      873 2023-08-07 14:26:24.000000 ebcdic_parser-3.2.2/CHANGES.md
+-rw-rw-rw-   0        0        0     1066 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.2/LICENSE
+-rw-rw-rw-   0        0        0     7936 2023-08-07 15:08:55.000000 ebcdic_parser-3.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11905 2023-08-06 03:19:34.000000 ebcdic_parser-3.2.2/README.md
+-rw-rw-rw-   0        0        0     6248 2023-08-06 03:19:18.000000 ebcdic_parser-3.2.2/READMEPYPI.md
+-rw-rw-rw-   0        0        0       86 2023-07-18 03:12:01.000000 ebcdic_parser-3.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      825 2023-08-07 15:08:55.000000 ebcdic_parser-3.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 15:08:54.000000 ebcdic_parser-3.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 15:08:55.000000 ebcdic_parser-3.2.2/src/ebcdic_parser/
+-rw-rw-rw-   0        0        0       32 2023-08-07 03:35:46.000000 ebcdic_parser-3.2.2/src/ebcdic_parser/__init__.py
+-rw-rw-rw-   0        0        0       67 2023-08-03 03:22:06.000000 ebcdic_parser-3.2.2/src/ebcdic_parser/__main__.py
+-rw-rw-rw-   0        0        0    59935 2023-08-07 03:36:41.000000 ebcdic_parser-3.2.2/src/ebcdic_parser/convert.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:08:55.000000 ebcdic_parser-3.2.2/src/ebcdic_parser.egg-info/
+-rw-rw-rw-   0        0        0     7936 2023-08-07 15:08:54.000000 ebcdic_parser-3.2.2/src/ebcdic_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-08-07 15:08:54.000000 ebcdic_parser-3.2.2/src/ebcdic_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 15:08:54.000000 ebcdic_parser-3.2.2/src/ebcdic_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-07 15:08:54.000000 ebcdic_parser-3.2.2/src/ebcdic_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 15:08:55.000000 ebcdic_parser-3.2.2/tests/
+-rw-rw-rw-   0        0        0    17737 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.2/tests/test_functional.py
+-rw-rw-rw-   0        0        0     6168 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.2/tests/test_system_311_calls_for_service_requests_all_strings.py
+-rw-rw-rw-   0        0        0     5949 2020-07-12 02:48:58.000000 ebcdic_parser-3.2.2/tests/test_system_common.py
```

### Comparing `ebcdic_parser-3.2.1/LICENSE` & `ebcdic_parser-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ebcdic_parser-3.2.1/PKG-INFO` & `ebcdic_parser-3.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebcdic_parser
-Version: 3.2.1
+Version: 3.2.2
 Summary: Convert mainframe EBCDIC data into Unicode ASCII delimited text files
 Home-page: https://github.com/larandvit/ebcdic-parser
 Author: Vitaly Saversky
 Author-email: larandvit@hotmail.com
 Project-URL: Bug Tracker, https://github.com/larandvit/ebcdic-parser/issues
 Project-URL: repository, https://github.com/larandvit/ebcdic-parser
 Classifier: Programming Language :: Python :: 3
@@ -97,15 +97,15 @@
 * **layoutfile** - layout file path. Mandatory parameter. Absolute and relative paths are acceptable.
 * **outputdelimiter** - output text file delimiter. Optional parameter. Default value is `\t`.
 * **outputfileextension** - output text file extension. Optional parameter. Default value is `.txt`.
 * **ignoreconversionerrors** - ignore any conversion error. Optional parameter. Default value is `False`.
 * **logfolder** - output folder to store log file. Optional parameter. Default value is the current folder. Absolute and relative paths are acceptable.
 * **pythonencoding** - use Python encoding rather than Java. Optional parameter. Default value is `True`.
 * **encodingname** - code page name to encode characters (Python or Java). Optional parameter. Default value is `cp037`.
-* **grouprecords** - create relationships between records. Optional parameter. Default value is `False'.
+* **grouprecords** - create relationships between records. Optional parameter. Default value is `False`.
 * **grouprecordslevel2** - create relationships between records for level 2. Optional parameter. Default value is `False`.
 * **verbose** - show extended information on screen. Optional parameter. Default value is `True`.
 * **debug** - show debug information. Optional parameter. Default value is `False`.
 * **cliMode** - a flag how it run in command prompt or Pip installation.
 
 ## python -m ebcdic_parser Usage
 
@@ -158,7 +158,45 @@
 Exit codes: 0 - successful completion, 1 - completion with any error
 ```
 
 ## Java Encodings
 It doesn't request any special installation if you are planning to use only Python encodings.
 
 In case of using Java encodings, it has to be installed [javabridge](https://pypi.org/project/javabridge/) Python library. There is a constant in the code for including the javabridge library.
+# Release Notes
+
+## Release 3.2.2
+* Automate version management.
+* Add CHANGES.md documentation.
+
+## Release 3.2.1
+* Added dedicated PyPI README file.
+* Refined documentation.
+
+
+## Release 3.2.0
+* Provide a command-line interface for ebcdic_parser package running via python -m ebcdic_parser. 
+
+## Release 3.1.0
+* Fixed relative path parameters in command prompt mode.
+* Refined documentation.
+
+
+## Release 3.0.0
+* Added to PyPI.
+
+## Release 2.4.1
+* Fixed issue with "Multi-schema fixed record length" layout type.
+
+## Release 2.4.0 
+* Added "Single schema variable record length" layout type.
+
+## Release 2.3.0
+* Implemented debug mode.
+
+## Release 2.1.1
+* Improved sign parsing in packedDecimal data type.
+* Added sign parsing to decimal data type.
+* Developed functional tests.
+
+## Release 2.1.0
+* The first public available release.
```

### Comparing `ebcdic_parser-3.2.1/README.md` & `ebcdic_parser-3.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 * **layoutfile** - layout file path. Mandatory parameter. Absolute and relative paths are acceptable.
 * **outputdelimiter** - output text file delimiter. Optional parameter. Default value is `\t`.
 * **outputfileextension** - output text file extension. Optional parameter. Default value is `.txt`.
 * **ignoreconversionerrors** - ignore any conversion error. Optional parameter. Default value is `False`.
 * **logfolder** - output folder to store log file. Optional parameter. Default value is the current folder. Absolute and relative paths are acceptable.
 * **pythonencoding** - use Python encoding rather than Java. Optional parameter. Default value is `True`.
 * **encodingname** - code page name to encode characters (Python or Java). Optional parameter. Default value is `cp037`.
-* **grouprecords** - create relationships between records. Optional parameter. Default value is `False'.
+* **grouprecords** - create relationships between records. Optional parameter. Default value is `False`.
 * **grouprecordslevel2** - create relationships between records for level 2. Optional parameter. Default value is `False`.
 * **verbose** - show extended information on screen. Optional parameter. Default value is `True`.
 * **debug** - show debug information. Optional parameter. Default value is `False`.
 * **cliMode** - a flag how it run in command prompt or Pip installation.  
 
 
 ## Command Prompt Usage
```

### Comparing `ebcdic_parser-3.2.1/READMEPYPI.md` & `ebcdic_parser-3.2.2/READMEPYPI.md`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 * **layoutfile** - layout file path. Mandatory parameter. Absolute and relative paths are acceptable.
 * **outputdelimiter** - output text file delimiter. Optional parameter. Default value is `\t`.
 * **outputfileextension** - output text file extension. Optional parameter. Default value is `.txt`.
 * **ignoreconversionerrors** - ignore any conversion error. Optional parameter. Default value is `False`.
 * **logfolder** - output folder to store log file. Optional parameter. Default value is the current folder. Absolute and relative paths are acceptable.
 * **pythonencoding** - use Python encoding rather than Java. Optional parameter. Default value is `True`.
 * **encodingname** - code page name to encode characters (Python or Java). Optional parameter. Default value is `cp037`.
-* **grouprecords** - create relationships between records. Optional parameter. Default value is `False'.
+* **grouprecords** - create relationships between records. Optional parameter. Default value is `False`.
 * **grouprecordslevel2** - create relationships between records for level 2. Optional parameter. Default value is `False`.
 * **verbose** - show extended information on screen. Optional parameter. Default value is `True`.
 * **debug** - show debug information. Optional parameter. Default value is `False`.
 * **cliMode** - a flag how it run in command prompt or Pip installation.
 
 ## python -m ebcdic_parser Usage
```

### Comparing `ebcdic_parser-3.2.1/setup.cfg` & `ebcdic_parser-3.2.2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6263 6469 635f 7061 7273 6572   = ebcdic_parser
-00000020: 0d0a 7665 7273 696f 6e20 3d20 332e 322e  ..version = 3.2.
-00000030: 310d 0a61 7574 686f 7220 3d20 5669 7461  1..author = Vita
-00000040: 6c79 2053 6176 6572 736b 790d 0a61 7574  ly Saversky..aut
-00000050: 686f 725f 656d 6169 6c20 3d20 6c61 7261  hor_email = lara
-00000060: 6e64 7669 7440 686f 746d 6169 6c2e 636f  ndvit@hotmail.co
-00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
-00000080: 2043 6f6e 7665 7274 206d 6169 6e66 7261   Convert mainfra
-00000090: 6d65 2045 4243 4449 4320 6461 7461 2069  me EBCDIC data i
-000000a0: 6e74 6f20 556e 6963 6f64 6520 4153 4349  nto Unicode ASCI
-000000b0: 4920 6465 6c69 6d69 7465 6420 7465 7874  I delimited text
-000000c0: 2066 696c 6573 0d0a 6c6f 6e67 5f64 6573   files..long_des
-000000d0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
-000000e0: 2052 4541 444d 4550 5950 492e 6d64 2c20   READMEPYPI.md, 
-000000f0: 4c49 4345 4e53 452e 7478 740d 0a6c 6f6e  LICENSE.txt..lon
-00000100: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
-00000110: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
-00000120: 742f 6d61 726b 646f 776e 0d0a 7572 6c20  t/markdown..url 
-00000130: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000140: 2e63 6f6d 2f6c 6172 616e 6476 6974 2f65  .com/larandvit/e
-00000150: 6263 6469 632d 7061 7273 6572 0d0a 7072  bcdic-parser..pr
-00000160: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
-00000170: 4275 6720 5472 6163 6b65 7220 3d20 6874  Bug Tracker = ht
-00000180: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000190: 2f6c 6172 616e 6476 6974 2f65 6263 6469  /larandvit/ebcdi
-000001a0: 632d 7061 7273 6572 2f69 7373 7565 730d  c-parser/issues.
-000001b0: 0a09 7265 706f 7369 746f 7279 203d 2068  ..repository = h
-000001c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000001d0: 6d2f 6c61 7261 6e64 7669 742f 6562 6364  m/larandvit/ebcd
-000001e0: 6963 2d70 6172 7365 720d 0a63 6c61 7373  ic-parser..class
-000001f0: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
-00000200: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000210: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
-00000220: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-00000230: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000240: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
-00000250: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-00000260: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
-00000270: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-00000280: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
-00000290: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
-000002a0: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
-000002b0: 7569 7265 7320 3d20 3e3d 332e 370d 0a0d  uires = >=3.7...
-000002c0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-000002d0: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-000002e0: 3d20 7372 630d 0a0d 0a5b 6567 675f 696e  = src....[egg_in
-000002f0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000300: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-00000310: 0a0d 0a                                  ...
+00000020: 0d0a 7665 7273 696f 6e20 3d20 6174 7472  ..version = attr
+00000030: 3a20 6562 6364 6963 5f70 6172 7365 722e  : ebcdic_parser.
+00000040: 5f5f 7665 7273 696f 6e5f 5f0d 0a61 7574  __version__..aut
+00000050: 686f 7220 3d20 5669 7461 6c79 2053 6176  hor = Vitaly Sav
+00000060: 6572 736b 790d 0a61 7574 686f 725f 656d  ersky..author_em
+00000070: 6169 6c20 3d20 6c61 7261 6e64 7669 7440  ail = larandvit@
+00000080: 686f 746d 6169 6c2e 636f 6d0d 0a64 6573  hotmail.com..des
+00000090: 6372 6970 7469 6f6e 203d 2043 6f6e 7665  cription = Conve
+000000a0: 7274 206d 6169 6e66 7261 6d65 2045 4243  rt mainframe EBC
+000000b0: 4449 4320 6461 7461 2069 6e74 6f20 556e  DIC data into Un
+000000c0: 6963 6f64 6520 4153 4349 4920 6465 6c69  icode ASCII deli
+000000d0: 6d69 7465 6420 7465 7874 2066 696c 6573  mited text files
+000000e0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000f0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
+00000100: 4550 5950 492e 6d64 2c20 4348 414e 4745  EPYPI.md, CHANGE
+00000110: 532e 6d64 2c20 4c49 4345 4e53 452e 7478  S.md, LICENSE.tx
+00000120: 740d 0a6c 6f6e 675f 6465 7363 7269 7074  t..long_descript
+00000130: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
+00000140: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
+00000150: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
+00000160: 6769 7468 7562 2e63 6f6d 2f6c 6172 616e  github.com/laran
+00000170: 6476 6974 2f65 6263 6469 632d 7061 7273  dvit/ebcdic-pars
+00000180: 6572 0d0a 7072 6f6a 6563 745f 7572 6c73  er..project_urls
+00000190: 203d 200d 0a09 4275 6720 5472 6163 6b65   = ...Bug Tracke
+000001a0: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
+000001b0: 7562 2e63 6f6d 2f6c 6172 616e 6476 6974  ub.com/larandvit
+000001c0: 2f65 6263 6469 632d 7061 7273 6572 2f69  /ebcdic-parser/i
+000001d0: 7373 7565 730d 0a09 7265 706f 7369 746f  ssues...reposito
+000001e0: 7279 203d 2068 7474 7073 3a2f 2f67 6974  ry = https://git
+000001f0: 6875 622e 636f 6d2f 6c61 7261 6e64 7669  hub.com/larandvi
+00000200: 742f 6562 6364 6963 2d70 6172 7365 720d  t/ebcdic-parser.
+00000210: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
+00000220: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000230: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000240: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
+00000250: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000260: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
+00000270: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+00000280: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000290: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
+000002a0: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
+000002b0: 0d0a 093d 2073 7263 0d0a 7061 636b 6167  ...= src..packag
+000002c0: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
+000002d0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+000002e0: 332e 370d 0a0d 0a5b 6f70 7469 6f6e 732e  3.7....[options.
+000002f0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+00000300: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
+00000310: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000320: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000330: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `ebcdic_parser-3.2.1/src/ebcdic_parser/convert.py` & `ebcdic_parser-3.2.2/src/ebcdic_parser/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import re
 
 import unicodedata
 
 __author__ = "Vitaly Saversky"
 __date__ = "2017-10-04"
 __credits__ = ["Vitaly Saversky"]
-__version__ = "3.2.1"
+__version__ = "3.2.2"
 __maintainer__ = "Vitaly Saversky"
 __email__ = "larandvit@hotmail.com"
 __status__ = "Production"
 
 class FileFormat(IntEnum):
     SingleSchema = 1
     MultiSchemaFixed = 2
```

### Comparing `ebcdic_parser-3.2.1/src/ebcdic_parser.egg-info/PKG-INFO` & `ebcdic_parser-3.2.2/src/ebcdic_parser.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebcdic-parser
-Version: 3.2.1
+Version: 3.2.2
 Summary: Convert mainframe EBCDIC data into Unicode ASCII delimited text files
 Home-page: https://github.com/larandvit/ebcdic-parser
 Author: Vitaly Saversky
 Author-email: larandvit@hotmail.com
 Project-URL: Bug Tracker, https://github.com/larandvit/ebcdic-parser/issues
 Project-URL: repository, https://github.com/larandvit/ebcdic-parser
 Classifier: Programming Language :: Python :: 3
@@ -97,15 +97,15 @@
 * **layoutfile** - layout file path. Mandatory parameter. Absolute and relative paths are acceptable.
 * **outputdelimiter** - output text file delimiter. Optional parameter. Default value is `\t`.
 * **outputfileextension** - output text file extension. Optional parameter. Default value is `.txt`.
 * **ignoreconversionerrors** - ignore any conversion error. Optional parameter. Default value is `False`.
 * **logfolder** - output folder to store log file. Optional parameter. Default value is the current folder. Absolute and relative paths are acceptable.
 * **pythonencoding** - use Python encoding rather than Java. Optional parameter. Default value is `True`.
 * **encodingname** - code page name to encode characters (Python or Java). Optional parameter. Default value is `cp037`.
-* **grouprecords** - create relationships between records. Optional parameter. Default value is `False'.
+* **grouprecords** - create relationships between records. Optional parameter. Default value is `False`.
 * **grouprecordslevel2** - create relationships between records for level 2. Optional parameter. Default value is `False`.
 * **verbose** - show extended information on screen. Optional parameter. Default value is `True`.
 * **debug** - show debug information. Optional parameter. Default value is `False`.
 * **cliMode** - a flag how it run in command prompt or Pip installation.
 
 ## python -m ebcdic_parser Usage
 
@@ -158,7 +158,45 @@
 Exit codes: 0 - successful completion, 1 - completion with any error
 ```
 
 ## Java Encodings
 It doesn't request any special installation if you are planning to use only Python encodings.
 
 In case of using Java encodings, it has to be installed [javabridge](https://pypi.org/project/javabridge/) Python library. There is a constant in the code for including the javabridge library.
+# Release Notes
+
+## Release 3.2.2
+* Automate version management.
+* Add CHANGES.md documentation.
+
+## Release 3.2.1
+* Added dedicated PyPI README file.
+* Refined documentation.
+
+
+## Release 3.2.0
+* Provide a command-line interface for ebcdic_parser package running via python -m ebcdic_parser. 
+
+## Release 3.1.0
+* Fixed relative path parameters in command prompt mode.
+* Refined documentation.
+
+
+## Release 3.0.0
+* Added to PyPI.
+
+## Release 2.4.1
+* Fixed issue with "Multi-schema fixed record length" layout type.
+
+## Release 2.4.0 
+* Added "Single schema variable record length" layout type.
+
+## Release 2.3.0
+* Implemented debug mode.
+
+## Release 2.1.1
+* Improved sign parsing in packedDecimal data type.
+* Added sign parsing to decimal data type.
+* Developed functional tests.
+
+## Release 2.1.0
+* The first public available release.
```

### Comparing `ebcdic_parser-3.2.1/tests/test_functional.py` & `ebcdic_parser-3.2.2/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `ebcdic_parser-3.2.1/tests/test_system_311_calls_for_service_requests_all_strings.py` & `ebcdic_parser-3.2.2/tests/test_system_311_calls_for_service_requests_all_strings.py`

 * *Files identical despite different names*

### Comparing `ebcdic_parser-3.2.1/tests/test_system_common.py` & `ebcdic_parser-3.2.2/tests/test_system_common.py`

 * *Files identical despite different names*

