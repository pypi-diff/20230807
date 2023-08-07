# Comparing `tmp/ftmq-0.2.0.tar.gz` & `tmp/ftmq-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftmq-0.2.0.tar", max compression
+gzip compressed data, was "ftmq-0.2.1.tar", max compression
```

## Comparing `ftmq-0.2.0.tar` & `ftmq-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.2.0/LICENSE
--rw-r--r--   0        0        0     5162 2023-07-30 16:07:06.752065 ftmq-0.2.0/README.md
--rw-r--r--   0        0        0       22 2023-07-31 12:06:31.470588 ftmq-0.2.0/ftmq/__init__.py
--rw-r--r--   0        0        0     3583 2023-07-31 11:55:19.470970 ftmq-0.2.0/ftmq/cli.py
--rw-r--r--   0        0        0     1148 2023-07-28 20:08:27.942739 ftmq-0.2.0/ftmq/enums.py
--rw-r--r--   0        0        0       43 2023-02-17 15:30:40.666516 ftmq-0.2.0/ftmq/exceptions.py
--rw-r--r--   0        0        0     4998 2023-07-31 11:53:34.994545 ftmq-0.2.0/ftmq/filters.py
--rw-r--r--   0        0        0     2868 2023-07-31 11:55:19.474970 ftmq-0.2.0/ftmq/io.py
--rw-r--r--   0        0        0      175 2023-07-30 15:52:21.016040 ftmq-0.2.0/ftmq/model/__init__.py
--rw-r--r--   0        0        0     2368 2023-07-30 15:33:11.604008 ftmq-0.2.0/ftmq/model/coverage.py
--rw-r--r--   0        0        0     3899 2023-07-29 08:53:06.255213 ftmq-0.2.0/ftmq/model/dataset.py
--rw-r--r--   0        0        0     2311 2023-07-31 11:41:09.826459 ftmq-0.2.0/ftmq/model/mixins.py
--rw-r--r--   0        0        0     1784 2023-06-14 17:04:10.502390 ftmq-0.2.0/ftmq/query.py
--rw-r--r--   0        0        0      896 2023-07-29 07:48:44.982562 ftmq-0.2.0/ftmq/types.py
--rw-r--r--   0        0        0      698 2023-07-28 13:56:13.237817 ftmq-0.2.0/ftmq/util.py
--rw-r--r--   0        0        0     1448 2023-07-31 12:06:31.470588 ftmq-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6514 1970-01-01 00:00:00.000000 ftmq-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5162 2023-07-30 16:07:06.752065 ftmq-0.2.1/README.md
+-rw-r--r--   0        0        0       22 2023-08-07 13:20:45.672701 ftmq-0.2.1/ftmq/__init__.py
+-rw-r--r--   0        0        0     3583 2023-07-31 11:55:19.470970 ftmq-0.2.1/ftmq/cli.py
+-rw-r--r--   0        0        0     1148 2023-07-28 20:08:27.942739 ftmq-0.2.1/ftmq/enums.py
+-rw-r--r--   0        0        0       43 2023-02-17 15:30:40.666516 ftmq-0.2.1/ftmq/exceptions.py
+-rw-r--r--   0        0        0     4998 2023-07-31 11:53:34.994545 ftmq-0.2.1/ftmq/filters.py
+-rw-r--r--   0        0        0     3740 2023-08-07 12:48:16.858112 ftmq-0.2.1/ftmq/io.py
+-rw-r--r--   0        0        0      175 2023-07-30 15:52:21.016040 ftmq-0.2.1/ftmq/model/__init__.py
+-rw-r--r--   0        0        0     2377 2023-08-07 10:09:40.334305 ftmq-0.2.1/ftmq/model/coverage.py
+-rw-r--r--   0        0        0     3899 2023-07-29 08:53:06.255213 ftmq-0.2.1/ftmq/model/dataset.py
+-rw-r--r--   0        0        0     2311 2023-07-31 11:41:09.826459 ftmq-0.2.1/ftmq/model/mixins.py
+-rw-r--r--   0        0        0     1784 2023-06-14 17:04:10.502390 ftmq-0.2.1/ftmq/query.py
+-rw-r--r--   0        0        0     1112 2023-08-07 10:32:46.835553 ftmq-0.2.1/ftmq/types.py
+-rw-r--r--   0        0        0      742 2023-08-07 11:00:10.785458 ftmq-0.2.1/ftmq/util.py
+-rw-r--r--   0        0        0     1488 2023-08-07 13:20:45.672701 ftmq-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6608 1970-01-01 00:00:00.000000 ftmq-0.2.1/PKG-INFO
```

### Comparing `ftmq-0.2.0/LICENSE` & `ftmq-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ftmq-0.2.0/README.md` & `ftmq-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ftmq-0.2.0/ftmq/cli.py` & `ftmq-0.2.1/ftmq/cli.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.2.0/ftmq/enums.py` & `ftmq-0.2.1/ftmq/enums.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.2.0/ftmq/filters.py` & `ftmq-0.2.1/ftmq/filters.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.2.0/ftmq/model/coverage.py` & `ftmq-0.2.1/ftmq/model/coverage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from collections import Counter
-from datetime import date
 from typing import Any
 
 from nomenklatura.dataset.coverage import DataCoverage as NKCoverage
 from pydantic import PrivateAttr
 
 from ftmq.enums import Properties
-from ftmq.types import CE, CEGenerator, Frequencies, Schemata
-
-from .mixins import NKModel
+from ftmq.model.mixins import NKModel
+from ftmq.types import CE, CEGenerator, DateLike, Frequencies, Schemata
 
 
 class Collector:
     schemata: Counter = None
     countries: set[str] = None
-    start: set[date] = None
-    end: set[date] = None
+    start: set[DateLike] = None
+    end: set[DateLike] = None
 
     def __init__(self):
         self.schemata = Counter()
         self.countries = set()
         self.start = set()
         self.end = set()
 
@@ -55,16 +53,16 @@
         return cov.export()
 
 
 class Coverage(NKModel):
     _nk_model = NKCoverage
     _collector: Collector | None = PrivateAttr()
 
-    start: date | None = None
-    end: date | None = None
+    start: DateLike | None = None
+    end: DateLike | None = None
     countries: list[str] | None = []
     frequency: Frequencies | None = "unknown"
 
     # own additions:
     schemata: dict[Schemata, int] = None
     entities: int = 0
```

### Comparing `ftmq-0.2.0/ftmq/model/dataset.py` & `ftmq-0.2.1/ftmq/model/dataset.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.2.0/ftmq/model/mixins.py` & `ftmq-0.2.1/ftmq/model/mixins.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.2.0/ftmq/query.py` & `ftmq-0.2.1/ftmq/query.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.2.0/ftmq/types.py` & `ftmq-0.2.1/ftmq/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import os
+from collections.abc import Generator
+from datetime import date, datetime
 from pathlib import Path
-from typing import Any, Generator, Literal, TypeAlias
+from typing import Any, Literal, TypeAlias
 
 from nomenklatura.entity import CE
+from nomenklatura.statement.statement import S
 
-from .enums import Frequencies, Properties, Schemata
+from ftmq.enums import Frequencies, Properties, Schemata
 
 # a string-keyed dict
 SDict: TypeAlias = dict[str, Any]
 
 # property multi-value
 Value: TypeAlias = list[str]
 
 # composite entity generator
 CEGenerator: TypeAlias = Generator[CE, None, None]
+SGenerator: TypeAlias = Generator[S, None, None]
 
 StrGenerator: TypeAlias = Generator[str, None, None]
 BytesGenerator: TypeAlias = Generator[bytes, None, None]
 
 Schemata: TypeAlias = Literal[tuple(s.name for s in Schemata)]
 Properties: TypeAlias = Literal[tuple(p.name for p in Properties)]
 Frequencies: TypeAlias = Literal[tuple(f.name for f in Frequencies)]
 
 PathLike: TypeAlias = str | os.PathLike[str] | Path
-
+DateLike: TypeAlias = date | datetime
 
 __all__ = [
     BytesGenerator,
     CE,
     CEGenerator,
     Frequencies,
     PathLike,
     Properties,
     Schemata,
     SDict,
+    SGenerator,
     StrGenerator,
     Value,
 ]
```

### Comparing `ftmq-0.2.0/pyproject.toml` & `ftmq-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftmq"
-version = "0.2.0"
+version = "0.2.1"
 description = "followthemoney query dsl and io helpers"
 authors = ["Simon Wörpel <simon.woerpel@pm.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/investigativedata/ftmq"
 repository = "https://github.com/investigativedata/ftmq"
 documentation = "https://github.com/investigativedata/ftmq"
@@ -24,25 +24,27 @@
 "Bug Tracker" = "https://github.com/investigativedata/ftmq/issues"
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 banal = "^1.0.6"
 followthemoney = "^3.4.0"
-nomenklatura = "2.14.1"
+nomenklatura = "^3.3.7"
 orjson = "^3.9.1"
 PyICU = "^2.11"
 click = "^8.1.3"
 click-default-group = "^1.2.2"
 cryptography = ">=41.0.2"
 certifi = ">=2023.07.22"
 scipy = ">=1.10.0"
 pydantic = "<2"
 fsspec = "^2023.6.0"
 s3fs = "^2023.6.0"
+gcsfs = "^2023.6.0"
+adlfs = "^2023.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
```

### Comparing `ftmq-0.2.0/PKG-INFO` & `ftmq-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: ftmq
-Version: 0.2.0
+Version: 0.2.1
 Summary: followthemoney query dsl and io helpers
 Home-page: https://github.com/investigativedata/ftmq
 License: MIT
 Author: Simon Wörpel
 Author-email: simon.woerpel@pm.me
 Requires-Python: >=3.10,<3.13
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyICU (>=2.11,<3.0)
+Requires-Dist: adlfs (>=2023.4.0,<2024.0.0)
 Requires-Dist: banal (>=1.0.6,<2.0.0)
 Requires-Dist: certifi (>=2023.07.22)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: cryptography (>=41.0.2)
 Requires-Dist: followthemoney (>=3.4.0,<4.0.0)
 Requires-Dist: fsspec (>=2023.6.0,<2024.0.0)
-Requires-Dist: nomenklatura (==2.14.1)
+Requires-Dist: gcsfs (>=2023.6.0,<2024.0.0)
+Requires-Dist: nomenklatura (>=3.3.7,<4.0.0)
 Requires-Dist: orjson (>=3.9.1,<4.0.0)
 Requires-Dist: pydantic (<2)
 Requires-Dist: s3fs (>=2023.6.0,<2024.0.0)
 Requires-Dist: scipy (>=1.10.0)
 Project-URL: Bug Tracker, https://github.com/investigativedata/ftmq/issues
 Project-URL: Documentation, https://github.com/investigativedata/ftmq
 Project-URL: Repository, https://github.com/investigativedata/ftmq
```

