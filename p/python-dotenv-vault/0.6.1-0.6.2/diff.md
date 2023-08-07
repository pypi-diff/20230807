# Comparing `tmp/python-dotenv-vault-0.6.1.tar.gz` & `tmp/python-dotenv-vault-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dotenv-vault-0.6.1.tar", last modified: Tue Aug  1 00:45:06 2023, max compression
+gzip compressed data, was "python-dotenv-vault-0.6.2.tar", last modified: Mon Aug  7 04:39:54 2023, max compression
```

## Comparing `python-dotenv-vault-0.6.1.tar` & `python-dotenv-vault-0.6.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:45:06.788162 python-dotenv-vault-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-08-01 00:45:06.788162 python-dotenv-vault-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:45:06.788162 python-dotenv-vault-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:45:06.780162 python-dotenv-vault-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:45:06.788162 python-dotenv-vault-0.6.1/src/dotenv_vault/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/src/dotenv_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/src/dotenv_vault/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/src/dotenv_vault/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-08-01 00:44:45.000000 python-dotenv-vault-0.6.1/src/dotenv_vault/test_vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:45:06.788162 python-dotenv-vault-0.6.1/src/python_dotenv_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-08-01 00:45:06.000000 python-dotenv-vault-0.6.1/src/python_dotenv_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-01 00:45:06.000000 python-dotenv-vault-0.6.1/src/python_dotenv_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:45:06.000000 python-dotenv-vault-0.6.1/src/python_dotenv_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-01 00:45:06.000000 python-dotenv-vault-0.6.1/src/python_dotenv_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 00:45:06.000000 python-dotenv-vault-0.6.1/src/python_dotenv_vault.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:39:54.595458 python-dotenv-vault-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-08-07 04:39:54.591458 python-dotenv-vault-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 04:39:54.595458 python-dotenv-vault-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:39:54.591458 python-dotenv-vault-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:39:54.591458 python-dotenv-vault-0.6.2/src/dotenv_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/src/dotenv_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/src/dotenv_vault/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/src/dotenv_vault/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/src/dotenv_vault/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:39:54.591458 python-dotenv-vault-0.6.2/src/python_dotenv_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-08-07 04:39:54.000000 python-dotenv-vault-0.6.2/src/python_dotenv_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-07 04:39:54.000000 python-dotenv-vault-0.6.2/src/python_dotenv_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 04:39:54.000000 python-dotenv-vault-0.6.2/src/python_dotenv_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 04:39:54.000000 python-dotenv-vault-0.6.2/src/python_dotenv_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 04:39:54.000000 python-dotenv-vault-0.6.2/src/python_dotenv_vault.egg-info/top_level.txt
```

### Comparing `python-dotenv-vault-0.6.1/CHANGELOG.md` & `python-dotenv-vault-0.6.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
 ## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.1...master)
 
+## 0.6.2
+
+### Changed
+
+- Look for .env.vault file at same location as .env file. Finds .env file anywhere in app (just like original python lib) [#13](https://github.com/dotenv-org/python-dotenv-vault/pull/13)
+
 ## 0.6.1
 
 ### Changed
 
 - Fix fallback issue with gunicorn not respecting the current working directory when attempting to call `find_dotenv`. [#17](https://github.com/dotenv-org/python-dotenv-vault/pull/17)
 
 ## 0.6.0
```

### Comparing `python-dotenv-vault-0.6.1/LICENSE` & `python-dotenv-vault-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.6.1/PKG-INFO` & `python-dotenv-vault-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dotenv-vault
-Version: 0.6.1
+Version: 0.6.2
 Summary: Decrypt .env.vault file.
 Home-page: https://github.com/dotenv-org/python-dotenv-vault
 Author: dotenv
 Author-email: mot@dotenv.org
 License: MIT
 Keywords: environment,environment variables,deployments,settings,env,dotenv,configurations,python,dotenv-vault
 Description-Content-Type: text/markdown
@@ -172,14 +172,20 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
 ## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.1...master)
 
+## 0.6.2
+
+### Changed
+
+- Look for .env.vault file at same location as .env file. Finds .env file anywhere in app (just like original python lib) [#13](https://github.com/dotenv-org/python-dotenv-vault/pull/13)
+
 ## 0.6.1
 
 ### Changed
 
 - Fix fallback issue with gunicorn not respecting the current working directory when attempting to call `find_dotenv`. [#17](https://github.com/dotenv-org/python-dotenv-vault/pull/17)
 
 ## 0.6.0
```

### Comparing `python-dotenv-vault-0.6.1/README.md` & `python-dotenv-vault-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.6.1/setup.py` & `python-dotenv-vault-0.6.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import sys
 from setuptools import setup, find_packages
 
 src = {}
 dir = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(dir, "src/dotenv_vault", "__version__.py"), "r") as f:
     exec(f.read(), src)
```

### Comparing `python-dotenv-vault-0.6.1/src/dotenv_vault/main.py` & `python-dotenv-vault-0.6.2/src/dotenv_vault/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 from __future__ import annotations
 
 from base64 import b64decode
 import io
 import os
+import logging
+
 from typing import (IO, Optional, Union)
 from urllib.parse import urlparse, parse_qsl
 
 from cryptography.hazmat.primitives.ciphers.aead import AESGCM
 from cryptography.exceptions import InvalidTag
 import dotenv.main as dotenv
 
+logger = logging.getLogger(__name__)
+
+def load_dotenv_vault() -> str:
+    path = dotenv.find_dotenv()
+    if not path:
+        return path
+    path = os.path.dirname(path)
+    if '.env.vault' not in os.listdir(path):
+        # we fall back to .env
+        logger.warning(f"You set DOTENV_KEY but you are missing a .env.vault file at {path}. Did you forget to build it?")
+        return f"{path}/.env"
+    return f"{path}/.env.vault"
+
 
 def load_dotenv(
     dotenv_path: Union[str, os.PathLike, None] = None,
     stream: Optional[IO[str]] = None,
     verbose: bool = False,
     override: bool = True,
     interpolate: bool = True,
@@ -36,15 +51,15 @@
     Other parameters to `load_dotenv` are passed througg to the
     python-dotenv loader. In particular, whether `load_dotenv`
     overrides existing environment settings or not is determined by
     the `override` flag.
 
     """
     if "DOTENV_KEY" in os.environ:
-        vault_stream = parse_vault(open(".env.vault"))
+        vault_stream = parse_vault(open(load_dotenv_vault()))
         return dotenv.load_dotenv(
             stream=vault_stream,
             verbose=verbose,
             override=override,
             interpolate=interpolate,
             encoding=encoding
         )
@@ -71,15 +86,15 @@
     """Parse information from DOTENV_KEY, and decrypt vault.
     """
     dotenv_key = os.environ.get("DOTENV_KEY")
     if dotenv_key is None:
         raise DotEnvVaultError("NOT_FOUND_DOTENV_KEY: Cannot find ENV['DOTENV_KEY']")
 
     # Use the python-dotenv library to read the .env.vault file.
-    vault = dotenv.DotEnv(dotenv_path=".env.vault", stream=vault_stream)
+    vault = dotenv.DotEnv(dotenv_path=load_dotenv_vault(), stream=vault_stream)
 
     # Extract segments from the DOTENV_KEY environment variable one by
     # one and retrieve the corresponding ciphertext from the vault
     # data.
     keys = []
     for dotenv_key_entry in [i.strip() for i in dotenv_key.split(',')]:
         key, environment_key = parse_key(dotenv_key_entry)
```

### Comparing `python-dotenv-vault-0.6.1/src/python_dotenv_vault.egg-info/PKG-INFO` & `python-dotenv-vault-0.6.2/src/python_dotenv_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dotenv-vault
-Version: 0.6.1
+Version: 0.6.2
 Summary: Decrypt .env.vault file.
 Home-page: https://github.com/dotenv-org/python-dotenv-vault
 Author: dotenv
 Author-email: mot@dotenv.org
 License: MIT
 Keywords: environment,environment variables,deployments,settings,env,dotenv,configurations,python,dotenv-vault
 Description-Content-Type: text/markdown
@@ -172,14 +172,20 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
 ## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.1...master)
 
+## 0.6.2
+
+### Changed
+
+- Look for .env.vault file at same location as .env file. Finds .env file anywhere in app (just like original python lib) [#13](https://github.com/dotenv-org/python-dotenv-vault/pull/13)
+
 ## 0.6.1
 
 ### Changed
 
 - Fix fallback issue with gunicorn not respecting the current working directory when attempting to call `find_dotenv`. [#17](https://github.com/dotenv-org/python-dotenv-vault/pull/17)
 
 ## 0.6.0
```

