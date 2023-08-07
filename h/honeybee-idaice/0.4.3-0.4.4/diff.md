# Comparing `tmp/honeybee-idaice-0.4.3.tar.gz` & `tmp/honeybee-idaice-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-idaice-0.4.3.tar", last modified: Thu Jul 27 18:22:09 2023, max compression
+gzip compressed data, was "dist/honeybee-idaice-0.4.4.tar", last modified: Mon Aug  7 21:42:02 2023, max compression
```

## Comparing `honeybee-idaice-0.4.3.tar` & `honeybee-idaice-0.4.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    16340 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/bldgbody.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/shade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/templates/ahu.idc
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/templates/ahu.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/templates/building.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/templates/plant.idc
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/templates/plant.idm
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/templates/room.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20568 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/writer_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:42:02.000000 honeybee-idaice-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-07 21:42:02.000000 honeybee-idaice-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:42:02.000000 honeybee-idaice-0.4.4/honeybee_idaice/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16340 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/bldgbody.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:42:02.000000 honeybee-idaice-0.4.4/honeybee_idaice/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/shade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:42:02.000000 honeybee-idaice-0.4.4/honeybee_idaice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/templates/ahu.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/templates/ahu.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/templates/building.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/templates/plant.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/templates/plant.idm
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/templates/room.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20756 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/honeybee_idaice/writer_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:42:02.000000 honeybee-idaice-0.4.4/honeybee_idaice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-07 21:42:01.000000 honeybee-idaice-0.4.4/honeybee_idaice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-07 21:42:01.000000 honeybee-idaice-0.4.4/honeybee_idaice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 21:42:01.000000 honeybee-idaice-0.4.4/honeybee_idaice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-07 21:42:01.000000 honeybee-idaice-0.4.4/honeybee_idaice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 21:42:01.000000 honeybee-idaice-0.4.4/honeybee_idaice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 21:42:01.000000 honeybee-idaice-0.4.4/honeybee_idaice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-07 21:42:02.000000 honeybee-idaice-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-07 21:40:47.000000 honeybee-idaice-0.4.4/setup.py
```

### Comparing `honeybee-idaice-0.4.3/LICENSE` & `honeybee-idaice-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/PKG-INFO` & `honeybee-idaice-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.4.3
+Version: 0.4.4
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.4.3/README.md` & `honeybee-idaice-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice/archive.py` & `honeybee-idaice-0.4.4/honeybee_idaice/archive.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice/bldgbody.py` & `honeybee-idaice-0.4.4/honeybee_idaice/bldgbody.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice/cli/translate.py` & `honeybee-idaice-0.4.4/honeybee_idaice/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice/face.py` & `honeybee-idaice-0.4.4/honeybee_idaice/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice/shade.py` & `honeybee-idaice-0.4.4/honeybee_idaice/shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice/templates/ahu.idc` & `honeybee-idaice-0.4.4/honeybee_idaice/templates/ahu.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice/templates/ahu.idm` & `honeybee-idaice-0.4.4/honeybee_idaice/templates/ahu.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice/templates/building.idm` & `honeybee-idaice-0.4.4/honeybee_idaice/templates/building.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice/templates/plant.idc` & `honeybee-idaice-0.4.4/honeybee_idaice/templates/plant.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice/templates/plant.idm` & `honeybee-idaice-0.4.4/honeybee_idaice/templates/plant.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice/templates/room.idm` & `honeybee-idaice-0.4.4/honeybee_idaice/templates/room.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice/writer.py` & `honeybee-idaice-0.4.4/honeybee_idaice/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,14 +397,18 @@
     model = model.duplicate()
 
     # scale the model if the units are not meters
     if model.units != 'Meters':
         model.convert_to_units('Meters')
     # remove degenerate geometry within the model tolerance
     model.remove_degenerate_geometry()
+    # merge coplanar faces across the model's rooms
+    for room in model.rooms:
+        room.merge_coplanar_faces(
+            model.tolerance, model.angle_tolerance, vertical_only=True)
     # convert all apertures to be rectangular, using the model tolerances
     ap_dist = max_frame_thickness if max_frame_thickness > model.tolerance \
         else model.tolerance
     model.rectangularize_apertures(max_separation=ap_dist, resolve_adjacency=False)
 
     # edit the model display_names and add user_data to help with the translation
     adj_dist = max_adjacent_sub_face_dist \
```

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice/writer_obj.py` & `honeybee-idaice-0.4.4/honeybee_idaice/writer_obj.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice.egg-info/PKG-INFO` & `honeybee-idaice-0.4.4/honeybee_idaice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.4.3
+Version: 0.4.4
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.4.3/honeybee_idaice.egg-info/SOURCES.txt` & `honeybee-idaice-0.4.4/honeybee_idaice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.3/setup.py` & `honeybee-idaice-0.4.4/setup.py`

 * *Files identical despite different names*

