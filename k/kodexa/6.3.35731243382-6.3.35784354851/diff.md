# Comparing `tmp/kodexa-6.3.35731243382.tar.gz` & `tmp/kodexa-6.3.35784354851.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-6.3.35731243382.tar", max compression
+gzip compressed data, was "kodexa-6.3.35784354851.tar", max compression
```

## Comparing `kodexa-6.3.35731243382.tar` & `kodexa-6.3.35784354851.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2023-08-01 19:56:17.864668 kodexa-6.3.35731243382/LICENSE
--rw-r--r--   0        0        0     2804 2023-08-01 19:56:17.864668 kodexa-6.3.35731243382/README.md
--rw-r--r--   0        0        0      847 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    12530 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      297 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0     7722 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      720 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/model/__init__.py
--rw-r--r--   0        0        0      906 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/model/base.py
--rw-r--r--   0        0        0    97073 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/model/model.py
--rw-r--r--   0        0        0   118834 2023-08-01 19:56:17.872668 kodexa-6.3.35731243382/kodexa/model/objects.py
--rw-r--r--   0        0        0    38816 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    19505 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   112700 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/platform/client.py
--rw-r--r--   0        0        0    25644 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13499 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3698 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3735 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     2354 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       60 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7054 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       60 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    21267 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       60 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    18991 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     2738 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    34222 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      160 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/steps/__init__.py
--rw-r--r--   0        0        0     9587 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/steps/common.py
--rw-r--r--   0        0        0      159 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/testing/__init__.py
--rw-r--r--   0        0        0      932 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    13596 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 19:56:17.876668 kodexa-6.3.35731243382/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1279 2023-08-01 19:56:37.228480 kodexa-6.3.35731243382/pyproject.toml
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 kodexa-6.3.35731243382/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-07 11:09:41.604607 kodexa-6.3.35784354851/LICENSE
+-rw-r--r--   0        0        0     2804 2023-08-07 11:09:41.604607 kodexa-6.3.35784354851/README.md
+-rw-r--r--   0        0        0      847 2023-08-07 11:09:41.608608 kodexa-6.3.35784354851/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2023-08-07 11:09:41.608608 kodexa-6.3.35784354851/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    12530 2023-08-07 11:09:41.608608 kodexa-6.3.35784354851/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      297 2023-08-07 11:09:41.608608 kodexa-6.3.35784354851/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0     7722 2023-08-07 11:09:41.608608 kodexa-6.3.35784354851/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      720 2023-08-07 11:09:41.608608 kodexa-6.3.35784354851/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      906 2023-08-07 11:09:41.608608 kodexa-6.3.35784354851/kodexa/model/base.py
+-rw-r--r--   0        0        0    97073 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/model/model.py
+-rw-r--r--   0        0        0   118834 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/model/objects.py
+-rw-r--r--   0        0        0    38816 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    19505 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   112682 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/platform/client.py
+-rw-r--r--   0        0        0    25644 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13499 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3698 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3735 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     2354 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       60 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7054 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       60 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    21267 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       60 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    18991 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     2738 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    34222 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      160 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0     9587 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/steps/common.py
+-rw-r--r--   0        0        0      159 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0      932 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    13596 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:09:41.612608 kodexa-6.3.35784354851/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1279 2023-08-07 11:09:58.778051 kodexa-6.3.35784354851/pyproject.toml
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 kodexa-6.3.35784354851/PKG-INFO
```

### Comparing `kodexa-6.3.35731243382/LICENSE` & `kodexa-6.3.35784354851/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/README.md` & `kodexa-6.3.35784354851/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/__init__.py` & `kodexa-6.3.35784354851/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/assistant/assistant.py` & `kodexa-6.3.35784354851/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/connectors/connectors.py` & `kodexa-6.3.35784354851/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/model/__init__.py` & `kodexa-6.3.35784354851/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/model/base.py` & `kodexa-6.3.35784354851/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/model/model.py` & `kodexa-6.3.35784354851/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/model/objects.py` & `kodexa-6.3.35784354851/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/model/persistence.py` & `kodexa-6.3.35784354851/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/pipeline/pipeline.py` & `kodexa-6.3.35784354851/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/platform/client.py` & `kodexa-6.3.35784354851/kodexa/platform/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2002,29 +2002,29 @@
 
         data_objects_response = self.client.get(url, params=params)
         data_object_page = PageDataObject.model_validate(data_objects_response.json())
         data_object_page.content = [DataObjectEndpoint.model_validate(data_object) for data_object in
                                     data_object_page.content]
         return data_object_page
 
-    def get_stream_data_objects_request(self, path: str, query="*", document_family: Optional[DocumentFamily] = None,
+    def stream_data_objects(self, path: str, query="*", document_family: Optional[DocumentFamily] = None,
                                         parent_id: Optional[str] = None):
         """
         Stream page request
         :param path (str): The parent taxon (/ is root)
         :param query (str): The query to limit results (Default *)
         :param document_family (Optional[DocumentFamily): Optionally the document family to limit results to
         :param parent_id (Optional[str]): Optionally the parent ID to limit results to
         :return:
         """
         page_size = 20
         page = 1
 
         while True:
-            data_object_response = self.get_data_objects_page_request(self, path, page, page_size, query,
+            data_object_response = self.get_data_objects_page_request(path, page, page_size, query,
                                                                       document_family, parent_id)
             if not data_object_response.content:
                 break
 
             yield data_object_response.content
             for data_object in data_object_response.content:
                 yield data_object
```

### Comparing `kodexa-6.3.35731243382/kodexa/platform/kodexa.py` & `kodexa-6.3.35784354851/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/selectors/ast.py` & `kodexa-6.3.35784354851/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/selectors/core.py` & `kodexa-6.3.35784354851/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/selectors/lexrules.py` & `kodexa-6.3.35784354851/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/selectors/lextab.py` & `kodexa-6.3.35784354851/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/selectors/parserules.py` & `kodexa-6.3.35784354851/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/selectors/parsetab.py` & `kodexa-6.3.35784354851/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/spatial/azure_models.py` & `kodexa-6.3.35784354851/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/spatial/bbox_common.py` & `kodexa-6.3.35784354851/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/spatial/table_form_common.py` & `kodexa-6.3.35784354851/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/steps/common.py` & `kodexa-6.3.35784354851/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/testing/test_components.py` & `kodexa-6.3.35784354851/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/kodexa/testing/test_utils.py` & `kodexa-6.3.35784354851/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35731243382/pyproject.toml` & `kodexa-6.3.35784354851/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "6.3.35731243382"
+version = "6.3.35784354851"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-6.3.35731243382/PKG-INFO` & `kodexa-6.3.35784354851/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 6.3.35731243382
+Version: 6.3.35784354851
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

