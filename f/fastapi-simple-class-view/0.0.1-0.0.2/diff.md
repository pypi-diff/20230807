# Comparing `tmp/fastapi_simple_class_view-0.0.1.tar.gz` & `tmp/fastapi_simple_class_view-0.0.2.tar.gz`

## Comparing `fastapi_simple_class_view-0.0.1.tar` & `fastapi_simple_class_view-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/requirements.in
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/example/__init__.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/example/database.py
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/example/database.sqlite3
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/example/main.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/example/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/example/app/__init__.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/example/app/permissions.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/example/app/scheme.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/example/app/service.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/example/app/urls.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/example/app/view.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/example/tests/__init__.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/example/tests/test_users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/fastapi_simple_class_view/__init__.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/fastapi_simple_class_view/abc.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/fastapi_simple_class_view/base.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/fastapi_simple_class_view/controller.py
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/fastapi_simple_class_view/meta.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/fastapi_simple_class_view/mixins.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/src/fastapi_simple_class_view/type.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/LICENSE
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/README.md
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/requirements.in
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/example/__init__.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/example/database.py
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/example/database.sqlite3
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/example/main.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/example/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/example/app/__init__.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/example/app/permissions.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/example/app/scheme.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/example/app/service.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/example/app/urls.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/example/app/view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/example/tests/__init__.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/example/tests/test_users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/fastapi_simple_class_view/__init__.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/fastapi_simple_class_view/abc.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/fastapi_simple_class_view/base.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/fastapi_simple_class_view/controller.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/fastapi_simple_class_view/meta.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/fastapi_simple_class_view/mixins.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/src/fastapi_simple_class_view/type.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/README.md
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 fastapi_simple_class_view-0.0.2/PKG-INFO
```

### Comparing `fastapi_simple_class_view-0.0.1/.pre-commit-config.yaml` & `fastapi_simple_class_view-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fastapi_simple_class_view-0.0.1/requirements.txt` & `fastapi_simple_class_view-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `fastapi_simple_class_view-0.0.1/src/example/database.py` & `fastapi_simple_class_view-0.0.2/src/example/database.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_class_view-0.0.1/src/example/database.sqlite3` & `fastapi_simple_class_view-0.0.2/src/example/database.sqlite3`

 * *Files identical despite different names*

### Comparing `fastapi_simple_class_view-0.0.1/src/example/app/view.py` & `fastapi_simple_class_view-0.0.2/src/example/app/view.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_class_view-0.0.1/src/example/tests/test_users.py` & `fastapi_simple_class_view-0.0.2/src/example/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_class_view-0.0.1/src/fastapi_simple_class_view/abc.py` & `fastapi_simple_class_view-0.0.2/src/fastapi_simple_class_view/abc.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_class_view-0.0.1/src/fastapi_simple_class_view/base.py` & `fastapi_simple_class_view-0.0.2/src/fastapi_simple_class_view/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_class_view-0.0.1/src/fastapi_simple_class_view/controller.py` & `fastapi_simple_class_view-0.0.2/src/fastapi_simple_class_view/controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_class_view-0.0.1/src/fastapi_simple_class_view/meta.py` & `fastapi_simple_class_view-0.0.2/src/fastapi_simple_class_view/meta.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_class_view-0.0.1/src/fastapi_simple_class_view/mixins.py` & `fastapi_simple_class_view-0.0.2/src/fastapi_simple_class_view/mixins.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_class_view-0.0.1/.gitignore` & `fastapi_simple_class_view-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_simple_class_view-0.0.1/LICENSE` & `fastapi_simple_class_view-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_simple_class_view-0.0.1/README.md` & `fastapi_simple_class_view-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This package gives you convenient access for writing and maintaining class based
 controllers in FastAPI framework
 
 ## Install package
 
 ```shell
-pip install gspot-fastapi-auth
+pip install fastapi-simple-class-view
 ```
 
 ## Quickstart
 
 ### Typical app structure
 
 An example of a typical application structure, you can redefine it at your discretion
```

### Comparing `fastapi_simple_class_view-0.0.1/pyproject.toml` & `fastapi_simple_class_view-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_simple_class_view"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "gravity48", email = "gravity4849@gmail.com" },
 ]
 description = "Class based view for FastAPI"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `fastapi_simple_class_view-0.0.1/PKG-INFO` & `fastapi_simple_class_view-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_simple_class_view
-Version: 0.0.1
+Version: 0.0.2
 Summary: Class based view for FastAPI
 Project-URL: Homepage, https://github.com/gravity48/fastapi_class_view
 Project-URL: Bug Tracker, https://github.com/gravity48/fastapi_class_view/issues
 Author-email: gravity48 <gravity4849@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 
 This package gives you convenient access for writing and maintaining class based
 controllers in FastAPI framework
 
 ## Install package
 
 ```shell
-pip install gspot-fastapi-auth
+pip install fastapi-simple-class-view
 ```
 
 ## Quickstart
 
 ### Typical app structure
 
 An example of a typical application structure, you can redefine it at your discretion
```

