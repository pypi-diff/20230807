# Comparing `tmp/dxsp-4.2.8.tar.gz` & `tmp/dxsp-4.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-4.2.8.tar", max compression
+gzip compressed data, was "dxsp-4.2.9.tar", max compression
```

## Comparing `dxsp-4.2.8.tar` & `dxsp-4.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-08-07 10:20:25.760173 dxsp-4.2.8/LICENSE
--rw-r--r--   0        0        0     2740 2023-08-07 10:20:25.760173 dxsp-4.2.8/README.md
--rw-r--r--   0        0        0      158 2023-08-07 10:20:25.760173 dxsp-4.2.8/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-08-07 10:20:25.760173 dxsp-4.2.8/dxsp/config.py
--rw-r--r--   0        0        0    12124 2023-08-07 10:20:25.764173 dxsp-4.2.8/dxsp/default_settings.toml
--rw-r--r--   0        0        0     5743 2023-08-07 10:20:25.764173 dxsp-4.2.8/dxsp/main.py
--rw-r--r--   0        0        0      104 2023-08-07 10:20:25.764173 dxsp-4.2.8/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-08-07 10:20:25.764173 dxsp-4.2.8/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1864 2023-08-07 10:20:25.764173 dxsp-4.2.8/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0     1037 2023-08-07 10:20:25.764173 dxsp-4.2.8/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0      102 2023-08-07 10:20:25.764173 dxsp-4.2.8/dxsp/utils/__init__.py
--rw-r--r--   0        0        0     4834 2023-08-07 10:20:25.764173 dxsp-4.2.8/dxsp/utils/account_utils.py
--rw-r--r--   0        0        0     6619 2023-08-07 10:20:25.764173 dxsp-4.2.8/dxsp/utils/contract_utils.py
--rw-r--r--   0        0        0     1990 2023-08-07 10:20:25.764173 dxsp-4.2.8/dxsp/utils/explorer_utils.py
--rw-r--r--   0        0        0      363 2023-08-07 10:20:25.764173 dxsp-4.2.8/dxsp/utils/utils.py
--rw-r--r--   0        0        0     4014 2023-08-07 10:20:29.720267 dxsp-4.2.8/pyproject.toml
--rw-r--r--   0        0        0     3628 1970-01-01 00:00:00.000000 dxsp-4.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-07 10:24:41.067292 dxsp-4.2.9/LICENSE
+-rw-r--r--   0        0        0     2442 2023-08-07 10:24:41.067292 dxsp-4.2.9/README.md
+-rw-r--r--   0        0        0      158 2023-08-07 10:24:41.067292 dxsp-4.2.9/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-08-07 10:24:41.067292 dxsp-4.2.9/dxsp/config.py
+-rw-r--r--   0        0        0    12124 2023-08-07 10:24:41.067292 dxsp-4.2.9/dxsp/default_settings.toml
+-rw-r--r--   0        0        0     5743 2023-08-07 10:24:41.067292 dxsp-4.2.9/dxsp/main.py
+-rw-r--r--   0        0        0      104 2023-08-07 10:24:41.067292 dxsp-4.2.9/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-08-07 10:24:41.067292 dxsp-4.2.9/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1864 2023-08-07 10:24:41.067292 dxsp-4.2.9/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0     1037 2023-08-07 10:24:41.067292 dxsp-4.2.9/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0      102 2023-08-07 10:24:41.067292 dxsp-4.2.9/dxsp/utils/__init__.py
+-rw-r--r--   0        0        0     4834 2023-08-07 10:24:41.067292 dxsp-4.2.9/dxsp/utils/account_utils.py
+-rw-r--r--   0        0        0     6619 2023-08-07 10:24:41.067292 dxsp-4.2.9/dxsp/utils/contract_utils.py
+-rw-r--r--   0        0        0     1990 2023-08-07 10:24:41.067292 dxsp-4.2.9/dxsp/utils/explorer_utils.py
+-rw-r--r--   0        0        0      363 2023-08-07 10:24:41.067292 dxsp-4.2.9/dxsp/utils/utils.py
+-rw-r--r--   0        0        0     4016 2023-08-07 10:24:45.315331 dxsp-4.2.9/pyproject.toml
+-rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 dxsp-4.2.9/PKG-INFO
```

### Comparing `dxsp-4.2.8/LICENSE` & `dxsp-4.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.8/README.md` & `dxsp-4.2.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 
 <table style="border: 1px solid transparent">
   <tr>
     <td>
 <a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a>
-<a href="https://github.com/mraniki/tt/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
-<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a><br>
-<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a>
-<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a><br>
+<a href="https://github.com/mraniki/tt/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a><br>
+<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a><br>
   </td>
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/dxsp/"><img src="https://img.shields.io/pypi/v/dxsp?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/dxsp/"><img src="https://img.shields.io/pypi/dm/dxsp?style=for-the-badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey"></a><br>
```

#### html2text {}

```diff
@@ -1,16 +1,13 @@
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
 the-badge&logo=wikipedia&logoColor=white] [https://
-img.shields.io/badge/github-%23000000.svg?style=for-the-
-badge&logo=github&logoColor=white] [https://img.shields.io/
-badge/tips-000000?style=for-the-                                     [Logo]
-badge&logo=buymeacoffee&logoColor=white]
+img.shields.io/badge/github-%23000000.svg?style=for-the-             [Logo]
+badge&logo=github&logoColor=white]
 [https://img.shields.io/docker/pulls/mraniki/tt?style=for-
-the-badge] [https://img.shields.io/badge/talky-
-blue?style=for-the-badge&logo=telegram&logoColor=white]
+the-badge]
 [https://img.shields.io/pypi/v/dxsp?style=for-the-
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/pypi/dm/dxsp?style=for-the-
 badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey]
 [https://img.shields.io/github/actions/workflow/status/     Swap made easy
 mraniki/dxsp/%F0%9F%91%B7Flow.yml?style=for-the-            Trade on any
 badge&logo=GitHub&logoColor=white]                          blockchains
```

### Comparing `dxsp-4.2.8/dxsp/default_settings.toml` & `dxsp-4.2.9/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.8/dxsp/main.py` & `dxsp-4.2.9/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.8/dxsp/protocols/oneinch.py` & `dxsp-4.2.9/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.8/dxsp/protocols/uniswap.py` & `dxsp-4.2.9/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.8/dxsp/protocols/zerox.py` & `dxsp-4.2.9/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.8/dxsp/utils/account_utils.py` & `dxsp-4.2.9/dxsp/utils/account_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.8/dxsp/utils/contract_utils.py` & `dxsp-4.2.9/dxsp/utils/contract_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.8/dxsp/utils/explorer_utils.py` & `dxsp-4.2.9/dxsp/utils/explorer_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.8/pyproject.toml` & `dxsp-4.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "4.2.8"
+version = "4.2.9"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
@@ -49,14 +49,15 @@
 format = "github"
 fixable = ["ALL"]
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.2.0"
 eth_tester = "^0.9.0b2"
@@ -75,14 +76,15 @@
     "docs/*",
     "*/config.py"
 ]
 
 
 
 
+
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.0.0"
 pydata-sphinx-theme = "^0.13.3"
 sphinx-hoverxref = "^1.3.0"
```

### Comparing `dxsp-4.2.8/PKG-INFO` & `dxsp-4.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 4.2.8
+Version: 4.2.9
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,18 +21,16 @@
 Description-Content-Type: text/markdown
 
 
 <table style="border: 1px solid transparent">
   <tr>
     <td>
 <a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a>
-<a href="https://github.com/mraniki/tt/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
-<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a><br>
-<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a>
-<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a><br>
+<a href="https://github.com/mraniki/tt/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a><br>
+<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a><br>
   </td>
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/dxsp/"><img src="https://img.shields.io/pypi/v/dxsp?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/dxsp/"><img src="https://img.shields.io/pypi/dm/dxsp?style=for-the-badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey"></a><br>
```

#### html2text {}

```diff
@@ -1,28 +1,25 @@
-Metadata-Version: 2.1 Name: dxsp Version: 4.2.8 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 4.2.9 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist:
 pycoingecko (>=3.1.0,<4.0.0) Requires-Dist: uniswap-python (>=0.7.0,<0.8.0)
 Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-URL: Changelog, https://
 github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst Project-URL: Issues, https://
 github.com/mraniki/dxsp/issues Project-URL: Support, https://github.com/
 mraniki/dxsp/discussions Description-Content-Type: text/markdown
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
 the-badge&logo=wikipedia&logoColor=white] [https://
-img.shields.io/badge/github-%23000000.svg?style=for-the-
-badge&logo=github&logoColor=white] [https://img.shields.io/
-badge/tips-000000?style=for-the-                                     [Logo]
-badge&logo=buymeacoffee&logoColor=white]
+img.shields.io/badge/github-%23000000.svg?style=for-the-             [Logo]
+badge&logo=github&logoColor=white]
 [https://img.shields.io/docker/pulls/mraniki/tt?style=for-
-the-badge] [https://img.shields.io/badge/talky-
-blue?style=for-the-badge&logo=telegram&logoColor=white]
+the-badge]
 [https://img.shields.io/pypi/v/dxsp?style=for-the-
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/pypi/dm/dxsp?style=for-the-
 badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey]
 [https://img.shields.io/github/actions/workflow/status/     Swap made easy
 mraniki/dxsp/%F0%9F%91%B7Flow.yml?style=for-the-            Trade on any
 badge&logo=GitHub&logoColor=white]                          blockchains
```

