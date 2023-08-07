# Comparing `tmp/linkml_renderer-0.2.0.tar.gz` & `tmp/linkml_renderer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_renderer-0.2.0.tar", max compression
+gzip compressed data, was "linkml_renderer-0.2.1.tar", max compression
```

## Comparing `linkml_renderer-0.2.0.tar` & `linkml_renderer-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11358 2023-05-27 01:25:07.262133 linkml_renderer-0.2.0/LICENSE
--rw-r--r--   0        0        0     3061 2023-05-27 01:25:07.262133 linkml_renderer-0.2.0/README.md
--rw-r--r--   0        0        0     1331 2023-05-27 01:25:42.358662 linkml_renderer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      224 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/__init__.py
--rw-r--r--   0        0        0     3257 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/cli.py
--rw-r--r--   0        0        0        0 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/paths/__init__.py
--rw-r--r--   0        0        0     4952 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/paths/context.py
--rw-r--r--   0        0        0      373 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/paths/html_context.py
--rw-r--r--   0        0        0        0 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/renderers/__init__.py
--rw-r--r--   0        0        0    16264 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/renderers/html_renderer.py
--rw-r--r--   0        0        0    13975 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/renderers/markdown_renderer.py
--rw-r--r--   0        0        0     7308 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/renderers/mermaid_renderer.py
--rw-r--r--   0        0        0     3894 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/renderers/renderer.py
--rw-r--r--   0        0        0        0 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/style/__init__.py
--rw-r--r--   0        0        0     3140 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/style/model.py
--rw-r--r--   0        0        0     3211 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/style/model.yaml
--rw-r--r--   0        0        0     1976 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/style/style_engine.py
--rw-r--r--   0        0        0     4097 1970-01-01 00:00:00.000000 linkml_renderer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-08-07 19:05:16.775189 linkml_renderer-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3061 2023-08-07 19:05:16.775189 linkml_renderer-0.2.1/README.md
+-rw-r--r--   0        0        0     1322 2023-08-07 19:05:41.848785 linkml_renderer-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      224 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/__init__.py
+-rw-r--r--   0        0        0     3257 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/cli.py
+-rw-r--r--   0        0        0        0 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/paths/__init__.py
+-rw-r--r--   0        0        0     4952 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/paths/context.py
+-rw-r--r--   0        0        0      373 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/paths/html_context.py
+-rw-r--r--   0        0        0        0 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/renderers/__init__.py
+-rw-r--r--   0        0        0    16264 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/renderers/html_renderer.py
+-rw-r--r--   0        0        0    13975 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/renderers/markdown_renderer.py
+-rw-r--r--   0        0        0     7308 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/renderers/mermaid_renderer.py
+-rw-r--r--   0        0        0     3894 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/renderers/renderer.py
+-rw-r--r--   0        0        0        0 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/style/__init__.py
+-rw-r--r--   0        0        0     3140 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/style/model.py
+-rw-r--r--   0        0        0     3211 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/style/model.yaml
+-rw-r--r--   0        0        0     1976 2023-08-07 19:05:16.779189 linkml_renderer-0.2.1/src/linkml_renderer/style/style_engine.py
+-rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 linkml_renderer-0.2.1/PKG-INFO
```

### Comparing `linkml_renderer-0.2.0/LICENSE` & `linkml_renderer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.0/README.md` & `linkml_renderer-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.0/pyproject.toml` & `linkml_renderer-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "linkml-renderer"
-version = "0.2.0"
+version = "0.2.1"
 description = "linkml-renderer"
 authors = ["Harshad Hegde <hhegde@lbl.gov>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
+pydantic = "<2"
 airium = "^0.2.5"
 click = "^8.1.3"
 linkml-runtime = ">=1.4.1"
-myst-parser = {version = "^0.18.1", extras = ["docs"]}
-sphinx = {version = "^5.3.0", extras = ["docs"]}
-sphinx-autodoc-typehints = {version = "^1.19.4", extras = ["docs"]}
-sphinx-click = {version = "^4.3.0", extras = ["docs"]}
-sphinx-rtd-theme = {version = "^1.0.0", extras = ["docs"]}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 poetry-dynamic-versioning = "^0.21.3"
 tox = "^3.25.1"
 linkml = ">=1.4.1"
+sphinx = {version = ">=5", extras = ["docs"]}
+myst-parser = {version = "*", extras = ["docs"]}
+sphinx-click = {version = "*", extras = ["docs"]}
+sphinx-autodoc-typehints = {version = "*", extras = ["docs"]}
+sphinx-rtd-theme = {version = "*", extras = ["docs"]}
 
 [tool.poetry.scripts]
 linkml-render = "linkml_renderer.cli:main"
 
 [tool.poetry.extras]
 docs = [
     "sphinx",
```

### Comparing `linkml_renderer-0.2.0/src/linkml_renderer/cli.py` & `linkml_renderer-0.2.1/src/linkml_renderer/cli.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.0/src/linkml_renderer/paths/context.py` & `linkml_renderer-0.2.1/src/linkml_renderer/paths/context.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.0/src/linkml_renderer/renderers/html_renderer.py` & `linkml_renderer-0.2.1/src/linkml_renderer/renderers/html_renderer.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.0/src/linkml_renderer/renderers/markdown_renderer.py` & `linkml_renderer-0.2.1/src/linkml_renderer/renderers/markdown_renderer.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.0/src/linkml_renderer/renderers/mermaid_renderer.py` & `linkml_renderer-0.2.1/src/linkml_renderer/renderers/mermaid_renderer.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.0/src/linkml_renderer/renderers/renderer.py` & `linkml_renderer-0.2.1/src/linkml_renderer/renderers/renderer.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.0/src/linkml_renderer/style/model.py` & `linkml_renderer-0.2.1/src/linkml_renderer/style/model.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.0/src/linkml_renderer/style/model.yaml` & `linkml_renderer-0.2.1/src/linkml_renderer/style/model.yaml`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.0/src/linkml_renderer/style/style_engine.py` & `linkml_renderer-0.2.1/src/linkml_renderer/style/style_engine.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.2.0/PKG-INFO` & `linkml_renderer-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml-renderer
-Version: 0.2.0
+Version: 0.2.1
 Summary: linkml-renderer
 License: Apache Software License 2.0
 Author: Harshad Hegde
 Author-email: hhegde@lbl.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,19 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: airium (>=0.2.5,<0.3.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: linkml-runtime (>=1.4.1)
-Requires-Dist: myst-parser[docs] (>=0.18.1,<0.19.0) ; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints[docs] (>=1.19.4,<2.0.0) ; extra == "docs"
-Requires-Dist: sphinx-click[docs] (>=4.3.0,<5.0.0) ; extra == "docs"
-Requires-Dist: sphinx-rtd-theme[docs] (>=1.0.0,<2.0.0) ; extra == "docs"
-Requires-Dist: sphinx[docs] (>=5.3.0,<6.0.0) ; extra == "docs"
+Requires-Dist: pydantic (<2)
 Description-Content-Type: text/markdown
 
 # linkml-renderer
 
 Generating HTML, Markdown, Mermaid, and other rendering artefacts from LinkML data.
 
 This applies a configurable *generic* mapping between instance data and the target output file.
```

