# Comparing `tmp/encoded_core-0.0.1.tar.gz` & `tmp/encoded_core-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encoded_core-0.0.1.tar", max compression
+gzip compressed data, was "encoded_core-0.0.2.tar", max compression
```

## Comparing `encoded_core-0.0.1.tar` & `encoded_core-0.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1083 2023-04-28 13:49:44.781887 encoded_core-0.0.1/LICENSE
--rw-r--r--   0        0        0      174 2023-06-07 14:07:51.232231 encoded_core-0.0.1/README.rst
--rw-r--r--   0        0        0     3648 2023-06-07 14:07:51.235179 encoded_core-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2378 2023-06-07 14:07:51.236266 encoded_core-0.0.1/src/encoded_core/__init__.py
--rw-r--r--   0        0        0    21571 2023-06-07 14:07:51.236733 encoded_core-0.0.1/src/encoded_core/file_views.py
--rw-r--r--   0        0        0     4847 2023-06-07 14:07:51.237157 encoded_core-0.0.1/src/encoded_core/local_roles.py
--rw-r--r--   0        0        0    12807 2023-06-07 14:07:51.237626 encoded_core-0.0.1/src/encoded_core/page_views.py
--rw-r--r--   0        0        0     2490 2023-06-07 14:07:51.238087 encoded_core-0.0.1/src/encoded_core/qc_views.py
--rw-r--r--   0        0        0     1915 2023-06-07 14:07:51.238493 encoded_core-0.0.1/src/encoded_core/schemas/document.json
--rw-r--r--   0        0        0    18925 2023-06-07 14:07:51.239049 encoded_core-0.0.1/src/encoded_core/schemas/file.json
--rw-r--r--   0        0        0     5070 2023-06-07 14:07:51.239312 encoded_core-0.0.1/src/encoded_core/schemas/file_format.json
--rw-r--r--   0        0        0     6170 2023-06-07 14:07:51.239610 encoded_core-0.0.1/src/encoded_core/schemas/file_processed.json
--rw-r--r--   0        0        0     2336 2023-06-07 14:07:51.239884 encoded_core-0.0.1/src/encoded_core/schemas/file_reference.json
--rw-r--r--   0        0        0     1334 2023-06-07 14:07:51.240304 encoded_core-0.0.1/src/encoded_core/schemas/file_submitted.json
--rw-r--r--   0        0        0     1831 2023-06-07 14:07:51.240585 encoded_core-0.0.1/src/encoded_core/schemas/higlass_view_config.json
--rw-r--r--   0        0        0     1528 2023-06-07 14:07:51.240923 encoded_core-0.0.1/src/encoded_core/schemas/image.json
--rw-r--r--   0        0        0    18352 2023-06-07 14:07:51.241363 encoded_core-0.0.1/src/encoded_core/schemas/meta_workflow.json
--rw-r--r--   0        0        0    14409 2023-06-07 14:07:51.241808 encoded_core-0.0.1/src/encoded_core/schemas/meta_workflow_run.json
--rw-r--r--   0        0        0    17295 2023-06-07 14:07:51.242186 encoded_core-0.0.1/src/encoded_core/schemas/mixins.json
--rw-r--r--   0        0        0     4581 2023-06-07 14:07:51.242579 encoded_core-0.0.1/src/encoded_core/schemas/page.json
--rw-r--r--   0        0        0     1454 2023-06-07 14:07:51.243061 encoded_core-0.0.1/src/encoded_core/schemas/quality_metric.json
--rw-r--r--   0        0        0     3228 2023-06-07 14:07:51.243351 encoded_core-0.0.1/src/encoded_core/schemas/quality_metric_generic.json
--rw-r--r--   0        0        0     5715 2023-06-07 14:07:51.243653 encoded_core-0.0.1/src/encoded_core/schemas/software.json
--rw-r--r--   0        0        0     5010 2023-06-07 14:07:51.244093 encoded_core-0.0.1/src/encoded_core/schemas/static_section.json
--rw-r--r--   0        0        0    20411 2023-06-07 14:07:51.244521 encoded_core-0.0.1/src/encoded_core/schemas/tracking_item.json
--rw-r--r--   0        0        0     3749 2023-06-07 14:07:51.244808 encoded_core-0.0.1/src/encoded_core/schemas/user_content.json
--rw-r--r--   0        0        0    28089 2023-06-07 14:07:51.245271 encoded_core-0.0.1/src/encoded_core/schemas/workflow.json
--rw-r--r--   0        0        0    10491 2023-06-07 14:07:51.245547 encoded_core-0.0.1/src/encoded_core/schemas/workflow_run.json
--rw-r--r--   0        0        0     1908 2023-06-07 14:07:51.245969 encoded_core-0.0.1/src/encoded_core/schemas/workflow_run_awsem.json
--rw-r--r--   0        0        0        0 2023-06-07 14:07:51.246263 encoded_core-0.0.1/src/encoded_core/tests/__init__.py
--rw-r--r--   0        0        0    14054 2023-06-07 14:08:07.651422 encoded_core-0.0.1/src/encoded_core/tests/conftest.py
--rw-r--r--   0        0        0     1873 2023-06-07 14:07:51.247040 encoded_core-0.0.1/src/encoded_core/tests/conftest_settings.py
--rw-r--r--   0        0        0     7765 2023-06-07 14:07:51.247305 encoded_core-0.0.1/src/encoded_core/tests/datafixtures.py
--rw-r--r--   0        0        0    10832 2023-06-07 14:07:51.247761 encoded_core-0.0.1/src/encoded_core/tests/test_types_file.py
--rw-r--r--   0        0        0      262 2023-06-07 14:07:51.247989 encoded_core-0.0.1/src/encoded_core/tests/test_types_file_format.py
--rw-r--r--   0        0        0      239 2023-06-07 14:07:51.248304 encoded_core-0.0.1/src/encoded_core/tests/test_types_meta_workflow.py
--rw-r--r--   0        0        0      212 2023-06-07 14:07:51.248590 encoded_core-0.0.1/src/encoded_core/tests/test_types_software.py
--rw-r--r--   0        0        0      502 2023-06-07 14:07:51.248826 encoded_core-0.0.1/src/encoded_core/tests/test_types_workflow.py
--rw-r--r--   0        0        0       70 2023-06-07 14:07:51.249072 encoded_core-0.0.1/src/encoded_core/types/__init__.py
--rw-r--r--   0        0        0     1284 2023-06-07 14:07:51.249504 encoded_core-0.0.1/src/encoded_core/types/document.py
--rw-r--r--   0        0        0    20031 2023-06-07 14:07:51.249985 encoded_core-0.0.1/src/encoded_core/types/file.py
--rw-r--r--   0        0        0      789 2023-06-07 14:07:51.250399 encoded_core-0.0.1/src/encoded_core/types/file_format.py
--rw-r--r--   0        0        0     2297 2023-06-07 14:07:51.250690 encoded_core-0.0.1/src/encoded_core/types/file_processed.py
--rw-r--r--   0        0        0      462 2023-06-07 14:07:51.250942 encoded_core-0.0.1/src/encoded_core/types/file_reference.py
--rw-r--r--   0        0        0     1970 2023-06-07 14:07:51.251277 encoded_core-0.0.1/src/encoded_core/types/file_submitted.py
--rw-r--r--   0        0        0      584 2023-06-07 14:07:51.251811 encoded_core-0.0.1/src/encoded_core/types/higlass_view_config.py
--rw-r--r--   0        0        0     1040 2023-06-07 14:07:51.252223 encoded_core-0.0.1/src/encoded_core/types/image.py
--rw-r--r--   0        0        0     3136 2023-06-07 14:07:51.252605 encoded_core-0.0.1/src/encoded_core/types/meta_workflow.py
--rw-r--r--   0        0        0      858 2023-06-07 14:07:51.252830 encoded_core-0.0.1/src/encoded_core/types/page.py
--rw-r--r--   0        0        0     1705 2023-06-07 14:07:51.253054 encoded_core-0.0.1/src/encoded_core/types/quality_metric.py
--rw-r--r--   0        0        0     2750 2023-06-07 14:07:51.253281 encoded_core-0.0.1/src/encoded_core/types/software.py
--rw-r--r--   0        0        0     3847 2023-06-07 14:07:51.253509 encoded_core-0.0.1/src/encoded_core/types/tracking_item.py
--rw-r--r--   0        0        0     5468 2023-06-07 14:07:51.253828 encoded_core-0.0.1/src/encoded_core/types/user_content.py
--rw-r--r--   0        0        0    12886 2023-06-07 14:07:51.254085 encoded_core-0.0.1/src/encoded_core/types/workflow.py
--rw-r--r--   0        0        0     1316 2023-06-07 14:07:51.254451 encoded_core-0.0.1/src/encoded_core/upgrade.py
--rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 encoded_core-0.0.1/setup.py
--rw-r--r--   0        0        0     2581 1970-01-01 00:00:00.000000 encoded_core-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-28 13:49:44.781887 encoded_core-0.0.2/LICENSE
+-rw-r--r--   0        0        0      174 2023-06-07 14:07:51.232231 encoded_core-0.0.2/README.rst
+-rw-r--r--   0        0        0     3648 2023-06-22 17:50:25.462905 encoded_core-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2378 2023-06-07 14:07:51.236266 encoded_core-0.0.2/src/encoded_core/__init__.py
+-rw-r--r--   0        0        0    21571 2023-06-07 14:07:51.236733 encoded_core-0.0.2/src/encoded_core/file_views.py
+-rw-r--r--   0        0        0     4847 2023-06-07 14:07:51.237157 encoded_core-0.0.2/src/encoded_core/local_roles.py
+-rw-r--r--   0        0        0    12807 2023-06-07 14:07:51.237626 encoded_core-0.0.2/src/encoded_core/page_views.py
+-rw-r--r--   0        0        0     2490 2023-06-07 14:07:51.238087 encoded_core-0.0.2/src/encoded_core/qc_views.py
+-rw-r--r--   0        0        0     1915 2023-06-07 14:07:51.238493 encoded_core-0.0.2/src/encoded_core/schemas/document.json
+-rw-r--r--   0        0        0    18925 2023-06-07 14:07:51.239049 encoded_core-0.0.2/src/encoded_core/schemas/file.json
+-rw-r--r--   0        0        0     5070 2023-06-07 14:07:51.239312 encoded_core-0.0.2/src/encoded_core/schemas/file_format.json
+-rw-r--r--   0        0        0     6170 2023-06-07 14:07:51.239610 encoded_core-0.0.2/src/encoded_core/schemas/file_processed.json
+-rw-r--r--   0        0        0     2336 2023-06-07 14:07:51.239884 encoded_core-0.0.2/src/encoded_core/schemas/file_reference.json
+-rw-r--r--   0        0        0     1334 2023-06-07 14:07:51.240304 encoded_core-0.0.2/src/encoded_core/schemas/file_submitted.json
+-rw-r--r--   0        0        0     1831 2023-06-07 14:07:51.240585 encoded_core-0.0.2/src/encoded_core/schemas/higlass_view_config.json
+-rw-r--r--   0        0        0     1528 2023-06-07 14:07:51.240923 encoded_core-0.0.2/src/encoded_core/schemas/image.json
+-rw-r--r--   0        0        0    18352 2023-06-07 14:07:51.241363 encoded_core-0.0.2/src/encoded_core/schemas/meta_workflow.json
+-rw-r--r--   0        0        0    14175 2023-06-22 17:49:01.019739 encoded_core-0.0.2/src/encoded_core/schemas/meta_workflow_run.json
+-rw-r--r--   0        0        0    17104 2023-06-22 17:49:01.015017 encoded_core-0.0.2/src/encoded_core/schemas/mixins.json
+-rw-r--r--   0        0        0     4581 2023-06-07 14:07:51.242579 encoded_core-0.0.2/src/encoded_core/schemas/page.json
+-rw-r--r--   0        0        0     1454 2023-06-07 14:07:51.243061 encoded_core-0.0.2/src/encoded_core/schemas/quality_metric.json
+-rw-r--r--   0        0        0     3228 2023-06-07 14:07:51.243351 encoded_core-0.0.2/src/encoded_core/schemas/quality_metric_generic.json
+-rw-r--r--   0        0        0     5715 2023-06-07 14:07:51.243653 encoded_core-0.0.2/src/encoded_core/schemas/software.json
+-rw-r--r--   0        0        0     5010 2023-06-07 14:07:51.244093 encoded_core-0.0.2/src/encoded_core/schemas/static_section.json
+-rw-r--r--   0        0        0    20411 2023-06-07 14:07:51.244521 encoded_core-0.0.2/src/encoded_core/schemas/tracking_item.json
+-rw-r--r--   0        0        0     3749 2023-06-07 14:07:51.244808 encoded_core-0.0.2/src/encoded_core/schemas/user_content.json
+-rw-r--r--   0        0        0    28089 2023-06-07 14:07:51.245271 encoded_core-0.0.2/src/encoded_core/schemas/workflow.json
+-rw-r--r--   0        0        0    10491 2023-06-07 14:07:51.245547 encoded_core-0.0.2/src/encoded_core/schemas/workflow_run.json
+-rw-r--r--   0        0        0     1908 2023-06-07 14:07:51.245969 encoded_core-0.0.2/src/encoded_core/schemas/workflow_run_awsem.json
+-rw-r--r--   0        0        0        0 2023-06-07 14:07:51.246263 encoded_core-0.0.2/src/encoded_core/tests/__init__.py
+-rw-r--r--   0        0        0    14054 2023-06-07 14:08:07.651422 encoded_core-0.0.2/src/encoded_core/tests/conftest.py
+-rw-r--r--   0        0        0     1873 2023-06-07 14:07:51.247040 encoded_core-0.0.2/src/encoded_core/tests/conftest_settings.py
+-rw-r--r--   0        0        0     7765 2023-06-07 14:07:51.247305 encoded_core-0.0.2/src/encoded_core/tests/datafixtures.py
+-rw-r--r--   0        0        0    10832 2023-06-07 14:07:51.247761 encoded_core-0.0.2/src/encoded_core/tests/test_types_file.py
+-rw-r--r--   0        0        0      262 2023-06-07 14:07:51.247989 encoded_core-0.0.2/src/encoded_core/tests/test_types_file_format.py
+-rw-r--r--   0        0        0      239 2023-06-07 14:07:51.248304 encoded_core-0.0.2/src/encoded_core/tests/test_types_meta_workflow.py
+-rw-r--r--   0        0        0      212 2023-06-07 14:07:51.248590 encoded_core-0.0.2/src/encoded_core/tests/test_types_software.py
+-rw-r--r--   0        0        0      502 2023-06-07 14:07:51.248826 encoded_core-0.0.2/src/encoded_core/tests/test_types_workflow.py
+-rw-r--r--   0        0        0       70 2023-06-07 14:07:51.249072 encoded_core-0.0.2/src/encoded_core/types/__init__.py
+-rw-r--r--   0        0        0     1284 2023-06-07 14:07:51.249504 encoded_core-0.0.2/src/encoded_core/types/document.py
+-rw-r--r--   0        0        0    19984 2023-06-22 17:53:39.844794 encoded_core-0.0.2/src/encoded_core/types/file.py
+-rw-r--r--   0        0        0      789 2023-06-07 14:07:51.250399 encoded_core-0.0.2/src/encoded_core/types/file_format.py
+-rw-r--r--   0        0        0     2297 2023-06-07 14:07:51.250690 encoded_core-0.0.2/src/encoded_core/types/file_processed.py
+-rw-r--r--   0        0        0      462 2023-06-07 14:07:51.250942 encoded_core-0.0.2/src/encoded_core/types/file_reference.py
+-rw-r--r--   0        0        0     1970 2023-06-07 14:07:51.251277 encoded_core-0.0.2/src/encoded_core/types/file_submitted.py
+-rw-r--r--   0        0        0      584 2023-06-07 14:07:51.251811 encoded_core-0.0.2/src/encoded_core/types/higlass_view_config.py
+-rw-r--r--   0        0        0     1040 2023-06-07 14:07:51.252223 encoded_core-0.0.2/src/encoded_core/types/image.py
+-rw-r--r--   0        0        0     3136 2023-06-07 14:07:51.252605 encoded_core-0.0.2/src/encoded_core/types/meta_workflow.py
+-rw-r--r--   0        0        0      858 2023-06-07 14:07:51.252830 encoded_core-0.0.2/src/encoded_core/types/page.py
+-rw-r--r--   0        0        0     1705 2023-06-07 14:07:51.253054 encoded_core-0.0.2/src/encoded_core/types/quality_metric.py
+-rw-r--r--   0        0        0     2750 2023-06-07 14:07:51.253281 encoded_core-0.0.2/src/encoded_core/types/software.py
+-rw-r--r--   0        0        0     3847 2023-06-07 14:07:51.253509 encoded_core-0.0.2/src/encoded_core/types/tracking_item.py
+-rw-r--r--   0        0        0     5468 2023-06-07 14:07:51.253828 encoded_core-0.0.2/src/encoded_core/types/user_content.py
+-rw-r--r--   0        0        0    12886 2023-06-07 14:07:51.254085 encoded_core-0.0.2/src/encoded_core/types/workflow.py
+-rw-r--r--   0        0        0     1316 2023-06-07 14:07:51.254451 encoded_core-0.0.2/src/encoded_core/upgrade.py
+-rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 encoded_core-0.0.2/setup.py
+-rw-r--r--   0        0        0     2581 1970-01-01 00:00:00.000000 encoded_core-0.0.2/PKG-INFO
```

### Comparing `encoded_core-0.0.1/LICENSE` & `encoded_core-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/pyproject.toml` & `encoded_core-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encoded-core"
-version = "0.0.1"
+version = "0.0.2"
 description = "Core data models for Park Lab ENCODE based projects"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/smaht-dac/encoded-core"
 repository = "https://github.com/smaht-dac/encoded-core"
 documentation = "https://github.com/smaht-dac/encoded-core"
```

### Comparing `encoded_core-0.0.1/src/encoded_core/__init__.py` & `encoded_core-0.0.2/src/encoded_core/__init__.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/file_views.py` & `encoded_core-0.0.2/src/encoded_core/file_views.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/local_roles.py` & `encoded_core-0.0.2/src/encoded_core/local_roles.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/page_views.py` & `encoded_core-0.0.2/src/encoded_core/page_views.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/qc_views.py` & `encoded_core-0.0.2/src/encoded_core/qc_views.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/document.json` & `encoded_core-0.0.2/src/encoded_core/schemas/document.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/file.json` & `encoded_core-0.0.2/src/encoded_core/schemas/file.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/file_format.json` & `encoded_core-0.0.2/src/encoded_core/schemas/file_format.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/file_processed.json` & `encoded_core-0.0.2/src/encoded_core/schemas/file_processed.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/file_reference.json` & `encoded_core-0.0.2/src/encoded_core/schemas/file_reference.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/file_submitted.json` & `encoded_core-0.0.2/src/encoded_core/schemas/file_submitted.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/higlass_view_config.json` & `encoded_core-0.0.2/src/encoded_core/schemas/higlass_view_config.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/image.json` & `encoded_core-0.0.2/src/encoded_core/schemas/image.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/meta_workflow.json` & `encoded_core-0.0.2/src/encoded_core/schemas/meta_workflow.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/meta_workflow_run.json` & `encoded_core-0.0.2/src/encoded_core/schemas/meta_workflow_run.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999666132478632%*

 * *Differences: {"'properties'": "{'common_fields': {'properties': {delete: ['project']}}}"}*

```diff
@@ -83,20 +83,14 @@
                     "type": "array"
                 },
                 "institution": {
                     "description": "Institution associated with the MWFR",
                     "format": "uuid",
                     "title": "Institution",
                     "type": "string"
-                },
-                "project": {
-                    "description": "Project associated with the MWFR",
-                    "format": "uuid",
-                    "title": "Project",
-                    "type": "string"
                 }
             },
             "title": "Common Fields",
             "type": "object"
         },
         "cost": {
             "description": "Total cost of the meta workflow run (includes failed jobs)",
```

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/mixins.json` & `encoded_core-0.0.2/src/encoded_core/schemas/mixins.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9523809523809523%*

 * *Differences: {'delete': "['facets_common']"}*

```diff
@@ -160,22 +160,14 @@
                 "type": "string"
             },
             "title": "Documents",
             "type": "array",
             "uniqueItems": true
         }
     },
-    "facets_common": {
-        "institution.display_title": {
-            "title": "Institution"
-        },
-        "project.display_title": {
-            "title": "Project"
-        }
-    },
     "ingestion_ids": {
         "ingestion_ids": {
             "description": "uuids of the IngestionSubmission items that created/edited this case",
             "items": {
                 "description": "an IngestionSubmission item that created or edited this case",
                 "title": "Submission ID",
                 "type": "string"
```

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/page.json` & `encoded_core-0.0.2/src/encoded_core/schemas/page.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/quality_metric.json` & `encoded_core-0.0.2/src/encoded_core/schemas/quality_metric.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/quality_metric_generic.json` & `encoded_core-0.0.2/src/encoded_core/schemas/quality_metric_generic.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/software.json` & `encoded_core-0.0.2/src/encoded_core/schemas/software.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/static_section.json` & `encoded_core-0.0.2/src/encoded_core/schemas/static_section.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/tracking_item.json` & `encoded_core-0.0.2/src/encoded_core/schemas/tracking_item.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/user_content.json` & `encoded_core-0.0.2/src/encoded_core/schemas/user_content.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/workflow.json` & `encoded_core-0.0.2/src/encoded_core/schemas/workflow.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/workflow_run.json` & `encoded_core-0.0.2/src/encoded_core/schemas/workflow_run.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/schemas/workflow_run_awsem.json` & `encoded_core-0.0.2/src/encoded_core/schemas/workflow_run_awsem.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/tests/conftest.py` & `encoded_core-0.0.2/src/encoded_core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/tests/conftest_settings.py` & `encoded_core-0.0.2/src/encoded_core/tests/conftest_settings.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/tests/datafixtures.py` & `encoded_core-0.0.2/src/encoded_core/tests/datafixtures.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/tests/test_types_file.py` & `encoded_core-0.0.2/src/encoded_core/tests/test_types_file.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/types/document.py` & `encoded_core-0.0.2/src/encoded_core/types/document.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/types/file.py` & `encoded_core-0.0.2/src/encoded_core/types/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,16 +153,14 @@
         "related_files.file.accession",
         "related_files.file.file_format.file_format",
 
         # QC
         "quality_metric.@type",
         "quality_metric.qc_list.qc_type",
         "quality_metric.qc_list.value.uuid",
-
-        "project.lifecycle_management_active"
     ]
 
 
 @abstract_collection(
     name='files',
     unique_key='accession',
     properties={
```

### Comparing `encoded_core-0.0.1/src/encoded_core/types/file_format.py` & `encoded_core-0.0.2/src/encoded_core/types/file_format.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/types/file_processed.py` & `encoded_core-0.0.2/src/encoded_core/types/file_processed.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/types/file_submitted.py` & `encoded_core-0.0.2/src/encoded_core/types/file_submitted.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/types/higlass_view_config.py` & `encoded_core-0.0.2/src/encoded_core/types/higlass_view_config.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/types/image.py` & `encoded_core-0.0.2/src/encoded_core/types/image.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/types/meta_workflow.py` & `encoded_core-0.0.2/src/encoded_core/types/meta_workflow.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/types/page.py` & `encoded_core-0.0.2/src/encoded_core/types/page.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/types/quality_metric.py` & `encoded_core-0.0.2/src/encoded_core/types/quality_metric.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/types/software.py` & `encoded_core-0.0.2/src/encoded_core/types/software.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/types/tracking_item.py` & `encoded_core-0.0.2/src/encoded_core/types/tracking_item.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/types/user_content.py` & `encoded_core-0.0.2/src/encoded_core/types/user_content.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/types/workflow.py` & `encoded_core-0.0.2/src/encoded_core/types/workflow.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/src/encoded_core/upgrade.py` & `encoded_core-0.0.2/src/encoded_core/upgrade.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.1/setup.py` & `encoded_core-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                      'show-image-manifest = '
                      'dcicutils.ecr_scripts:show_image_manifest_main',
                      'unrelease-most-recent-image = '
                      'dcicutils.ecr_scripts:unrelease_most_recent_image_main']}
 
 setup_kwargs = {
     'name': 'encoded-core',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Core data models for Park Lab ENCODE based projects',
     'long_description': '============\nencoded-core\n============\n\n\nWelcome to ``encoded-core``!\n\nThis library contains common data models used across ENCODE style projects\nimplemented by the Park Lab.',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/smaht-dac/encoded-core',
```

### Comparing `encoded_core-0.0.1/PKG-INFO` & `encoded_core-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encoded-core
-Version: 0.0.1
+Version: 0.0.2
 Summary: Core data models for Park Lab ENCODE based projects
 Home-page: https://github.com/smaht-dac/encoded-core
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 3 - Alpha
```

