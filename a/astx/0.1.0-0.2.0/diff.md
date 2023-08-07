# Comparing `tmp/astx-0.1.0.tar.gz` & `tmp/astx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astx-0.1.0.tar", max compression
+gzip compressed data, was "astx-0.2.0.tar", max compression
```

## Comparing `astx-0.1.0.tar` & `astx-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     1498 2023-07-14 00:33:13.468943 astx-0.1.0/LICENSE
--rw-r--r--   0        0        0     1658 2023-07-15 16:46:31.816481 astx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      633 2023-07-15 16:54:46.455127 astx-0.1.0/src/astx/__init__.py
--rw-r--r--   0        0        0     2018 2023-07-15 15:47:06.006761 astx-0.1.0/src/astx/base.py
--rw-r--r--   0        0        0      862 2023-07-15 16:46:31.908482 astx-0.1.0/src/astx/blocks.py
--rw-r--r--   0        0        0     2203 2023-07-15 16:46:31.908482 astx-0.1.0/src/astx/callables.py
--rw-r--r--   0        0        0     1634 2023-07-15 16:46:31.908482 astx-0.1.0/src/astx/datatypes.py
--rw-r--r--   0        0        0      158 2023-07-14 00:54:58.915624 astx-0.1.0/src/astx/modifiers.py
--rw-r--r--   0        0        0      884 2023-07-15 16:46:31.872482 astx-0.1.0/src/astx/operators.py
--rw-r--r--   0        0        0     1793 2023-07-15 16:46:31.912482 astx-0.1.0/src/astx/statements.py
--rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 astx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-08-07 03:26:26.709841 astx-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1744 2023-08-07 03:28:47.893229 astx-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      686 2023-08-07 03:28:47.889229 astx-0.2.0/src/astx/__init__.py
+-rw-r--r--   0        0        0     2378 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/base.py
+-rw-r--r--   0        0        0      859 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/blocks.py
+-rw-r--r--   0        0        0     2302 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/callables.py
+-rw-r--r--   0        0        0     2515 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/datatypes.py
+-rw-r--r--   0        0        0      318 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/mixes.py
+-rw-r--r--   0        0        0      158 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/modifiers.py
+-rw-r--r--   0        0        0     1502 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/operators.py
+-rw-r--r--   0        0        0        0 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/py.typed
+-rw-r--r--   0        0        0     1793 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/statements.py
+-rw-r--r--   0        0        0     3455 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/symbol_table.py
+-rw-r--r--   0        0        0      611 1970-01-01 00:00:00.000000 astx-0.2.0/PKG-INFO
```

### Comparing `astx-0.1.0/LICENSE` & `astx-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astx-0.1.0/pyproject.toml` & `astx-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "astx"
-version = "0.1.0"  # semantic-release
+version = "0.2.0"  # semantic-release
 description = "OSL Python Package contains all the boilerplate you need to create a Python package."
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD 3 Clause"
 exclude = [
   ".git/*",
   ".env*",
 ]
 packages = [
   {include = "astx", from="src"},
 ]
+include = ["src/astx/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 atpublic = "^4.0"
+typing-extensions = { version = "^4", python = "<3.9" }
 
 [tool.poetry.dev-dependencies]
 urllib3 = "<2"  # fix poetry issues
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 coverage = "^7.2.7"
 black = "^23.3.0"
@@ -35,16 +37,14 @@
 mkdocs-jupyter = "^0.24.1"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-macros-plugin = ">=0.7.0,<1"
 mkdocs-material = "^9.1.15"
 mkdocstrings = "^0.21.2"
 mkdocstrings-python = "^1.1.2"
 
-
-
 [tool.poetry.group.dev.dependencies]
 makim = "^1.8.1"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
```

### Comparing `astx-0.1.0/src/astx/__init__.py` & `astx-0.2.0/src/astx/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 
 from astx import base
 from astx import blocks
 from astx import callables
 from astx import datatypes
 from astx import operators
 from astx import statements
+from astx import mixes
+from astx import symbol_table
 
 
 def get_version() -> str:
     """Return the program version."""
     try:
         return importlib_metadata.version(__name__)
     except importlib_metadata.PackageNotFoundError:  # pragma: no cover
-        return "0.1.0"  # semantic-release
+        return "0.2.0"  # semantic-release
 
 
 version: str = get_version()
 
 __author__ = "Ivan Ogasawara"
 __email__ = "ivan.ogasawara@gmail.com"
 __version__: str = version
```

### Comparing `astx-0.1.0/src/astx/base.py` & `astx-0.2.0/src/astx/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 """AST classes and functions."""
 from enum import Enum
-from typing import TypeAlias, Type
+from typing import Type, ClassVar
+
+try:
+    from typing import TypeAlias
+except ImportError:
+    from typing_extensions import TypeAlias
 
 
 class SourceLocation:
     line: int
     col: int
 
     def __init__(self, line: int, col: int):
@@ -67,37 +72,50 @@
 
 
 class AST(metaclass=ASTMeta):
     """AST main expression class."""
 
     loc: SourceLocation
     kind: ASTKind
+    comment: str
 
     def __init__(self, loc: SourceLocation = SourceLocation(0, 0)) -> None:
         """Initialize the AST instance."""
         self.kind = ASTKind.GenericKind
         self.loc = loc
+        self.comment: str = ""
 
     def __str__(self) -> str:
         return self.__repr__()
 
     def __repr__(self) -> str:
         return self.__class__.__name__
 
 
 class Expr(AST):
     """AST main expression class."""
 
+    nbytes: int = 0
+
 
 ExprType: TypeAlias = Type[Expr]
 
 
 class DataType(Expr):
     """AST main expression class."""
 
+    type_: ExprType
+    name: str
+
 
-class OperatorType(Expr):
+class OperatorType(DataType):
     """AST main expression class."""
 
+    _tmp_id: ClassVar[int] = 0
+
+    def __init__(self) -> None:
+        self.name = f"temp_{OperatorType._tmp_id}"
+        OperatorType._tmp_id += 1
+
 
 class StatementType(AST):
     """AST main expression class."""
```

### Comparing `astx-0.1.0/src/astx/blocks.py` & `astx-0.2.0/src/astx/blocks.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 
 from astx.base import AST, Expr, ASTKind
 
 
 class Block(AST):
     """The AST tree."""
 
-    nodes: List[Expr]
+    nodes: List[AST]
     position: int = 0
 
     def __init__(self):
         self.nodes: List[Expr] = []
         self.position: int = 0
 
-    def append(self, value: Expr):
+    def append(self, value: AST):
         self.nodes.append(value)
 
     def __iter__(self) -> Block:
         return self
 
-    def __next__(self) -> Expr:
+    def __next__(self) -> AST:
         if self.position >= len(self.nodes):
             raise StopIteration()
 
         i = self.position
         self.position += 1
         return self.nodes[i]
```

### Comparing `astx-0.1.0/src/astx/callables.py` & `astx-0.2.0/src/astx/callables.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 
 from astx.base import (
     ASTKind,
     SourceLocation,
     Expr,
+    DataType,
     ExprType,
     StatementType,
 )
 from astx.blocks import Block
 from astx.datatypes import Variable
 from astx.modifiers import ScopeKind, VisibilityKind
 
@@ -55,18 +56,18 @@
         self.scope = scope
         self.visibility = visibility
 
 
 class Return(StatementType):
     """AST class for function `return` statement."""
 
-    value: Expr
+    value: DataType
 
     def __init__(
-        self, value: Expr, loc: SourceLocation = SourceLocation(0, 0)
+        self, value: DataType, loc: SourceLocation = SourceLocation(0, 0)
     ) -> None:
         """Initialize the Return instance."""
         self.loc = loc
         self.value = value
         self.kind = ASTKind.ReturnKind
 
 
@@ -83,7 +84,11 @@
         loc: SourceLocation = SourceLocation(0, 0),
     ) -> None:
         """Initialize the Function instance."""
         self.loc = loc
         self.prototype = prototype
         self.body = body
         self.kind = ASTKind.FunctionKind
+
+    @property
+    def name(self) -> str:
+        return self.prototype.name
```

### Comparing `astx-0.1.0/src/astx/statements.py` & `astx-0.2.0/src/astx/statements.py`

 * *Files identical despite different names*

### Comparing `astx-0.1.0/PKG-INFO` & `astx-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: astx
-Version: 0.1.0
+Version: 0.2.0
 Summary: OSL Python Package contains all the boilerplate you need to create a Python package.
 License: BSD 3 Clause
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: atpublic (>=4.0,<5.0)
+Requires-Dist: typing-extensions (>=4,<5) ; python_version < "3.9"
```

