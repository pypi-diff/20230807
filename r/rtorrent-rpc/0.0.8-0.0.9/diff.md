# Comparing `tmp/rtorrent_rpc-0.0.8.tar.gz` & `tmp/rtorrent_rpc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.0.8.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.0.9.tar", max compression
```

## Comparing `rtorrent_rpc-0.0.8.tar` & `rtorrent_rpc-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1084 2023-07-02 01:56:37.638747 rtorrent_rpc-0.0.8/LICENSE
--rw-r--r--   0        0        0     2523 2023-07-02 01:56:37.638747 rtorrent_rpc-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      741 2023-07-02 01:56:37.638747 rtorrent_rpc-0.0.8/readme.md
--rw-r--r--   0        0        0    22594 2023-07-02 01:56:37.638747 rtorrent_rpc-0.0.8/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2098 2023-07-02 01:56:37.638747 rtorrent_rpc-0.0.8/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2023-07-02 01:56:37.638747 rtorrent_rpc-0.0.8/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 rtorrent_rpc-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-04 01:49:30.455587 rtorrent_rpc-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2496 2023-07-04 01:49:30.455587 rtorrent_rpc-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      741 2023-07-04 01:49:30.455587 rtorrent_rpc-0.0.9/readme.md
+-rw-r--r--   0        0        0    22584 2023-07-04 01:49:30.455587 rtorrent_rpc-0.0.9/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2098 2023-07-04 01:49:30.455587 rtorrent_rpc-0.0.9/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2023-07-04 01:49:30.455587 rtorrent_rpc-0.0.9/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     6262 2023-07-04 01:49:30.455587 rtorrent_rpc-0.0.9/rtorrent_rpc/scgi.py
+-rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 rtorrent_rpc-0.0.9/PKG-INFO
```

### Comparing `rtorrent_rpc-0.0.8/LICENSE` & `rtorrent_rpc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.8/pyproject.toml` & `rtorrent_rpc-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.0.8"
+version = "0.0.9"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
@@ -22,15 +22,14 @@
     'Programming Language :: Python :: Implementation :: CPython',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 # dependencies
 typing-extensions = ">=4.1.0"
-rtorrent-xmlrpc = "^0.0.3"
 bencode-py = "^4.0.0"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = { version = "^7.0.0", python = "^3.9" }
 furo = { version = "2023.05.20", python = "^3.9" }
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `rtorrent_rpc-0.0.8/readme.md` & `rtorrent_rpc-0.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.8/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.0.9/rtorrent_rpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 import urllib.parse
 import xmlrpc.client
 from collections.abc import Iterable
 from typing import Any, Literal, Protocol, TypeAlias, TypedDict
 
-from rtorrent_xmlrpc import SCGIServerProxy
+from .scgi import SCGIServerProxy
 from typing_extensions import NotRequired
 
 __all__ = ["RTorrent", "MultiCall"]
 
 Unknown: TypeAlias = Any
```

### Comparing `rtorrent_rpc-0.0.8/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.0.9/rtorrent_rpc/helper.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.8/PKG-INFO` & `rtorrent_rpc-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.0.8
+Version: 0.0.9
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.10,<4.0
@@ -13,15 +13,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: bencode-py (>=4.0.0,<5.0.0)
-Requires-Dist: rtorrent-xmlrpc (>=0.0.3,<0.0.4)
 Requires-Dist: typing-extensions (>=4.1.0)
 Project-URL: Repository, https://github.com/trim21/rtorrent-rpc
 Description-Content-Type: text/markdown
 
 # Typed rtorrent rpc client
 
 [![PyPI](https://img.shields.io/pypi/v/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
```

