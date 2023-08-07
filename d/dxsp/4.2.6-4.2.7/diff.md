# Comparing `tmp/dxsp-4.2.6.tar.gz` & `tmp/dxsp-4.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-4.2.6.tar", max compression
+gzip compressed data, was "dxsp-4.2.7.tar", max compression
```

## Comparing `dxsp-4.2.6.tar` & `dxsp-4.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-08-06 14:02:37.371137 dxsp-4.2.6/LICENSE
--rw-r--r--   0        0        0     2740 2023-08-06 14:02:37.371137 dxsp-4.2.6/README.md
--rw-r--r--   0        0        0      158 2023-08-06 14:02:37.371137 dxsp-4.2.6/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-08-06 14:02:37.371137 dxsp-4.2.6/dxsp/config.py
--rw-r--r--   0        0        0    12124 2023-08-06 14:02:37.371137 dxsp-4.2.6/dxsp/default_settings.toml
--rw-r--r--   0        0        0     5743 2023-08-06 14:02:37.371137 dxsp-4.2.6/dxsp/main.py
--rw-r--r--   0        0        0      104 2023-08-06 14:02:37.371137 dxsp-4.2.6/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-08-06 14:02:37.371137 dxsp-4.2.6/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1864 2023-08-06 14:02:37.371137 dxsp-4.2.6/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0     1037 2023-08-06 14:02:37.371137 dxsp-4.2.6/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0      102 2023-08-06 14:02:37.371137 dxsp-4.2.6/dxsp/utils/__init__.py
--rw-r--r--   0        0        0     4834 2023-08-06 14:02:37.371137 dxsp-4.2.6/dxsp/utils/account_utils.py
--rw-r--r--   0        0        0     6619 2023-08-06 14:02:37.371137 dxsp-4.2.6/dxsp/utils/contract_utils.py
--rw-r--r--   0        0        0     1990 2023-08-06 14:02:37.371137 dxsp-4.2.6/dxsp/utils/explorer_utils.py
--rw-r--r--   0        0        0      363 2023-08-06 14:02:37.371137 dxsp-4.2.6/dxsp/utils/utils.py
--rw-r--r--   0        0        0     3933 2023-08-06 14:02:41.315234 dxsp-4.2.6/pyproject.toml
--rw-r--r--   0        0        0     3628 1970-01-01 00:00:00.000000 dxsp-4.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-07 08:39:25.883600 dxsp-4.2.7/LICENSE
+-rw-r--r--   0        0        0     2740 2023-08-07 08:39:25.883600 dxsp-4.2.7/README.md
+-rw-r--r--   0        0        0      158 2023-08-07 08:39:25.887600 dxsp-4.2.7/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-08-07 08:39:25.887600 dxsp-4.2.7/dxsp/config.py
+-rw-r--r--   0        0        0    12124 2023-08-07 08:39:25.887600 dxsp-4.2.7/dxsp/default_settings.toml
+-rw-r--r--   0        0        0     5743 2023-08-07 08:39:25.887600 dxsp-4.2.7/dxsp/main.py
+-rw-r--r--   0        0        0      104 2023-08-07 08:39:25.887600 dxsp-4.2.7/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-08-07 08:39:25.887600 dxsp-4.2.7/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1864 2023-08-07 08:39:25.887600 dxsp-4.2.7/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0     1037 2023-08-07 08:39:25.887600 dxsp-4.2.7/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0      102 2023-08-07 08:39:25.887600 dxsp-4.2.7/dxsp/utils/__init__.py
+-rw-r--r--   0        0        0     4834 2023-08-07 08:39:25.887600 dxsp-4.2.7/dxsp/utils/account_utils.py
+-rw-r--r--   0        0        0     6619 2023-08-07 08:39:25.887600 dxsp-4.2.7/dxsp/utils/contract_utils.py
+-rw-r--r--   0        0        0     1990 2023-08-07 08:39:25.887600 dxsp-4.2.7/dxsp/utils/explorer_utils.py
+-rw-r--r--   0        0        0      363 2023-08-07 08:39:25.887600 dxsp-4.2.7/dxsp/utils/utils.py
+-rw-r--r--   0        0        0     4012 2023-08-07 08:39:35.179856 dxsp-4.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3628 1970-01-01 00:00:00.000000 dxsp-4.2.7/PKG-INFO
```

### Comparing `dxsp-4.2.6/LICENSE` & `dxsp-4.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.6/README.md` & `dxsp-4.2.7/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.6/dxsp/default_settings.toml` & `dxsp-4.2.7/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.6/dxsp/main.py` & `dxsp-4.2.7/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.6/dxsp/protocols/oneinch.py` & `dxsp-4.2.7/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.6/dxsp/protocols/uniswap.py` & `dxsp-4.2.7/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.6/dxsp/protocols/zerox.py` & `dxsp-4.2.7/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.6/dxsp/utils/account_utils.py` & `dxsp-4.2.7/dxsp/utils/account_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.6/dxsp/utils/contract_utils.py` & `dxsp-4.2.7/dxsp/utils/contract_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.6/dxsp/utils/explorer_utils.py` & `dxsp-4.2.7/dxsp/utils/explorer_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.6/pyproject.toml` & `dxsp-4.2.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "4.2.6"
+version = "4.2.7"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
 
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/dxsp/discussions"
 "Issues" =  "https://github.com/mraniki/dxsp/issues"
 
+
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
 loguru = "^0.7.0"
 web3 = "^6.4.0"
 pycoingecko = "^3.1.0"
 uniswap-python = "^0.7.0"
 
+
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^8.0.2"
 ruff = "^0.0.280"
+
+
   
 [tool.ruff]
 select = [
   "E",  # pycodestyle
   "F",  # pyflakes
   "I",  # isort
 ]
@@ -44,21 +48,14 @@
 ignore = ["F401"]
 format = "github"
 fixable = ["ALL"]
 
 
 
 
-
-
-
-
-
-
-
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.2.0"
 eth_tester = "^0.9.0b2"
@@ -76,31 +73,25 @@
     "examples/*",
     "docs/*",
     "*/config.py"
 ]
 
 
 
-
-
-
-
-
-
-
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = ">=5,<6"
-sphinx_bootstrap_theme = "^0.8.1"
-sphinxext-remoteliteralinclude = "^0.4.0"
-
-
-
+sphinx = "^7.0.0"
+pydata-sphinx-theme = "^0.13.3"
+sphinx-hoverxref = "^1.3.0"
+sphinx-notfound-page = "^0.8.3"
+sphinx_copybutton = "0.5.2"
+myst_parser = "^2.0.0"
+sphinx_design = "^0.5.0"
 
 
 # [tool.semantic_release]
 # version_variable = ["pyproject.toml:version","dxsp/__init__.py:__version__"]
 # branch = "main"
 # upload_to_pypi = true
 # upload_to_release = true
```

### Comparing `dxsp-4.2.6/PKG-INFO` & `dxsp-4.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 4.2.6
+Version: 4.2.7
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dxsp Version: 4.2.6 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 4.2.7 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist:
 pycoingecko (>=3.1.0,<4.0.0) Requires-Dist: uniswap-python (>=0.7.0,<0.8.0)
```

