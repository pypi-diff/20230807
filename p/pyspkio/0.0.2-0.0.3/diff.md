# Comparing `tmp/pyspkio-0.0.2.tar.gz` & `tmp/pyspkio-0.0.3.tar.gz`

## Comparing `pyspkio-0.0.2.tar` & `pyspkio-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyspkio-0.0.2/src/pyspkio/__init__.py
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 pyspkio-0.0.2/src/pyspkio/spkio.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 pyspkio-0.0.2/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyspkio-0.0.2/LICENSE
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pyspkio-0.0.2/README.md
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pyspkio-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pyspkio-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyspkio-0.0.3/src/pyspkio/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pyspkio-0.0.3/src/pyspkio/example.py
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 pyspkio-0.0.3/src/pyspkio/spkio.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 pyspkio-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyspkio-0.0.3/LICENSE
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pyspkio-0.0.3/README.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pyspkio-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pyspkio-0.0.3/PKG-INFO
```

### Comparing `pyspkio-0.0.2/src/pyspkio/spkio.py` & `pyspkio-0.0.3/src/pyspkio/spkio.py`

 * *Files identical despite different names*

### Comparing `pyspkio-0.0.2/.gitignore` & `pyspkio-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyspkio-0.0.2/LICENSE` & `pyspkio-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspkio-0.0.2/pyproject.toml` & `pyspkio-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyspkio"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Spkio", email="spkio@proton.me" },
 ]
 description = "Python framework to connect Spkio Server"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

