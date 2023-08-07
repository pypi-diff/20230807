# Comparing `tmp/tensorshare-0.0.2.tar.gz` & `tmp/tensorshare-0.0.3.tar.gz`

## Comparing `tensorshare-0.0.2.tar` & `tensorshare-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 tensorshare-0.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 tensorshare-0.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 tensorshare-0.0.2/mkdocs.yml
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 tensorshare-0.0.2/src/tensorshare/__init__.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 tensorshare-0.0.2/src/tensorshare/import_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tensorshare-0.0.2/src/tensorshare/py.typed
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 tensorshare-0.0.2/src/tensorshare/schema.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 tensorshare-0.0.2/src/tensorshare/converter/__init__.py
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 tensorshare-0.0.2/src/tensorshare/converter/utils.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 tensorshare-0.0.2/.gitignore
--rw-r--r--   0        0        0    10758 2020-02-02 00:00:00.000000 tensorshare-0.0.2/LICENSE
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 tensorshare-0.0.2/README.md
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tensorshare-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 tensorshare-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 tensorshare-0.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 tensorshare-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 tensorshare-0.0.3/mkdocs.yml
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 tensorshare-0.0.3/src/tensorshare/__init__.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 tensorshare-0.0.3/src/tensorshare/import_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tensorshare-0.0.3/src/tensorshare/py.typed
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 tensorshare-0.0.3/src/tensorshare/schema.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 tensorshare-0.0.3/src/tensorshare/converter/__init__.py
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 tensorshare-0.0.3/src/tensorshare/converter/utils.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 tensorshare-0.0.3/.gitignore
+-rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 tensorshare-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 tensorshare-0.0.3/README.md
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tensorshare-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 tensorshare-0.0.3/PKG-INFO
```

### Comparing `tensorshare-0.0.2/CODE_OF_CONDUCT.md` & `tensorshare-0.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tensorshare-0.0.2/CONTRIBUTING.md` & `tensorshare-0.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tensorshare-0.0.2/mkdocs.yml` & `tensorshare-0.0.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tensorshare-0.0.2/src/tensorshare/__init__.py` & `tensorshare-0.0.3/src/tensorshare/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """`tensorshare `: 🤝 Trade any tensors over the network"""
 
 __author__ = "Thomas Chaigneau <t.chaigneau.tc@gmail.com>"
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 
 from tensorshare.schema import TensorShare
 
 __all__ = ["TensorShare"]
```

### Comparing `tensorshare-0.0.2/src/tensorshare/import_utils.py` & `tensorshare-0.0.3/src/tensorshare/import_utils.py`

 * *Files identical despite different names*

### Comparing `tensorshare-0.0.2/src/tensorshare/schema.py` & `tensorshare-0.0.3/src/tensorshare/converter/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,17 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Pydantic schemas to enable resilient and secure tensor sharing."""
-
-from pydantic import BaseModel, ByteSize
-
-
-class TensorShare(BaseModel):
-    """Base model for tensor sharing."""
-
-    tensors: bytes
-    size: ByteSize
+"""Converter is used to convert any tensors format to safetensors format"""
```

### Comparing `tensorshare-0.0.2/src/tensorshare/converter/utils.py` & `tensorshare-0.0.3/src/tensorshare/converter/utils.py`

 * *Files identical despite different names*

### Comparing `tensorshare-0.0.2/.gitignore` & `tensorshare-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tensorshare-0.0.2/LICENSE` & `tensorshare-0.0.3/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright 2023 Thomas Chaigneau. All rights reserved.
-
                              Apache License
                        Version 2.0, January 2004
                     http://www.apache.org/licenses/
 
 TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
 1. Definitions.
@@ -184,15 +182,15 @@
   replaced with your own identifying information. (Don't include
   the brackets!)  The text should be enclosed in the appropriate
   comment syntax for the file format. We also recommend that a
   file or class name and description of purpose be included on the
   same "printed page" as the copyright notice for easier
   identification within third-party archives.
 
-Copyright [yyyy] [name of copyright owner]
+Copyright 2023 Thomas Chaigneau. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `tensorshare-0.0.2/README.md` & `tensorshare-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tensorshare-0.0.2/pyproject.toml` & `tensorshare-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tensorshare-0.0.2/PKG-INFO` & `tensorshare-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorshare
-Version: 0.0.2
+Version: 0.0.3
 Summary: 🤝 Trade any tensors over the network
 Project-URL: Documentation, https://chainyo.github.io/tensorshare
 Project-URL: Issues, https://github.com/chainyo/tensorshare/issues
 Project-URL: Source, https://github.com/chainyo/tensorshare
 Author: Thomas Chaigneau
 License-Expression: Apache-2.0
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensorshare Version: 0.0.2 Summary: ð¤ Trade any
+Metadata-Version: 2.1 Name: tensorshare Version: 0.0.3 Summary: ð¤ Trade any
 tensors over the network Project-URL: Documentation, https://chainyo.github.io/
 tensorshare Project-URL: Issues, https://github.com/chainyo/tensorshare/issues
 Project-URL: Source, https://github.com/chainyo/tensorshare Author: Thomas
 Chaigneau License-Expression: Apache-2.0 License-File: LICENSE Keywords:
 artificial intelligence,deep learning,machine learning,tensors Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

