# Comparing `tmp/sanctify-1.1.8.tar.gz` & `tmp/sanctify-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanctify-1.1.8.tar", last modified: Tue Jul 25 19:43:34 2023, max compression
+gzip compressed data, was "sanctify-1.1.9.tar", last modified: Mon Aug  7 05:47:41 2023, max compression
```

## Comparing `sanctify-1.1.8.tar` & `sanctify-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-25 19:43:34.264052 sanctify-1.1.8/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11349 2023-07-24 05:34:49.000000 sanctify-1.1.8/LICENSE
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18575 2023-07-25 19:43:34.262789 sanctify-1.1.8/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    17964 2023-07-25 19:38:03.000000 sanctify-1.1.8/README.md
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1415 2023-07-25 19:39:51.000000 sanctify-1.1.8/pyproject.toml
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-25 19:43:34.261698 sanctify-1.1.8/sanctify/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1059 2023-07-25 19:40:02.000000 sanctify-1.1.8/sanctify/__init__.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     7648 2023-07-17 13:52:28.000000 sanctify-1.1.8/sanctify/cleanser.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2632 2023-07-17 13:52:28.000000 sanctify-1.1.8/sanctify/constants.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      332 2023-07-25 19:35:23.000000 sanctify-1.1.8/sanctify/exception.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    13269 2023-07-25 19:40:02.000000 sanctify-1.1.8/sanctify/processor.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4145 2023-07-25 19:13:47.000000 sanctify-1.1.8/sanctify/serializer.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     8782 2023-07-17 13:52:28.000000 sanctify-1.1.8/sanctify/transformer.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4545 2023-07-25 16:13:58.000000 sanctify-1.1.8/sanctify/utils.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11128 2023-07-25 19:40:02.000000 sanctify-1.1.8/sanctify/validator.py
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-25 19:43:34.262492 sanctify-1.1.8/sanctify.egg-info/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18575 2023-07-25 19:43:34.000000 sanctify-1.1.8/sanctify.egg-info/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      355 2023-07-25 19:43:34.000000 sanctify-1.1.8/sanctify.egg-info/SOURCES.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2023-07-25 19:43:34.000000 sanctify-1.1.8/sanctify.egg-info/dependency_links.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2023-07-25 19:43:34.000000 sanctify-1.1.8/sanctify.egg-info/top_level.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2023-07-25 19:43:34.264111 sanctify-1.1.8/setup.cfg
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-08-07 05:47:41.762198 sanctify-1.1.9/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11349 2023-07-24 05:34:49.000000 sanctify-1.1.9/LICENSE
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18587 2023-08-07 05:47:41.761900 sanctify-1.1.9/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    17964 2023-08-07 05:30:23.000000 sanctify-1.1.9/README.md
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1427 2023-08-07 05:47:20.000000 sanctify-1.1.9/pyproject.toml
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-08-07 05:47:41.760233 sanctify-1.1.9/sanctify/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1286 2023-08-07 05:44:56.000000 sanctify-1.1.9/sanctify/__init__.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     7648 2023-07-17 13:52:28.000000 sanctify-1.1.9/sanctify/cleanser.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2632 2023-07-17 13:52:28.000000 sanctify-1.1.9/sanctify/constants.py
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-08-07 05:47:41.761531 sanctify-1.1.9/sanctify/examples/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      329 2023-08-07 05:44:56.000000 sanctify-1.1.9/sanctify/examples/__init__.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2354 2023-08-07 05:32:45.000000 sanctify-1.1.9/sanctify/examples/column_mapping_schema.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3309 2023-08-07 05:32:45.000000 sanctify-1.1.9/sanctify/examples/data_type_schema.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      332 2023-08-07 05:30:23.000000 sanctify-1.1.9/sanctify/exception.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    13269 2023-08-07 05:44:56.000000 sanctify-1.1.9/sanctify/processor.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4145 2023-08-07 05:30:23.000000 sanctify-1.1.9/sanctify/serializer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9344 2023-08-07 05:38:52.000000 sanctify-1.1.9/sanctify/transformer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4545 2023-08-07 05:30:23.000000 sanctify-1.1.9/sanctify/utils.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11128 2023-08-07 05:44:56.000000 sanctify-1.1.9/sanctify/validator.py
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-08-07 05:47:41.760900 sanctify-1.1.9/sanctify.egg-info/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18587 2023-08-07 05:47:41.000000 sanctify-1.1.9/sanctify.egg-info/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      466 2023-08-07 05:47:41.000000 sanctify-1.1.9/sanctify.egg-info/SOURCES.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2023-08-07 05:47:41.000000 sanctify-1.1.9/sanctify.egg-info/dependency_links.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2023-08-07 05:47:41.000000 sanctify-1.1.9/sanctify.egg-info/top_level.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2023-08-07 05:47:41.762245 sanctify-1.1.9/setup.cfg
```

### Comparing `sanctify-1.1.8/LICENSE` & `sanctify-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sanctify-1.1.8/PKG-INFO` & `sanctify-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.1.8
+Version: 1.1.9
 Summary: Column Mapping based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sanctify [![codecov](https://codecov.io/gh/skit-ai/sanctify/branch/main/graph/badge.svg?token=WZHSY8T8SC)](https://codecov.io/gh/skit-ai/sanctify)
```

### Comparing `sanctify-1.1.8/README.md` & `sanctify-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sanctify-1.1.8/pyproject.toml` & `sanctify-1.1.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -53,22 +53,22 @@
 
 [tool.pytest.ini_options]
 log_cli=true
 log_cli_level='DEBUG'
 
 [project]
 name = "sanctify"
-version = "1.1.8"
+version = "1.1.9"
 authors = [{name = "Avijeet Diwaker", email = "avijeetdiwaker@gmail.com"}]
 description = "Column Mapping based cleansing and validations for a given pandas dataframe"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.11",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/skit-ai/sanctify"
 "Bug Tracker" = "https://github.com/skit-ai/sanctify/issues"
```

### Comparing `sanctify-1.1.8/sanctify/__init__.py` & `sanctify-1.1.9/sanctify/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     CalendarDateComponents,
     ComparisonOperations,
     Constants,
     DateOrderTuples,
     DefaultColumns,
     PrimitiveDataTypes,
 )
+from sanctify.examples import EXAMPLE_COLUMN_MAPPING, EXAMPLE_COLUMN_MAPPING_USING_DATA_TYPE, EXAMPLE_DATA_TYPE_SCHEMA
 from sanctify.exception import DataTypeParseError, ValidationError
 from sanctify.processor import process_cleansed_df
 from sanctify.serializer import CustomJSONDecoder, CustomJSONEncoder, SchemaDeSerializer, SchemaSerializer
 from sanctify.transformer import Transformer
 from sanctify.validator import Validator
 
 __all__ = [
@@ -31,8 +32,11 @@
     "DataTypeParseError",
     "ValidationError",
     "process_cleansed_df",
     "SchemaDeSerializer",
     "SchemaSerializer",
     "Transformer",
     "Validator",
+    "EXAMPLE_COLUMN_MAPPING",
+    "EXAMPLE_COLUMN_MAPPING_USING_DATA_TYPE",
+    "EXAMPLE_DATA_TYPE_SCHEMA",
 ]
```

### Comparing `sanctify-1.1.8/sanctify/cleanser.py` & `sanctify-1.1.9/sanctify/cleanser.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.1.8/sanctify/constants.py` & `sanctify-1.1.9/sanctify/constants.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.1.8/sanctify/processor.py` & `sanctify-1.1.9/sanctify/processor.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.1.8/sanctify/serializer.py` & `sanctify-1.1.9/sanctify/serializer.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.1.8/sanctify/transformer.py` & `sanctify-1.1.9/sanctify/transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,14 +95,40 @@
 
         Returns:
             str: The lowercase string.
         """
         return str(value).lower()
 
     @staticmethod
+    def convert_to_uppercase(value: str) -> str:
+        """
+        Converts a string to uppercase.
+
+        Args:
+            value (str): The input string.
+
+        Returns:
+            str: The uppercase string.
+        """
+        return str(value).upper()
+
+    @staticmethod
+    def convert_to_titlecase(value: str) -> str:
+        """
+        Converts a string to titlecase.
+
+        Args:
+            value (str): The input string.
+
+        Returns:
+            str: The titlecase string.
+        """
+        return str(value).title()
+
+    @staticmethod
     def replace_ii_with_II(value: str) -> str:
         """
         Replaces "ii" with "II" in a string.
 
         Args:
             value (str): The input string.
```

### Comparing `sanctify-1.1.8/sanctify/utils.py` & `sanctify-1.1.9/sanctify/utils.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.1.8/sanctify/validator.py` & `sanctify-1.1.9/sanctify/validator.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.1.8/sanctify.egg-info/PKG-INFO` & `sanctify-1.1.9/sanctify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.1.8
+Version: 1.1.9
 Summary: Column Mapping based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sanctify [![codecov](https://codecov.io/gh/skit-ai/sanctify/branch/main/graph/badge.svg?token=WZHSY8T8SC)](https://codecov.io/gh/skit-ai/sanctify)
```

