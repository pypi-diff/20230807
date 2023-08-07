# Comparing `tmp/scoda-tk-0.4.8.tar.gz` & `tmp/scoda-tk-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.4.8.tar", last modified: Sun Aug  6 17:21:16 2023, max compression
+gzip compressed data, was "scoda-tk-0.4.9.tar", last modified: Mon Aug  7 05:40:28 2023, max compression
```

## Comparing `scoda-tk-0.4.8.tar` & `scoda-tk-0.4.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 17:21:16.939525 scoda-tk-0.4.8/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-04 16:51:18.000000 scoda-tk-0.4.8/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-04 16:51:18.000000 scoda-tk-0.4.8/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 17:21:16.939525 scoda-tk-0.4.8/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-04 16:51:24.000000 scoda-tk-0.4.8/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-06 17:20:36.000000 scoda-tk-0.4.8/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-06 17:21:16.939525 scoda-tk-0.4.8/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-04 16:51:18.000000 scoda-tk-0.4.8/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 17:21:16.915525 scoda-tk-0.4.8/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 17:21:16.915525 scoda-tk-0.4.8/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-04 16:51:24.000000 scoda-tk-0.4.8/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31646 2023-08-06 14:32:11.000000 scoda-tk-0.4.8/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 17:21:16.935525 scoda-tk-0.4.8/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-04 16:51:21.000000 scoda-tk-0.4.8/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-04 16:51:23.000000 scoda-tk-0.4.8/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-04 16:51:23.000000 scoda-tk-0.4.8/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-04 16:51:22.000000 scoda-tk-0.4.8/src/scoda/default_optional_files/kegg_human.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-04 16:51:23.000000 scoda-tk-0.4.8/src/scoda/default_optional_files/kegg_mouse.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-04 16:51:21.000000 scoda-tk-0.4.8/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-04 16:51:20.000000 scoda-tk-0.4.8/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-04 16:51:24.000000 scoda-tk-0.4.8/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-04 16:51:22.000000 scoda-tk-0.4.8/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17013 2023-08-06 13:08:04.000000 scoda-tk-0.4.8/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    14381 2023-08-06 13:11:44.000000 scoda-tk-0.4.8/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-04 16:51:20.000000 scoda-tk-0.4.8/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37583 2023-08-06 15:14:11.000000 scoda-tk-0.4.8/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31437 2023-08-06 13:15:03.000000 scoda-tk-0.4.8/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    25990 2023-08-06 15:28:05.000000 scoda-tk-0.4.8/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    65416 2023-08-06 17:20:19.000000 scoda-tk-0.4.8/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 17:21:16.939525 scoda-tk-0.4.8/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 17:21:16.000000 scoda-tk-0.4.8/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-06 17:21:16.000000 scoda-tk-0.4.8/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-06 17:21:16.000000 scoda-tk-0.4.8/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-06 17:21:16.000000 scoda-tk-0.4.8/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-06 17:21:16.000000 scoda-tk-0.4.8/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-06 17:21:16.000000 scoda-tk-0.4.8/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-07 05:40:28.544602 scoda-tk-0.4.9/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-04 16:51:18.000000 scoda-tk-0.4.9/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-04 16:51:18.000000 scoda-tk-0.4.9/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-07 05:40:28.544602 scoda-tk-0.4.9/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-04 16:51:24.000000 scoda-tk-0.4.9/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-07 05:40:03.000000 scoda-tk-0.4.9/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-07 05:40:28.544602 scoda-tk-0.4.9/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-04 16:51:18.000000 scoda-tk-0.4.9/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-07 05:40:28.404605 scoda-tk-0.4.9/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-07 05:40:28.432604 scoda-tk-0.4.9/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-04 16:51:24.000000 scoda-tk-0.4.9/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31646 2023-08-06 14:32:11.000000 scoda-tk-0.4.9/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-07 05:40:28.540602 scoda-tk-0.4.9/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-04 16:51:21.000000 scoda-tk-0.4.9/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-04 16:51:23.000000 scoda-tk-0.4.9/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-04 16:51:23.000000 scoda-tk-0.4.9/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-04 16:51:22.000000 scoda-tk-0.4.9/src/scoda/default_optional_files/kegg_human.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-04 16:51:23.000000 scoda-tk-0.4.9/src/scoda/default_optional_files/kegg_mouse.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-04 16:51:21.000000 scoda-tk-0.4.9/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-04 16:51:20.000000 scoda-tk-0.4.9/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-04 16:51:24.000000 scoda-tk-0.4.9/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-04 16:51:22.000000 scoda-tk-0.4.9/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17013 2023-08-06 13:08:04.000000 scoda-tk-0.4.9/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    14381 2023-08-06 13:11:44.000000 scoda-tk-0.4.9/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-04 16:51:20.000000 scoda-tk-0.4.9/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37639 2023-08-07 05:39:47.000000 scoda-tk-0.4.9/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31437 2023-08-06 13:15:03.000000 scoda-tk-0.4.9/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    25990 2023-08-06 15:28:05.000000 scoda-tk-0.4.9/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    65416 2023-08-06 17:20:19.000000 scoda-tk-0.4.9/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-07 05:40:28.540602 scoda-tk-0.4.9/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-07 05:40:28.000000 scoda-tk-0.4.9/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-07 05:40:28.000000 scoda-tk-0.4.9/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-07 05:40:28.000000 scoda-tk-0.4.9/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-07 05:40:28.000000 scoda-tk-0.4.9/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-07 05:40:28.000000 scoda-tk-0.4.9/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-07 05:40:28.000000 scoda-tk-0.4.9/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.4.8/LICENSE` & `scoda-tk-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/PKG-INFO` & `scoda-tk-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.4.8
+Version: 0.4.9
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.4.8/pyproject.toml` & `scoda-tk-0.4.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.4.8"
+version = "0.4.9"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.4.8/src/scoda/cpdb.py` & `scoda-tk-0.4.9/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.4.9/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.4.9/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda/default_optional_files/kegg_human.gmt` & `scoda-tk-0.4.9/src/scoda/default_optional_files/kegg_human.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda/default_optional_files/kegg_mouse.gmt` & `scoda-tk-0.4.9/src/scoda/default_optional_files/kegg_mouse.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.4.9/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.4.9/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.4.9/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.4.9/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda/deg.py` & `scoda-tk-0.4.9/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda/gsea.py` & `scoda-tk-0.4.9/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda/hicat.py` & `scoda-tk-0.4.9/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda/icnv.py` & `scoda-tk-0.4.9/src/scoda/icnv.py`

 * *Files 0% similar despite different names*

```diff
@@ -843,16 +843,17 @@
         adj = kneighbors_graph(X_vec, int(n_neighbors), mode = 'connectivity', 
                                include_self=True, n_jobs = n_cores)
     
     etime = round(time.time() - start_time) 
     print('C(%i, Nc:%i) .. ' % (etime, N_clusters), end = '', flush = True)
     start_time = time.time()
     
+    cnv_clust_lst = list(set(y_clust))
     ## Compute Cluster size, Aggregated Adj.Mat and Merge Small clusters 
-    for kk in range(2):
+    for kk in range(len(cnv_clust_lst)):
         
         cnv_clust_lst = list(set(y_clust))
         cnv_clust_lst.sort()
 
         cluster_size = [] 
         for c in cnv_clust_lst:
             b = y_clust == c
```

### Comparing `scoda-tk-0.4.8/src/scoda/misc.py` & `scoda-tk-0.4.9/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda/pipeline.py` & `scoda-tk-0.4.9/src/scoda/pipeline.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda/viz.py` & `scoda-tk-0.4.9/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.8/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.4.9/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.4.8
+Version: 0.4.9
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.4.8/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.4.9/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

