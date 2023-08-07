# Comparing `tmp/kgcl_schema-0.5.0.tar.gz` & `tmp/kgcl_schema-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgcl_schema-0.5.0.tar", max compression
+gzip compressed data, was "kgcl_schema-0.6.0.tar", max compression
```

## Comparing `kgcl_schema-0.5.0.tar` & `kgcl_schema-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1071 2023-05-09 00:24:35.170769 kgcl_schema-0.5.0/LICENSE
--rw-r--r--   0        0        0      330 2023-05-09 00:24:35.170769 kgcl_schema-0.5.0/README.md
--rw-r--r--   0        0        0      828 2023-05-09 00:25:20.200258 kgcl_schema-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7695 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/README.md
--rw-r--r--   0        0        0        0 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/__init__.py
--rw-r--r--   0        0        0   137919 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/datamodel/kgcl.py
--rw-r--r--   0        0        0    15269 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/datamodel/ontology_model.py
--rw-r--r--   0        0        0        0 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/grammar/__init__.py
--rw-r--r--   0        0        0     4242 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/grammar/kgcl.lark
--rw-r--r--   0        0        0    14441 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/grammar/kgcl_2_rdf.py
--rw-r--r--   0        0        0    20274 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/grammar/parser.py
--rw-r--r--   0        0        0     9975 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/grammar/render_operations.py
--rw-r--r--   0        0        0      208 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/schema/__init__.py
--rw-r--r--   0        0        0      501 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/schema/basics.yaml
--rw-r--r--   0        0        0    32080 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/schema/kgcl.yaml
--rw-r--r--   0        0        0     4414 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/schema/ontology_model.yaml
--rw-r--r--   0        0        0     1544 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/schema/prov.yaml
--rw-r--r--   0        0        0     4415 2023-05-09 00:24:35.182770 kgcl_schema-0.5.0/src/kgcl_schema/utils.py
--rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 kgcl_schema-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-07 18:25:43.518466 kgcl_schema-0.6.0/LICENSE
+-rw-r--r--   0        0        0      330 2023-08-07 18:25:43.518466 kgcl_schema-0.6.0/README.md
+-rw-r--r--   0        0        0      844 2023-08-07 18:26:21.819545 kgcl_schema-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7695 2023-08-07 18:25:43.534467 kgcl_schema-0.6.0/src/kgcl_schema/README.md
+-rw-r--r--   0        0        0        0 2023-08-07 18:25:43.534467 kgcl_schema-0.6.0/src/kgcl_schema/__init__.py
+-rw-r--r--   0        0        0   137919 2023-08-07 18:25:43.534467 kgcl_schema-0.6.0/src/kgcl_schema/datamodel/kgcl.py
+-rw-r--r--   0        0        0    15269 2023-08-07 18:25:43.534467 kgcl_schema-0.6.0/src/kgcl_schema/datamodel/ontology_model.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:25:43.534467 kgcl_schema-0.6.0/src/kgcl_schema/grammar/__init__.py
+-rw-r--r--   0        0        0     4242 2023-08-07 18:25:43.534467 kgcl_schema-0.6.0/src/kgcl_schema/grammar/kgcl.lark
+-rw-r--r--   0        0        0    14441 2023-08-07 18:25:43.534467 kgcl_schema-0.6.0/src/kgcl_schema/grammar/kgcl_2_rdf.py
+-rw-r--r--   0        0        0    20508 2023-08-07 18:25:43.538467 kgcl_schema-0.6.0/src/kgcl_schema/grammar/parser.py
+-rw-r--r--   0        0        0     9975 2023-08-07 18:25:43.538467 kgcl_schema-0.6.0/src/kgcl_schema/grammar/render_operations.py
+-rw-r--r--   0        0        0      208 2023-08-07 18:25:43.538467 kgcl_schema-0.6.0/src/kgcl_schema/schema/__init__.py
+-rw-r--r--   0        0        0      501 2023-08-07 18:25:43.538467 kgcl_schema-0.6.0/src/kgcl_schema/schema/basics.yaml
+-rw-r--r--   0        0        0    32080 2023-08-07 18:25:43.538467 kgcl_schema-0.6.0/src/kgcl_schema/schema/kgcl.yaml
+-rw-r--r--   0        0        0     4414 2023-08-07 18:25:43.538467 kgcl_schema-0.6.0/src/kgcl_schema/schema/ontology_model.yaml
+-rw-r--r--   0        0        0     1544 2023-08-07 18:25:43.538467 kgcl_schema-0.6.0/src/kgcl_schema/schema/prov.yaml
+-rw-r--r--   0        0        0     4415 2023-08-07 18:25:43.538467 kgcl_schema-0.6.0/src/kgcl_schema/utils.py
+-rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 kgcl_schema-0.6.0/PKG-INFO
```

### Comparing `kgcl_schema-0.5.0/LICENSE` & `kgcl_schema-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.5.0/pyproject.toml` & `kgcl_schema-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "kgcl_schema"
-version = "v0.5.0"
+version = "v0.6.0"
 description = "Schema for the KGCL project."
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harshad Hegde <hhegde@lbl.gov>"
     ]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 linkml-runtime = ">=1.1.24"
 lark = ">=1.1.2"
-bioregistry = ">=0.6.0"
+prefixmaps = "^0.1.5"
+curies = "^0.6.0"
 
 [tool.poetry.dev-dependencies]
 linkml = ">=1.5.2"
 pytest = "^7.1.2"
 mkdocs-material = "^8.2.8"
 mkdocs-mermaid2-plugin = "^0.6.0"
```

### Comparing `kgcl_schema-0.5.0/src/kgcl_schema/README.md` & `kgcl_schema-0.6.0/src/kgcl_schema/README.md`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.5.0/src/kgcl_schema/datamodel/kgcl.py` & `kgcl_schema-0.6.0/src/kgcl_schema/datamodel/kgcl.py`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.5.0/src/kgcl_schema/datamodel/ontology_model.py` & `kgcl_schema-0.6.0/src/kgcl_schema/datamodel/ontology_model.py`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.5.0/src/kgcl_schema/grammar/kgcl.lark` & `kgcl_schema-0.6.0/src/kgcl_schema/grammar/kgcl.lark`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.5.0/src/kgcl_schema/grammar/kgcl_2_rdf.py` & `kgcl_schema-0.6.0/src/kgcl_schema/grammar/kgcl_2_rdf.py`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.5.0/src/kgcl_schema/grammar/parser.py` & `kgcl_schema-0.6.0/src/kgcl_schema/grammar/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """KGCL parser."""
 import logging
-import re
 import sys
+from functools import lru_cache
 from pathlib import Path
 from typing import List
 
 import click
-from bioregistry import parse_iri, get_preferred_prefix, curie_to_str
+from prefixmaps.io.parser import load_multi_context
+from curies import Converter
 from kgcl_schema.datamodel.kgcl import (
     Change,
     ClassCreation,
     EdgeCreation,
     EdgeDeletion,
     NewSynonym,
     NewTextDefinition,
@@ -34,14 +35,20 @@
     RemoveTextDefinition,
 )
 from kgcl_schema.datamodel.ontology_model import Edge
 from kgcl_schema.utils import to_json, to_rdf, to_yaml
 from lark import Lark, Token
 
 
+@lru_cache()
+def get_curie_converter() -> Converter:
+    context = load_multi_context(["obo", "bioregistry.upper", "linked_data"])
+    extended_prefix_map = context.as_extended_prefix_map()
+    return Converter.from_extended_prefix_map(extended_prefix_map)
+
 def id_generator():
     """Return a new ID for KGCL change operations."""
     id = 0
     while True:
         yield id
         id += 1
 
@@ -622,19 +629,17 @@
 
     # TODO: use predefined set of prefixes to identify CURIEs
     return contract_uri(str(entity)), "curie"
     # return entity, "error"
 
 
 def contract_uri(uri_or_curie: str):
+    converter = get_curie_converter()
     if uri_or_curie.startswith("http://") or uri_or_curie.startswith("https://"):
-        pref, i = parse_iri(uri_or_curie)
-        pref = get_preferred_prefix(pref)
-        curie = curie_to_str(pref, i)
-        return curie
+        return converter.compress(uri_or_curie)
     else:
         return uri_or_curie
 
 
 @click.command()
 @click.option("--output", "-o", type=click.File(mode="w"), default=sys.stdout)
 @click.option("--output-type", "-O", help="format for output")
```

### Comparing `kgcl_schema-0.5.0/src/kgcl_schema/grammar/render_operations.py` & `kgcl_schema-0.6.0/src/kgcl_schema/grammar/render_operations.py`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.5.0/src/kgcl_schema/schema/kgcl.yaml` & `kgcl_schema-0.6.0/src/kgcl_schema/schema/kgcl.yaml`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.5.0/src/kgcl_schema/schema/ontology_model.yaml` & `kgcl_schema-0.6.0/src/kgcl_schema/schema/ontology_model.yaml`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.5.0/src/kgcl_schema/schema/prov.yaml` & `kgcl_schema-0.6.0/src/kgcl_schema/schema/prov.yaml`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.5.0/src/kgcl_schema/utils.py` & `kgcl_schema-0.6.0/src/kgcl_schema/utils.py`

 * *Files identical despite different names*

### Comparing `kgcl_schema-0.5.0/PKG-INFO` & `kgcl_schema-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: kgcl-schema
-Version: 0.5.0
+Version: 0.6.0
 Summary: Schema for the KGCL project.
 License: MIT
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
-Requires-Dist: bioregistry (>=0.6.0)
+Requires-Dist: curies (>=0.6.0,<0.7.0)
 Requires-Dist: lark (>=1.1.2)
 Requires-Dist: linkml-runtime (>=1.1.24)
+Requires-Dist: prefixmaps (>=0.1.5,<0.2.0)
 Description-Content-Type: text/markdown
 
 # KGCL: Knowledge Graph Change Language
 
 KGCL is a standard datamodel for representing changes in ontologies and knowledge graphs.
 
 This repository houses:
```

