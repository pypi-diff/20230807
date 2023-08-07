# Comparing `tmp/linkml_renderer-0.2.1.tar.gz` & `tmp/linkml_renderer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_renderer-0.2.1.tar", max compression
+gzip compressed data, was "linkml_renderer-0.3.0.tar", max compression
```

## Comparing `linkml_renderer-0.2.1.tar` & `linkml_renderer-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11358 2023-08-07 19:05:16.775189 linkml_renderer-0.2.1/LICENSE
--rw-r--r--   0        0        0     3061 2023-08-07 19:05:16.775189 linkml_renderer-0.2.1/README.md
--rw-r--r--   0        0        0     1322 2023-08-07 19:05:41.848785 linkml_renderer-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      224 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/__init__.py
--rw-r--r--   0        0        0     3257 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/cli.py
--rw-r--r--   0        0        0        0 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/paths/__init__.py
--rw-r--r--   0        0        0     4952 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/paths/context.py
--rw-r--r--   0        0        0      373 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/paths/html_context.py
--rw-r--r--   0        0        0        0 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/renderers/__init__.py
--rw-r--r--   0        0        0    16264 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/renderers/html_renderer.py
--rw-r--r--   0        0        0    13975 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/renderers/markdown_renderer.py
--rw-r--r--   0        0        0     7308 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/renderers/mermaid_renderer.py
--rw-r--r--   0        0        0     3894 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/renderers/renderer.py
--rw-r--r--   0        0        0        0 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/style/__init__.py
--rw-r--r--   0        0        0     3140 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/style/model.py
--rw-r--r--   0        0        0     3211 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/style/model.yaml
--rw-r--r--   0        0        0     1976 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/style/style_engine.py
--rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 linkml_renderer-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-08-07 19:10:01.201087 linkml_renderer-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3061 2023-08-07 19:10:01.201087 linkml_renderer-0.3.0/README.md
+-rw-r--r--   0        0        0     1321 2023-08-07 19:10:23.809427 linkml_renderer-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      224 2023-08-07 19:10:01.201087 linkml_renderer-0.3.0/src/linkml_renderer/__init__.py
+-rw-r--r--   0        0        0     3257 2023-08-07 19:10:01.201087 linkml_renderer-0.3.0/src/linkml_renderer/cli.py
+-rw-r--r--   0        0        0        0 2023-08-07 19:10:01.201087 linkml_renderer-0.3.0/src/linkml_renderer/paths/__init__.py
+-rw-r--r--   0        0        0     4952 2023-08-07 19:10:01.201087 linkml_renderer-0.3.0/src/linkml_renderer/paths/context.py
+-rw-r--r--   0        0        0      373 2023-08-07 19:10:01.201087 linkml_renderer-0.3.0/src/linkml_renderer/paths/html_context.py
+-rw-r--r--   0        0        0        0 2023-08-07 19:10:01.201087 linkml_renderer-0.3.0/src/linkml_renderer/renderers/__init__.py
+-rw-r--r--   0        0        0    16264 2023-08-07 19:10:01.201087 linkml_renderer-0.3.0/src/linkml_renderer/renderers/html_renderer.py
+-rw-r--r--   0        0        0    13975 2023-08-07 19:10:01.201087 linkml_renderer-0.3.0/src/linkml_renderer/renderers/markdown_renderer.py
+-rw-r--r--   0        0        0     7308 2023-08-07 19:10:01.205087 linkml_renderer-0.3.0/src/linkml_renderer/renderers/mermaid_renderer.py
+-rw-r--r--   0        0        0     3894 2023-08-07 19:10:01.205087 linkml_renderer-0.3.0/src/linkml_renderer/renderers/renderer.py
+-rw-r--r--   0        0        0        0 2023-08-07 19:10:01.205087 linkml_renderer-0.3.0/src/linkml_renderer/style/__init__.py
+-rw-r--r--   0        0        0     3207 2023-08-07 19:10:01.205087 linkml_renderer-0.3.0/src/linkml_renderer/style/model.py
+-rw-r--r--   0        0        0     3211 2023-08-07 19:10:01.205087 linkml_renderer-0.3.0/src/linkml_renderer/style/model.yaml
+-rw-r--r--   0        0        0     1976 2023-08-07 19:10:01.205087 linkml_renderer-0.3.0/src/linkml_renderer/style/style_engine.py
+-rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 linkml_renderer-0.3.0/PKG-INFO
```

### Comparing `linkml_renderer-0.2.1/LICENSE` & `linkml_renderer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.1/README.md` & `linkml_renderer-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.1/pyproject.toml` & `linkml_renderer-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "linkml-renderer"
-version = "0.2.1"
+version = "0.3.0"
 description = "linkml-renderer"
 authors = ["Harshad Hegde <hhegde@lbl.gov>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = "<2"
+pydantic = "*"
 airium = "^0.2.5"
 click = "^8.1.3"
 linkml-runtime = ">=1.4.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 poetry-dynamic-versioning = "^0.21.3"
```

### Comparing `linkml_renderer-0.2.1/src/linkml_renderer/cli.py` & `linkml_renderer-0.3.0/src/linkml_renderer/cli.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.1/src/linkml_renderer/paths/context.py` & `linkml_renderer-0.3.0/src/linkml_renderer/paths/context.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.1/src/linkml_renderer/renderers/html_renderer.py` & `linkml_renderer-0.3.0/src/linkml_renderer/renderers/html_renderer.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.1/src/linkml_renderer/renderers/markdown_renderer.py` & `linkml_renderer-0.3.0/src/linkml_renderer/renderers/markdown_renderer.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.1/src/linkml_renderer/renderers/mermaid_renderer.py` & `linkml_renderer-0.3.0/src/linkml_renderer/renderers/mermaid_renderer.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.1/src/linkml_renderer/renderers/renderer.py` & `linkml_renderer-0.3.0/src/linkml_renderer/renderers/renderer.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.1/src/linkml_renderer/style/model.py` & `linkml_renderer-0.3.0/src/linkml_renderer/style/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 from datetime import date, datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from linkml_runtime.linkml_model import Decimal
-from pydantic import BaseModel as BaseModel
-from pydantic import Field
+try:
+    from pydantic.v1 import BaseModel as BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel as BaseModel, Field
 
 metamodel_version = "None"
 version = "None"
 
 
 class WeakRefShimBaseModel(BaseModel):
     __slots__ = "__weakref__"
```

### Comparing `linkml_renderer-0.2.1/src/linkml_renderer/style/model.yaml` & `linkml_renderer-0.3.0/src/linkml_renderer/style/model.yaml`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.1/src/linkml_renderer/style/style_engine.py` & `linkml_renderer-0.3.0/src/linkml_renderer/style/style_engine.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.1/PKG-INFO` & `linkml_renderer-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml-renderer
-Version: 0.2.1
+Version: 0.3.0
 Summary: linkml-renderer
 License: Apache Software License 2.0
 Author: Harshad Hegde
 Author-email: hhegde@lbl.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: airium (>=0.2.5,<0.3.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: linkml-runtime (>=1.4.1)
-Requires-Dist: pydantic (<2)
+Requires-Dist: pydantic
 Description-Content-Type: text/markdown
 
 # linkml-renderer
 
 Generating HTML, Markdown, Mermaid, and other rendering artefacts from LinkML data.
 
 This applies a configurable *generic* mapping between instance data and the target output file.
```

