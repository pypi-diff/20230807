# Comparing `tmp/entity-type-local-0.0.5.tar.gz` & `tmp/entity-type-local-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entity-type-local-0.0.5.tar", last modified: Fri Aug  4 07:26:17 2023, max compression
+gzip compressed data, was "entity-type-local-0.0.6.tar", last modified: Mon Aug  7 10:49:24 2023, max compression
```

## Comparing `entity-type-local-0.0.5.tar` & `entity-type-local-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:26:17.393357 entity-type-local-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-04 07:26:17.393357 entity-type-local-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-04 07:25:53.000000 entity-type-local-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:26:17.393357 entity-type-local-0.0.5/entity_type/
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-08-04 07:25:53.000000 entity-type-local-0.0.5/entity_type/EntityType.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:25:53.000000 entity-type-local-0.0.5/entity_type/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:26:17.393357 entity-type-local-0.0.5/entity_type_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-04 07:26:17.000000 entity-type-local-0.0.5/entity_type_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-04 07:26:17.000000 entity-type-local-0.0.5/entity_type_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 07:26:17.000000 entity-type-local-0.0.5/entity_type_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 07:26:17.000000 entity-type-local-0.0.5/entity_type_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-04 07:25:53.000000 entity-type-local-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 07:26:17.393357 entity-type-local-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-04 07:25:53.000000 entity-type-local-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:26:17.393357 entity-type-local-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-04 07:25:53.000000 entity-type-local-0.0.5/tests/test_entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:49:24.658053 entity-type-local-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-07 10:49:24.654053 entity-type-local-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-07 10:49:01.000000 entity-type-local-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:49:24.654053 entity-type-local-0.0.6/entity_type/
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-08-07 10:49:01.000000 entity-type-local-0.0.6/entity_type/EntityType.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 10:49:01.000000 entity-type-local-0.0.6/entity_type/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:49:24.654053 entity-type-local-0.0.6/entity_type_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-07 10:49:24.000000 entity-type-local-0.0.6/entity_type_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-07 10:49:24.000000 entity-type-local-0.0.6/entity_type_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:49:24.000000 entity-type-local-0.0.6/entity_type_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 10:49:24.000000 entity-type-local-0.0.6/entity_type_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-07 10:49:01.000000 entity-type-local-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:49:24.658053 entity-type-local-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-07 10:49:01.000000 entity-type-local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:49:24.654053 entity-type-local-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-07 10:49:01.000000 entity-type-local-0.0.6/tests/test_entity.py
```

### Comparing `entity-type-local-0.0.5/entity_type/EntityType.py` & `entity-type-local-0.0.6/entity_type/EntityType.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from dotenv import load_dotenv
 from logger_local.LoggerLocal import logger_local
-from circles_local_database_python.database import database
+#from circles_local_database_python.database import database
+from circles_local_database_python.connection import DatabaseFunctions
 load_dotenv()
 obj = {
     'component_id': 116
 }
 logger_local.init(object=obj)
-db = database()
-connection = db.connect_to_database()
+database_conn = DatabaseFunctions("entityType")
+connection = database_conn.connect()
 
 
 class EntityType:
 
     def __init__(self):
         pass
```

### Comparing `entity-type-local-0.0.5/setup.py` & `entity-type-local-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      name='entity-type-local',
-     version='0.0.5',
+     version='0.0.6',
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local Entity Type Python (Currently empty package)",
      long_description="This is a package for sharing common importer function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

### Comparing `entity-type-local-0.0.5/tests/test_entity.py` & `entity-type-local-0.0.6/tests/test_entity.py`

 * *Files identical despite different names*

