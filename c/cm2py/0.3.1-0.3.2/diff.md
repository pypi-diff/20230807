# Comparing `tmp/cm2py-0.3.1.tar.gz` & `tmp/cm2py-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm2py-0.3.1.tar", last modified: Wed Aug  2 07:21:19 2023, max compression
+gzip compressed data, was "cm2py-0.3.2.tar", last modified: Mon Aug  7 09:33:11 2023, max compression
```

## Comparing `cm2py-0.3.1.tar` & `cm2py-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 07:21:19.448405 cm2py-0.3.1/
--rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     3012 2023-08-02 07:21:19.447399 cm2py-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1189 2023-07-15 07:50:59.000000 cm2py-0.3.1/README.md
--rw-rw-rw-   0        0        0      675 2023-08-02 07:20:31.000000 cm2py-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-02 07:21:19.448405 cm2py-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-02 07:21:19.369396 cm2py-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-02 07:21:19.388400 cm2py-0.3.1/src/cm2py/
--rw-rw-rw-   0        0        0      237 2023-07-25 10:54:54.000000 cm2py-0.3.1/src/cm2py/__init__.py
--rw-rw-rw-   0        0        0     6585 2023-08-02 07:20:33.000000 cm2py-0.3.1/src/cm2py/cm2py.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:21:19.432397 cm2py-0.3.1/src/cm2py.egg-info/
--rw-rw-rw-   0        0        0     3012 2023-08-02 07:21:19.000000 cm2py-0.3.1/src/cm2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-08-02 07:21:19.000000 cm2py-0.3.1/src/cm2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 07:21:19.000000 cm2py-0.3.1/src/cm2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-08-02 07:21:19.000000 cm2py-0.3.1/src/cm2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-02 07:21:19.000000 cm2py-0.3.1/src/cm2py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 07:21:19.444404 cm2py-0.3.1/tests/
--rw-rw-rw-   0        0        0     2521 2023-08-02 05:26:24.000000 cm2py-0.3.1/tests/test_app.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:33:11.751461 cm2py-0.3.2/
+-rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     3012 2023-08-07 09:33:11.749466 cm2py-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1189 2023-07-15 07:50:59.000000 cm2py-0.3.2/README.md
+-rw-rw-rw-   0        0        0      687 2023-08-07 09:30:19.000000 cm2py-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 09:33:11.752465 cm2py-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 09:33:11.399460 cm2py-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 09:33:11.681461 cm2py-0.3.2/src/cm2py/
+-rw-rw-rw-   0        0        0      237 2023-07-25 10:54:54.000000 cm2py-0.3.2/src/cm2py/__init__.py
+-rw-rw-rw-   0        0        0     6592 2023-08-07 09:30:19.000000 cm2py-0.3.2/src/cm2py/cm2py.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:33:11.737460 cm2py-0.3.2/src/cm2py.egg-info/
+-rw-rw-rw-   0        0        0     3012 2023-08-07 09:33:11.000000 cm2py-0.3.2/src/cm2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-08-07 09:33:11.000000 cm2py-0.3.2/src/cm2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 09:33:11.000000 cm2py-0.3.2/src/cm2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-07 09:33:11.000000 cm2py-0.3.2/src/cm2py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-07 09:33:11.000000 cm2py-0.3.2/src/cm2py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 09:33:11.743464 cm2py-0.3.2/tests/
+-rw-rw-rw-   0        0        0     2521 2023-08-02 05:26:24.000000 cm2py-0.3.2/tests/test_app.py
```

### Comparing `cm2py-0.3.1/LICENSE` & `cm2py-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cm2py-0.3.1/PKG-INFO` & `cm2py-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.3.1
+Version: 0.3.2
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cm2py-0.3.1/README.md` & `cm2py-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cm2py-0.3.1/pyproject.toml` & `cm2py-0.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cm2py"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="SKM GEEK", email="qestudios17@gmail.com" },
 ]
 description = "Circuit Maker 2 save generation and manipulation package"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "uuid"
+  "uuid",
+  "regex"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/QEStudios/cm2py"
 "Bug Tracker" = "https://github.com/QEStudios/cm2py/issues"
```

### Comparing `cm2py-0.3.1/src/cm2py/cm2py.py` & `cm2py-0.3.2/src/cm2py/cm2py.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 """
 
 __author__ = "SKM GEEK"
 __contact__ = "qestudios17@gmail.com"
 __copyright__ = "Copyright 2023, SKM GEEK"
 __date__ = "2023/05/21"
 __deprecated__ = False
-__email__ = "qestudios17@example.com"
+__email__ = "qestudios17@gmail.com"
 __license__ = "MIT"
 __maintainer__ = "SKM GEEK"
 __status__ = "Production"
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
-import re
+import regex as re
 from uuid import UUID, uuid4
 import math
 
 
 class Save:
     """A class to represent a save, which can be modified."""
```

### Comparing `cm2py-0.3.1/src/cm2py.egg-info/PKG-INFO` & `cm2py-0.3.2/src/cm2py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.3.1
+Version: 0.3.2
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cm2py-0.3.1/tests/test_app.py` & `cm2py-0.3.2/tests/test_app.py`

 * *Files identical despite different names*

