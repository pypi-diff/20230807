# Comparing `tmp/cheapcone-0.1.2.tar.gz` & `tmp/cheapcone-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheapcone-0.1.2.tar", max compression
+gzip compressed data, was "cheapcone-0.1.3.tar", max compression
```

## Comparing `cheapcone-0.1.2.tar` & `cheapcone-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-08-07 04:48:50.791009 cheapcone-0.1.2/README.md
--rw-r--r--   0        0        0       22 2023-08-07 06:22:11.313840 cheapcone-0.1.2/cheapcone/__init__.py
--rw-r--r--   0        0        0     3878 2023-08-07 06:30:29.038873 cheapcone-0.1.2/cheapcone/client.py
--rw-r--r--   0        0        0     1391 2023-08-07 06:01:28.320170 cheapcone-0.1.2/cheapcone/json.py
--rw-r--r--   0        0        0      992 2023-08-07 06:05:53.534348 cheapcone-0.1.2/cheapcone/proxy.py
--rw-r--r--   0        0        0      668 2023-08-07 06:01:30.260225 cheapcone-0.1.2/cheapcone/schemas.py
--rw-r--r--   0        0        0      679 2023-08-07 06:01:31.988273 cheapcone-0.1.2/cheapcone/typedefs.py
--rw-r--r--   0        0        0      327 2023-08-07 07:22:44.067118 cheapcone-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 cheapcone-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-07 04:48:50.791009 cheapcone-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-08-07 06:22:11.313840 cheapcone-0.1.3/cheapcone/__init__.py
+-rw-r--r--   0        0        0     3909 2023-08-07 07:44:03.722790 cheapcone-0.1.3/cheapcone/client.py
+-rw-r--r--   0        0        0     1391 2023-08-07 07:43:59.462843 cheapcone-0.1.3/cheapcone/json.py
+-rw-r--r--   0        0        0      992 2023-08-07 06:05:53.534348 cheapcone-0.1.3/cheapcone/proxy.py
+-rw-r--r--   0        0        0      704 2023-08-07 07:44:03.194797 cheapcone-0.1.3/cheapcone/schemas.py
+-rw-r--r--   0        0        0      679 2023-08-07 07:44:02.378807 cheapcone-0.1.3/cheapcone/typedefs.py
+-rw-r--r--   0        0        0      327 2023-08-07 07:45:10.334027 cheapcone-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 cheapcone-0.1.3/PKG-INFO
```

### Comparing `cheapcone-0.1.2/cheapcone/client.py` & `cheapcone-0.1.3/cheapcone/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,11 +91,11 @@
 	
 	async def upsert(self, values:Vector, metadata:MetaData) -> UpsertResponse:
 		async with self.__load__() as session:
 			async with session.post("/upsert", json=UpsertRequest(values=values, metadata=metadata).dict()) as response:
 				return UpsertResponse(**await response.json())
 
 
-	async def query(self, topK:int, expr:Query, includeMetadata:bool=True) -> QueryResponse:
+	async def query(self, expr:Query, vector:Vector, includeMetadata:bool=True,topK:int=10) -> QueryResponse:
 		async with self.__load__() as session:
-			async with session.post("/vectors/query", json=QueryRequest(topK=topK, filter=expr, includeMetadata=includeMetadata).dict()) as response:
+			async with session.post("/vectors/query", json=QueryRequest(topK=topK, filter=expr,vector=vector, includeMetadata=includeMetadata).dict()) as response:
 				return QueryResponse(**await response.json())
```

### Comparing `cheapcone-0.1.2/cheapcone/json.py` & `cheapcone-0.1.3/cheapcone/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 			return self.named_tuple_hook(obj)
 		elif 'type' in obj and 'data' in obj:
 			return self.pydantic_hook(obj)
 		else:
 			return obj
 	
 	def named_tuple_hook(self, obj: Any) -> Any:
-		cls = namedtuple(obj['type'], obj['fields'])
+		cls = NamedTuple(obj['type'], obj['fields'])
 		return cls(*obj['values'])
 
 	def pydantic_hook(self, obj: Any) -> Any:
 		cls = getattr(__import__(obj['type']), obj['type'])
 		return cls(**obj['data'])
```

### Comparing `cheapcone-0.1.2/cheapcone/proxy.py` & `cheapcone-0.1.3/cheapcone/proxy.py`

 * *Files identical despite different names*

### Comparing `cheapcone-0.1.2/cheapcone/schemas.py` & `cheapcone-0.1.3/cheapcone/schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 class UpsertRequest(CheapModel):
 	id: str = Field(default_factory=lambda: str(uuid4()))
 	values: Vector = Field(...)
 	metadata:MetaData = Field(...)
 
 class QueryRequest(CheapModel):
-	topK: int = Field(...)
+	topK: int = Field(default=10)
 	filter: Query = Field(...)
 	includeMetadata: bool = Field(default=True)
+	vector: Vector = Field(...)
 
 class QueryMatch(CheapModel):
 	id: str = Field(...)
 	score: float = Field(...)
 	metadata:MetaData = Field(...)
 
 class QueryResponse(CheapModel):
```

### Comparing `cheapcone-0.1.2/cheapcone/typedefs.py` & `cheapcone-0.1.3/cheapcone/typedefs.py`

 * *Files identical despite different names*

