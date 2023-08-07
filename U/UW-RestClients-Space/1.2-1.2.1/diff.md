# Comparing `tmp/UW-RestClients-Space-1.2.tar.gz` & `tmp/UW-RestClients-Space-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UW-RestClients-Space-1.2.tar", last modified: Fri Aug  4 20:23:15 2023, max compression
+gzip compressed data, was "UW-RestClients-Space-1.2.1.tar", last modified: Mon Aug  7 20:12:10 2023, max compression
```

## Comparing `UW-RestClients-Space-1.2.tar` & `UW-RestClients-Space-1.2.1.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 20:23:15.765324 UW-RestClients-Space-1.2/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-08-04 20:23:05.000000 UW-RestClients-Space-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-08-04 20:23:05.000000 UW-RestClients-Space-1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-08-04 20:23:15.765324 UW-RestClients-Space-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-08-04 20:23:05.000000 UW-RestClients-Space-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 20:23:15.761325 UW-RestClients-Space-1.2/UW_RestClients_Space.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-08-04 20:23:15.000000 UW-RestClients-Space-1.2/UW_RestClients_Space.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-08-04 20:23:15.000000 UW-RestClients-Space-1.2/UW_RestClients_Space.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 20:23:15.000000 UW-RestClients-Space-1.2/UW_RestClients_Space.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-04 20:23:15.000000 UW-RestClients-Space-1.2/UW_RestClients_Space.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-08-04 20:23:15.000000 UW-RestClients-Space-1.2/UW_RestClients_Space.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-04 20:23:15.765324 UW-RestClients-Space-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-08-04 20:23:05.000000 UW-RestClients-Space-1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 20:23:15.761325 UW-RestClients-Space-1.2/uw_space/
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-08-04 20:23:15.000000 UW-RestClients-Space-1.2/uw_space/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-08-04 20:23:05.000000 UW-RestClients-Space-1.2/uw_space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-08-04 20:23:05.000000 UW-RestClients-Space-1.2/uw_space/dao.py
--rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-08-04 20:23:05.000000 UW-RestClients-Space-1.2/uw_space/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 20:23:15.757325 UW-RestClients-Space-1.2/uw_space/resources/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 20:23:15.757325 UW-RestClients-Space-1.2/uw_space/resources/space/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 20:23:15.757325 UW-RestClients-Space-1.2/uw_space/resources/space/file/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 20:23:15.757325 UW-RestClients-Space-1.2/uw_space/resources/space/file/space/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 20:23:15.761325 UW-RestClients-Space-1.2/uw_space/resources/space/file/space/v2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 20:23:15.761325 UW-RestClients-Space-1.2/uw_space/resources/space/file/space/v2/facility/
--rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-08-04 20:23:05.000000 UW-RestClients-Space-1.2/uw_space/resources/space/file/space/v2/facility/1347.json
--rw-r--r--   0 runner    (1001) docker     (122)     1334 2023-08-04 20:23:05.000000 UW-RestClients-Space-1.2/uw_space/resources/space/file/space/v2/facility.json_facility_code_MEB
--rw-r--r--   0 runner    (1001) docker     (122)      466 2023-08-04 20:23:05.000000 UW-RestClients-Space-1.2/uw_space/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 20:23:15.765324 UW-RestClients-Space-1.2/uw_space/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 20:23:05.000000 UW-RestClients-Space-1.2/uw_space/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-08-04 20:23:05.000000 UW-RestClients-Space-1.2/uw_space/tests/test_dao.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-08-04 20:23:05.000000 UW-RestClients-Space-1.2/uw_space/tests/test_facilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      402 2023-08-04 20:23:05.000000 UW-RestClients-Space-1.2/uw_space/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 20:12:10.063483 UW-RestClients-Space-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-08-07 20:12:10.063483 UW-RestClients-Space-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 20:12:10.059483 UW-RestClients-Space-1.2.1/UW_RestClients_Space.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-08-07 20:12:09.000000 UW-RestClients-Space-1.2.1/UW_RestClients_Space.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-08-07 20:12:09.000000 UW-RestClients-Space-1.2.1/UW_RestClients_Space.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-07 20:12:09.000000 UW-RestClients-Space-1.2.1/UW_RestClients_Space.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-07 20:12:09.000000 UW-RestClients-Space-1.2.1/UW_RestClients_Space.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-08-07 20:12:09.000000 UW-RestClients-Space-1.2.1/UW_RestClients_Space.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-07 20:12:10.063483 UW-RestClients-Space-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 20:12:10.059483 UW-RestClients-Space-1.2.1/uw_space/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-08-07 20:12:08.000000 UW-RestClients-Space-1.2.1/uw_space/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/uw_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/uw_space/dao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/uw_space/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 20:12:10.051483 UW-RestClients-Space-1.2.1/uw_space/resources/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 20:12:10.051483 UW-RestClients-Space-1.2.1/uw_space/resources/space/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 20:12:10.051483 UW-RestClients-Space-1.2.1/uw_space/resources/space/file/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 20:12:10.055482 UW-RestClients-Space-1.2.1/uw_space/resources/space/file/space/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 20:12:10.063483 UW-RestClients-Space-1.2.1/uw_space/resources/space/file/space/v2/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 20:12:10.063483 UW-RestClients-Space-1.2.1/uw_space/resources/space/file/space/v2/facility/
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/uw_space/resources/space/file/space/v2/facility/1347.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/uw_space/resources/space/file/space/v2/facility/6471.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/uw_space/resources/space/file/space/v2/facility.json_facility_code_MDR
+-rw-r--r--   0 runner    (1001) docker     (122)     1334 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/uw_space/resources/space/file/space/v2/facility.json_facility_code_MEB
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/uw_space/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 20:12:10.063483 UW-RestClients-Space-1.2.1/uw_space/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/uw_space/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/uw_space/tests/test_dao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/uw_space/tests/test_facilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      402 2023-08-07 20:11:57.000000 UW-RestClients-Space-1.2.1/uw_space/utils.py
```

### Comparing `UW-RestClients-Space-1.2/LICENSE` & `UW-RestClients-Space-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Space-1.2/PKG-INFO` & `UW-RestClients-Space-1.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: UW-RestClients-Space
-Version: 1.2
+Version: 1.2.1
 Summary: A library for connecting to HFS services at the University of Washington
 Home-page: https://github.com/uw-it-aca/uw-restclients-space
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `UW-RestClients-Space-1.2/README.md` & `UW-RestClients-Space-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Space-1.2/UW_RestClients_Space.egg-info/PKG-INFO` & `UW-RestClients-Space-1.2.1/UW_RestClients_Space.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: UW-RestClients-Space
-Version: 1.2
+Version: 1.2.1
 Summary: A library for connecting to HFS services at the University of Washington
 Home-page: https://github.com/uw-it-aca/uw-restclients-space
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `UW-RestClients-Space-1.2/setup.py` & `UW-RestClients-Space-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Space-1.2/uw_space/__init__.py` & `UW-RestClients-Space-1.2.1/uw_space/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,17 +43,21 @@
             {'url': url, 'status': response.status, 'data': response.data})
         if response.status != 200:
             raise DataFailureException(url, response.status, response.data)
         return Facility.from_json(json.loads(response.data))
 
     def __process_json(self, json_data):
         objs = []
-        facilitys = json_data.get("Facilitys")
-        for facility in facilitys:
-            status = facility.get("Status")
-            fnumber = facility.get("FacilityNumber")
-            if fnumber and len(fnumber):
-                fac = self.search_by_number(fnumber)
-                if fac:
-                    fac.status = status
-                    objs.append(fac)
+        if "Facilities" in json_data:
+            facilities = json_data.get("Facilities")
+        elif "Facilitys" in json_data:
+            facilities = json_data.get("Facilitys")
+        if facilities:
+            for facility in facilities:
+                status = facility.get("Status")
+                fnumber = facility.get("FacilityNumber")
+                if fnumber and len(fnumber):
+                    fac = self.search_by_number(fnumber)
+                    if fac:
+                        fac.status = status
+                        objs.append(fac)
         return objs
```

### Comparing `UW-RestClients-Space-1.2/uw_space/models.py` & `UW-RestClients-Space-1.2.1/uw_space/models.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Space-1.2/uw_space/resources/space/file/space/v2/facility/1347.json` & `UW-RestClients-Space-1.2.1/uw_space/resources/space/file/space/v2/facility/1347.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Space-1.2/uw_space/resources/space/file/space/v2/facility.json_facility_code_MEB` & `UW-RestClients-Space-1.2.1/uw_space/resources/space/file/space/v2/facility.json_facility_code_MEB`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Space-1.2/uw_space/tests/test_dao.py` & `UW-RestClients-Space-1.2.1/uw_space/tests/test_dao.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Space-1.2/uw_space/tests/test_facilities.py` & `UW-RestClients-Space-1.2.1/uw_space/tests/test_facilities.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,14 +28,28 @@
         self.assertEqual(fac[0].json_data(), data)
 
         self.assertRaises(
             DataFailureException,
             Facilities().search_by_code, "None"
         )
 
+        fac = Facilities().search_by_code("MDR")
+        self.assertEqual(len(fac), 1)
+        self.assertEqual(fac[0].json_data(), {
+            'code': 'MDR',
+            'last_updated': '2022-09-22 12:49:38',
+            'latitude': 47.6601320001,
+            'longitude': -122.305391,
+            'name': 'Madrona Hall',
+            'number': '6471',
+            'site': 'Seattle Main Campus',
+            'status': 'A',
+            'type': 'Building'
+            })
+
     def test_search_by_number(self):
         fac = Facilities().search_by_number("1347")
         data['status'] = ''
         self.assertEqual(fac.json_data(), data)
 
         self.assertRaises(
             DataFailureException,
```

