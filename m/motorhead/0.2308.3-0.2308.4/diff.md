# Comparing `tmp/motorhead-0.2308.3.tar.gz` & `tmp/motorhead-0.2308.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motorhead-0.2308.3.tar", max compression
+gzip compressed data, was "motorhead-0.2308.4.tar", max compression
```

## Comparing `motorhead-0.2308.3.tar` & `motorhead-0.2308.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-07-29 09:07:27.173242 motorhead-0.2308.3/LICENSE
--rw-r--r--   0        0        0     3010 2023-08-04 20:45:36.374798 motorhead-0.2308.3/README.md
--rw-r--r--   0        0        0     2096 2023-08-05 07:43:01.936504 motorhead-0.2308.3/motorhead/__init__.py
--rw-r--r--   0        0        0     3139 2023-07-30 12:39:04.829152 motorhead-0.2308.3/motorhead/bound_method_wrapper.py
--rw-r--r--   0        0        0     2631 2023-07-31 20:57:59.093587 motorhead-0.2308.3/motorhead/delete_rule.py
--rw-r--r--   0        0        0      259 2023-07-29 20:05:22.252317 motorhead-0.2308.3/motorhead/model/__init__.py
--rw-r--r--   0        0        0      133 2023-07-29 20:05:03.623604 motorhead-0.2308.3/motorhead/model/deleteresultmodel.py
--rw-r--r--   0        0        0      716 2023-07-29 20:03:57.265257 motorhead-0.2308.3/motorhead/model/document.py
--rw-r--r--   0        0        0     1677 2023-07-29 22:35:05.132760 motorhead-0.2308.3/motorhead/model/objectid.py
--rw-r--r--   0        0        0      877 2023-07-29 21:11:20.073753 motorhead-0.2308.3/motorhead/model/utcdatetime.py
--rw-r--r--   0        0        0     4900 2023-08-03 21:00:48.282511 motorhead-0.2308.3/motorhead/operator.py
--rw-r--r--   0        0        0        0 2023-07-29 09:07:27.173242 motorhead-0.2308.3/motorhead/py.typed
--rw-r--r--   0        0        0     6849 2023-08-03 20:55:30.603143 motorhead-0.2308.3/motorhead/query.py
--rw-r--r--   0        0        0    30486 2023-08-05 08:23:16.647640 motorhead-0.2308.3/motorhead/service.py
--rw-r--r--   0        0        0     6022 2023-08-03 18:52:05.408756 motorhead-0.2308.3/motorhead/typing.py
--rw-r--r--   0        0        0     1678 2023-08-03 18:51:37.484136 motorhead-0.2308.3/motorhead/validator.py
--rw-r--r--   0        0        0     2818 2023-08-05 11:33:40.609354 motorhead-0.2308.3/pyproject.toml
--rw-r--r--   0        0        0     3480 1970-01-01 00:00:00.000000 motorhead-0.2308.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-29 09:07:27.173242 motorhead-0.2308.4/LICENSE
+-rw-r--r--   0        0        0     3010 2023-08-04 20:45:36.374798 motorhead-0.2308.4/README.md
+-rw-r--r--   0        0        0     2213 2023-08-07 06:55:39.110605 motorhead-0.2308.4/motorhead/__init__.py
+-rw-r--r--   0        0        0     3139 2023-07-30 12:39:04.829152 motorhead-0.2308.4/motorhead/bound_method_wrapper.py
+-rw-r--r--   0        0        0     2631 2023-07-31 20:57:59.093587 motorhead-0.2308.4/motorhead/delete_rule.py
+-rw-r--r--   0        0        0      259 2023-07-29 20:05:22.252317 motorhead-0.2308.4/motorhead/model/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-29 20:05:03.623604 motorhead-0.2308.4/motorhead/model/deleteresultmodel.py
+-rw-r--r--   0        0        0      716 2023-07-29 20:03:57.265257 motorhead-0.2308.4/motorhead/model/document.py
+-rw-r--r--   0        0        0     1677 2023-07-29 22:35:05.132760 motorhead-0.2308.4/motorhead/model/objectid.py
+-rw-r--r--   0        0        0      877 2023-07-29 21:11:20.073753 motorhead-0.2308.4/motorhead/model/utcdatetime.py
+-rw-r--r--   0        0        0     4900 2023-08-03 21:00:48.282511 motorhead-0.2308.4/motorhead/operator.py
+-rw-r--r--   0        0        0        0 2023-07-29 09:07:27.173242 motorhead-0.2308.4/motorhead/py.typed
+-rw-r--r--   0        0        0     6849 2023-08-03 20:55:30.603143 motorhead-0.2308.4/motorhead/query.py
+-rw-r--r--   0        0        0    31359 2023-08-07 19:50:13.905370 motorhead-0.2308.4/motorhead/service.py
+-rw-r--r--   0        0        0     6349 2023-08-07 06:55:22.326628 motorhead-0.2308.4/motorhead/typing.py
+-rw-r--r--   0        0        0     1712 2023-08-06 21:50:39.365739 motorhead-0.2308.4/motorhead/validator.py
+-rw-r--r--   0        0        0     2864 2023-08-07 20:09:25.311989 motorhead-0.2308.4/pyproject.toml
+-rw-r--r--   0        0        0     3480 1970-01-01 00:00:00.000000 motorhead-0.2308.4/PKG-INFO
```

### Comparing `motorhead-0.2308.3/LICENSE` & `motorhead-0.2308.4/LICENSE`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.3/README.md` & `motorhead-0.2308.4/README.md`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.3/motorhead/__init__.py` & `motorhead-0.2308.4/motorhead/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .model import UTCDatetime as UTCDatetime
 from .operator import ensure_dict as ensure_dict
 from .query import Field as Field
 from .query import Q as Q
 from .query import Query as Query
 from .query import Queryable as Queryable
 from .service import DeleteResult as DeleteResult
+from .service import InsertManyResult as InsertManyResult
 from .service import InsertOneResult as InsertOneResult
 from .service import Service as Service
 from .service import ServiceException as ServiceException
 from .service import UpdateResult as UpdateResult
 from .typing import AgnosticClient as AgnosticClient
 from .typing import AgnosticCollection as AgnosticCollection
 from .typing import AgnosticDatabase as AgnosticDatabase
@@ -27,14 +28,15 @@
 from .typing import ClientProvider as ClientProvider
 from .typing import Collation as Collation
 from .typing import CollectionOptions as CollectionOptions
 from .typing import DatabaseProvider as DatabaseProvider
 from .typing import DeleteOptions as DeleteOptions
 from .typing import FindOptions as FindOptions
 from .typing import IndexData as IndexData
+from .typing import InsertManyOptions as InsertManyOptions
 from .typing import InsertOneOptions as InsertOneOptions
 from .typing import MongoProjection as MongoProjection
 from .typing import MongoQuery as MongoQuery
 from .typing import UpdateManyOptions as UpdateManyOptions
 from .typing import UpdateObject as UpdateObject
 from .typing import UpdateOneOptions as UpdateOneOptions
 from .validator import ValidationError as ValidationError
```

### Comparing `motorhead-0.2308.3/motorhead/bound_method_wrapper.py` & `motorhead-0.2308.4/motorhead/bound_method_wrapper.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.3/motorhead/delete_rule.py` & `motorhead-0.2308.4/motorhead/delete_rule.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.3/motorhead/model/document.py` & `motorhead-0.2308.4/motorhead/model/document.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.3/motorhead/model/objectid.py` & `motorhead-0.2308.4/motorhead/model/objectid.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.3/motorhead/model/utcdatetime.py` & `motorhead-0.2308.4/motorhead/model/utcdatetime.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.3/motorhead/operator.py` & `motorhead-0.2308.4/motorhead/operator.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.3/motorhead/query.py` & `motorhead-0.2308.4/motorhead/query.py`

 * *Files identical despite different names*

### Comparing `motorhead-0.2308.3/motorhead/service.py` & `motorhead-0.2308.4/motorhead/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
-from collections.abc import AsyncGenerator, Callable, Coroutine, Generator, Mapping, Sequence
+from collections.abc import AsyncGenerator, Callable, Coroutine, Generator, Iterable, Mapping, Sequence
 from contextlib import AbstractAsyncContextManager, asynccontextmanager, nullcontext
 from typing import TYPE_CHECKING, Any, Generic, TypeVar, get_args
 
 from bson import ObjectId
 from pydantic import BaseModel
-from pymongo.results import DeleteResult, InsertOneResult, UpdateResult
+from pymongo.results import DeleteResult, InsertManyResult, InsertOneResult, UpdateResult
 
 from .operator import ensure_dict
 from .typing import ClauseOrMongoQuery
 
 if TYPE_CHECKING:
     from motor.core import (
         AgnosticClientSession,
@@ -23,26 +23,28 @@
         AgnosticCollection,
         AgnosticDatabase,
         Collation,
         CollectionOptions,
         DeleteOptions,
         FindOptions,
         IndexData,
+        InsertManyOptions,
         InsertOneOptions,
         MongoProjection,
         UpdateManyOptions,
         UpdateObject,
         UpdateOneOptions,
     )
 
 from .delete_rule import DeleteRule
 from .validator import Validator
 
 __all__ = (
     "DeleteResult",
+    "InsertManyResult",
     "InsertOneResult",
     "Service",
     "UpdateResult",
 )
 
 TInsert = TypeVar("TInsert", bound=BaseModel)
 TUpdate = TypeVar("TUpdate", bound=BaseModel)
@@ -152,27 +154,27 @@
         Arguments:
             pipeline: The aggregation pipeline.
             session: An optional session to use.
         """
         return self.collection.aggregate(pipeline, session=session, **kwargs)
 
     async def count_documents(
-        self, query: ClauseOrMongoQuery, *, options: FindOptions | None = None
+        self, query: ClauseOrMongoQuery | None = None, *, options: FindOptions | None = None
     ) -> int:
         """
         Returns the number of documents that match the given query.
 
         Arguments:
             query: The query object.
             options: Query options, see the arguments of `collection.count_documents()` for details.
 
         Returns:
             The number of matching documents.
         """
-        query = ensure_dict(query)
+        query = {} if query is None else ensure_dict(query)
         return await self.collection.count_documents(query, **(options or {}))  # type: ignore[no-any-return]
 
     async def create_index(
         self,
         keys: str | Sequence[tuple[str, int | str | Mapping[str, Any]]],
         *,
         name: str,
@@ -311,15 +313,15 @@
         Arguments:
             query: Query object that matches the documents that should be deleted.
             options: Delete options, see the arguments of `collection.delete_many()`.
 
         Returns:
             The result of the operation.
         """
-        query = None if query is None else ensure_dict(query)
+        query = {} if query is None else ensure_dict(query)
         session_manager = self._get_session_context_manager(
             options.get("session", None) if options else None
         )
         async with await session_manager() as session:
             opts: DeleteOptions = options or {}
             opts["session"] = session
             ctxman = (
@@ -375,15 +377,15 @@
         Arguments:
             query: Query object that matches the document that should be deleted.
             options: Delete options, see the arguments of `collection.delete_one()`.
 
         Returns:
             The result of the operation.
         """
-        query = None if query is None else ensure_dict(query)
+        query = {} if query is None else ensure_dict(query)
         session_manager = self._get_session_context_manager(
             options.get("session", None) if options else None
         )
         async with await session_manager() as session:
             opts: DeleteOptions = options or {}
             opts["session"] = session
             ctxman = (
@@ -439,15 +441,15 @@
             query: The query object.
             projection: Optional projection.
             options: Query options, see the arguments of `collection.find()` for details.
 
         Returns:
             An async database cursor.
         """
-        query = None if query is None else ensure_dict(query)
+        query = {} if query is None else ensure_dict(query)
         return self.collection.find(query, projection, **(options or {}))
 
     async def find_ids(
         self,
         query: ClauseOrMongoQuery | None,
         *,
         session: AgnosticClientSession | None = None,
@@ -458,15 +460,15 @@
         Arguments:
             query: The query object.
             session: An optional database session to use.
 
         Returns:
             The IDs of all matching documents.
         """
-        query = None if query is None else ensure_dict(query)
+        query = {} if query is None else ensure_dict(query)
         return [
             doc["_id"]
             for doc in await self.collection.find(query, {"_id": True}, session=session).to_list(None)
         ]
 
     async def find_one(
         self,
@@ -482,29 +484,29 @@
             query: The query object.
             projection: Optional projection.
             options: Query options, see the arguments of `collection.find()` for details.
 
         Returns:
             A single matching document or `None` if there are no matches.
         """
-        query = None if query is None else ensure_dict(query)
+        query = {} if query is None else ensure_dict(query)
         return await self.collection.find_one(query, projection, **(options or {}))  # type: ignore[no-any-return]
 
     async def get_by_id(
         self,
         id: ObjectId,
         projection: MongoProjection | None = None,
         *,
         options: FindOptions | None = None,
     ) -> dict[str, Any] | None:
         """
         Returns the document with the given ID if it exists.
 
         Arguments:
-            id: The ID of the queried document. Must be an `ObjectID`, not a `str`.
+            id: The ID of the queried document. Must be an `ObjectId`, not a `str`.
             projection: Optional projection.
             options: Query options, see the arguments of `collection.find()` for details.
 
         Returns:
             The queried document if such a document exists.
         """
         return await self.find_one({"_id": id}, projection, options=options)
@@ -528,14 +530,36 @@
         insert_result = await self.insert_one(data, options=options)
         result = await self.get_by_id(insert_result.inserted_id)
         if result is None:
             raise ServiceException("Failed to query the inserted document by its ID.")
 
         return result
 
+    async def insert_many(
+        self, data: Iterable[TInsert], *, options: InsertManyOptions | None = None
+    ) -> InsertManyResult:
+        """
+        Inserts all the given objects into the collection.
+
+        Arguments:
+            data: The documents to be inserted.
+            options: Insert options, see the arguments of `collection.insert_many()` for details.
+
+        Returns
+            The result of the operation.
+
+        Raises:
+            Exception: If any of the documents is invalid.
+        """
+        insert_data = [await self._prepare_for_insert(d) for d in data]
+        return await self.collection.insert_many(  # type: ignore[no-any-return]
+            insert_data,
+            **(options or {}),
+        )
+
     async def insert_one(
         self, data: TInsert, *, options: InsertOneOptions | None = None
     ) -> InsertOneResult:
         """
         Inserts the given data into the collection.
 
         Arguments:
@@ -545,15 +569,15 @@
         Returns:
             The result of the operation.
 
         Raises:
             Exception: If the data is invalid.
         """
         return await self.collection.insert_one(  # type: ignore[no-any-return]
-            await self._prepare_for_insert(None, data),
+            await self._prepare_for_insert(data),
             **(options or {}),
         )
 
     async def update(
         self,
         id: ObjectId,
         changes: TUpdate,
@@ -623,18 +647,18 @@
 
         Returns:
             The result of the operation.
 
         Raises:
             Exception: If the data is invalid.
         """
-        query = None if query is None else ensure_dict(query)
+        query = {} if query is None else ensure_dict(query)
         return await self.collection.update_many(  # type: ignore[no-any-return]
             query,
-            await self._prepare_for_update(query, changes),
+            await self._prepare_for_update(changes, query),
             **(options or {}),
         )
 
     async def update_one(
         self,
         query: ClauseOrMongoQuery | None,
         changes: TUpdate,
@@ -651,18 +675,18 @@
 
         Returns:
             The result of the operation.
 
         Raises:
             Exception: If the data is invalid.
         """
-        query = None if query is None else ensure_dict(query)
+        query = {} if query is None else ensure_dict(query)
         return await self.collection.update_one(  # type: ignore[no-any-return]
             query,
-            await self._prepare_for_update(query, changes),
+            await self._prepare_for_update(changes, query),
             **(options or {}),
         )
 
     @classmethod
     def get_objectid_fields(cls, model: type[BaseModel]) -> set[str]:
         """
         Returns the names of all `ObjectId` fields.
@@ -787,52 +811,54 @@
                 exclude=objectid_fields,
                 by_alias=True,
                 exclude_unset=True,
                 mode="json",
             ),
         }
 
-    async def _prepare_for_insert(self, query: ClauseOrMongoQuery | None, data: TInsert) -> dict[str, Any]:
+    async def _prepare_for_insert(
+        self, data: TInsert, query: ClauseOrMongoQuery | None = None
+    ) -> dict[str, Any]:
         """
         Validates the given piece of data and converts it into its database representation
         if validation was successful.
 
         Arguments:
-            query: Query that matches the documents that will be updated.
             data: The data to be inserted.
+            query: Query that matches the documents that will be updated.
 
         Returns:
             The MongoDB-compatible, insertable data.
 
         Raises:
             Exception: If the data is invalid.
         """
-        await self._validate_insert(query, data)
+        await self._validate_insert(data, query)
         return await self._convert_for_insert(data)
 
     async def _prepare_for_update(
-        self, query: ClauseOrMongoQuery | None, data: TUpdate
+        self, data: TUpdate, query: ClauseOrMongoQuery | None
     ) -> UpdateObject | Sequence[UpdateObject]:
         """
         Validates the given piece of data and converts it into an update object.
 
         Arguments:
-            query: Query that matches the documents that will be updated.
             data: The update data.
+            query: Query that matches the documents that will be updated.
 
         Returns:
             The MongoDB-compatible update object.
 
         Raises:
             Exception: If the data is invalid.
         """
-        await self._validate_update(query, data)
+        await self._validate_update(data, query)
         return await self._convert_for_update(data)
 
-    async def _validate_insert(self, query: ClauseOrMongoQuery | None, data: TInsert) -> None:
+    async def _validate_insert(self, data: TInsert, query: ClauseOrMongoQuery | None = None) -> None:
         """
         Validates the given piece of data for insertion by executing all insert validators.
 
         See `Validator` for more information.
 
         Arguments:
             query: Query that matches the documents that will be updated.
@@ -840,15 +866,15 @@
 
         Raises:
             ValidationError: If validation failed.
         """
         # Sequential validation, slow but safe.
         for validator in self._validators():
             if "insert" in validator.config:
-                await validator(self, query, data)
+                await validator(self, data, query)
 
     async def _validate_deny_delete(self, session: AgnosticClientSession, ids: Sequence[ObjectId]) -> None:
         """
         Executes all "deny" delete rules.
 
         See `DeleteRule` for more information.
 
@@ -893,31 +919,31 @@
         Raises:
             DeleteError: if one of the executed delete rules fail.
         """
         for rule in self._delete_rules():
             if isinstance(rule, DeleteRule) and rule.config == "post":
                 await rule(self, session, ids)
 
-    async def _validate_update(self, query: ClauseOrMongoQuery | None, data: TUpdate) -> None:
+    async def _validate_update(self, data: TUpdate, query: ClauseOrMongoQuery | None = None) -> None:
         """
         Validates the given piece of data for update by executing all update validators.
 
         See `Validator` for more information.
 
         Arguments:
-            query: Query that matches the documents that will be updated.
             data: The data to validate.
+            query: Query that matches the documents that will be updated.
 
         Raises:
             ValidationError: If validation failed.
         """
         # Sequential validation, slow but safe.
         for validator in self._validators():
             if "update" in validator.config:
-                await validator(self, query, data)
+                await validator(self, data, query)
 
     def _validators(
         self,
     ) -> Generator[Validator["Service[TInsert, TUpdate]", TInsert | TUpdate], None, None]:
         """
         Generator that yields the validators that are registered on this service
         in the order they are present in `__class__.__dict__`.
```

### Comparing `motorhead-0.2308.3/motorhead/typing.py` & `motorhead-0.2308.4/motorhead/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "UpdateObject",
     "CollationDict",
     "Collation",
     "CollectionOptions",
     "DeleteOptions",
     "FindOptions",
     "IndexData",
+    "InsertManyOptions",
     "InsertOneOptions",
     "UpdateOneOptions",
     "UpdateManyOptions",
 )
 
 
 MongoProjection = dict[str, Any]
@@ -146,14 +147,25 @@
     unique: bool = False
     background: bool = False
     collation: Collation | None = None
     sparse: bool = False
     extra: dict[str, Any] = field(default_factory=dict)
 
 
+class InsertManyOptions(TypedDict, total=False):
+    """
+    Options for insert many operation.
+    """
+
+    bypass_document_validation: bool  # Default is False
+    comment: Any | None  # Default is None
+    ordered: bool  # Default is True
+    session: AgnosticCollection | None  # Default is None
+
+
 class InsertOneOptions(TypedDict, total=False):
     """
     Insert options.
     """
 
     bypass_document_validation: bool  # Default is False
     session: AgnosticCollection | None  # Default is None
```

### Comparing `motorhead-0.2308.3/motorhead/validator.py` & `motorhead-0.2308.4/motorhead/validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 TOwner = TypeVar("TOwner")
 TInsertOrUpdate = TypeVar("TInsertOrUpdate")
 InsertUpdateConfig = Literal["insert", "update", "insert-update"]
 
 
 class Validator(
-    BoundMethodWrapper[TOwner, [ClauseOrMongoQuery | None, TInsertOrUpdate], InsertUpdateConfig]
+    BoundMethodWrapper[TOwner, [TInsertOrUpdate, ClauseOrMongoQuery | None], InsertUpdateConfig]
 ):
     """
     Validator method wrapper.
 
     Validator methods receive an insert or update object, and execute some - potentially
     async - operations to make sure the inserted or updated data is valid.
     """
@@ -34,33 +34,33 @@
 
     exception = ValidationError
 
 
 def validator(
     config: InsertUpdateConfig = "insert-update",
 ) -> Callable[
-    [Callable[[TOwner, ClauseOrMongoQuery | None, TInsertOrUpdate], Coroutine[None, None, None]]],
+    [Callable[[TOwner, TInsertOrUpdate, ClauseOrMongoQuery | None], Coroutine[None, None, None]]],
     "Validator[TOwner, TInsertOrUpdate]",
 ]:
     """
     Service method decorator factory that converts the decorated method into a `Validator` instance.
 
     Example:
 
     ```python
     class SVC(Service):
         @validator("update")
-        def check_something(self, data: InsertData | CreateData) -> None:
+        def check_something(self, data: InsertData | CreateData, query: ClauseOrMongoQuery | None) -> None:
             raise ValueError("Always fail.")
     ```
 
     Arguments:
         config: Validatator config.
     """
 
     def decorator(
-        func: Callable[[TOwner, ClauseOrMongoQuery | None, TInsertOrUpdate], Coroutine[None, None, None]],
+        func: Callable[[TOwner, TInsertOrUpdate, ClauseOrMongoQuery | None], Coroutine[None, None, None]],
         /,
     ) -> "Validator[TOwner, TInsertOrUpdate]":
         return Validator(func=func, config=config)
 
     return decorator
```

### Comparing `motorhead-0.2308.3/pyproject.toml` & `motorhead-0.2308.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 [project.urls]
 Homepage = "https://github.com/volfpeter/motorhead"
 Documentation = "https://volfpeter.github.io/motorhead"
 
 [tool.poetry]
 name = "motorhead"
-version = "0.2308.3"
+version = "0.2308.4"
 description = "Async MongoDB with vanilla Pydantic v2+ - made easy."
 authors = ["Peter Volf <do.volfp@gmail.com>"]
 readme = "README.md"
 packages = [{include = "motorhead"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -47,14 +47,15 @@
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 mypy = "^1.4.1"
 ruff = "^0.0.280"
 poethepoet = "^0.21.1"
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
 pytest-docker = "^2.0.0"
+pytest-random-order = "^1.1.0"
 
 [tool.poetry.group.fastapi.dependencies]
 fastapi = {extras = ["all"], version = "^0.100.1"}
 
 [tool.black]
 line-length = 108
 
@@ -103,15 +104,15 @@
 
 [tool.poe.tasks]
 serve-docs = "mkdocs serve"
 black = "black ."
 black-check = "black . --check"
 mypy = "mypy ."
 ruff = "ruff check ."
-test = "python -m pytest tests"
+test = "python -m pytest tests --random-order"
 
 static-checks.sequence =  ["ruff", "black-check", "mypy"]
 static-checks.ignore_fail = "return_non_zero"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `motorhead-0.2308.3/PKG-INFO` & `motorhead-0.2308.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motorhead
-Version: 0.2308.3
+Version: 0.2308.4
 Summary: Async MongoDB with vanilla Pydantic v2+ - made easy.
 Author: Peter Volf
 Author-email: do.volfp@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

