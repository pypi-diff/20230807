# Comparing `tmp/secrets-vault-0.2.6.tar.gz` & `tmp/secrets-vault-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets-vault-0.2.6.tar", last modified: Sat Jul 29 18:29:02 2023, max compression
+gzip compressed data, was "secrets-vault-0.2.7.tar", last modified: Mon Aug  7 17:53:06 2023, max compression
```

## Comparing `secrets-vault-0.2.6.tar` & `secrets-vault-0.2.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:29:02.062596 secrets-vault-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-29 18:29:02.062596 secrets-vault-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:29:02.062596 secrets-vault-0.2.6/secrets_vault/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/secrets_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/secrets_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/secrets_vault/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/secrets_vault/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/secrets_vault/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/secrets_vault/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/secrets_vault/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:29:02.062596 secrets-vault-0.2.6/secrets_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-29 18:29:01.000000 secrets-vault-0.2.6/secrets_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-29 18:29:02.000000 secrets-vault-0.2.6/secrets_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 18:29:01.000000 secrets-vault-0.2.6/secrets_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-29 18:29:01.000000 secrets-vault-0.2.6/secrets_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-29 18:29:01.000000 secrets-vault-0.2.6/secrets_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 18:29:01.000000 secrets-vault-0.2.6/secrets_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 18:29:02.062596 secrets-vault-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:29:02.062596 secrets-vault-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/tests/test_backwards_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-29 18:28:36.000000 secrets-vault-0.2.6/tests/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:53:06.560177 secrets-vault-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-07 17:52:40.000000 secrets-vault-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-08-07 17:53:06.560177 secrets-vault-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-08-07 17:52:40.000000 secrets-vault-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:53:06.556177 secrets-vault-0.2.7/secrets_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-07 17:52:40.000000 secrets-vault-0.2.7/secrets_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-08-07 17:52:40.000000 secrets-vault-0.2.7/secrets_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-07 17:52:40.000000 secrets-vault-0.2.7/secrets_vault/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-07 17:52:40.000000 secrets-vault-0.2.7/secrets_vault/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-07 17:52:40.000000 secrets-vault-0.2.7/secrets_vault/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 17:52:40.000000 secrets-vault-0.2.7/secrets_vault/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-08-07 17:52:40.000000 secrets-vault-0.2.7/secrets_vault/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-07 17:52:40.000000 secrets-vault-0.2.7/secrets_vault/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:53:06.560177 secrets-vault-0.2.7/secrets_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-08-07 17:53:06.000000 secrets-vault-0.2.7/secrets_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-07 17:53:06.000000 secrets-vault-0.2.7/secrets_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 17:53:06.000000 secrets-vault-0.2.7/secrets_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-07 17:53:06.000000 secrets-vault-0.2.7/secrets_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-07 17:53:06.000000 secrets-vault-0.2.7/secrets_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 17:53:06.000000 secrets-vault-0.2.7/secrets_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 17:53:06.560177 secrets-vault-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-07 17:52:40.000000 secrets-vault-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:53:06.560177 secrets-vault-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-07 17:52:40.000000 secrets-vault-0.2.7/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-07 17:52:40.000000 secrets-vault-0.2.7/tests/test_backwards_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-08-07 17:52:40.000000 secrets-vault-0.2.7/tests/test_vault.py
```

### Comparing `secrets-vault-0.2.6/LICENSE` & `secrets-vault-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.6/PKG-INFO` & `secrets-vault-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.2.6
+Version: 0.2.7
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `secrets-vault-0.2.6/README.md` & `secrets-vault-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.6/secrets_vault/__main__.py` & `secrets-vault-0.2.7/secrets_vault/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import logging
 from io import BytesIO
 
 import click
-from ruamel.yaml import YAML
 
-from secrets_vault import SecretsVault, exceptions, constants, __version__
+from secrets_vault import SecretsVault, exceptions, constants, __version__, formatters
 
 
 def serialize(v, format="yaml"):
     assert format in {"yaml", "json", "dotenv"}
 
     if isinstance(v, bool) and format == "dotenv":
         return "1" if v else "0"
@@ -24,16 +23,15 @@
     if format == "json":
         return json.dumps(v, indent=2, default=str, sort_keys=False)
     if format == "dotenv":
         # encode non-value objects as json for use in env vars
         return json.dumps(v, default=str, sort_keys=False)
     if format == "yaml":
         fout = BytesIO()
-        yaml = YAML(typ="rt")
-        yaml.dump(v, fout)
+        formatters.yaml.dump(v, fout)
         result = fout.getvalue().decode()
         fout.close()
         return result.strip()
     raise NotImplementedError(f"Unsupported format: {format}")
 
 
 @click.group(help="Manage a local secrets vault.")
```

### Comparing `secrets-vault-0.2.6/secrets_vault/backends.py` & `secrets-vault-0.2.7/secrets_vault/backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.6/secrets_vault/constants.py` & `secrets-vault-0.2.7/secrets_vault/constants.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.6/secrets_vault/vault.py` & `secrets-vault-0.2.7/secrets_vault/vault.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 import os
 import subprocess
 import tempfile
 from io import BytesIO
 from pathlib import Path
 
 import pydash
-from ruamel.yaml import YAML
 
-from secrets_vault import exceptions, constants
+from secrets_vault import exceptions, constants, formatters
 
 log = logging.getLogger(__name__)
 
 
 class SecretsVault:
     def __init__(
         self,
@@ -137,26 +136,24 @@
                 "Could not find encryption master key. "
                 f"Set it as an environment variable 'MASTER_KEY', or in a file '{master_key_filepath}'"
             )
         return master_key
 
     def _deserialize(self, data: bytes) -> dict:
         if self.file_format in {"yaml", "json"}:
-            yaml = YAML(typ="rt")
             fin = BytesIO(data)
-            return yaml.load(fin)
+            return formatters.yaml.load(fin)
         raise NotImplementedError(f"Unknown file_format {self.file_format}")
 
     def _serialize(self, data: dict) -> bytes:
         if self.file_format == "json":
             return json.dumps(data, indent=4).encode()
         elif self.file_format == "yaml":
-            yaml = YAML(typ="rt")
             fout = BytesIO()
-            yaml.dump(data, fout)
+            formatters.yaml.dump(data, fout)
             result = fout.getvalue()
             fout.close()
             return result
 
         raise NotImplementedError(f"Unknown file_format {self.file_format}")
 
     @classmethod
```

### Comparing `secrets-vault-0.2.6/secrets_vault.egg-info/PKG-INFO` & `secrets-vault-0.2.7/secrets_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-vault
-Version: 0.2.6
+Version: 0.2.7
 Summary: Simple encrypted secrets for Python
 Home-page: https://github.com/anthonynsimon/secrets-vault
 Author: Anthony N. Simon
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `secrets-vault-0.2.6/setup.py` & `secrets-vault-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.6/tests/test_backends.py` & `secrets-vault-0.2.7/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.6/tests/test_backwards_compat.py` & `secrets-vault-0.2.7/tests/test_backwards_compat.py`

 * *Files identical despite different names*

### Comparing `secrets-vault-0.2.6/tests/test_vault.py` & `secrets-vault-0.2.7/tests/test_vault.py`

 * *Files identical despite different names*

