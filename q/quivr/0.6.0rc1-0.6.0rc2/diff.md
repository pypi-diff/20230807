# Comparing `tmp/quivr-0.6.0rc1.tar.gz` & `tmp/quivr-0.6.0rc2.tar.gz`

## Comparing `quivr-0.6.0rc1.tar` & `quivr-0.6.0rc2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/__version__.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/attributes.py
--rw-r--r--   0        0        0    45445 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/columns.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/concat.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/defragment.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/errors.py
--rw-r--r--   0        0        0    18327 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/linkage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/py.typed
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/schemagraph.py
--rw-r--r--   0        0        0    39757 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/tables.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/validators.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/LICENSE
--rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/README.md
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0    11435 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/__version__.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/attributes.py
+-rw-r--r--   0        0        0    46076 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/columns.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/concat.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/defragment.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/errors.py
+-rw-r--r--   0        0        0    18327 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/linkage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/py.typed
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/schemagraph.py
+-rw-r--r--   0        0        0    39757 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/tables.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/validators.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/LICENSE
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/README.md
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    11435 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/PKG-INFO
```

### Comparing `quivr-0.6.0rc1/quivr/__init__.py` & `quivr-0.6.0rc2/quivr/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,84 +39,86 @@
     UInt16Column,
     UInt32Column,
     UInt64Column,
 )
 from .concat import concatenate
 from .defragment import defragment
 from .errors import (
+    AttributeImmutableError,
     InvariantViolatedError,
     LinkageCombinationError,
     TableFragmentedError,
     TablesNotCompatibleError,
     ValidationError,
 )
 from .linkage import Linkage, MultiKeyLinkage, combine_linkages, combine_multilinkages
 from .tables import AnyTable, AttributeValueType, DataSourceType, Table
 from .validators import Validator, and_, eq, ge, gt, is_in, le, lt
 
 __all__ = [
-    "__version__",
-    "Table",
-    "concatenate",
+    "AnyTable",
+    "AttributeImmutableError",
+    "AttributeValueType",
+    "BinaryColumn",
+    "BooleanColumn",
+    "Byteslike",
     "Column",
-    "SubTableColumn",
-    "Int8Column",
-    "Int16Column",
-    "Int32Column",
-    "Int64Column",
-    "UInt8Column",
-    "UInt16Column",
-    "UInt32Column",
-    "UInt64Column",
+    "DataSourceType",
+    "Date32Column",
+    "Date64Column",
+    "Decimal128Column",
+    "Decimal256Column",
+    "DictionaryColumn",
+    "DurationColumn",
     "FixedSizeBinaryColumn",
     "FixedSizeListColumn",
     "Float16Column",
     "Float32Column",
     "Float64Column",
-    "BooleanColumn",
-    "StringColumn",
+    "FloatAttribute",
+    "Int16Column",
+    "Int32Column",
+    "Int64Column",
+    "Int8Column",
+    "IntAttribute",
+    "InvariantViolatedError",
     "LargeBinaryColumn",
+    "LargeListColumn",
     "LargeStringColumn",
-    "Date32Column",
-    "Date64Column",
-    "TimestampColumn",
-    "Time32Column",
-    "Time64Column",
-    "DurationColumn",
-    "MonthDayNanoIntervalColumn",
-    "BinaryColumn",
-    "Decimal128Column",
-    "Decimal256Column",
-    "NullColumn",
+    "Linkage",
+    "LinkageCombinationError",
     "ListColumn",
-    "LargeListColumn",
     "MapColumn",
-    "DictionaryColumn",
-    "StructColumn",
+    "MetadataDict",
+    "MonthDayNanoIntervalColumn",
+    "MultiKeyLinkage",
+    "NullColumn",
     "RunEndEncodedColumn",
-    "ValidationError",
+    "StringAttribute",
+    "StringColumn",
+    "StructColumn",
+    "SubTableColumn",
+    "Table",
     "TableFragmentedError",
-    "InvariantViolatedError",
-    "lt",
-    "le",
-    "gt",
-    "ge",
-    "eq",
-    "and_",
-    "is_in",
+    "TablesNotCompatibleError",
+    "Time32Column",
+    "Time64Column",
+    "TimestampColumn",
+    "UInt16Column",
+    "UInt32Column",
+    "UInt64Column",
+    "UInt8Column",
+    "ValidationError",
     "Validator",
-    "StringAttribute",
-    "IntAttribute",
-    "FloatAttribute",
-    "defragment",
-    "AttributeValueType",
-    "DataSourceType",
-    "AnyTable",
-    "MetadataDict",
-    "Byteslike",
-    "Linkage",
-    "MultiKeyLinkage",
+    "__version__",
+    "and_",
     "combine_linkages",
     "combine_multilinkages",
-    "LinkageCombinationError",
-    "TablesNotCompatibleError",
+    "concatenate",
+    "defragment",
+    "eq",
+    "ge",
+    "gt",
+    "is_in",
+    "le",
+    "lt",
 ]
```

### Comparing `quivr-0.6.0rc1/quivr/attributes.py` & `quivr-0.6.0rc2/quivr/attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import struct
 from typing import TYPE_CHECKING, Generic, Optional, TypeVar
 
+from . import errors
+
 if TYPE_CHECKING:
     from .tables import Table
 
 T = TypeVar("T")
 
 
 class Attribute(Generic[T]):
@@ -18,34 +20,39 @@
     Attributes are stored as metadata on the underlying Arrow table's schema.
     """
 
     _type: type[T]
 
     def __init__(
         self,
+        mutable: bool = False,
         default: Optional[T] = None,
     ):
         self.default = default
+        self.mutable = mutable
         self.name = "__ERR_UNSET_NAME"
 
     def __get__(self, instance: "Table", owner: type) -> T:
         if instance is None:
             return self
         name = self.name.encode("utf8")
         if instance.table.schema.metadata is None or name not in instance.table.schema.metadata:
             if self.default is not None:
                 return self.default
             raise AttributeError(f"Attribute {self.name} is not set and has no default")
         raw = instance.table.schema.metadata[name]
         return self.from_bytes(raw)
 
     def __set__(self, instance: "Table", value: T) -> None:
+        name = self.name.encode("utf8")
         metadata = instance.table.schema.metadata
         if metadata is None:
             metadata = {}
+        if name in metadata and not self.mutable:
+            raise errors.AttributeImmutableError(f"Attribute {self.name} is not mutable")
         metadata[self.name.encode("utf8")] = self.to_bytes(value)
         instance.table = instance.table.replace_schema_metadata(metadata)
 
     def __set_name__(self, owner: type, name: str) -> None:
         self.name = name
 
     def to_bytes(self, value: T) -> bytes:
@@ -79,16 +86,16 @@
 
     :param default: The default value for this attribute. If no default is provided,
         then the attribute must be set whenever constructing a table that uses it.
     """
 
     _type = str
 
-    def __init__(self, default: Optional[str] = None):
-        super().__init__(default=default)
+    def __init__(self, default: Optional[str] = None, mutable: bool = False):
+        super().__init__(default=default, mutable=mutable)
 
     def to_bytes(self, value: str) -> bytes:
         return value.encode("utf8")
 
     def from_bytes(self, raw: bytes) -> str:
         return raw.decode("utf8")
 
@@ -110,18 +117,20 @@
         then the attribute must be set whenever constructing a table that uses it.
     :param nbytes: The number of bytes to use to store the integer. Must be 1, 2, 4 or 8.
     :param signed: Whether the integer is signed or unsigned.
     """
 
     _type = int
 
-    def __init__(self, default: Optional[int] = None, nbytes: int = 8, signed: bool = True):
+    def __init__(
+        self, default: Optional[int] = None, mutable: bool = False, nbytes: int = 8, signed: bool = True
+    ):
         self.nbytes = nbytes
         self.signed = signed
-        super().__init__(default=default)
+        super().__init__(default=default, mutable=mutable)
 
     def to_bytes(self, value: int) -> bytes:
         return value.to_bytes(length=self.nbytes, byteorder="little", signed=self.signed)
 
     def from_bytes(self, raw: bytes) -> int:
         return int.from_bytes(raw, byteorder="little", signed=self.signed)
 
@@ -143,24 +152,24 @@
     :param default: The default value for this attribute. If no default is provided,
         then the attribute must be set whenever constructing a table that uses it.
     :param nbytes: The number of bytes to use to store the float. Must be 2, 4 or 8.
     """
 
     _type = float
 
-    def __init__(self, default: Optional[float] = None, nbytes: int = 8):
+    def __init__(self, default: Optional[float] = None, mutable: bool = False, nbytes: int = 8):
         if nbytes == 8:
             self._struct_fmt = "<d"
         elif nbytes == 4:
             self._struct_fmt = "<f"
         elif nbytes == 2:
             self._struct_fmt = "<e"
         else:
             raise ValueError("nbytes must be 2, 4 or 8")
-        super().__init__(default=default)
+        super().__init__(default=default, mutable=mutable)
 
     def to_bytes(self, value: float) -> bytes:
         return struct.pack(self._struct_fmt, value)
 
     def from_bytes(self, raw: bytes) -> float:
         return float(struct.unpack(self._struct_fmt, raw)[0])
```

### Comparing `quivr-0.6.0rc1/quivr/columns.py` & `quivr-0.6.0rc2/quivr/columns.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,26 @@
 
     def __init__(self, table_type: type[T], nullable: bool = True, metadata: Optional[MetadataDict] = None):
         self.table_type = table_type
         self.schema = table_type.schema
         dtype = pa.struct(table_type.schema)
         super().__init__(dtype, nullable=nullable, metadata=metadata)
 
+    def __set__(self, obj: tables.Table, value: T) -> None:
+        # Propagate the value's metadata through to the parent
+        metadata = obj.table.schema.metadata
+        value_meta = value.table.schema.metadata
+        if value_meta is not None:
+            for key, val in value_meta.items():
+                key = (self.name + "." + key.decode("utf-8")).encode("utf-8")
+                metadata[key] = val
+        idx = obj.table.schema.get_field_index(self.name)
+        obj.table = obj.table.replace_schema_metadata(metadata)
+        obj.table = obj.table.set_column(idx, self.pyarrow_field(), [value.to_structarray()])
+
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> T:
         ...
```

### Comparing `quivr-0.6.0rc1/quivr/concat.py` & `quivr-0.6.0rc2/quivr/concat.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.0rc1/quivr/errors.py` & `quivr-0.6.0rc2/quivr/errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,7 +64,15 @@
 
 class LinkageCombinationError(InvariantViolatedError):
     """Exception raised when linkages cannot be combined because they
     have incompatible table types or keys.
     """
 
     ...
+
+
+class AttributeImmutableError(RuntimeError):
+    """Exception raised when an attempt is made to modify an immutable
+    attribute.
+    """
+
+    ...
```

### Comparing `quivr-0.6.0rc1/quivr/linkage.py` & `quivr-0.6.0rc2/quivr/linkage.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.0rc1/quivr/schemagraph.py` & `quivr-0.6.0rc2/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.0rc1/quivr/tables.py` & `quivr-0.6.0rc2/quivr/tables.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.0rc1/quivr/validators.py` & `quivr-0.6.0rc2/quivr/validators.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.0rc1/LICENSE` & `quivr-0.6.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.6.0rc1/README.md` & `quivr-0.6.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `quivr-0.6.0rc1/pyproject.toml` & `quivr-0.6.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quivr-0.6.0rc1/PKG-INFO` & `quivr-0.6.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.6.0rc1
+Version: 0.6.0rc2
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: mmh3
 Requires-Dist: numpy
```

