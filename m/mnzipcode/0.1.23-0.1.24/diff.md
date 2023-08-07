# Comparing `tmp/mnzipcode-0.1.23.tar.gz` & `tmp/mnzipcode-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnzipcode-0.1.23.tar", last modified: Mon Aug  7 08:10:11 2023, max compression
+gzip compressed data, was "mnzipcode-0.1.24.tar", last modified: Mon Aug  7 08:12:58 2023, max compression
```

## Comparing `mnzipcode-0.1.23.tar` & `mnzipcode-0.1.24.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:10:11.017012 mnzipcode-0.1.23/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1442 2023-08-07 08:10:11.017012 mnzipcode-0.1.23/PKG-INFO
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1125 2023-08-07 07:00:10.000000 mnzipcode-0.1.23/README.md
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:10:11.017012 mnzipcode-0.1.23/mnzipcode/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      138 2023-08-07 08:06:11.000000 mnzipcode-0.1.23/mnzipcode/__init__.py
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)    15460 2023-08-07 05:33:10.000000 mnzipcode-0.1.23/mnzipcode/data.json.bz2
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2547 2023-08-07 08:10:04.000000 mnzipcode-0.1.23/mnzipcode/mnzipcode.py
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:10:11.017012 mnzipcode-0.1.23/mnzipcode.egg-info/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1442 2023-08-07 08:10:10.000000 mnzipcode-0.1.23/mnzipcode.egg-info/PKG-INFO
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      219 2023-08-07 08:10:10.000000 mnzipcode-0.1.23/mnzipcode.egg-info/SOURCES.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        1 2023-08-07 08:10:10.000000 mnzipcode-0.1.23/mnzipcode.egg-info/dependency_links.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       10 2023-08-07 08:10:10.000000 mnzipcode-0.1.23/mnzipcode.egg-info/top_level.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       38 2023-08-07 08:10:11.017012 mnzipcode-0.1.23/setup.cfg
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      557 2023-08-07 08:10:07.000000 mnzipcode-0.1.23/setup.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:12:58.105228 mnzipcode-0.1.24/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1810 2023-08-07 08:12:58.105228 mnzipcode-0.1.24/PKG-INFO
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1493 2023-08-07 08:11:58.000000 mnzipcode-0.1.24/README.md
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:12:58.105228 mnzipcode-0.1.24/mnzipcode/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      138 2023-08-07 08:06:11.000000 mnzipcode-0.1.24/mnzipcode/__init__.py
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)    15460 2023-08-07 05:33:10.000000 mnzipcode-0.1.24/mnzipcode/data.json.bz2
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2547 2023-08-07 08:12:45.000000 mnzipcode-0.1.24/mnzipcode/mnzipcode.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:12:58.105228 mnzipcode-0.1.24/mnzipcode.egg-info/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1810 2023-08-07 08:12:58.000000 mnzipcode-0.1.24/mnzipcode.egg-info/PKG-INFO
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      219 2023-08-07 08:12:58.000000 mnzipcode-0.1.24/mnzipcode.egg-info/SOURCES.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        1 2023-08-07 08:12:58.000000 mnzipcode-0.1.24/mnzipcode.egg-info/dependency_links.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       10 2023-08-07 08:12:58.000000 mnzipcode-0.1.24/mnzipcode.egg-info/top_level.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       38 2023-08-07 08:12:58.105228 mnzipcode-0.1.24/setup.cfg
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      557 2023-08-07 08:12:42.000000 mnzipcode-0.1.24/setup.py
```

### Comparing `mnzipcode-0.1.23/PKG-INFO` & `mnzipcode-0.1.24/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnzipcode
-Version: 0.1.23
+Version: 0.1.24
 Summary: mnzipcode is a simple library for querying Mongolian zip codes.
 Home-page: https://github.com/bekkage/mnzipcode
 Author: Bekkage
 Author-email: bilguunsec@gmail.com
 Keywords: mnzipcode zipcode mongolia mn zip code
 Description-Content-Type: text/markdown
 
@@ -61,8 +61,30 @@
     'mnname': 'Дархан-Уул', 
     'zipcode': '81063'
   }
 ]
 
 >>> mnzipcode.is_real(11000)
 True
+
+>>> mnzipcode.similar_to(8501)
+[
+  {'mnname': 'Зүүнхангай', 
+  'zipcode': '85010'
+  }, 
+  {
+    'mnname': 'Даланбулаг', 
+    'zipcode': '85011'
+  }, 
+  {
+    'mnname': 'Хайрхан', 'zipcode': '85013'
+  }, 
+  {
+    'mnname': 'Жаргалант', 
+    'zipcode': '85015'
+  }, 
+  {
+    'mnname': 'Баянгол', 
+    'zipcode': '85017'
+  }
+]
 ```
```

### Comparing `mnzipcode-0.1.23/README.md` & `mnzipcode-0.1.24/mnzipcode.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: mnzipcode
+Version: 0.1.24
+Summary: mnzipcode is a simple library for querying Mongolian zip codes.
+Home-page: https://github.com/bekkage/mnzipcode
+Author: Bekkage
+Author-email: bilguunsec@gmail.com
+Keywords: mnzipcode zipcode mongolia mn zip code
+Description-Content-Type: text/markdown
+
 # mnzipcode
 mnzipcode is a simple library for querying Mongolian zip codes.
 
   - Video introduction: [YOUTUBE](https://www.youtube.com/watch?v=vml3CxglLko)
   - PYPI: [MNZIPCODE](https://pypi.org/project/mnzipcode/)
 
 ### Installation
@@ -51,8 +61,30 @@
     'mnname': 'Дархан-Уул', 
     'zipcode': '81063'
   }
 ]
 
 >>> mnzipcode.is_real(11000)
 True
-```
+
+>>> mnzipcode.similar_to(8501)
+[
+  {'mnname': 'Зүүнхангай', 
+  'zipcode': '85010'
+  }, 
+  {
+    'mnname': 'Даланбулаг', 
+    'zipcode': '85011'
+  }, 
+  {
+    'mnname': 'Хайрхан', 'zipcode': '85013'
+  }, 
+  {
+    'mnname': 'Жаргалант', 
+    'zipcode': '85015'
+  }, 
+  {
+    'mnname': 'Баянгол', 
+    'zipcode': '85017'
+  }
+]
+```
```

### Comparing `mnzipcode-0.1.23/mnzipcode/data.json.bz2` & `mnzipcode-0.1.24/mnzipcode/data.json.bz2`

 * *Files identical despite different names*

### Comparing `mnzipcode-0.1.23/mnzipcode/mnzipcode.py` & `mnzipcode-0.1.24/mnzipcode/mnzipcode.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from os import path 
 from sys import version_info
 
 
 __author__: str = 'Bilguun Ganchuluun'
 __email__: str = 'bilguunsec@gmail.com'
 __package__: str = 'mnzipcode'
-__version__: str = '0.1.23'
+__version__: str = '0.1.24'
 
 VALID_ZIPCODE_LENGTH: int = 5
 
 def get_resource_path(relative_path) -> str:
   try: 
     # for PyInstaller
     from sys import _MEIPASS
```

### Comparing `mnzipcode-0.1.23/setup.py` & `mnzipcode-0.1.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open('README.md') as f: 
   readme = f.read()
 
 setuptools.setup(
   name='mnzipcode',
-  version='0.1.23',
+  version='0.1.24',
   author='Bekkage',
   author_email='bilguunsec@gmail.com',
   url='https://github.com/bekkage/mnzipcode',
   description='mnzipcode is a simple library for querying Mongolian zip codes.',
   package_data={
     'mnzipcode': ['data.json.bz2']
   },
```

