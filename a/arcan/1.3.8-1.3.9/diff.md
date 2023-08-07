# Comparing `tmp/arcan-1.3.8.tar.gz` & `tmp/arcan-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcan-1.3.8.tar", max compression
+gzip compressed data, was "arcan-1.3.9.tar", max compression
```

## Comparing `arcan-1.3.8.tar` & `arcan-1.3.9.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0     1711 2023-07-04 04:08:44.007490 arcan-1.3.8/LICENSE
--rw-r--r--   0        0        0     2888 2023-07-04 04:08:44.007490 arcan-1.3.8/README.md
--rw-r--r--   0        0        0      907 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/agent/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/engines/__init__.py
--rw-r--r--   0        0        0       24 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/engines/io.py
--rw-r--r--   0        0        0        0 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/governance/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/governance/catalog/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/governance/lifecycle/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/governance/mdm/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/governance/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/orchestrator/__init__.py
--rw-r--r--   0        0        0      478 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/processing/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/processing/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/processing/transformations/__init__.py
--rw-r--r--   0        0        0       91 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/session/__init__.py
--rw-r--r--   0        0        0       31 2023-07-04 04:08:44.007490 arcan-1.3.8/arcan/storage/__init__.py
--rw-r--r--   0        0        0       62 2023-07-04 04:08:44.007490 arcan-1.3.8/main.py
--rw-r--r--   0        0        0      768 2023-07-04 04:08:44.011490 arcan-1.3.8/pyproject.toml
--rw-r--r--   0        0        0     3648 1970-01-01 00:00:00.000000 arcan-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1711 2023-08-07 05:27:49.814621 arcan-1.3.9/LICENSE
+-rw-r--r--   0        0        0     2888 2023-08-07 05:27:49.814621 arcan-1.3.9/README.md
+-rw-r--r--   0        0        0     2610 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/agent/__init__.py
+-rw-r--r--   0        0        0     4154 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/agent/qanda.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/engines/__init__.py
+-rw-r--r--   0        0        0       24 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/engines/io.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/governance/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/governance/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/governance/lifecycle/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/governance/mdm/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/governance/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/ml/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/orchestrator/__init__.py
+-rw-r--r--   0        0        0      478 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/processing/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/processing/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/processing/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/processing/transformations/__init__.py
+-rw-r--r--   0        0        0       91 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/session/__init__.py
+-rw-r--r--   0        0        0       31 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/storage/__init__.py
+-rw-r--r--   0        0        0       62 2023-08-07 05:27:49.818621 arcan-1.3.9/main.py
+-rw-r--r--   0        0        0      930 2023-08-07 05:27:49.818621 arcan-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 arcan-1.3.9/PKG-INFO
```

### Comparing `arcan-1.3.8/LICENSE` & `arcan-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `arcan-1.3.8/README.md` & `arcan-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `arcan-1.3.8/PKG-INFO` & `arcan-1.3.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 2.1
 Name: arcan
-Version: 1.3.8
+Version: 1.3.9
 Summary: A multiheaded modern data bridging package based on pipeline manifests to integrate between any modern (and old) data stack tools
 License: arcan.ai Non-Commercial Open Source License
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: black (>=23.3.0,<24.0.0)
+Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: fastapi (>=0.98,<0.100)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: langchain (>=0.0.254,<0.0.255)
+Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: modal-client (>=0.49.2509,<0.51.0)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: urllib3 (<=2.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Description-Content-Type: text/markdown
 
 # Arcan: AI Driven Data Pipeline Orchestration
 
 <p align="center">
   <a href="https://arcanapp.io">
```

#### html2text {}

```diff
@@ -1,18 +1,23 @@
-Metadata-Version: 2.1 Name: arcan Version: 1.3.8 Summary: A multiheaded modern
+Metadata-Version: 2.1 Name: arcan Version: 1.3.9 Summary: A multiheaded modern
 data bridging package based on pipeline manifests to integrate between any
 modern (and old) data stack tools License: arcan.ai Non-Commercial Open Source
 License Author: Carlos D. Escobar-Valbuena Author-email:
 carlosdavidescobar@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: black (>=23.3.0,<24.0.0) Requires-
-Dist: fastapi (>=0.98,<0.100) Requires-Dist: modal-client (>=0.49.2509,<0.51.0)
-Requires-Dist: uvicorn (>=0.22.0,<0.23.0) Description-Content-Type: text/
-markdown # Arcan: AI Driven Data Pipeline Orchestration
+Language :: Python :: 3.11 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: black (>=23.3.0,<24.0.0) Requires-Dist: faiss-cpu
+(>=1.7.4,<2.0.0) Requires-Dist: fastapi (>=0.98,<0.100) Requires-Dist: httpx
+(>=0.24.1,<0.25.0) Requires-Dist: langchain (>=0.0.254,<0.0.255) Requires-Dist:
+lxml (>=4.9.3,<5.0.0) Requires-Dist: modal-client (>=0.49.2509,<0.51.0)
+Requires-Dist: openai (>=0.27.8,<0.28.0) Requires-Dist: tiktoken
+(>=0.4.0,<0.5.0) Requires-Dist: urllib3 (<=2.0) Requires-Dist: uvicorn
+(>=0.22.0,<0.23.0) Description-Content-Type: text/markdown # Arcan: AI Driven
+Data Pipeline Orchestration
                               [public/arcan.png]
  Your data bridging concierge. Leverage AI to integrate diverse big and small
         data stack tools with ease. Visit our live demo at arcanapp.io.
 
 # Introduction Arcan is an innovative open-source solution designed to bridge
 modern and legacy data stack tools through a multiheaded package based on a
 smart pipeline generation and orchestration. Leveraging a hybrid Next.js +
```

