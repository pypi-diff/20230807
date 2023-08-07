# Comparing `tmp/pyspkio-0.0.1.tar.gz` & `tmp/pyspkio-0.0.2.tar.gz`

## Comparing `pyspkio-0.0.1.tar` & `pyspkio-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyspkio-0.0.1/src/pyspkio/__init__.py
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 pyspkio-0.0.1/src/pyspkio/pyspkio.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyspkio-0.0.1/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyspkio-0.0.1/LICENSE
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pyspkio-0.0.1/README.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 pyspkio-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pyspkio-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyspkio-0.0.2/src/pyspkio/__init__.py
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 pyspkio-0.0.2/src/pyspkio/spkio.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 pyspkio-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyspkio-0.0.2/LICENSE
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pyspkio-0.0.2/README.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pyspkio-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pyspkio-0.0.2/PKG-INFO
```

### Comparing `pyspkio-0.0.1/src/pyspkio/pyspkio.py` & `pyspkio-0.0.2/src/pyspkio/spkio.py`

 * *Files identical despite different names*

### Comparing `pyspkio-0.0.1/.gitignore` & `pyspkio-0.0.2/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+token.txt
```

### Comparing `pyspkio-0.0.1/LICENSE` & `pyspkio-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspkio-0.0.1/pyproject.toml` & `pyspkio-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyspkio"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
-  { name="Spkio", email="spkio@spk.io" },
+  { name="Spkio", email="spkio@proton.me" },
 ]
 description = "Python framework to connect Spkio Server"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

