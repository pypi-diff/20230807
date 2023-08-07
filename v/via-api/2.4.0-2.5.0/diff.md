# Comparing `tmp/via-api-2.4.0.tar.gz` & `tmp/via-api-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "via-api-2.4.0.tar", last modified: Sat Aug  5 15:45:00 2023, max compression
+gzip compressed data, was "via-api-2.5.0.tar", last modified: Mon Aug  7 04:41:23 2023, max compression
```

## Comparing `via-api-2.4.0.tar` & `via-api-2.5.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:45:00.033763 via-api-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-05 15:45:00.033763 via-api-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-05 15:44:12.000000 via-api-2.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 15:45:00.033763 via-api-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-05 15:44:12.000000 via-api-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:45:00.029763 via-api-2.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:45:00.029763 via-api-2.4.0/src/via/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:45:00.029763 via-api-2.4.0/src/via/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/bounding_graph_gdfs_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/edge_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:45:00.029763 via-api-2.4.0/src/via/geojson/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/geojson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/geojson/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/geojson/retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/geojson/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:45:00.033763 via-api-2.4.0/src/via/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/models/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/models/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/models/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/models/journey.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/models/journey_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/models/journeys.py
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/models/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/network_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/place_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-08-05 15:44:12.000000 via-api-2.4.0/src/via/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:45:00.033763 via-api-2.4.0/src/via_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-05 15:45:00.000000 via-api-2.4.0/src/via_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-05 15:45:00.000000 via-api-2.4.0/src/via_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 15:45:00.000000 via-api-2.4.0/src/via_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-05 15:45:00.000000 via-api-2.4.0/src/via_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-05 15:45:00.000000 via-api-2.4.0/src/via_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-05 15:45:00.000000 via-api-2.4.0/src/via_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:45:00.033763 via-api-2.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-08-05 15:44:12.000000 via-api-2.4.0/test/test_edge_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-08-05 15:44:12.000000 via-api-2.4.0/test/test_network_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-05 15:44:12.000000 via-api-2.4.0/test/test_place_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-08-05 15:44:12.000000 via-api-2.4.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:41:23.181481 via-api-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-07 04:41:23.181481 via-api-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-07 04:40:35.000000 via-api-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 04:41:23.181481 via-api-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-07 04:40:35.000000 via-api-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:41:23.173481 via-api-2.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:41:23.177481 via-api-2.5.0/src/via/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:41:23.177481 via-api-2.5.0/src/via/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/bounding_graph_gdfs_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/edge_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:41:23.177481 via-api-2.5.0/src/via/geojson/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/geojson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/geojson/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/geojson/retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/geojson/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:41:23.177481 via-api-2.5.0/src/via/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/models/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/models/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/models/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/models/journey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/models/journey_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/models/journeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/models/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/network_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/place_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-08-07 04:40:35.000000 via-api-2.5.0/src/via/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:41:23.177481 via-api-2.5.0/src/via_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-07 04:41:23.000000 via-api-2.5.0/src/via_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-07 04:41:23.000000 via-api-2.5.0/src/via_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 04:41:23.000000 via-api-2.5.0/src/via_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-07 04:41:23.000000 via-api-2.5.0/src/via_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-07 04:41:23.000000 via-api-2.5.0/src/via_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-07 04:41:23.000000 via-api-2.5.0/src/via_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:41:23.177481 via-api-2.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-08-07 04:40:35.000000 via-api-2.5.0/test/test_edge_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-08-07 04:40:35.000000 via-api-2.5.0/test/test_network_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-07 04:40:35.000000 via-api-2.5.0/test/test_place_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-08-07 04:40:35.000000 via-api-2.5.0/test/test_utils.py
```

### Comparing `via-api-2.4.0/README.md` & `via-api-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/setup.py` & `via-api-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     'pymongo',
     'cachetools',
     'mappymatch'
 )
 
 setup(
     name='via-api',
-    version='2.4.0',
+    version='2.5.0',
     python_requires='>=3.6',
     description='Analysing and serving crowdsourced road quality data',
     long_description='Analysing and serving crowdsourced road quality data',
     author='Robert Lucey',
     url='https://github.com/RobertLucey/via',
     packages=find_packages('src'),
     package_dir={'': 'src'},
```

### Comparing `via-api-2.4.0/src/via/__init__.py` & `via-api-2.5.0/src/via/__init__.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/api/main.py` & `via-api-2.5.0/src/via/api/main.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/bounding_graph_gdfs_cache.py` & `via-api-2.5.0/src/via/bounding_graph_gdfs_cache.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/constants.py` & `via-api-2.5.0/src/via/constants.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/edge_cache.py` & `via-api-2.5.0/src/via/edge_cache.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/geojson/generate.py` & `via-api-2.5.0/src/via/geojson/generate.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/geojson/retrieve.py` & `via-api-2.5.0/src/via/geojson/retrieve.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/geojson/utils.py` & `via-api-2.5.0/src/via/geojson/utils.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/log.py` & `via-api-2.5.0/src/via/log.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/models/frame.py` & `via-api-2.5.0/src/via/models/frame.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/models/generic.py` & `via-api-2.5.0/src/via/models/generic.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/models/gps.py` & `via-api-2.5.0/src/via/models/gps.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/models/journey.py` & `via-api-2.5.0/src/via/models/journey.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/models/journey_mixins.py` & `via-api-2.5.0/src/via/models/journey_mixins.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/models/journeys.py` & `via-api-2.5.0/src/via/models/journeys.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/models/point.py` & `via-api-2.5.0/src/via/models/point.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/network_cache.py` & `via-api-2.5.0/src/via/network_cache.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/place_cache.py` & `via-api-2.5.0/src/via/place_cache.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/settings.py` & `via-api-2.5.0/src/via/settings.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via/utils.py` & `via-api-2.5.0/src/via/utils.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/src/via_api.egg-info/SOURCES.txt` & `via-api-2.5.0/src/via_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/test/test_edge_cache.py` & `via-api-2.5.0/test/test_edge_cache.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/test/test_network_cache.py` & `via-api-2.5.0/test/test_network_cache.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/test/test_place_cache.py` & `via-api-2.5.0/test/test_place_cache.py`

 * *Files identical despite different names*

### Comparing `via-api-2.4.0/test/test_utils.py` & `via-api-2.5.0/test/test_utils.py`

 * *Files identical despite different names*

