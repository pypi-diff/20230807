# Comparing `tmp/wafermap-clustering-0.3.8.tar.gz` & `tmp/wafermap-clustering-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-clustering-0.3.8.tar", last modified: Tue Aug  1 08:08:41 2023, max compression
+gzip compressed data, was "wafermap-clustering-0.3.9.tar", last modified: Tue Aug  1 08:42:06 2023, max compression
```

## Comparing `wafermap-clustering-0.3.8.tar` & `wafermap-clustering-0.3.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:08:41.649325 wafermap-clustering-0.3.8/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.3.8/LICENSE.txt
--rw-rw-rw-   0        0        0      568 2023-08-01 08:08:41.647445 wafermap-clustering-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.3.8/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 08:08:41.649828 wafermap-clustering-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-08-01 08:08:18.000000 wafermap-clustering-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:08:41.586929 wafermap-clustering-0.3.8/tests/
--rw-rw-rw-   0        0        0    12755 2023-07-26 14:59:03.000000 wafermap-clustering-0.3.8/tests/test_clustering.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:08:41.590927 wafermap-clustering-0.3.8/wafermap_clustering/
-drwxrwxrwx   0        0        0        0 2023-08-01 08:08:41.620495 wafermap-clustering-0.3.8/wafermap_clustering/configs/
--rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.8/wafermap_clustering/configs/config.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:08:41.625508 wafermap-clustering-0.3.8/wafermap_clustering/libs/
--rw-rw-rw-   0        0        0     4572 2023-07-26 14:53:07.000000 wafermap-clustering-0.3.8/wafermap_clustering/libs/klarf_lib.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:08:41.641495 wafermap-clustering-0.3.8/wafermap_clustering/models/
--rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.3.8/wafermap_clustering/models/clustered_defect.py
--rw-rw-rw-   0        0        0      468 2023-07-19 09:50:06.000000 wafermap-clustering-0.3.8/wafermap_clustering/models/clustering_performance.py
--rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.3.8/wafermap_clustering/models/clustering_result.py
--rw-rw-rw-   0        0        0     7739 2023-08-01 08:08:04.000000 wafermap-clustering-0.3.8/wafermap_clustering/wafermap_clustering.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:08:41.615732 wafermap-clustering-0.3.8/wafermap_clustering.egg-info/
--rw-rw-rw-   0        0        0      568 2023-08-01 08:08:41.000000 wafermap-clustering-0.3.8/wafermap_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-08-01 08:08:41.000000 wafermap-clustering-0.3.8/wafermap_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:08:41.000000 wafermap-clustering-0.3.8/wafermap_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-08-01 08:08:41.000000 wafermap-clustering-0.3.8/wafermap_clustering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-08-01 08:08:41.000000 wafermap-clustering-0.3.8/wafermap_clustering.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 08:42:06.953845 wafermap-clustering-0.3.9/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.3.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      568 2023-08-01 08:42:06.951162 wafermap-clustering-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.3.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:42:06.954844 wafermap-clustering-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      960 2023-08-01 08:41:35.000000 wafermap-clustering-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:42:06.888800 wafermap-clustering-0.3.9/tests/
+-rw-rw-rw-   0        0        0    12755 2023-07-26 14:59:03.000000 wafermap-clustering-0.3.9/tests/test_clustering.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:42:06.892805 wafermap-clustering-0.3.9/wafermap_clustering/
+drwxrwxrwx   0        0        0        0 2023-08-01 08:42:06.925300 wafermap-clustering-0.3.9/wafermap_clustering/configs/
+-rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.9/wafermap_clustering/configs/config.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:42:06.929307 wafermap-clustering-0.3.9/wafermap_clustering/libs/
+-rw-rw-rw-   0        0        0     4572 2023-07-26 14:53:07.000000 wafermap-clustering-0.3.9/wafermap_clustering/libs/klarf_lib.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:42:06.944980 wafermap-clustering-0.3.9/wafermap_clustering/models/
+-rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.3.9/wafermap_clustering/models/clustered_defect.py
+-rw-rw-rw-   0        0        0      468 2023-07-19 09:50:06.000000 wafermap-clustering-0.3.9/wafermap_clustering/models/clustering_performance.py
+-rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.3.9/wafermap_clustering/models/clustering_result.py
+-rw-rw-rw-   0        0        0     7824 2023-08-01 08:41:16.000000 wafermap-clustering-0.3.9/wafermap_clustering/wafermap_clustering.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:42:06.920318 wafermap-clustering-0.3.9/wafermap_clustering.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-08-01 08:42:06.000000 wafermap-clustering-0.3.9/wafermap_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-08-01 08:42:06.000000 wafermap-clustering-0.3.9/wafermap_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:42:06.000000 wafermap-clustering-0.3.9/wafermap_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-08-01 08:42:06.000000 wafermap-clustering-0.3.9/wafermap_clustering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-01 08:42:06.000000 wafermap-clustering-0.3.9/wafermap_clustering.egg-info/top_level.txt
```

### Comparing `wafermap-clustering-0.3.8/LICENSE.txt` & `wafermap-clustering-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.8/PKG-INFO` & `wafermap-clustering-0.3.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.3.8
+Version: 0.3.9
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.8.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.9.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.3.8/setup.py` & `wafermap-clustering-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.8"
+version = "0.3.9"
 
 setup(
     name="wafermap-clustering",
     version=version,
     packages=[
         "wafermap_clustering",
         "wafermap_clustering.configs",
```

### Comparing `wafermap-clustering-0.3.8/tests/test_clustering.py` & `wafermap-clustering-0.3.9/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.8/wafermap_clustering/configs/config.py` & `wafermap-clustering-0.3.9/wafermap_clustering/configs/config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.8/wafermap_clustering/libs/klarf_lib.py` & `wafermap-clustering-0.3.9/wafermap_clustering/libs/klarf_lib.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.8/wafermap_clustering/models/clustering_result.py` & `wafermap-clustering-0.3.9/wafermap_clustering/models/clustering_result.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.8/wafermap_clustering/wafermap_clustering.py` & `wafermap-clustering-0.3.9/wafermap_clustering/wafermap_clustering.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,16 @@
         klarf_content, raw_content = content
 
         match clustering_mode:
             case ClusteringMode.DBSCAN.value:
                 clustering = DBSCAN(
                     eps=self.config.clustering.dbscan.eps,
                     min_samples=self.config.clustering.dbscan.min_samples,
+                    algorithm="ball_tree",
+                    metric="haversine",
                 )
             case ClusteringMode.HDBSCAN.value:
                 clustering = HDBSCAN(
                     min_samples=self.config.clustering.hdbscan.min_samples,
                     min_cluster_size=self.config.clustering.hdbscan.min_cluster_size,
                 )
             case _:
```

### Comparing `wafermap-clustering-0.3.8/wafermap_clustering.egg-info/PKG-INFO` & `wafermap-clustering-0.3.9/wafermap_clustering.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.3.8
+Version: 0.3.9
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.8.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.9.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.3.8/wafermap_clustering.egg-info/SOURCES.txt` & `wafermap-clustering-0.3.9/wafermap_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

