# Comparing `tmp/dataflows-airtable-0.1.2.tar.gz` & `tmp/dataflows-airtable-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataflows-airtable-0.1.2.tar", last modified: Mon Aug  7 11:02:27 2023, max compression
+gzip compressed data, was "dataflows-airtable-0.1.3.tar", last modified: Mon Aug  7 11:40:27 2023, max compression
```

## Comparing `dataflows-airtable-0.1.2.tar` & `dataflows-airtable-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-07 11:02:27.594752 dataflows-airtable-0.1.2/
--rw-r--r--   0 adam       (501) staff       (20)     1065 2021-05-14 10:24:07.000000 dataflows-airtable-0.1.2/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)      154 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.2/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)      473 2021-05-14 13:36:59.000000 dataflows-airtable-0.1.2/Makefile
--rw-r--r--   0 adam       (501) staff       (20)      932 2023-08-07 11:02:27.594910 dataflows-airtable-0.1.2/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)       77 2021-05-14 10:24:07.000000 dataflows-airtable-0.1.2/README.md
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-07 11:02:27.591072 dataflows-airtable-0.1.2/dataflows_airtable/
--rw-r--r--   0 adam       (501) staff       (20)        5 2023-08-07 11:00:12.000000 dataflows-airtable-0.1.2/dataflows_airtable/VERSION
--rw-r--r--   0 adam       (501) staff       (20)      136 2021-05-14 17:39:08.000000 dataflows-airtable-0.1.2/dataflows_airtable/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)       36 2021-05-14 17:40:48.000000 dataflows-airtable-0.1.2/dataflows_airtable/consts.py
--rw-r--r--   0 adam       (501) staff       (20)     3049 2023-03-15 11:12:35.000000 dataflows-airtable-0.1.2/dataflows_airtable/dump_to_airtable.py
--rw-r--r--   0 adam       (501) staff       (20)     3852 2023-08-07 11:00:04.000000 dataflows-airtable-0.1.2/dataflows_airtable/load_from_airtable.py
--rw-r--r--   0 adam       (501) staff       (20)      752 2023-06-14 12:00:00.000000 dataflows-airtable-0.1.2/dataflows_airtable/utilities.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-07 11:02:27.594428 dataflows-airtable-0.1.2/dataflows_airtable.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)      932 2023-08-07 11:02:27.000000 dataflows-airtable-0.1.2/dataflows_airtable.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      536 2023-08-07 11:02:27.000000 dataflows-airtable-0.1.2/dataflows_airtable.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-08-07 11:02:27.000000 dataflows-airtable-0.1.2/dataflows_airtable.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2021-05-14 15:56:11.000000 dataflows-airtable-0.1.2/dataflows_airtable.egg-info/not-zip-safe
--rw-r--r--   0 adam       (501) staff       (20)       72 2023-08-07 11:02:27.000000 dataflows-airtable-0.1.2/dataflows_airtable.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       19 2023-08-07 11:02:27.000000 dataflows-airtable-0.1.2/dataflows_airtable.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)      221 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.2/pylama.ini
--rw-r--r--   0 adam       (501) staff       (20)       27 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.2/pytest.ini
--rw-r--r--   0 adam       (501) staff       (20)       67 2023-08-07 11:02:27.595520 dataflows-airtable-0.1.2/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     1946 2021-05-14 10:46:25.000000 dataflows-airtable-0.1.2/setup.py
--rw-r--r--   0 adam       (501) staff       (20)      318 2021-05-14 10:46:39.000000 dataflows-airtable-0.1.2/tox.ini
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-07 11:40:27.199184 dataflows-airtable-0.1.3/
+-rw-r--r--   0 adam       (501) staff       (20)     1065 2021-05-14 10:24:07.000000 dataflows-airtable-0.1.3/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)      154 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.3/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)      473 2021-05-14 13:36:59.000000 dataflows-airtable-0.1.3/Makefile
+-rw-r--r--   0 adam       (501) staff       (20)      932 2023-08-07 11:40:27.199412 dataflows-airtable-0.1.3/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)       77 2021-05-14 10:24:07.000000 dataflows-airtable-0.1.3/README.md
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-07 11:40:27.174916 dataflows-airtable-0.1.3/dataflows_airtable/
+-rw-r--r--   0 adam       (501) staff       (20)        5 2023-08-07 11:39:56.000000 dataflows-airtable-0.1.3/dataflows_airtable/VERSION
+-rw-r--r--   0 adam       (501) staff       (20)      136 2021-05-14 17:39:08.000000 dataflows-airtable-0.1.3/dataflows_airtable/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)       36 2021-05-14 17:40:48.000000 dataflows-airtable-0.1.3/dataflows_airtable/consts.py
+-rw-r--r--   0 adam       (501) staff       (20)     3049 2023-03-15 11:12:35.000000 dataflows-airtable-0.1.3/dataflows_airtable/dump_to_airtable.py
+-rw-r--r--   0 adam       (501) staff       (20)     3951 2023-08-07 11:40:11.000000 dataflows-airtable-0.1.3/dataflows_airtable/load_from_airtable.py
+-rw-r--r--   0 adam       (501) staff       (20)      752 2023-06-14 12:00:00.000000 dataflows-airtable-0.1.3/dataflows_airtable/utilities.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-08-07 11:40:27.198614 dataflows-airtable-0.1.3/dataflows_airtable.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)      932 2023-08-07 11:40:26.000000 dataflows-airtable-0.1.3/dataflows_airtable.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      536 2023-08-07 11:40:27.000000 dataflows-airtable-0.1.3/dataflows_airtable.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-08-07 11:40:26.000000 dataflows-airtable-0.1.3/dataflows_airtable.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2021-05-14 15:56:11.000000 dataflows-airtable-0.1.3/dataflows_airtable.egg-info/not-zip-safe
+-rw-r--r--   0 adam       (501) staff       (20)       72 2023-08-07 11:40:26.000000 dataflows-airtable-0.1.3/dataflows_airtable.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)       19 2023-08-07 11:40:26.000000 dataflows-airtable-0.1.3/dataflows_airtable.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)      221 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.3/pylama.ini
+-rw-r--r--   0 adam       (501) staff       (20)       27 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.3/pytest.ini
+-rw-r--r--   0 adam       (501) staff       (20)       67 2023-08-07 11:40:27.200096 dataflows-airtable-0.1.3/setup.cfg
+-rw-r--r--   0 adam       (501) staff       (20)     1946 2021-05-14 10:46:25.000000 dataflows-airtable-0.1.3/setup.py
+-rw-r--r--   0 adam       (501) staff       (20)      318 2021-05-14 10:46:39.000000 dataflows-airtable-0.1.3/tox.ini
```

### Comparing `dataflows-airtable-0.1.2/LICENSE` & `dataflows-airtable-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dataflows-airtable-0.1.2/PKG-INFO` & `dataflows-airtable-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflows-airtable
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python library for adding AirTable support to dataflows
 Home-page: https://github.com/dataspot/dataflows-airtable
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Keywords: frictionless data,open data,airtable,dataflows,table schema,data package,tabular data package
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dataflows-airtable-0.1.2/dataflows_airtable/dump_to_airtable.py` & `dataflows-airtable-0.1.3/dataflows_airtable/dump_to_airtable.py`

 * *Files identical despite different names*

### Comparing `dataflows-airtable-0.1.2/dataflows_airtable/load_from_airtable.py` & `dataflows-airtable-0.1.3/dataflows_airtable/load_from_airtable.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,17 +39,17 @@
         rollup='any',
         singleCollaborator='object',
         singleLineText='string',
         singleSelect='string',
         url='string',
     )
     EXTRA_FIELDS = dict(
-        dateTime=dict(
-            format='%Y-%m-%dT%H:%M:%S.%fZ'
-        ),
+        createdTime=dict(format='%Y-%m-%dT%H:%M:%S.%fZ'),
+        dateTime=dict(format='%Y-%m-%dT%H:%M:%S.%fZ'),
+        lastModifiedTime=dict(format='%Y-%m-%dT%H:%M:%S.%fZ'),
     )
 
 
     def describe_table():
         try:
             url = f'https://api.airtable.com/v0/meta/bases/{base}/tables'
             resp = rate_limiter.execute(lambda: session.get(url, timeout=10).json())
```

### Comparing `dataflows-airtable-0.1.2/dataflows_airtable/utilities.py` & `dataflows-airtable-0.1.3/dataflows_airtable/utilities.py`

 * *Files identical despite different names*

### Comparing `dataflows-airtable-0.1.2/dataflows_airtable.egg-info/PKG-INFO` & `dataflows-airtable-0.1.3/dataflows_airtable.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflows-airtable
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python library for adding AirTable support to dataflows
 Home-page: https://github.com/dataspot/dataflows-airtable
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Keywords: frictionless data,open data,airtable,dataflows,table schema,data package,tabular data package
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dataflows-airtable-0.1.2/dataflows_airtable.egg-info/SOURCES.txt` & `dataflows-airtable-0.1.3/dataflows_airtable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataflows-airtable-0.1.2/setup.py` & `dataflows-airtable-0.1.3/setup.py`

 * *Files identical despite different names*

