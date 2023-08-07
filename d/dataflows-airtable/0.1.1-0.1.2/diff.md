# Comparing `tmp/dataflows-airtable-0.1.1.tar.gz` & `tmp/dataflows-airtable-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataflows-airtable-0.1.1.tar", last modified: Sun Jun 18 14:34:59 2023, max compression
+gzip compressed data, was "dataflows-airtable-0.1.2.tar", last modified: Mon Aug  7 11:02:27 2023, max compression
```

## Comparing `dataflows-airtable-0.1.1.tar` & `dataflows-airtable-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-18 14:34:59.635222 dataflows-airtable-0.1.1/
--rw-r--r--   0 adam       (501) staff       (20)      154 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.1/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)      473 2021-05-14 13:36:59.000000 dataflows-airtable-0.1.1/Makefile
--rw-r--r--   0 adam       (501) staff       (20)      948 2023-06-18 14:34:59.635401 dataflows-airtable-0.1.1/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)       77 2021-05-14 10:24:07.000000 dataflows-airtable-0.1.1/README.md
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-18 14:34:59.631721 dataflows-airtable-0.1.1/dataflows_airtable/
--rw-r--r--   0 adam       (501) staff       (20)        5 2023-06-18 14:17:13.000000 dataflows-airtable-0.1.1/dataflows_airtable/VERSION
--rw-r--r--   0 adam       (501) staff       (20)      136 2021-05-14 17:39:08.000000 dataflows-airtable-0.1.1/dataflows_airtable/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)       36 2021-05-14 17:40:48.000000 dataflows-airtable-0.1.1/dataflows_airtable/consts.py
--rw-r--r--   0 adam       (501) staff       (20)     3049 2023-03-15 11:12:35.000000 dataflows-airtable-0.1.1/dataflows_airtable/dump_to_airtable.py
--rw-r--r--   0 adam       (501) staff       (20)     3705 2023-06-18 14:17:08.000000 dataflows-airtable-0.1.1/dataflows_airtable/load_from_airtable.py
--rw-r--r--   0 adam       (501) staff       (20)      752 2023-06-14 12:00:00.000000 dataflows-airtable-0.1.1/dataflows_airtable/utilities.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-18 14:34:59.634908 dataflows-airtable-0.1.1/dataflows_airtable.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)      948 2023-06-18 14:34:59.000000 dataflows-airtable-0.1.1/dataflows_airtable.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      528 2023-06-18 14:34:59.000000 dataflows-airtable-0.1.1/dataflows_airtable.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-06-18 14:34:59.000000 dataflows-airtable-0.1.1/dataflows_airtable.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2021-05-14 15:56:11.000000 dataflows-airtable-0.1.1/dataflows_airtable.egg-info/not-zip-safe
--rw-r--r--   0 adam       (501) staff       (20)       72 2023-06-18 14:34:59.000000 dataflows-airtable-0.1.1/dataflows_airtable.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       19 2023-06-18 14:34:59.000000 dataflows-airtable-0.1.1/dataflows_airtable.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)      221 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.1/pylama.ini
--rw-r--r--   0 adam       (501) staff       (20)       27 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.1/pytest.ini
--rw-r--r--   0 adam       (501) staff       (20)       67 2023-06-18 14:34:59.635968 dataflows-airtable-0.1.1/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     1946 2021-05-14 10:46:25.000000 dataflows-airtable-0.1.1/setup.py
--rw-r--r--   0 adam       (501) staff       (20)      318 2021-05-14 10:46:39.000000 dataflows-airtable-0.1.1/tox.ini
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-07 11:02:27.594752 dataflows-airtable-0.1.2/
+-rw-r--r--   0 adam       (501) staff       (20)     1065 2021-05-14 10:24:07.000000 dataflows-airtable-0.1.2/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)      154 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.2/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)      473 2021-05-14 13:36:59.000000 dataflows-airtable-0.1.2/Makefile
+-rw-r--r--   0 adam       (501) staff       (20)      932 2023-08-07 11:02:27.594910 dataflows-airtable-0.1.2/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)       77 2021-05-14 10:24:07.000000 dataflows-airtable-0.1.2/README.md
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-07 11:02:27.591072 dataflows-airtable-0.1.2/dataflows_airtable/
+-rw-r--r--   0 adam       (501) staff       (20)        5 2023-08-07 11:00:12.000000 dataflows-airtable-0.1.2/dataflows_airtable/VERSION
+-rw-r--r--   0 adam       (501) staff       (20)      136 2021-05-14 17:39:08.000000 dataflows-airtable-0.1.2/dataflows_airtable/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)       36 2021-05-14 17:40:48.000000 dataflows-airtable-0.1.2/dataflows_airtable/consts.py
+-rw-r--r--   0 adam       (501) staff       (20)     3049 2023-03-15 11:12:35.000000 dataflows-airtable-0.1.2/dataflows_airtable/dump_to_airtable.py
+-rw-r--r--   0 adam       (501) staff       (20)     3852 2023-08-07 11:00:04.000000 dataflows-airtable-0.1.2/dataflows_airtable/load_from_airtable.py
+-rw-r--r--   0 adam       (501) staff       (20)      752 2023-06-14 12:00:00.000000 dataflows-airtable-0.1.2/dataflows_airtable/utilities.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-07 11:02:27.594428 dataflows-airtable-0.1.2/dataflows_airtable.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)      932 2023-08-07 11:02:27.000000 dataflows-airtable-0.1.2/dataflows_airtable.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      536 2023-08-07 11:02:27.000000 dataflows-airtable-0.1.2/dataflows_airtable.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-08-07 11:02:27.000000 dataflows-airtable-0.1.2/dataflows_airtable.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2021-05-14 15:56:11.000000 dataflows-airtable-0.1.2/dataflows_airtable.egg-info/not-zip-safe
+-rw-r--r--   0 adam       (501) staff       (20)       72 2023-08-07 11:02:27.000000 dataflows-airtable-0.1.2/dataflows_airtable.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)       19 2023-08-07 11:02:27.000000 dataflows-airtable-0.1.2/dataflows_airtable.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)      221 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.2/pylama.ini
+-rw-r--r--   0 adam       (501) staff       (20)       27 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.2/pytest.ini
+-rw-r--r--   0 adam       (501) staff       (20)       67 2023-08-07 11:02:27.595520 dataflows-airtable-0.1.2/setup.cfg
+-rw-r--r--   0 adam       (501) staff       (20)     1946 2021-05-14 10:46:25.000000 dataflows-airtable-0.1.2/setup.py
+-rw-r--r--   0 adam       (501) staff       (20)      318 2021-05-14 10:46:39.000000 dataflows-airtable-0.1.2/tox.ini
```

### Comparing `dataflows-airtable-0.1.1/PKG-INFO` & `dataflows-airtable-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dataflows-airtable
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python library for adding AirTable support to dataflows
 Home-page: https://github.com/dataspot/dataflows-airtable
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
-Description: # dataflows-airtable
-        Python library for adding AirTable support to dataflows
 Keywords: frictionless data,open data,airtable,dataflows,table schema,data package,tabular data package
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: develop
+License-File: LICENSE
+
+# dataflows-airtable
+Python library for adding AirTable support to dataflows
```

### Comparing `dataflows-airtable-0.1.1/dataflows_airtable/dump_to_airtable.py` & `dataflows-airtable-0.1.2/dataflows_airtable/dump_to_airtable.py`

 * *Files identical despite different names*

### Comparing `dataflows-airtable-0.1.1/dataflows_airtable/load_from_airtable.py` & `dataflows-airtable-0.1.2/dataflows_airtable/load_from_airtable.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,19 @@
         richText='string',
         rollup='any',
         singleCollaborator='object',
         singleLineText='string',
         singleSelect='string',
         url='string',
     )
+    EXTRA_FIELDS = dict(
+        dateTime=dict(
+            format='%Y-%m-%dT%H:%M:%S.%fZ'
+        ),
+    )
 
 
     def describe_table():
         try:
             url = f'https://api.airtable.com/v0/meta/bases/{base}/tables'
             resp = rate_limiter.execute(lambda: session.get(url, timeout=10).json())
             tables = resp.get('tables', [])
@@ -54,15 +59,15 @@
                 steps = [
                     [],
                     DF.update_resource(-1, name=table),
                     DF.add_field(AIRTABLE_ID_FIELD, 'string', resources=table),
                 ]
                 for field in table_rec['fields']:
                     steps.append(
-                        DF.add_field(field['name'], TYPE_CONVERSION[field['type']], resources=table),
+                        DF.add_field(field['name'], TYPE_CONVERSION[field['type']], resources=table, **EXTRA_FIELDS.get(field['type'], {})),
                     )
                 return DF.Flow(*steps)
         except Exception as e:
             print('Error fetching schema:', e)
         print(f'Failed to find table {table} in base schema')
 
     def records():
```

### Comparing `dataflows-airtable-0.1.1/dataflows_airtable/utilities.py` & `dataflows-airtable-0.1.2/dataflows_airtable/utilities.py`

 * *Files identical despite different names*

### Comparing `dataflows-airtable-0.1.1/dataflows_airtable.egg-info/PKG-INFO` & `dataflows-airtable-0.1.2/dataflows_airtable.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dataflows-airtable
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python library for adding AirTable support to dataflows
 Home-page: https://github.com/dataspot/dataflows-airtable
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
-Description: # dataflows-airtable
-        Python library for adding AirTable support to dataflows
 Keywords: frictionless data,open data,airtable,dataflows,table schema,data package,tabular data package
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: develop
+License-File: LICENSE
+
+# dataflows-airtable
+Python library for adding AirTable support to dataflows
```

### Comparing `dataflows-airtable-0.1.1/dataflows_airtable.egg-info/SOURCES.txt` & `dataflows-airtable-0.1.2/dataflows_airtable.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 Makefile
 README.md
 pylama.ini
 pytest.ini
 setup.cfg
 setup.py
```

### Comparing `dataflows-airtable-0.1.1/setup.py` & `dataflows-airtable-0.1.2/setup.py`

 * *Files identical despite different names*

