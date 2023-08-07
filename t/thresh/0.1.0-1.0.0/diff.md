# Comparing `tmp/thresh-0.1.0.tar.gz` & `tmp/thresh-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\heine\Documents\research\nlproc.tools\data_tools\dist\.tmp-w6xakl92\thresh-0.1.0.tar", last modified: Mon Jul 31 06:05:37 2023, max compression
+gzip compressed data, was "C:\Users\heine\Documents\research\thresh.tools\data_tools\dist\.tmp-ormqdzqh\thresh-1.0.0.tar", last modified: Mon Aug  7 05:18:52 2023, max compression
```

## Comparing `thresh-0.1.0.tar` & `thresh-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 06:05:37.319338 thresh-0.1.0/
--rw-rw-rw-   0        0        0     1091 2023-07-23 23:56:05.000000 thresh-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      755 2023-07-31 06:05:37.320336 thresh-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-31 05:37:54.000000 thresh-0.1.0/README.md
--rw-rw-rw-   0        0        0      110 2023-07-23 23:55:48.000000 thresh-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      731 2023-07-31 06:05:37.326335 thresh-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-31 06:05:37.262338 thresh-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 06:05:37.277335 thresh-0.1.0/src/thresh/
--rw-rw-rw-   0        0        0       76 2023-07-29 01:51:02.000000 thresh-0.1.0/src/thresh/__init__.py
--rw-rw-rw-   0        0        0     2207 2023-07-31 05:38:39.000000 thresh-0.1.0/src/thresh/convert.py
--rw-rw-rw-   0        0        0     1868 2023-07-31 05:37:54.000000 thresh-0.1.0/src/thresh/dataloader.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:05:37.316357 thresh-0.1.0/src/thresh/datasets/
--rw-rw-rw-   0        0        0        0 2023-07-24 00:28:54.000000 thresh-0.1.0/src/thresh/datasets/__init__.py
--rw-rw-rw-   0        0        0     2332 2023-07-29 06:21:41.000000 thresh-0.1.0/src/thresh/datasets/da-san-martino-etal-2019.py
--rw-rw-rw-   0        0        0      980 2023-07-29 06:05:30.000000 thresh-0.1.0/src/thresh/datasets/frank.py
--rw-rw-rw-   0        0        0     4056 2023-07-29 06:28:43.000000 thresh-0.1.0/src/thresh/datasets/mqm.py
--rw-rw-rw-   0        0        0      168 2023-07-29 05:47:24.000000 thresh-0.1.0/src/thresh/datasets/salsa.py
--rw-rw-rw-   0        0        0     2104 2023-07-29 06:29:02.000000 thresh-0.1.0/src/thresh/datasets/scarecrow.py
--rw-rw-rw-   0        0        0     1270 2023-07-29 06:05:07.000000 thresh-0.1.0/src/thresh/datasets/snac.py
--rw-rw-rw-   0        0        0     2575 2023-07-29 06:14:00.000000 thresh-0.1.0/src/thresh/datasets/wu-etal-2023.py
--rw-rw-rw-   0        0        0    12956 2023-07-31 05:38:39.000000 thresh-0.1.0/src/thresh/names.py
--rw-rw-rw-   0        0        0      935 2023-07-29 01:38:47.000000 thresh-0.1.0/src/thresh/util.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:05:37.304336 thresh-0.1.0/src/thresh.egg-info/
--rw-rw-rw-   0        0        0      755 2023-07-31 06:05:37.000000 thresh-0.1.0/src/thresh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-07-31 06:05:37.000000 thresh-0.1.0/src/thresh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 06:05:37.000000 thresh-0.1.0/src/thresh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-31 06:05:37.000000 thresh-0.1.0/src/thresh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-31 06:05:37.000000 thresh-0.1.0/src/thresh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 05:18:52.600947 thresh-1.0.0/
+-rw-rw-rw-   0        0        0    11558 2023-08-07 05:15:27.000000 thresh-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      839 2023-08-07 05:18:52.600947 thresh-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-31 05:37:54.000000 thresh-1.0.0/README.md
+-rw-rw-rw-   0        0        0      110 2023-07-23 23:55:48.000000 thresh-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      804 2023-08-07 05:18:52.602946 thresh-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 05:18:52.551463 thresh-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 05:18:52.565950 thresh-1.0.0/src/thresh/
+-rw-rw-rw-   0        0        0       76 2023-07-29 01:51:02.000000 thresh-1.0.0/src/thresh/__init__.py
+-rw-rw-rw-   0        0        0     2193 2023-08-07 05:10:47.000000 thresh-1.0.0/src/thresh/convert.py
+-rw-rw-rw-   0        0        0     1877 2023-08-04 23:36:17.000000 thresh-1.0.0/src/thresh/dataloader.py
+drwxrwxrwx   0        0        0        0 2023-08-07 05:18:52.599946 thresh-1.0.0/src/thresh/datasets/
+-rw-rw-rw-   0        0        0        0 2023-07-24 00:28:54.000000 thresh-1.0.0/src/thresh/datasets/__init__.py
+-rw-rw-rw-   0        0        0     2792 2023-08-03 01:42:51.000000 thresh-1.0.0/src/thresh/datasets/arxivedits.py
+-rw-rw-rw-   0        0        0     2575 2023-07-29 06:14:00.000000 thresh-1.0.0/src/thresh/datasets/fg-rlhf.py
+-rw-rw-rw-   0        0        0      980 2023-07-29 06:05:30.000000 thresh-1.0.0/src/thresh/datasets/frank.py
+-rw-rw-rw-   0        0        0     4056 2023-07-29 06:28:43.000000 thresh-1.0.0/src/thresh/datasets/mqm.py
+-rw-rw-rw-   0        0        0     2332 2023-07-29 06:21:41.000000 thresh-1.0.0/src/thresh/datasets/propaganda.py
+-rw-rw-rw-   0        0        0      168 2023-07-29 05:47:24.000000 thresh-1.0.0/src/thresh/datasets/salsa.py
+-rw-rw-rw-   0        0        0     2104 2023-07-29 06:29:02.000000 thresh-1.0.0/src/thresh/datasets/scarecrow.py
+-rw-rw-rw-   0        0        0     1270 2023-07-29 06:05:07.000000 thresh-1.0.0/src/thresh/datasets/snac.py
+-rw-rw-rw-   0        0        0    12956 2023-08-04 23:37:59.000000 thresh-1.0.0/src/thresh/names.py
+-rw-rw-rw-   0        0        0      935 2023-07-29 01:38:47.000000 thresh-1.0.0/src/thresh/util.py
+drwxrwxrwx   0        0        0        0 2023-08-07 05:18:52.586980 thresh-1.0.0/src/thresh.egg-info/
+-rw-rw-rw-   0        0        0      839 2023-08-07 05:18:52.000000 thresh-1.0.0/src/thresh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-08-07 05:18:52.000000 thresh-1.0.0/src/thresh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 05:18:52.000000 thresh-1.0.0/src/thresh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-07 05:18:52.000000 thresh-1.0.0/src/thresh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 05:18:52.000000 thresh-1.0.0/src/thresh.egg-info/top_level.txt
```

### Comparing `thresh-0.1.0/PKG-INFO` & `thresh-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: thresh
-Version: 0.1.0
+Version: 1.0.0
 Summary: Load and manage data collection with thresh.tools
 Home-page: https://github.com/davidheineman/thresh.tools
 Author: David Heineman
 Author-email: dheineman3@gatech.edu
 Project-URL: Bug Tracker, https://github.com/davidheineman/thresh.tools/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Data Tools for thresh.tools
 
 This is a helper library for [**thresh.tools**](https://thresh.tools/). Please see the [**main repo**](https://github.com/davidheineman/thresh.tools) for documentation.
```

### Comparing `thresh-0.1.0/setup.cfg` & `thresh-1.0.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6872 6573 680d 0a76 6572 7369   = thresh..versi
-00000020: 6f6e 203d 2030 2e31 2e30 0d0a 6175 7468  on = 0.1.0..auth
+00000020: 6f6e 203d 2031 2e30 2e30 0d0a 6175 7468  on = 1.0.0..auth
 00000030: 6f72 203d 2044 6176 6964 2048 6569 6e65  or = David Heine
 00000040: 6d61 6e0d 0a61 7574 686f 725f 656d 6169  man..author_emai
 00000050: 6c20 3d20 6468 6569 6e65 6d61 6e33 4067  l = dheineman3@g
 00000060: 6174 6563 682e 6564 750d 0a64 6573 6372  atech.edu..descr
 00000070: 6970 7469 6f6e 203d 204c 6f61 6420 616e  iption = Load an
 00000080: 6420 6d61 6e61 6765 2064 6174 6120 636f  d manage data co
 00000090: 6c6c 6563 7469 6f6e 2077 6974 6820 7468  llection with th
@@ -23,24 +23,29 @@
 00000160: 7562 2e63 6f6d 2f64 6176 6964 6865 696e  ub.com/davidhein
 00000170: 656d 616e 2f74 6872 6573 682e 746f 6f6c  eman/thresh.tool
 00000180: 732f 6973 7375 6573 0d0a 636c 6173 7369  s/issues..classi
 00000190: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
 000001a0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
 000001b0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
 000001c0: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-000001d0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-000001e0: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
-000001f0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-00000200: 2049 6e64 6570 656e 6465 6e74 0d0a 0d0a   Independent....
-00000210: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
-00000220: 6765 5f64 6972 203d 200d 0a09 3d20 7372  ge_dir = ...= sr
-00000230: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
-00000240: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
-00000250: 6972 6573 203d 203e 3d33 2e36 0d0a 696e  ires = >=3.6..in
-00000260: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-00000270: 200d 0a09 7079 7961 6d6c 0d0a 0964 6565   ...pyyaml...dee
-00000280: 7064 6966 660d 0a0d 0a5b 6f70 7469 6f6e  pdiff....[option
-00000290: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-000002a0: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
-000002b0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-000002c0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-000002d0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+000001d0: 4170 7072 6f76 6564 203a 3a20 4170 6163  Approved :: Apac
+000001e0: 6865 2053 6f66 7477 6172 6520 4c69 6365  he Software Lice
+000001f0: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
+00000200: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+00000210: 6570 656e 6465 6e74 0d0a 0954 6f70 6963  ependent...Topic
+00000220: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
+00000230: 6e67 696e 6565 7269 6e67 203a 3a20 4172  ngineering :: Ar
+00000240: 7469 6669 6369 616c 2049 6e74 656c 6c69  tificial Intelli
+00000250: 6765 6e63 650d 0a0d 0a5b 6f70 7469 6f6e  gence....[option
+00000260: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
+00000270: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
+00000280: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+00000290: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+000002a0: 3e3d 332e 360d 0a69 6e73 7461 6c6c 5f72  >=3.6..install_r
+000002b0: 6571 7569 7265 7320 3d20 0d0a 0970 7979  equires = ...pyy
+000002c0: 616d 6c0d 0a09 6465 6570 6469 6666 0d0a  aml...deepdiff..
+000002d0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+000002e0: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
+000002f0: 203d 2073 7263 0d0a 0d0a 5b65 6767 5f69   = src....[egg_i
+00000300: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+00000310: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+00000320: 0d0a 0d0a                                ....
```

### Comparing `thresh-0.1.0/src/thresh/convert.py` & `thresh-1.0.0/src/thresh/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .util import verify_exists
 import csv, json, os, copy, logging, importlib
 
 utils_path = "datasets"
-folder_based_datasets = ["da-san-martino-etal-2019"]
+folder_based_datasets = ["propaganda"]
 
 logging.basicConfig(level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s")
 logger = logging.getLogger(__name__)
 
 
 def convert_dataset(dataset_name: str, data_path: str, reverse: bool=False, output_path: str=None, limit: int=None) -> dict:
     """
```

### Comparing `thresh-0.1.0/src/thresh/dataloader.py` & `thresh-1.0.0/src/thresh/dataloader.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .names import Entry, Edit, Interface
 from typing import List
 import json, yaml
 
 
 def load_interface(typology_dict: str) -> Interface:
     """
-    Load an thresh.tools interface given its typology
+    Load a thresh.tools interface given its typology
     """
 
     # Verify and load files
     verify_exists(typology_dict)
     with open(typology_dict, 'r', encoding='utf-8') as f:
         typology_dict = yaml.safe_load(f)
 
@@ -25,22 +25,22 @@
     # Create custom init function
     def custom_init(self, typology: dict):
         for key, value in typology.items():
             setattr(self, key, value)
         self.entry_class = self.create_entry_class()
 
         # Create classes for each edit
-        primitive_edits = [e for e in self.edits if 'type' not in e.keys() or e['type'] == 'primitive']
+        single_span_edits = [e for e in self.edits if 'type' not in e.keys() or e['type'] == 'single_span']
         composite_edits = [e for e in self.edits if 'type' in e.keys() and e['type'] == 'composite']
 
         self.edit_classes = {}
         self.annotation_classes = {}
 
-        primitive_edit_classes = {k: self.create_edit_class(k) for k in set([e['name'] for e in primitive_edits])}
-        self.edit_classes.update(primitive_edit_classes)
+        single_span_edit_classes = {k: self.create_edit_class(k) for k in set([e['name'] for e in single_span_edits])}
+        self.edit_classes.update(single_span_edit_classes)
 
         composite_edit_classes = {k: self.create_edit_class(k) for k in set([e['name'] for e in composite_edits])}
         self.edit_classes.update(composite_edit_classes)
 
     # Create typology class
     TypologyClass = type(f'{class_name}', (Interface,), {"__init__": custom_init})
```

### Comparing `thresh-0.1.0/src/thresh/datasets/da-san-martino-etal-2019.py` & `thresh-1.0.0/src/thresh/datasets/propaganda.py`

 * *Files identical despite different names*

### Comparing `thresh-0.1.0/src/thresh/datasets/frank.py` & `thresh-1.0.0/src/thresh/datasets/frank.py`

 * *Files identical despite different names*

### Comparing `thresh-0.1.0/src/thresh/datasets/mqm.py` & `thresh-1.0.0/src/thresh/datasets/mqm.py`

 * *Files identical despite different names*

### Comparing `thresh-0.1.0/src/thresh/datasets/scarecrow.py` & `thresh-1.0.0/src/thresh/datasets/scarecrow.py`

 * *Files identical despite different names*

### Comparing `thresh-0.1.0/src/thresh/datasets/snac.py` & `thresh-1.0.0/src/thresh/datasets/snac.py`

 * *Files identical despite different names*

### Comparing `thresh-0.1.0/src/thresh/datasets/wu-etal-2023.py` & `thresh-1.0.0/src/thresh/datasets/fg-rlhf.py`

 * *Files identical despite different names*

### Comparing `thresh-0.1.0/src/thresh/names.py` & `thresh-1.0.0/src/thresh/names.py`

 * *Files identical despite different names*

### Comparing `thresh-0.1.0/src/thresh/util.py` & `thresh-1.0.0/src/thresh/util.py`

 * *Files identical despite different names*

### Comparing `thresh-0.1.0/src/thresh.egg-info/PKG-INFO` & `thresh-1.0.0/src/thresh.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: thresh
-Version: 0.1.0
+Version: 1.0.0
 Summary: Load and manage data collection with thresh.tools
 Home-page: https://github.com/davidheineman/thresh.tools
 Author: David Heineman
 Author-email: dheineman3@gatech.edu
 Project-URL: Bug Tracker, https://github.com/davidheineman/thresh.tools/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Data Tools for thresh.tools
 
 This is a helper library for [**thresh.tools**](https://thresh.tools/). Please see the [**main repo**](https://github.com/davidheineman/thresh.tools) for documentation.
```

