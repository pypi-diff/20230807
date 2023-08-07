# Comparing `tmp/reasoner_validator-3.7.6.tar.gz` & `tmp/reasoner_validator-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.7.6.tar", max compression
+gzip compressed data, was "reasoner_validator-3.8.0.tar", max compression
```

## Comparing `reasoner_validator-3.7.6.tar` & `reasoner_validator-3.8.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1153 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/LICENSE
--rw-r--r--   0        0        0    12920 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/README.md
--rw-r--r--   0        0        0      131 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/Makefile
--rw-r--r--   0        0        0     2291 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/conf.py
--rw-r--r--   0        0        0    20273 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/index.rst
--rw-r--r--   0        0        0      795 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/make.bat
--rw-r--r--   0        0        0      136 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    37242 2023-08-04 05:22:07.549872 reasoner_validator-3.7.6/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2248 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/pyproject.toml
--rw-r--r--   0        0        0      990 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    83629 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    40494 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     3382 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/message.py
--rw-r--r--   0        0        0    26619 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    13885 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1112 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14569 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    38887 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/validator.py
--rw-r--r--   0        0        0    12532 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/reasoner_validator/versioning.py
--rw-r--r--   0        0        0     1477 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/conftest.py
--rw-r--r--   0        0        0   118956 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    40854 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/test_semver.py
--rw-r--r--   0        0        0     2278 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    27158 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/test_validate.py
--rw-r--r--   0        0        0    20409 2023-08-04 05:22:07.553872 reasoner_validator-3.7.6/tests/test_validation_report.py
--rw-r--r--   0        0        0     2042 2023-08-04 05:22:07.557872 reasoner_validator-3.7.6/tests/test_workflows.py
--rw-r--r--   0        0        0    14905 1970-01-01 00:00:00.000000 reasoner_validator-3.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-08-07 17:33:51.537834 reasoner_validator-3.8.0/LICENSE
+-rw-r--r--   0        0        0    13186 2023-08-07 17:33:51.537834 reasoner_validator-3.8.0/README.md
+-rw-r--r--   0        0        0      131 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/docs/conf.py
+-rw-r--r--   0        0        0    20304 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    37242 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2248 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/pyproject.toml
+-rw-r--r--   0        0        0      990 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    83629 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    40494 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     3382 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/reasoner_validator/message.py
+-rw-r--r--   0        0        0    26619 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    13885 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1112 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14569 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    38887 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    12532 2023-08-07 17:33:51.541834 reasoner_validator-3.8.0/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0     1477 2023-08-07 17:33:51.545834 reasoner_validator-3.8.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 17:33:51.545834 reasoner_validator-3.8.0/tests/conftest.py
+-rw-r--r--   0        0        0   118956 2023-08-07 17:33:51.545834 reasoner_validator-3.8.0/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2023-08-07 17:33:51.545834 reasoner_validator-3.8.0/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    40854 2023-08-07 17:33:51.545834 reasoner_validator-3.8.0/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2023-08-07 17:33:51.545834 reasoner_validator-3.8.0/tests/test_semver.py
+-rw-r--r--   0        0        0     2278 2023-08-07 17:33:51.545834 reasoner_validator-3.8.0/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    27158 2023-08-07 17:33:51.545834 reasoner_validator-3.8.0/tests/test_validate.py
+-rw-r--r--   0        0        0    20409 2023-08-07 17:33:51.545834 reasoner_validator-3.8.0/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2042 2023-08-07 17:33:51.545834 reasoner_validator-3.8.0/tests/test_workflows.py
+-rw-r--r--   0        0        0    15171 1970-01-01 00:00:00.000000 reasoner_validator-3.8.0/PKG-INFO
```

### Comparing `reasoner_validator-3.7.6/LICENSE` & `reasoner_validator-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/README.md` & `reasoner_validator-3.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -146,15 +146,15 @@
   "biolink_version": "3.5.0",
   "target_provenance": {
     "ara_source": "infores:aragorn",
     "kp_source": "infores:panther",
     "kp_source_type": "primary"
   },
   "strict_validation": true,
-  "response": {<some full JSON object of a TRAPI query Response...>}
+  "response": "{<some full JSON object of a TRAPI query Response...>}"
 }
 ```
 
 The request body consists of JSON data structure with two top level tag:
 
 - An **optional** `trapi_version` tag can be given a value of the TRAPI version against which the message will be validated, expressed as a SemVer string (defaults to 'latest' if omitted; partial SemVer strings are resolved to their 'latest' minor and patch releases). This value may also be a GitHub branch name (e.g. '**master**').
 - An **optional** `biolink_version` tag can be given a value of the Biolink Model version against which the message knowledge graph semantic contents will be validated, expressed as a SemVer string (defaults to 'latest' Biolink Model Toolkit supported version, if omitted). 
@@ -226,35 +226,38 @@
 one should typically get a response body something like the following JSON validation result back:
 
 ```json
 {
   "trapi_version": "1.4.1",
   "biolink_version": "3.2.1",
   "messages": {
-    # some categories of messages may be absent, hence, empty dictionaries
+    "_comment": "some categories of messages may be absent, hence, empty dictionaries",
     "critical": {},
     "errors": {
       "error.knowledge_graph.node.category.missing": {
-          # this message template does not have any additional parameters
-          # other than identifier hence it just has the unique identifier 
-          # value as a dictionary key, with associated value None
-           "MONDO:0005148": None
+          "_comment": "source scope of the validation error ('global' or some knowledge source path string)",
+          "global": {
+              "_comment": "this message template does not have any additional parameters other than identifier hence it just has the unique identifier  value as a dictionary key, with associated value None",
+               "MONDO:0005148": null            
+          }
         }
     },
     "warnings": {
-      # validation code
+      "_comment": "validation code",
       "warning.knowledge_graph.node.unmapped_prefix": {
-          # template identifier field value
-          "CHEBI:6801": [  
-              {
-                # additional message template field values, if applicable
-                "categories": "['biolink:Drug']"  
-              }
-          ]
-          
+          "global": {
+              "_comment": "template identifier field value",
+              "CHEBI:6801": [  
+                  {
+                    "_comment": "additional message template field values, if applicable",
+                    "categories": "['biolink:Drug']"  
+                  }
+              ]       
+          }
+
         }
     },
     "information": {},
   }
 }
 ```
```

### Comparing `reasoner_validator-3.7.6/docs/Makefile` & `reasoner_validator-3.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/docs/conf.py` & `reasoner_validator-3.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/docs/index.rst` & `reasoner_validator-3.8.0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 in a dictionary looking something like the following (as an example):
 
 .. code-block:: python
 
     messages: Dict[str, List[Dict[str,str]]] = {
         "information": {
             "info.excluded": {
-                # source scope of the validation error ("global" or some knowledge source path string
+                # source scope of the validation error ("global" or some knowledge source path string)
                 "global": {
                     # the uniquely discriminating 'identifier' here is the edge_id
                     "(ZFIN:ZDB-GENE-060825-345$biolink:Gene)--[biolink:active_in]->(GO:0042645$biolink:CellularComponent)": None
                     # messages with only a contextual identifier may have no additional parameters
                 },
                 {...}  # another message (same code type)
             },
@@ -242,32 +242,32 @@
 ---------------
 
 The web service has a single POST endpoint `/validate` taking a simple JSON request body, as follows:
 
 .. code-block:: json
 
     {
-        # If the TRAPI version is omitted or set to None, then the 'latest' TRAPI version is used.
+        "_comment": "If the TRAPI version is omitted or set to None, then the 'latest' TRAPI version is used.
 
         # Note: for TRAPI releases from 1.4.0 onwards, the Response message will state the assumed 'schema_version'.
         # This modifies slightly the interpretation of this parameter, as follows:
         # If the following trapi_version parameter is given, then it overrides the TRAPI Response 'schema_version';
-        # Otherwise, a TRAPI 1.4.0 Response embedded 'schema_version' (not 'latest') becomes the default validation version.
+        # Otherwise, a TRAPI 1.4.0 Response embedded 'schema_version' (not 'latest') becomes the default validation version."
 
-        trapi_version="1.4.2",
+        "trapi_version": "1.4.2",
 
-        # If the Biolink Model version is omitted or set to None, then the current Biolink Model Toolkit is used.
+        "_comment": "If the Biolink Model version is omitted or set to None, then the current Biolink Model Toolkit is used.
 
         # Note: for TRAPI releases from 1.4.0 onwards, the Response message will state the assumed 'biolink_version'.
         # This modifies slightly the interpretation of this parameter, as follows:
         # If the 'biolink_version' given here is assumed, which overrides the TRAPI Response stated 'biolink_version';
         # Otherwise, a TRAPI 1.4.0 Response embedded 'biolink_version' (not BMT) becomes the default validation version.
-        # The biolink_version may also be set to the string 'suppress', in which case, most Biolink Model validation is NOT done during the validation of a TRAPI Response.
+        # The biolink_version may also be set to the string 'suppress', in which case, most Biolink Model validation is NOT done during the validation of a TRAPI Response."
 
-        biolink_version="3.5.0",
+        "biolink_version": "3.5.0",
 
         "sources": {
             "ara_source": "infores:aragorn",
             "kp_source": "infores:panther",
             "kp_source_type": "primary"
         },
         "strict_validation": true,
```

### Comparing `reasoner_validator-3.7.6/docs/make.bat` & `reasoner_validator-3.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/docs/validation_codes_dictionary.md` & `reasoner_validator-3.8.0/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/pyproject.toml` & `reasoner_validator-3.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.7.6"
+version = "3.8.0"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.7.6/reasoner_validator/__init__.py` & `reasoner_validator-3.8.0/reasoner_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.8.0/reasoner_validator/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/reasoner_validator/codes.yaml` & `reasoner_validator-3.8.0/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/reasoner_validator/message.py` & `reasoner_validator-3.8.0/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/reasoner_validator/report.py` & `reasoner_validator-3.8.0/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/reasoner_validator/sri/util.py` & `reasoner_validator-3.8.0/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.8.0/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.8.0/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/reasoner_validator/validation_codes.py` & `reasoner_validator-3.8.0/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/reasoner_validator/validator.py` & `reasoner_validator-3.8.0/reasoner_validator/validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/reasoner_validator/versioning.py` & `reasoner_validator-3.8.0/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/tests/__init__.py` & `reasoner_validator-3.8.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.8.0/tests/test_biolink_compliance_validation.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-3.8.0/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/tests/test_response_validator.py` & `reasoner_validator-3.8.0/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/tests/test_semver.py` & `reasoner_validator-3.8.0/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/tests/test_trapi_versioning.py` & `reasoner_validator-3.8.0/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/tests/test_validate.py` & `reasoner_validator-3.8.0/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/tests/test_validation_report.py` & `reasoner_validator-3.8.0/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/tests/test_workflows.py` & `reasoner_validator-3.8.0/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.6/PKG-INFO` & `reasoner_validator-3.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.7.6
+Version: 3.8.0
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -188,15 +188,15 @@
   "biolink_version": "3.5.0",
   "target_provenance": {
     "ara_source": "infores:aragorn",
     "kp_source": "infores:panther",
     "kp_source_type": "primary"
   },
   "strict_validation": true,
-  "response": {<some full JSON object of a TRAPI query Response...>}
+  "response": "{<some full JSON object of a TRAPI query Response...>}"
 }
 ```
 
 The request body consists of JSON data structure with two top level tag:
 
 - An **optional** `trapi_version` tag can be given a value of the TRAPI version against which the message will be validated, expressed as a SemVer string (defaults to 'latest' if omitted; partial SemVer strings are resolved to their 'latest' minor and patch releases). This value may also be a GitHub branch name (e.g. '**master**').
 - An **optional** `biolink_version` tag can be given a value of the Biolink Model version against which the message knowledge graph semantic contents will be validated, expressed as a SemVer string (defaults to 'latest' Biolink Model Toolkit supported version, if omitted). 
@@ -268,35 +268,38 @@
 one should typically get a response body something like the following JSON validation result back:
 
 ```json
 {
   "trapi_version": "1.4.1",
   "biolink_version": "3.2.1",
   "messages": {
-    # some categories of messages may be absent, hence, empty dictionaries
+    "_comment": "some categories of messages may be absent, hence, empty dictionaries",
     "critical": {},
     "errors": {
       "error.knowledge_graph.node.category.missing": {
-          # this message template does not have any additional parameters
-          # other than identifier hence it just has the unique identifier 
-          # value as a dictionary key, with associated value None
-           "MONDO:0005148": None
+          "_comment": "source scope of the validation error ('global' or some knowledge source path string)",
+          "global": {
+              "_comment": "this message template does not have any additional parameters other than identifier hence it just has the unique identifier  value as a dictionary key, with associated value None",
+               "MONDO:0005148": null            
+          }
         }
     },
     "warnings": {
-      # validation code
+      "_comment": "validation code",
       "warning.knowledge_graph.node.unmapped_prefix": {
-          # template identifier field value
-          "CHEBI:6801": [  
-              {
-                # additional message template field values, if applicable
-                "categories": "['biolink:Drug']"  
-              }
-          ]
-          
+          "global": {
+              "_comment": "template identifier field value",
+              "CHEBI:6801": [  
+                  {
+                    "_comment": "additional message template field values, if applicable",
+                    "categories": "['biolink:Drug']"  
+                  }
+              ]       
+          }
+
         }
     },
     "information": {},
   }
 }
 ```
```

