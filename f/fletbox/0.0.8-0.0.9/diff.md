# Comparing `tmp/fletbox-0.0.8.tar.gz` & `tmp/fletbox-0.0.9.tar.gz`

## Comparing `fletbox-0.0.8.tar` & `fletbox-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fletbox-0.0.8/requirements.txt
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fletbox-0.0.8/src/setup.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 fletbox-0.0.8/src/fletbox/__init__.py
--rw-r--r--   0        0        0     7826 2020-02-02 00:00:00.000000 fletbox-0.0.8/src/fletbox/fletbox.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fletbox-0.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fletbox-0.0.8/LICENSE
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fletbox-0.0.8/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fletbox-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 fletbox-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fletbox-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fletbox-0.0.9/src/setup.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 fletbox-0.0.9/src/fletbox/__init__.py
+-rw-r--r--   0        0        0     7826 2020-02-02 00:00:00.000000 fletbox-0.0.9/src/fletbox/fletbox.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fletbox-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fletbox-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fletbox-0.0.9/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 fletbox-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 fletbox-0.0.9/PKG-INFO
```

### Comparing `fletbox-0.0.8/src/fletbox/fletbox.py` & `fletbox-0.0.9/src/fletbox/fletbox.py`

 * *Files identical despite different names*

### Comparing `fletbox-0.0.8/LICENSE` & `fletbox-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fletbox-0.0.8/README.md` & `fletbox-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fletbox-0.0.8/pyproject.toml` & `fletbox-0.0.9/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fletbox"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Xynon", email="" },
 ]
 description = "A box for flet, abusing contextmanagers and decorators"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha"
 ]
 dynamic = ["dependencies"]
 
-# [project.urls]
-# "Homepage" = ""
-# "Bug Tracker" = ""
+[project.urls]
+"Homepage" = "https://github.com/Xynonners/fletbox"
+"Bug Tracker" = "https://github.com/Xynonners/fletbox/issues"
 
 [tool.hatch.metadata.hooks.requirements_txt]
 files = ["requirements.txt"]
```

### Comparing `fletbox-0.0.8/PKG-INFO` & `fletbox-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: fletbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: A box for flet, abusing contextmanagers and decorators
+Project-URL: Homepage, https://github.com/Xynonners/fletbox
+Project-URL: Bug Tracker, https://github.com/Xynonners/fletbox/issues
 Author: Xynon
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

