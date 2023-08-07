# Comparing `tmp/gedcom5-0.1.1.tar.gz` & `tmp/gedcom5-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gedcom5-0.1.1.tar", last modified: Sun Aug  6 02:55:30 2023, max compression
+gzip compressed data, was "gedcom5-0.1.2.tar", last modified: Mon Aug  7 02:23:30 2023, max compression
```

## Comparing `gedcom5-0.1.1.tar` & `gedcom5-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-06 02:55:30.031176 gedcom5-0.1.1/
--rw-r--r--   0 david     (1000) david     (1000)     1074 2023-08-06 02:53:40.000000 gedcom5-0.1.1/LICENSE.txt
--rw-r--r--   0 david     (1000) david     (1000)     1947 2023-08-06 02:55:30.031176 gedcom5-0.1.1/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      155 2023-08-06 01:00:42.000000 gedcom5-0.1.1/README.md
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-06 02:55:30.031176 gedcom5-0.1.1/gedcom5/
--rw-r--r--   0 david     (1000) david     (1000)     2256 2023-08-06 00:56:42.000000 gedcom5-0.1.1/gedcom5/__init__.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-06 02:55:30.031176 gedcom5-0.1.1/gedcom5.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)     1947 2023-08-06 02:55:30.000000 gedcom5-0.1.1/gedcom5.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      202 2023-08-06 02:55:30.000000 gedcom5-0.1.1/gedcom5.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-08-06 02:55:30.000000 gedcom5-0.1.1/gedcom5.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)        8 2023-08-06 02:55:30.000000 gedcom5-0.1.1/gedcom5.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)      778 2023-08-06 02:53:40.000000 gedcom5-0.1.1/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)       38 2023-08-06 02:55:30.031176 gedcom5-0.1.1/setup.cfg
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-06 02:55:30.031176 gedcom5-0.1.1/tests/
--rw-r--r--   0 david     (1000) david     (1000)      621 2023-08-06 00:57:46.000000 gedcom5-0.1.1/tests/test_gedcom5.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-07 02:23:30.720021 gedcom5-0.1.2/
+-rw-r--r--   0 david     (1000) david     (1000)     1074 2023-08-06 02:53:40.000000 gedcom5-0.1.2/LICENSE.txt
+-rw-r--r--   0 david     (1000) david     (1000)     1947 2023-08-07 02:23:30.720021 gedcom5-0.1.2/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      155 2023-08-06 01:00:42.000000 gedcom5-0.1.2/README.md
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-07 02:23:30.719021 gedcom5-0.1.2/gedcom5/
+-rw-r--r--   0 david     (1000) david     (1000)     2396 2023-08-07 02:22:24.000000 gedcom5-0.1.2/gedcom5/__init__.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-07 02:23:30.720021 gedcom5-0.1.2/gedcom5.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)     1947 2023-08-07 02:23:30.000000 gedcom5-0.1.2/gedcom5.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      202 2023-08-07 02:23:30.000000 gedcom5-0.1.2/gedcom5.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-08-07 02:23:30.000000 gedcom5-0.1.2/gedcom5.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)        8 2023-08-07 02:23:30.000000 gedcom5-0.1.2/gedcom5.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)      778 2023-08-07 02:22:24.000000 gedcom5-0.1.2/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)       38 2023-08-07 02:23:30.720021 gedcom5-0.1.2/setup.cfg
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-08-07 02:23:30.720021 gedcom5-0.1.2/tests/
+-rw-r--r--   0 david     (1000) david     (1000)      621 2023-08-06 00:57:46.000000 gedcom5-0.1.2/tests/test_gedcom5.py
```

### Comparing `gedcom5-0.1.1/LICENSE.txt` & `gedcom5-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gedcom5-0.1.1/PKG-INFO` & `gedcom5-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gedcom5
-Version: 0.1.1
+Version: 0.1.2
 Summary: GEDCOM v5 parser
 Author-email: David <c0d3@gpobox.net>
 Maintainer-email: David <c0d3@gpobox.net>
 License: Copyright © 2023 David <c0d3@gpobox.net>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the “Software”), to deal in the Software without restriction,
```

### Comparing `gedcom5-0.1.1/gedcom5/__init__.py` & `gedcom5-0.1.2/gedcom5/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,20 @@
 
     def find(self, tags):
         nodes = [self]
         for tag in tags.split('.'):
             nodes = [item for node in nodes for item in node.items if item.tag == tag]
         return nodes
 
+    def find_first(self, tags):
+        nodes = self.find(tags)
+        if len(nodes) > 0:
+            return nodes[0]
+        return None
+
     def __getitem__(self, item):
         return self.items[item]
 
 
 class Entry(GEDCOM):
     def __init__(self, level: int, xref_id: str = None, tag: str = None, value: str = None):
         super().__init__(level=level)
```

### Comparing `gedcom5-0.1.1/gedcom5.egg-info/PKG-INFO` & `gedcom5-0.1.2/gedcom5.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gedcom5
-Version: 0.1.1
+Version: 0.1.2
 Summary: GEDCOM v5 parser
 Author-email: David <c0d3@gpobox.net>
 Maintainer-email: David <c0d3@gpobox.net>
 License: Copyright © 2023 David <c0d3@gpobox.net>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the “Software”), to deal in the Software without restriction,
```

### Comparing `gedcom5-0.1.1/pyproject.toml` & `gedcom5-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gedcom5"
-version = "0.1.1"
+version = "0.1.2"
 description = "GEDCOM v5 parser"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 requires-python = ">=3.11"
 dependencies = []
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `gedcom5-0.1.1/tests/test_gedcom5.py` & `gedcom5-0.1.2/tests/test_gedcom5.py`

 * *Files identical despite different names*

