# Comparing `tmp/drf_pydantic_openapi-0.4.2.tar.gz` & `tmp/drf_pydantic_openapi-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_pydantic_openapi-0.4.2.tar", max compression
+gzip compressed data, was "drf_pydantic_openapi-0.4.3.tar", max compression
```

## Comparing `drf_pydantic_openapi-0.4.2.tar` & `drf_pydantic_openapi-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1070 2023-04-27 13:44:08.423219 drf_pydantic_openapi-0.4.2/LICENSE
--rw-r--r--   0        0        0     2596 2023-05-09 09:59:45.223778 drf_pydantic_openapi-0.4.2/README.md
--rw-r--r--   0        0        0        0 2023-05-31 10:00:59.144732 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/__init__.py
--rw-r--r--   0        0        0      164 2023-04-27 14:01:32.336379 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/apps.py
--rw-r--r--   0        0        0     1456 2023-05-08 13:59:43.276920 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/errors.py
--rw-r--r--   0        0        0      489 2023-04-27 13:44:28.146816 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/exception_handler.py
--rw-r--r--   0        0        0     6097 2023-07-25 13:31:14.696792 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/generator.py
--rw-r--r--   0        0        0     2289 2023-06-02 08:27:03.420495 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/patches.py
--rw-r--r--   0        0        0     1476 2023-06-02 09:32:06.456794 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/path.py
--rw-r--r--   0        0        0     1517 2023-05-23 13:35:05.835776 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/ref_source.py
--rw-r--r--   0        0        0     4143 2023-05-26 14:34:32.395942 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/ref_utils.py
--rw-r--r--   0        0        0     1112 2023-07-24 14:01:09.538626 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/settings.py
--rw-r--r--   0        0        0      435 2023-06-01 16:41:18.204945 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/templates/drf_pydantic_openapi/rapidoc.html
--rw-r--r--   0        0        0      534 2023-06-01 15:09:21.868622 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html
--rw-r--r--   0        0        0      246 2023-07-24 13:38:54.240481 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/urls.py
--rw-r--r--   0        0        0     4198 2023-07-25 13:30:08.336692 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/utils.py
--rw-r--r--   0        0        0     2186 2023-07-24 14:04:40.140850 drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/views.py
--rw-r--r--   0        0        0     1231 2023-08-04 10:21:51.516331 drf_pydantic_openapi-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3253 1970-01-01 00:00:00.000000 drf_pydantic_openapi-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-27 13:44:08.423219 drf_pydantic_openapi-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2596 2023-05-09 09:59:45.223778 drf_pydantic_openapi-0.4.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 10:00:59.144732 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-27 14:01:32.336379 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/apps.py
+-rw-r--r--   0        0        0     1456 2023-05-08 13:59:43.276920 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/errors.py
+-rw-r--r--   0        0        0      489 2023-04-27 13:44:28.146816 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/exception_handler.py
+-rw-r--r--   0        0        0     6097 2023-07-25 13:31:14.696792 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/generator.py
+-rw-r--r--   0        0        0     2289 2023-06-02 08:27:03.420495 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/patches.py
+-rw-r--r--   0        0        0     1476 2023-06-02 09:32:06.456794 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/path.py
+-rw-r--r--   0        0        0     1517 2023-05-23 13:35:05.835776 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/ref_source.py
+-rw-r--r--   0        0        0     4143 2023-05-26 14:34:32.395942 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/ref_utils.py
+-rw-r--r--   0        0        0     1112 2023-07-24 14:01:09.538626 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/settings.py
+-rw-r--r--   0        0        0      435 2023-06-01 16:41:18.204945 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/templates/drf_pydantic_openapi/rapidoc.html
+-rw-r--r--   0        0        0      534 2023-06-01 15:09:21.868622 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html
+-rw-r--r--   0        0        0      246 2023-07-24 13:38:54.240481 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/urls.py
+-rw-r--r--   0        0        0     4198 2023-07-25 13:30:08.336692 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/utils.py
+-rw-r--r--   0        0        0     2186 2023-07-24 14:04:40.140850 drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/views.py
+-rw-r--r--   0        0        0     1231 2023-08-07 11:54:02.562784 drf_pydantic_openapi-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     3253 1970-01-01 00:00:00.000000 drf_pydantic_openapi-0.4.3/PKG-INFO
```

### Comparing `drf_pydantic_openapi-0.4.2/LICENSE` & `drf_pydantic_openapi-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.2/README.md` & `drf_pydantic_openapi-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/errors.py` & `drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/errors.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/generator.py` & `drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/generator.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/patches.py` & `drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/patches.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/path.py` & `drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/path.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/ref_source.py` & `drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/ref_source.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/ref_utils.py` & `drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/ref_utils.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/settings.py` & `drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/settings.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html` & `drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/utils.py` & `drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/utils.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.2/drf_pydantic_openapi/views.py` & `drf_pydantic_openapi-0.4.3/drf_pydantic_openapi/views.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.4.2/pyproject.toml` & `drf_pydantic_openapi-0.4.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "drf-pydantic-openapi"
-version = "0.4.2"
+version = "0.4.3"
 description = "OpenAPI (v3) schema generation via Pydantic models using Django REST Framework."
 authors = ["iKlotho <umutkahrimanedu@gmail.com>"]
 readme = "README.md"
 packages = [{include = "drf_pydantic_openapi"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 django = "^3.2.1"
 djangorestframework = "3.13.1"
 openapi-schema-pydantic = "^1.2.4"
 docstring-parser = "^0.15"
-loguru = "^0.4.0"
+loguru = "^0.5.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
```

### Comparing `drf_pydantic_openapi-0.4.2/PKG-INFO` & `drf_pydantic_openapi-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: drf-pydantic-openapi
-Version: 0.4.2
+Version: 0.4.3
 Summary: OpenAPI (v3) schema generation via Pydantic models using Django REST Framework.
 Author: iKlotho
 Author-email: umutkahrimanedu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=3.2.1,<4.0.0)
 Requires-Dist: djangorestframework (==3.13.1)
 Requires-Dist: docstring-parser (>=0.15,<0.16)
-Requires-Dist: loguru (>=0.4.0,<0.5.0)
+Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: openapi-schema-pydantic (>=1.2.4,<2.0.0)
 Description-Content-Type: text/markdown
 
 Generate OpenAPI schema with DRF code using pydantic models. Supports referencing other service's components.
 
 # Usage
```

