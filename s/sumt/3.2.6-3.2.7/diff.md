# Comparing `tmp/sumt-3.2.6.tar.gz` & `tmp/sumt-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumt-3.2.6.tar", last modified: Mon Aug  7 11:27:28 2023, max compression
+gzip compressed data, was "sumt-3.2.7.tar", last modified: Mon Aug  7 12:06:45 2023, max compression
```

## Comparing `sumt-3.2.6.tar` & `sumt-3.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-08-07 11:27:28.829062 sumt-3.2.6/
--rw-r--r--   0 agpe       (502) staff       (20)    35149 2022-02-20 16:31:26.000000 sumt-3.2.6/LICENSE
--rw-r--r--   0 agpe       (502) staff       (20)    21313 2023-08-07 11:27:28.829369 sumt-3.2.6/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)    20838 2023-08-07 11:26:56.000000 sumt-3.2.6/README.md
--rw-r--r--   0 agpe       (502) staff       (20)      104 2021-11-24 21:14:07.000000 sumt-3.2.6/pyproject.toml
--rw-r--r--   0 agpe       (502) staff       (20)      650 2023-08-07 11:27:28.830198 sumt-3.2.6/setup.cfg
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-08-07 11:27:28.828728 sumt-3.2.6/sumt.egg-info/
--rw-r--r--   0 agpe       (502) staff       (20)    21313 2023-08-07 11:27:28.000000 sumt-3.2.6/sumt.egg-info/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)      220 2023-08-07 11:27:28.000000 sumt-3.2.6/sumt.egg-info/SOURCES.txt
--rw-r--r--   0 agpe       (502) staff       (20)        1 2023-08-07 11:27:28.000000 sumt-3.2.6/sumt.egg-info/dependency_links.txt
--rw-r--r--   0 agpe       (502) staff       (20)       35 2023-08-07 11:27:28.000000 sumt-3.2.6/sumt.egg-info/entry_points.txt
--rw-r--r--   0 agpe       (502) staff       (20)       28 2023-08-07 11:27:28.000000 sumt-3.2.6/sumt.egg-info/requires.txt
--rw-r--r--   0 agpe       (502) staff       (20)        5 2023-08-07 11:27:28.000000 sumt-3.2.6/sumt.egg-info/top_level.txt
--rwxr-xr-x   0 agpe       (502) staff       (20)    32052 2023-08-07 11:07:59.000000 sumt-3.2.6/sumt.py
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-08-07 12:06:45.357507 sumt-3.2.7/
+-rw-r--r--   0 agpe       (502) staff       (20)    35149 2022-02-20 16:31:26.000000 sumt-3.2.7/LICENSE
+-rw-r--r--   0 agpe       (502) staff       (20)    21313 2023-08-07 12:06:45.357595 sumt-3.2.7/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)    20838 2023-08-07 12:05:09.000000 sumt-3.2.7/README.md
+-rw-r--r--   0 agpe       (502) staff       (20)      104 2021-11-24 21:14:07.000000 sumt-3.2.7/pyproject.toml
+-rw-r--r--   0 agpe       (502) staff       (20)      650 2023-08-07 12:06:45.357916 sumt-3.2.7/setup.cfg
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-08-07 12:06:45.357397 sumt-3.2.7/sumt.egg-info/
+-rw-r--r--   0 agpe       (502) staff       (20)    21313 2023-08-07 12:06:45.000000 sumt-3.2.7/sumt.egg-info/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)      220 2023-08-07 12:06:45.000000 sumt-3.2.7/sumt.egg-info/SOURCES.txt
+-rw-r--r--   0 agpe       (502) staff       (20)        1 2023-08-07 12:06:45.000000 sumt-3.2.7/sumt.egg-info/dependency_links.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       35 2023-08-07 12:06:45.000000 sumt-3.2.7/sumt.egg-info/entry_points.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       28 2023-08-07 12:06:45.000000 sumt-3.2.7/sumt.egg-info/requires.txt
+-rw-r--r--   0 agpe       (502) staff       (20)        5 2023-08-07 12:06:45.000000 sumt-3.2.7/sumt.egg-info/top_level.txt
+-rwxr-xr-x   0 agpe       (502) staff       (20)    31981 2023-08-07 12:06:05.000000 sumt-3.2.7/sumt.py
```

### Comparing `sumt-3.2.6/LICENSE` & `sumt-3.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sumt-3.2.6/PKG-INFO` & `sumt-3.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sumt
-Version: 3.2.6
+Version: 3.2.7
 Summary: Computes consensus trees and other phylogenetic tree summaries
 Home-page: https://github.com/agormp/sumt
 Author: Anders Gorm Pedersen
 Author-email: agpe@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sumt
 
-![](https://img.shields.io/badge/version-3.2.6-blue)
+![](https://img.shields.io/badge/version-3.2.7-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=PyPI%20downloads&service=github)](https://pepy.tech/project/sumt)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute three different kinds of main tree summaries:
 
 * Majority rule consensus tree
```

### Comparing `sumt-3.2.6/README.md` & `sumt-3.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # sumt
 
-![](https://img.shields.io/badge/version-3.2.6-blue)
+![](https://img.shields.io/badge/version-3.2.7-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=PyPI%20downloads&service=github)](https://pepy.tech/project/sumt)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute three different kinds of main tree summaries:
 
 * Majority rule consensus tree
```

### Comparing `sumt-3.2.6/setup.cfg` & `sumt-3.2.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sumt
-version = 3.2.6
+version = 3.2.7
 author = Anders Gorm Pedersen
 author_email = agpe@dtu.dk
 description = Computes consensus trees and other phylogenetic tree summaries
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/agormp/sumt
 classifiers =
```

### Comparing `sumt-3.2.6/sumt.egg-info/PKG-INFO` & `sumt-3.2.7/sumt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sumt
-Version: 3.2.6
+Version: 3.2.7
 Summary: Computes consensus trees and other phylogenetic tree summaries
 Home-page: https://github.com/agormp/sumt
 Author: Anders Gorm Pedersen
 Author-email: agpe@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sumt
 
-![](https://img.shields.io/badge/version-3.2.6-blue)
+![](https://img.shields.io/badge/version-3.2.7-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=PyPI%20downloads&service=github)](https://pepy.tech/project/sumt)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute three different kinds of main tree summaries:
 
 * Majority rule consensus tree
```

### Comparing `sumt-3.2.6/sumt.py` & `sumt-3.2.7/sumt.py`

 * *Files 1% similar despite different names*

```diff
@@ -712,10 +712,8 @@
 
     return toporeport
 
 ##########################################################################################
 ##########################################################################################
 
 if __name__ == "__main__":
-    # main()
-    import cProfile
-    cProfile.run('main()', 'tmp/profile.pstats')
+    main()
```

