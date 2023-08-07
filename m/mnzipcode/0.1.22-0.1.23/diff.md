# Comparing `tmp/mnzipcode-0.1.22.tar.gz` & `tmp/mnzipcode-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnzipcode-0.1.22.tar", last modified: Mon Aug  7 08:08:07 2023, max compression
+gzip compressed data, was "mnzipcode-0.1.23.tar", last modified: Mon Aug  7 08:10:11 2023, max compression
```

## Comparing `mnzipcode-0.1.22.tar` & `mnzipcode-0.1.23.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:08:07.009884 mnzipcode-0.1.22/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1442 2023-08-07 08:08:07.009884 mnzipcode-0.1.22/PKG-INFO
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1125 2023-08-07 07:00:10.000000 mnzipcode-0.1.22/README.md
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:08:07.009884 mnzipcode-0.1.22/mnzipcode/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      138 2023-08-07 08:06:11.000000 mnzipcode-0.1.22/mnzipcode/__init__.py
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)    15460 2023-08-07 05:33:10.000000 mnzipcode-0.1.22/mnzipcode/data.json.bz2
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2534 2023-08-07 08:07:59.000000 mnzipcode-0.1.22/mnzipcode/mnzipcode.py
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:08:07.009884 mnzipcode-0.1.22/mnzipcode.egg-info/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1442 2023-08-07 08:08:06.000000 mnzipcode-0.1.22/mnzipcode.egg-info/PKG-INFO
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      219 2023-08-07 08:08:06.000000 mnzipcode-0.1.22/mnzipcode.egg-info/SOURCES.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        1 2023-08-07 08:08:06.000000 mnzipcode-0.1.22/mnzipcode.egg-info/dependency_links.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       10 2023-08-07 08:08:06.000000 mnzipcode-0.1.22/mnzipcode.egg-info/top_level.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       38 2023-08-07 08:08:07.009884 mnzipcode-0.1.22/setup.cfg
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      557 2023-08-07 08:08:03.000000 mnzipcode-0.1.22/setup.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:10:11.017012 mnzipcode-0.1.23/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1442 2023-08-07 08:10:11.017012 mnzipcode-0.1.23/PKG-INFO
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1125 2023-08-07 07:00:10.000000 mnzipcode-0.1.23/README.md
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:10:11.017012 mnzipcode-0.1.23/mnzipcode/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      138 2023-08-07 08:06:11.000000 mnzipcode-0.1.23/mnzipcode/__init__.py
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)    15460 2023-08-07 05:33:10.000000 mnzipcode-0.1.23/mnzipcode/data.json.bz2
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2547 2023-08-07 08:10:04.000000 mnzipcode-0.1.23/mnzipcode/mnzipcode.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:10:11.017012 mnzipcode-0.1.23/mnzipcode.egg-info/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1442 2023-08-07 08:10:10.000000 mnzipcode-0.1.23/mnzipcode.egg-info/PKG-INFO
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      219 2023-08-07 08:10:10.000000 mnzipcode-0.1.23/mnzipcode.egg-info/SOURCES.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        1 2023-08-07 08:10:10.000000 mnzipcode-0.1.23/mnzipcode.egg-info/dependency_links.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       10 2023-08-07 08:10:10.000000 mnzipcode-0.1.23/mnzipcode.egg-info/top_level.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       38 2023-08-07 08:10:11.017012 mnzipcode-0.1.23/setup.cfg
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      557 2023-08-07 08:10:07.000000 mnzipcode-0.1.23/setup.py
```

### Comparing `mnzipcode-0.1.22/PKG-INFO` & `mnzipcode-0.1.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnzipcode
-Version: 0.1.22
+Version: 0.1.23
 Summary: mnzipcode is a simple library for querying Mongolian zip codes.
 Home-page: https://github.com/bekkage/mnzipcode
 Author: Bekkage
 Author-email: bilguunsec@gmail.com
 Keywords: mnzipcode zipcode mongolia mn zip code
 Description-Content-Type: text/markdown
```

### Comparing `mnzipcode-0.1.22/README.md` & `mnzipcode-0.1.23/README.md`

 * *Files identical despite different names*

### Comparing `mnzipcode-0.1.22/mnzipcode/data.json.bz2` & `mnzipcode-0.1.23/mnzipcode/data.json.bz2`

 * *Files identical despite different names*

### Comparing `mnzipcode-0.1.22/mnzipcode/mnzipcode.py` & `mnzipcode-0.1.23/mnzipcode/mnzipcode.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from os import path 
 from sys import version_info
 
 
 __author__: str = 'Bilguun Ganchuluun'
 __email__: str = 'bilguunsec@gmail.com'
 __package__: str = 'mnzipcode'
-__version__: str = '0.1.22'
+__version__: str = '0.1.23'
 
 VALID_ZIPCODE_LENGTH: int = 5
 
 def get_resource_path(relative_path) -> str:
   try: 
     # for PyInstaller
     from sys import _MEIPASS
@@ -47,32 +47,32 @@
     
     if 'sub_items' in _it: 
       return_data = matching_by_zipcode(zipcode, _it['sub_items'])
       if return_data: 
         return return_data
   return None 
 
-def similar_to(zipcode: int, data: dict = DATA['zipcode']) -> dict: 
+def similar_to(zipcode: int, data: dict = DATA['zipcode']) -> list: 
   similar_data: list = []
   for _it in data:
-    if _it['zipcode'].startswith(zipcode):
+    if _it['zipcode'].startswith(str(zipcode)):
       if 'sub_items' in _it: 
         filtered_dict: dict = _it.copy()
         filtered_dict.pop('sub_items', None) 
         similar_data.append(filtered_dict)
       else: 
         similar_data.append(_it)
     
     if 'sub_items' in _it: 
       return_data = similar_to(zipcode, _it['sub_items'])
       if return_data: 
         [similar_data.append(_ret_data) for _ret_data in return_data]
   return similar_data 
 
-def filter(data: dict = DATA['zipcode'], **filter_values):
+def filter(data: dict = DATA['zipcode'], **filter_values) -> list:
   filtered_data: list = []
   for _it in data:
     if all([key in _it and _it[key] == value for key, value in filter_values.items()]):
       filtered__it_dict: dict = _it.copy()
       filtered__it_dict.pop('sub_items', None) 
       filtered_data.append(filtered__it_dict)
```

### Comparing `mnzipcode-0.1.22/mnzipcode.egg-info/PKG-INFO` & `mnzipcode-0.1.23/mnzipcode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnzipcode
-Version: 0.1.22
+Version: 0.1.23
 Summary: mnzipcode is a simple library for querying Mongolian zip codes.
 Home-page: https://github.com/bekkage/mnzipcode
 Author: Bekkage
 Author-email: bilguunsec@gmail.com
 Keywords: mnzipcode zipcode mongolia mn zip code
 Description-Content-Type: text/markdown
```

### Comparing `mnzipcode-0.1.22/setup.py` & `mnzipcode-0.1.23/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open('README.md') as f: 
   readme = f.read()
 
 setuptools.setup(
   name='mnzipcode',
-  version='0.1.22',
+  version='0.1.23',
   author='Bekkage',
   author_email='bilguunsec@gmail.com',
   url='https://github.com/bekkage/mnzipcode',
   description='mnzipcode is a simple library for querying Mongolian zip codes.',
   package_data={
     'mnzipcode': ['data.json.bz2']
   },
```

