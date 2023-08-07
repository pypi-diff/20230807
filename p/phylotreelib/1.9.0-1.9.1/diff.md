# Comparing `tmp/phylotreelib-1.9.0.tar.gz` & `tmp/phylotreelib-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phylotreelib-1.9.0.tar", last modified: Thu Dec  8 21:20:37 2022, max compression
+gzip compressed data, was "phylotreelib-1.9.1.tar", last modified: Tue Dec 13 11:39:09 2022, max compression
```

## Comparing `phylotreelib-1.9.0.tar` & `phylotreelib-1.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2022-12-08 21:20:37.894236 phylotreelib-1.9.0/
--rw-r--r--   0 agpe       (502) staff       (20)    35149 2021-11-22 15:11:54.000000 phylotreelib-1.9.0/LICENSE
--rw-r--r--   0 agpe       (502) staff       (20)    47554 2022-12-08 21:20:37.894369 phylotreelib-1.9.0/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)    47084 2022-12-08 21:17:56.000000 phylotreelib-1.9.0/README.md
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2022-12-08 21:20:37.894121 phylotreelib-1.9.0/phylotreelib.egg-info/
--rw-r--r--   0 agpe       (502) staff       (20)    47554 2022-12-08 21:20:37.000000 phylotreelib-1.9.0/phylotreelib.egg-info/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)      237 2022-12-08 21:20:37.000000 phylotreelib-1.9.0/phylotreelib.egg-info/SOURCES.txt
--rw-r--r--   0 agpe       (502) staff       (20)        1 2022-12-08 21:20:37.000000 phylotreelib-1.9.0/phylotreelib.egg-info/dependency_links.txt
--rw-r--r--   0 agpe       (502) staff       (20)       26 2022-12-08 21:20:37.000000 phylotreelib-1.9.0/phylotreelib.egg-info/requires.txt
--rw-r--r--   0 agpe       (502) staff       (20)       13 2022-12-08 21:20:37.000000 phylotreelib-1.9.0/phylotreelib.egg-info/top_level.txt
--rw-r--r--   0 agpe       (502) staff       (20)   178066 2022-12-08 20:54:31.000000 phylotreelib-1.9.0/phylotreelib.py
--rw-r--r--   0 agpe       (502) staff       (20)      104 2021-11-24 21:14:07.000000 phylotreelib-1.9.0/pyproject.toml
--rw-r--r--   0 agpe       (502) staff       (20)      590 2022-12-08 21:20:37.894656 phylotreelib-1.9.0/setup.cfg
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2022-12-13 11:39:09.314632 phylotreelib-1.9.1/
+-rw-r--r--   0 agpe       (502) staff       (20)    35149 2021-11-22 15:11:54.000000 phylotreelib-1.9.1/LICENSE
+-rw-r--r--   0 agpe       (502) staff       (20)    47554 2022-12-13 11:39:09.314690 phylotreelib-1.9.1/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)    47084 2022-12-13 11:37:32.000000 phylotreelib-1.9.1/README.md
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2022-12-13 11:39:09.314514 phylotreelib-1.9.1/phylotreelib.egg-info/
+-rw-r--r--   0 agpe       (502) staff       (20)    47554 2022-12-13 11:39:09.000000 phylotreelib-1.9.1/phylotreelib.egg-info/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)      237 2022-12-13 11:39:09.000000 phylotreelib-1.9.1/phylotreelib.egg-info/SOURCES.txt
+-rw-r--r--   0 agpe       (502) staff       (20)        1 2022-12-13 11:39:09.000000 phylotreelib-1.9.1/phylotreelib.egg-info/dependency_links.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       26 2022-12-13 11:39:09.000000 phylotreelib-1.9.1/phylotreelib.egg-info/requires.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       13 2022-12-13 11:39:09.000000 phylotreelib-1.9.1/phylotreelib.egg-info/top_level.txt
+-rw-r--r--   0 agpe       (502) staff       (20)   178081 2022-12-13 11:16:29.000000 phylotreelib-1.9.1/phylotreelib.py
+-rw-r--r--   0 agpe       (502) staff       (20)      104 2021-11-24 21:14:07.000000 phylotreelib-1.9.1/pyproject.toml
+-rw-r--r--   0 agpe       (502) staff       (20)      590 2022-12-13 11:39:09.314952 phylotreelib-1.9.1/setup.cfg
```

### Comparing `phylotreelib-1.9.0/LICENSE` & `phylotreelib-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phylotreelib-1.9.0/PKG-INFO` & `phylotreelib-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: phylotreelib
-Version: 1.9.0
+Version: 1.9.1
 Summary: Analyze and manipulate phylogenetic trees
 Home-page: https://github.com/agormp/phylotreelib
 Author: Anders Gorm Pedersen
 Author-email: agpe@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # phylotreelib: python library for analyzing and manipulating phylogenetic trees
 
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/phylotreelib?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/phylotreelib)
-![](https://img.shields.io/badge/version-1.9.0-blue)
+![](https://img.shields.io/badge/version-1.9.1-blue)
 
 
 Using classes and methods in phylotreelib.py it is possible to read and write treefiles and to analyze and manipulate the trees in various ways.
 
 ![](https://github.com/agormp/phylotreelib/raw/main/treefig.png?raw=true)
 
 ## Availability
```

### Comparing `phylotreelib-1.9.0/README.md` & `phylotreelib-1.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # phylotreelib: python library for analyzing and manipulating phylogenetic trees
 
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/phylotreelib?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/phylotreelib)
-![](https://img.shields.io/badge/version-1.9.0-blue)
+![](https://img.shields.io/badge/version-1.9.1-blue)
 
 
 Using classes and methods in phylotreelib.py it is possible to read and write treefiles and to analyze and manipulate the trees in various ways.
 
 ![](https://github.com/agormp/phylotreelib/raw/main/treefig.png?raw=true)
 
 ## Availability
```

### Comparing `phylotreelib-1.9.0/phylotreelib.egg-info/PKG-INFO` & `phylotreelib-1.9.1/phylotreelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: phylotreelib
-Version: 1.9.0
+Version: 1.9.1
 Summary: Analyze and manipulate phylogenetic trees
 Home-page: https://github.com/agormp/phylotreelib
 Author: Anders Gorm Pedersen
 Author-email: agpe@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # phylotreelib: python library for analyzing and manipulating phylogenetic trees
 
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/phylotreelib?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/phylotreelib)
-![](https://img.shields.io/badge/version-1.9.0-blue)
+![](https://img.shields.io/badge/version-1.9.1-blue)
 
 
 Using classes and methods in phylotreelib.py it is possible to read and write treefiles and to analyze and manipulate the trees in various ways.
 
 ![](https://github.com/agormp/phylotreelib/raw/main/treefig.png?raw=true)
 
 ## Availability
```

### Comparing `phylotreelib-1.9.0/phylotreelib.py` & `phylotreelib-1.9.1/phylotreelib.py`

 * *Files 0% similar despite different names*

```diff
@@ -3822,21 +3822,22 @@
 
         return "".join(tmplist)
 
     #######################################################################################
 
     def clean_names(self, rep="_"):
         """Rename items to avoid characters that are problematic in Newick tree strings:
-        Replaces all occurrences of comma, colon, and semicolon, by 'rep'"""
+        Replaces all occurrences of ,:;()[] by 'rep'"""
 
         if self.namelist is None:
             raise TreeError("There are no items in Distmatrix object. Can not run clean_names()")
+        translation_table = "".maketrans(",:;()[]", rep * 7)
         old_new_tuples = []
         for old in self.namelist:
-            new = old.replace(",", rep).replace(":", rep).replace(";", rep)
+            new = old.translate(translation_table)
             old_new_tuples.append((old, new))
         for old,new in old_new_tuples:
             self.rename(old, new)
 
     #######################################################################################
 
     def rename(self, oldname, newname):
```

### Comparing `phylotreelib-1.9.0/setup.cfg` & `phylotreelib-1.9.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phylotreelib
-version = 1.9.0
+version = 1.9.1
 author = Anders Gorm Pedersen
 author_email = agpe@dtu.dk
 description = Analyze and manipulate phylogenetic trees
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/agormp/phylotreelib
 classifiers =
```

