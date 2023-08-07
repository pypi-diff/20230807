# Comparing `tmp/astx-0.2.0.tar.gz` & `tmp/astx-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astx-0.2.0.tar", max compression
+gzip compressed data, was "astx-0.2.1.tar", max compression
```

## Comparing `astx-0.2.0.tar` & `astx-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1498 2023-08-07 03:26:26.709841 astx-0.2.0/LICENSE
--rw-r--r--   0        0        0     1744 2023-08-07 03:28:47.893229 astx-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      686 2023-08-07 03:28:47.889229 astx-0.2.0/src/astx/__init__.py
--rw-r--r--   0        0        0     2378 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/base.py
--rw-r--r--   0        0        0      859 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/blocks.py
--rw-r--r--   0        0        0     2302 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/callables.py
--rw-r--r--   0        0        0     2515 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/datatypes.py
--rw-r--r--   0        0        0      318 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/mixes.py
--rw-r--r--   0        0        0      158 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/modifiers.py
--rw-r--r--   0        0        0     1502 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/operators.py
--rw-r--r--   0        0        0        0 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/py.typed
--rw-r--r--   0        0        0     1793 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/statements.py
--rw-r--r--   0        0        0     3455 2023-08-07 03:26:26.709841 astx-0.2.0/src/astx/symbol_table.py
--rw-r--r--   0        0        0      611 1970-01-01 00:00:00.000000 astx-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-08-07 20:53:17.043858 astx-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1744 2023-08-07 20:56:08.926877 astx-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      834 2023-08-07 20:56:08.926877 astx-0.2.1/src/astx/__init__.py
+-rw-r--r--   0        0        0     2378 2023-08-07 20:53:17.047859 astx-0.2.1/src/astx/base.py
+-rw-r--r--   0        0        0      859 2023-08-07 20:53:17.047859 astx-0.2.1/src/astx/blocks.py
+-rw-r--r--   0        0        0     2302 2023-08-07 20:53:17.047859 astx-0.2.1/src/astx/callables.py
+-rw-r--r--   0        0        0     2509 2023-08-07 20:53:17.047859 astx-0.2.1/src/astx/datatypes.py
+-rw-r--r--   0        0        0     1269 2023-08-07 20:53:17.047859 astx-0.2.1/src/astx/flows.py
+-rw-r--r--   0        0        0      318 2023-08-07 20:53:17.047859 astx-0.2.1/src/astx/mixes.py
+-rw-r--r--   0        0        0      158 2023-08-07 20:53:17.047859 astx-0.2.1/src/astx/modifiers.py
+-rw-r--r--   0        0        0     1502 2023-08-07 20:53:17.047859 astx-0.2.1/src/astx/operators.py
+-rw-r--r--   0        0        0        0 2023-08-07 20:53:17.047859 astx-0.2.1/src/astx/py.typed
+-rw-r--r--   0        0        0     3455 2023-08-07 20:53:17.047859 astx-0.2.1/src/astx/symbol_table.py
+-rw-r--r--   0        0        0      676 2023-08-07 20:53:17.047859 astx-0.2.1/src/astx/variables.py
+-rw-r--r--   0        0        0      611 1970-01-01 00:00:00.000000 astx-0.2.1/PKG-INFO
```

### Comparing `astx-0.2.0/LICENSE` & `astx-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astx-0.2.0/pyproject.toml` & `astx-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "astx"
-version = "0.2.0"  # semantic-release
+version = "0.2.1"  # semantic-release
 description = "OSL Python Package contains all the boilerplate you need to create a Python package."
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD 3 Clause"
 exclude = [
   ".git/*",
   ".env*",
 ]
```

### Comparing `astx-0.2.0/src/astx/base.py` & `astx-0.2.1/src/astx/base.py`

 * *Files identical despite different names*

### Comparing `astx-0.2.0/src/astx/blocks.py` & `astx-0.2.1/src/astx/blocks.py`

 * *Files identical despite different names*

### Comparing `astx-0.2.0/src/astx/callables.py` & `astx-0.2.1/src/astx/callables.py`

 * *Files identical despite different names*

### Comparing `astx-0.2.0/src/astx/datatypes.py` & `astx-0.2.1/src/astx/datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from astx.base import DataType, ASTKind, SourceLocation, Expr, ExprType
+from astx.base import DataType, ASTKind, SourceLocation, ExprType
 from astx.operators import BinaryOp
 
 
 class DataTypeOps(DataType):
     def __add__(self, other: DataType) -> BinaryOp:
         return BinaryOp("+", self, other)
```

### Comparing `astx-0.2.0/src/astx/operators.py` & `astx-0.2.1/src/astx/operators.py`

 * *Files identical despite different names*

### Comparing `astx-0.2.0/src/astx/statements.py` & `astx-0.2.1/src/astx/flows.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import List, Tuple, Optional
+"""Module for controle flow AST."""
+from typing import Optional
 
 from astx.base import StatementType, Expr, SourceLocation, ASTKind
 from astx.blocks import Block
 
 
 class IfStmt(StatementType):
     """AST class for `if` statement."""
@@ -48,29 +49,7 @@
         self.loc = loc
         self.var_name = var_name
         self.start = start
         self.end = end
         self.step = step
         self.body = body
         self.kind = ASTKind.ForKind
-
-
-class VarExprAST(StatementType):
-    """AST class for variable declaration."""
-
-    var_names: List[Tuple[str, Expr]]
-    type_name: str
-    body: Block
-
-    def __init__(
-        self,
-        var_names: List[Tuple[str, Expr]],
-        type_name: str,
-        body: Block,
-        loc: SourceLocation = SourceLocation(0, 0),
-    ) -> None:
-        """Initialize the VarExprAST instance."""
-        self.loc = loc
-        self.var_names = var_names
-        self.type_name = type_name
-        self.body = body
-        self.kind = ASTKind.VarKind
```

### Comparing `astx-0.2.0/src/astx/symbol_table.py` & `astx-0.2.1/src/astx/symbol_table.py`

 * *Files identical despite different names*

### Comparing `astx-0.2.0/PKG-INFO` & `astx-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astx
-Version: 0.2.0
+Version: 0.2.1
 Summary: OSL Python Package contains all the boilerplate you need to create a Python package.
 License: BSD 3 Clause
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

