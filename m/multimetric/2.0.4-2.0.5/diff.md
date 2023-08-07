# Comparing `tmp/multimetric-2.0.4.tar.gz` & `tmp/multimetric-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimetric-2.0.4.tar", last modified: Wed Aug  2 14:04:19 2023, max compression
+gzip compressed data, was "multimetric-2.0.5.tar", last modified: Mon Aug  7 14:52:57 2023, max compression
```

## Comparing `multimetric-2.0.4.tar` & `multimetric-2.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:04:19.441821 multimetric-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-02 14:03:54.000000 multimetric-2.0.4/LICENSE.Zlib
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 14:03:54.000000 multimetric-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-08-02 14:04:19.441821 multimetric-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-08-02 14:03:54.000000 multimetric-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:04:19.437821 multimetric-2.0.4/multimetric/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:04:19.437821 multimetric-2.0.4/multimetric/cls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/base_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/base_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:04:19.437821 multimetric-2.0.4/multimetric/cls/calc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/calc/halstead.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/calc/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/calc/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/calc/tiobe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:04:19.441821 multimetric-2.0.4/multimetric/cls/importer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/importer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/importer/filtered.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:04:19.441821 multimetric-2.0.4/multimetric/cls/importer/mods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/importer/mods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/importer/mods/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/importer/mods/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/importer/pick.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:04:19.441821 multimetric-2.0.4/multimetric/cls/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/metric/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/metric/cyclomatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/metric/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/metric/loc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/metric/operands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/metric/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:04:19.441821 multimetric-2.0.4/multimetric/cls/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/stats/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-08-02 14:03:54.000000 multimetric-2.0.4/multimetric/cls/tokentree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:04:19.437821 multimetric-2.0.4/multimetric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-08-02 14:04:19.000000 multimetric-2.0.4/multimetric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-02 14:04:19.000000 multimetric-2.0.4/multimetric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:04:19.000000 multimetric-2.0.4/multimetric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 14:04:19.000000 multimetric-2.0.4/multimetric.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 14:04:19.000000 multimetric-2.0.4/multimetric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:03:54.000000 multimetric-2.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-02 14:04:19.441821 multimetric-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-02 14:04:19.000000 multimetric-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:57.367683 multimetric-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-07 14:52:38.000000 multimetric-2.0.5/LICENSE.Zlib
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-07 14:52:38.000000 multimetric-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-08-07 14:52:57.367683 multimetric-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-08-07 14:52:38.000000 multimetric-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:57.363683 multimetric-2.0.5/multimetric/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:57.363683 multimetric-2.0.5/multimetric/cls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/base_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/base_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:57.363683 multimetric-2.0.5/multimetric/cls/calc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/calc/halstead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/calc/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/calc/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/calc/tiobe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:57.367683 multimetric-2.0.5/multimetric/cls/importer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/importer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/importer/filtered.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:57.367683 multimetric-2.0.5/multimetric/cls/importer/mods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/importer/mods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/importer/mods/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/importer/mods/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/importer/pick.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:57.367683 multimetric-2.0.5/multimetric/cls/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/metric/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/metric/cyclomatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/metric/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/metric/loc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/metric/operands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/metric/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:57.367683 multimetric-2.0.5/multimetric/cls/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/stats/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-08-07 14:52:38.000000 multimetric-2.0.5/multimetric/cls/tokentree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:52:57.363683 multimetric-2.0.5/multimetric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-08-07 14:52:57.000000 multimetric-2.0.5/multimetric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-07 14:52:57.000000 multimetric-2.0.5/multimetric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:52:57.000000 multimetric-2.0.5/multimetric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-07 14:52:57.000000 multimetric-2.0.5/multimetric.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 14:52:57.000000 multimetric-2.0.5/multimetric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 14:52:38.000000 multimetric-2.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-07 14:52:57.367683 multimetric-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-07 14:52:57.000000 multimetric-2.0.5/setup.py
```

### Comparing `multimetric-2.0.4/LICENSE.Zlib` & `multimetric-2.0.5/LICENSE.Zlib`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/PKG-INFO` & `multimetric-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimetric
-Version: 2.0.4
+Version: 2.0.5
 Summary: Calculate code metrics in various languages
 Home-page: https://github.com/priv-kweihmann/multimetric
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `multimetric-2.0.4/README.md` & `multimetric-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/__main__.py` & `multimetric-2.0.5/multimetric/__main__.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/base.py` & `multimetric-2.0.5/multimetric/cls/base.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/calc/halstead.py` & `multimetric-2.0.5/multimetric/cls/calc/halstead.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/calc/maintenance.py` & `multimetric-2.0.5/multimetric/cls/calc/maintenance.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/calc/pylint.py` & `multimetric-2.0.5/multimetric/cls/calc/pylint.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/calc/tiobe.py` & `multimetric-2.0.5/multimetric/cls/calc/tiobe.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/importer/base.py` & `multimetric-2.0.5/multimetric/cls/importer/base.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/importer/mods/csv.py` & `multimetric-2.0.5/multimetric/cls/importer/mods/csv.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/importer/mods/json.py` & `multimetric-2.0.5/multimetric/cls/importer/mods/json.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/importer/pick.py` & `multimetric-2.0.5/multimetric/cls/importer/pick.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/metric/comments.py` & `multimetric-2.0.5/multimetric/cls/metric/comments.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/metric/cyclomatic.py` & `multimetric-2.0.5/multimetric/cls/metric/cyclomatic.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/metric/fanout.py` & `multimetric-2.0.5/multimetric/cls/metric/fanout.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/metric/loc.py` & `multimetric-2.0.5/multimetric/cls/metric/loc.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/metric/operands.py` & `multimetric-2.0.5/multimetric/cls/metric/operands.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/metric/operators.py` & `multimetric-2.0.5/multimetric/cls/metric/operators.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/modules.py` & `multimetric-2.0.5/multimetric/cls/modules.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/stats/stats.py` & `multimetric-2.0.5/multimetric/cls/stats/stats.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric/cls/tokentree.py` & `multimetric-2.0.5/multimetric/cls/tokentree.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/multimetric.egg-info/PKG-INFO` & `multimetric-2.0.5/multimetric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimetric
-Version: 2.0.4
+Version: 2.0.5
 Summary: Calculate code metrics in various languages
 Home-page: https://github.com/priv-kweihmann/multimetric
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `multimetric-2.0.4/multimetric.egg-info/SOURCES.txt` & `multimetric-2.0.5/multimetric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multimetric-2.0.4/setup.py` & `multimetric-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="multimetric",
-    version="2.0.4",
+    version="2.0.5",
     author="Konrad Weihmann",
     author_email="kweihmann@outlook.com",
     description="Calculate code metrics in various languages",
     long_description=_long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/priv-kweihmann/multimetric",
     packages=setuptools.find_packages(exclude=('tests',)),
```

