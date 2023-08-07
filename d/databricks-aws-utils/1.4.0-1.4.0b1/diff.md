# Comparing `tmp/databricks_aws_utils-1.4.0.tar.gz` & `tmp/databricks_aws_utils-1.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_aws_utils-1.4.0.tar", max compression
+gzip compressed data, was "databricks_aws_utils-1.4.0b1.tar", max compression
```

## Comparing `databricks_aws_utils-1.4.0.tar` & `databricks_aws_utils-1.4.0b1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-08-07 12:26:39.063935 databricks_aws_utils-1.4.0/LICENSE
--rw-r--r--   0        0        0      489 2023-08-07 12:26:39.063935 databricks_aws_utils-1.4.0/README.md
--rw-r--r--   0        0        0     2087 2023-08-07 12:26:39.063935 databricks_aws_utils-1.4.0/databricks_aws_utils/__init__.py
--rw-r--r--   0        0        0    12212 2023-08-07 12:26:39.063935 databricks_aws_utils-1.4.0/databricks_aws_utils/delta_table.py
--rw-r--r--   0        0        0     4331 2023-08-07 12:26:39.063935 databricks_aws_utils-1.4.0/databricks_aws_utils/rds.py
--rw-r--r--   0        0        0     2174 2023-08-07 12:26:39.063935 databricks_aws_utils-1.4.0/databricks_aws_utils/s3.py
--rw-r--r--   0        0        0     1499 2023-08-07 12:26:39.063935 databricks_aws_utils-1.4.0/databricks_aws_utils/session.py
--rw-r--r--   0        0        0      959 2023-08-07 12:26:39.063935 databricks_aws_utils-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 databricks_aws_utils-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2021-11-22 20:10:33.420205 databricks_aws_utils-1.4.0b1/LICENSE
+-rw-r--r--   0        0        0      489 2021-11-22 20:21:50.459403 databricks_aws_utils-1.4.0b1/README.md
+-rw-r--r--   0        0        0     2087 2021-11-22 20:10:54.570545 databricks_aws_utils-1.4.0b1/databricks_aws_utils/__init__.py
+-rw-r--r--   0        0        0    12212 2023-07-25 10:27:54.566105 databricks_aws_utils-1.4.0b1/databricks_aws_utils/delta_table.py
+-rw-r--r--   0        0        0     4331 2021-11-22 20:10:54.576363 databricks_aws_utils-1.4.0b1/databricks_aws_utils/rds.py
+-rw-r--r--   0        0        0     2174 2021-11-22 20:10:54.577305 databricks_aws_utils-1.4.0b1/databricks_aws_utils/s3.py
+-rw-r--r--   0        0        0     1499 2021-11-22 20:10:54.578167 databricks_aws_utils-1.4.0b1/databricks_aws_utils/session.py
+-rw-r--r--   0        0        0      961 2023-08-03 09:47:19.119531 databricks_aws_utils-1.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 databricks_aws_utils-1.4.0b1/PKG-INFO
```

### Comparing `databricks_aws_utils-1.4.0/LICENSE` & `databricks_aws_utils-1.4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.4.0/databricks_aws_utils/__init__.py` & `databricks_aws_utils-1.4.0b1/databricks_aws_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.4.0/databricks_aws_utils/delta_table.py` & `databricks_aws_utils-1.4.0b1/databricks_aws_utils/delta_table.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.4.0/databricks_aws_utils/rds.py` & `databricks_aws_utils-1.4.0b1/databricks_aws_utils/rds.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.4.0/databricks_aws_utils/s3.py` & `databricks_aws_utils-1.4.0b1/databricks_aws_utils/s3.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.4.0/databricks_aws_utils/session.py` & `databricks_aws_utils-1.4.0b1/databricks_aws_utils/session.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.4.0/pyproject.toml` & `databricks_aws_utils-1.4.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-aws-utils"
-version = "1.4.0"
+version = "1.4.0b1"
 description = "Databricks AWS Utils"
 license = "Proprietary"
 authors = [ "Lucas Vieira <lucas.vieira94@outlook.com>" ]
 maintainers = [ "Lucas Vieira <lucas.vieira94@outlook.com>" ]
 readme = "README.md"
 repository = "https://github.com/lucasvieirasilva/databricks-aws-utils"
```

### Comparing `databricks_aws_utils-1.4.0/PKG-INFO` & `databricks_aws_utils-1.4.0b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-aws-utils
-Version: 1.4.0
+Version: 1.4.0b1
 Summary: Databricks AWS Utils
 Home-page: https://github.com/lucasvieirasilva/databricks-aws-utils
 License: Proprietary
 Author: Lucas Vieira
 Author-email: lucas.vieira94@outlook.com
 Maintainer: Lucas Vieira
 Maintainer-email: lucas.vieira94@outlook.com
```

