# Comparing `tmp/cheapcone-0.1.3.tar.gz` & `tmp/cheapcone-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheapcone-0.1.3.tar", max compression
+gzip compressed data, was "cheapcone-0.1.4.tar", max compression
```

## Comparing `cheapcone-0.1.3.tar` & `cheapcone-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-08-07 04:48:50.791009 cheapcone-0.1.3/README.md
--rw-r--r--   0        0        0       22 2023-08-07 06:22:11.313840 cheapcone-0.1.3/cheapcone/__init__.py
--rw-r--r--   0        0        0     3909 2023-08-07 07:44:03.722790 cheapcone-0.1.3/cheapcone/client.py
--rw-r--r--   0        0        0     1391 2023-08-07 07:43:59.462843 cheapcone-0.1.3/cheapcone/json.py
--rw-r--r--   0        0        0      992 2023-08-07 06:05:53.534348 cheapcone-0.1.3/cheapcone/proxy.py
--rw-r--r--   0        0        0      704 2023-08-07 07:44:03.194797 cheapcone-0.1.3/cheapcone/schemas.py
--rw-r--r--   0        0        0      679 2023-08-07 07:44:02.378807 cheapcone-0.1.3/cheapcone/typedefs.py
--rw-r--r--   0        0        0      327 2023-08-07 07:45:10.334027 cheapcone-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 cheapcone-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-07 04:48:50.791009 cheapcone-0.1.4/README.md
+-rw-r--r--   0        0        0       22 2023-08-07 06:22:11.313840 cheapcone-0.1.4/cheapcone/__init__.py
+-rw-r--r--   0        0        0     4208 2023-08-07 09:34:44.510872 cheapcone-0.1.4/cheapcone/client.py
+-rw-r--r--   0        0        0     1595 2023-08-07 09:31:42.362613 cheapcone-0.1.4/cheapcone/json.py
+-rw-r--r--   0        0        0      993 2023-08-07 09:31:42.354613 cheapcone-0.1.4/cheapcone/proxy.py
+-rw-r--r--   0        0        0      747 2023-08-07 09:31:42.362613 cheapcone-0.1.4/cheapcone/schemas.py
+-rw-r--r--   0        0        0     2385 2023-08-07 09:34:46.402875 cheapcone-0.1.4/cheapcone/typedefs.py
+-rw-r--r--   0        0        0      327 2023-08-07 09:34:58.962894 cheapcone-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 cheapcone-0.1.4/PKG-INFO
```

### Comparing `cheapcone-0.1.3/cheapcone/client.py` & `cheapcone-0.1.4/cheapcone/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 from dotenv import load_dotenv
 from multidict import CIMultiDict
 from pydantic import BaseModel, Field
 
 from .proxy import LazyProxy
 from .schemas import (MetaData, Query, QueryMatch, QueryRequest, QueryResponse,
                       UpsertRequest, UpsertResponse, Vector)
-from .typedefs import Filter, Value
+from .typedefs import Filter, QueryBuilder, Value
 
 load_dotenv()
 
+
 @dataclass(init=True, repr=True, unsafe_hash=False, frozen=False)
 class APIClient(LazyProxy[ClientSession]):
     """
     HTTP Client:
     Base class to create HTTP clients that wrap `aiohttp.ClientSession`.
     Provides Lazy Loading through proxy objects and session reuse using the singleton pattern.
     Constructor Signature:
@@ -74,28 +75,38 @@
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} {self.base_url}>"
 
 
 @dataclass(init=True, repr=True, unsafe_hash=False, frozen=False)
 class PineconeClient(APIClient):
-	"""
-	Cheapcone went greedy so I had to make this one.
-	"""
-	base_url: str = field(default=environ["PINECONE_API_URL"], init=True, repr=True)
-	api_key: str = field(default=environ["PINECONE_API_KEY"], init=True, repr=False)
-
-
-	def __load__(self) -> ClientSession:
-		return ClientSession(base_url=self.base_url, headers={"api-key": self.api_key})
-
-	
-	async def upsert(self, values:Vector, metadata:MetaData) -> UpsertResponse:
-		async with self.__load__() as session:
-			async with session.post("/upsert", json=UpsertRequest(values=values, metadata=metadata).dict()) as response:
-				return UpsertResponse(**await response.json())
-
-
-	async def query(self, expr:Query, vector:Vector, includeMetadata:bool=True,topK:int=10) -> QueryResponse:
-		async with self.__load__() as session:
-			async with session.post("/vectors/query", json=QueryRequest(topK=topK, filter=expr,vector=vector, includeMetadata=includeMetadata).dict()) as response:
-				return QueryResponse(**await response.json())
+    """
+    Cheapcone went greedy so I had to make this one.
+    """
+
+    base_url: str = field(default=environ["PINECONE_API_URL"], init=True, repr=True)
+    api_key: str = field(default=environ["PINECONE_API_KEY"], init=True, repr=False)
+
+    def __load__(self) -> ClientSession:
+        return ClientSession(base_url=self.base_url, headers={"api-key": self.api_key})
+
+    async def upsert(self, values: Vector, metadata: MetaData) -> UpsertResponse:
+        async with self.__load__() as session:
+            async with session.post(
+                "/upsert", json=UpsertRequest(values=values, metadata=metadata).dict()
+            ) as response:
+                return UpsertResponse(**await response.json())
+
+    async def query(
+        self, expr: Query, vector: Vector, includeMetadata: bool = True, topK: int = 10
+    ) -> QueryResponse:
+        async with self.__load__() as session:
+            async with session.post(
+                "/vectors/query",
+                json=QueryRequest(
+                    topK=topK,
+                    filter=expr,
+                    vector=vector,
+                    includeMetadata=includeMetadata,
+                ).dict(),
+            ) as response:
+                return QueryResponse(**await response.json())
```

### Comparing `cheapcone-0.1.3/cheapcone/proxy.py` & `cheapcone-0.1.4/cheapcone/proxy.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 
     def __as_proxied__(self) -> T:
         """Helper method that returns the current proxy, typed as the loaded object"""
         return cast(T, self)
 
     @abstractmethod
     def __load__(self) -> T:
-        ...
+        ...
```

### Comparing `cheapcone-0.1.3/cheapcone/schemas.py` & `cheapcone-0.1.4/cheapcone/schemas.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 
 from pydantic import Field
 
 from .typedefs import CheapModel, MetaData, Query, Vector
 
 
 class UpsertRequest(CheapModel):
-	id: str = Field(default_factory=lambda: str(uuid4()))
-	values: Vector = Field(...)
-	metadata:MetaData = Field(...)
+    id: str = Field(default_factory=lambda: str(uuid4()))
+    values: Vector = Field(...)
+    metadata: MetaData = Field(...)
+
 
 class QueryRequest(CheapModel):
-	topK: int = Field(default=10)
-	filter: Query = Field(...)
-	includeMetadata: bool = Field(default=True)
-	vector: Vector = Field(...)
+    topK: int = Field(default=10)
+    filter: Query = Field(...)
+    includeMetadata: bool = Field(default=True)
+    vector: Vector = Field(...)
+
 
 class QueryMatch(CheapModel):
-	id: str = Field(...)
-	score: float = Field(...)
-	metadata:MetaData = Field(...)
+    id: str = Field(...)
+    score: float = Field(...)
+    metadata: MetaData = Field(...)
+
 
 class QueryResponse(CheapModel):
-	matches:List[QueryMatch] = Field(...)
+    matches: List[QueryMatch] = Field(...)
+
 
 class UpsertResponse(CheapModel):
-	upsertedCount: int = Field(...)
+    upsertedCount: int = Field(...)
```

