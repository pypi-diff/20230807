# Comparing `tmp/genefeast-0.0.8.tar.gz` & `tmp/genefeast-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/avigailtaylor/Projects/GeneFEAST/genefeast/dist/tmp2oot8tm_/genefeast-0.0.8.tar", last modified: Tue Oct 18 20:38:51 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `genefeast-0.0.8.tar` & `genefeast-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 avigailtaylor   (503) staff       (20)        0 2022-10-18 20:38:51.000000 genefeast-0.0.8/
--rw-r--r--   0 avigailtaylor   (503) staff       (20)     1617 2022-09-15 16:37:56.000000 genefeast-0.0.8/LICENSE
--rw-r--r--   0 avigailtaylor   (503) staff       (20)       64 2022-10-18 17:02:07.000000 genefeast-0.0.8/MANIFEST.in
--rw-r--r--   0 avigailtaylor   (503) staff       (20)     1545 2022-10-18 20:38:51.000000 genefeast-0.0.8/PKG-INFO
--rw-r--r--   0 avigailtaylor   (503) staff       (20)      991 2022-10-17 13:36:27.000000 genefeast-0.0.8/README.md
-drwxr-xr-x   0 avigailtaylor   (503) staff       (20)        0 2022-10-18 20:38:51.000000 genefeast-0.0.8/genefeast/
-drwxr-xr-x   0 avigailtaylor   (503) staff       (20)        0 2022-10-18 20:38:51.000000 genefeast-0.0.8/genefeast/genefeast.egg-info/
--rw-r--r--   0 avigailtaylor   (503) staff       (20)     1545 2022-10-18 20:38:51.000000 genefeast-0.0.8/genefeast/genefeast.egg-info/PKG-INFO
--rw-r--r--   0 avigailtaylor   (503) staff       (20)      317 2022-10-18 20:38:51.000000 genefeast-0.0.8/genefeast/genefeast.egg-info/SOURCES.txt
--rw-r--r--   0 avigailtaylor   (503) staff       (20)        1 2022-10-18 20:38:51.000000 genefeast-0.0.8/genefeast/genefeast.egg-info/dependency_links.txt
--rw-r--r--   0 avigailtaylor   (503) staff       (20)      160 2022-10-18 20:38:51.000000 genefeast-0.0.8/genefeast/genefeast.egg-info/requires.txt
--rw-r--r--   0 avigailtaylor   (503) staff       (20)        1 2022-10-18 20:38:51.000000 genefeast-0.0.8/genefeast/genefeast.egg-info/top_level.txt
--rw-r--r--   0 avigailtaylor   (503) staff       (20) 30968209 2022-09-15 16:42:19.000000 genefeast-0.0.8/genefeast/go-basic.obo
--rw-r--r--   0 avigailtaylor   (503) staff       (20) 38550989 2022-09-15 16:42:26.000000 genefeast-0.0.8/genefeast/msigdb_v7.2.filtered.html
--rw-r--r--   0 avigailtaylor   (503) staff       (20)     1000 2022-10-18 20:34:46.000000 genefeast-0.0.8/pyproject.toml
--rw-r--r--   0 avigailtaylor   (503) staff       (20)       38 2022-10-18 20:38:51.000000 genefeast-0.0.8/setup.cfg
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 genefeast-0.0.9/.DS_Store
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 genefeast-0.0.9/MANIFEST.in
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 genefeast-0.0.9/genefeast/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 genefeast-0.0.9/genefeast/__init.py__
+-rw-r--r--   0        0        0    16874 2020-02-02 00:00:00.000000 genefeast-0.0.9/genefeast/gf.py
+-rw-r--r--   0        0        0    39211 2020-02-02 00:00:00.000000 genefeast-0.0.9/genefeast/gf_base.py
+-rw-r--r--   0        0        0   134085 2020-02-02 00:00:00.000000 genefeast-0.0.9/genefeast/gf_classes.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 genefeast-0.0.9/genefeast/gf_config.py
+-rw-r--r--   0        0        0    17905 2020-02-02 00:00:00.000000 genefeast-0.0.9/genefeast/gf_multi.py
+-rw-r--r--   0        0        0 30968209 2020-02-02 00:00:00.000000 genefeast-0.0.9/genefeast/go-basic.obo
+-rw-r--r--   0        0        0 38550989 2020-02-02 00:00:00.000000 genefeast-0.0.9/genefeast/msigdb_v7.2.filtered.html
+-rw-r--r--   0        0        0   716099 2020-02-02 00:00:00.000000 genefeast-0.0.9/tests/test_gf_base.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 genefeast-0.0.9/LICENSE
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 genefeast-0.0.9/README.md
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 genefeast-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 genefeast-0.0.9/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `genefeast-0.0.8/LICENSE` & `genefeast-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `genefeast-0.0.8/PKG-INFO` & `genefeast-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: genefeast
-Version: 0.0.8
+Version: 0.0.9
 Summary: Gene-centric functional enrichment analysis summarisation tool
-Author-email: Avigail Taylor <avigail.taylor@well.ox.ac.uk>
 Project-URL: Homepage, https://avigailtaylor.github.io/GeneFEAST/
 Project-URL: Source Code, https://github.com/avigailtaylor/GeneFEAST
-Classifier: Programming Language :: Python :: 3.7
+Author-email: Avigail Taylor <avigail.taylor@well.ox.ac.uk>
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
+Requires-Dist: beautifulsoup4==4.8.0
+Requires-Dist: goatools==1.0.14
+Requires-Dist: matplotlib==3.3.3
+Requires-Dist: networkx==2.5
+Requires-Dist: numpy==1.17.2
+Requires-Dist: pandas==0.25.1
+Requires-Dist: pillow==6.2.0
+Requires-Dist: scipy==1.3.2
+Requires-Dist: seaborn==0.11.2
+Requires-Dist: upsetplot==0.4.1
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # GeneFEAST
 
 GeneFEAST, implemented in Python, is a gene-centric functional enrichment analysis summarisation and visualisation tool that can be applied to large functional enrichment analysis (FEA) results arising from any upstream FEA pipeline. It produces a systematic, navigable HTML report, making it easy to identify sets of genes putatively driving multiple enrichments and to explore gene-level quantitative data first used to identify input genes. Further, GeneFEAST can compare FEA results from multiple studies, making it possible to, for example, highlight patterns of gene expression amongst genes commonly differentially expressed in two sets of conditions, and giving rise to shared enrichments under those conditions. GeneFEAST offers a novel, effective way to address the complexities of linking up many, overlapping FEA results to their underlying genes and data; advancing gene-centric hypotheses, and providing pivotal information for downstream validation experiments.
```

### Comparing `genefeast-0.0.8/README.md` & `genefeast-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `genefeast-0.0.8/genefeast/go-basic.obo` & `genefeast-0.0.9/genefeast/go-basic.obo`

 * *Files identical despite different names*

### Comparing `genefeast-0.0.8/genefeast/msigdb_v7.2.filtered.html` & `genefeast-0.0.9/genefeast/msigdb_v7.2.filtered.html`

 * *Files identical despite different names*

### Comparing `genefeast-0.0.8/pyproject.toml` & `genefeast-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "genefeast"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Avigail Taylor", email="avigail.taylor@well.ox.ac.uk" },
 ]
 description = "Gene-centric functional enrichment analysis summarisation tool"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -32,10 +32,13 @@
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["genefeast"]
 
+[tool.setuptools.package-data]
+genefeast = ["*.obo", "*.html"]
+
 [project.urls]
 "Homepage" = "https://avigailtaylor.github.io/GeneFEAST/"
 "Source Code" = "https://github.com/avigailtaylor/GeneFEAST"
```

