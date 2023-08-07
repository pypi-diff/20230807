# Comparing `tmp/mnzipcode-0.1.1.tar.gz` & `tmp/mnzipcode-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnzipcode-0.1.1.tar", last modified: Mon Aug  7 08:02:04 2023, max compression
+gzip compressed data, was "mnzipcode-0.1.2.tar", last modified: Mon Aug  7 08:05:07 2023, max compression
```

## Comparing `mnzipcode-0.1.1.tar` & `mnzipcode-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:02:04.584741 mnzipcode-0.1.1/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1441 2023-08-07 08:02:04.584741 mnzipcode-0.1.1/PKG-INFO
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1125 2023-08-07 07:00:10.000000 mnzipcode-0.1.1/README.md
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:02:04.584741 mnzipcode-0.1.1/mnzipcode/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      104 2023-08-07 06:34:57.000000 mnzipcode-0.1.1/mnzipcode/__init__.py
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2531 2023-08-07 08:01:43.000000 mnzipcode-0.1.1/mnzipcode/mnzipcode.py
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:02:04.584741 mnzipcode-0.1.1/mnzipcode.egg-info/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1441 2023-08-07 08:02:04.000000 mnzipcode-0.1.1/mnzipcode.egg-info/PKG-INFO
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      195 2023-08-07 08:02:04.000000 mnzipcode-0.1.1/mnzipcode.egg-info/SOURCES.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        1 2023-08-07 08:02:04.000000 mnzipcode-0.1.1/mnzipcode.egg-info/dependency_links.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       10 2023-08-07 08:02:04.000000 mnzipcode-0.1.1/mnzipcode.egg-info/top_level.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       38 2023-08-07 08:02:04.584741 mnzipcode-0.1.1/setup.cfg
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      559 2023-08-07 08:01:38.000000 mnzipcode-0.1.1/setup.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:05:07.949367 mnzipcode-0.1.2/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1441 2023-08-07 08:05:07.949367 mnzipcode-0.1.2/PKG-INFO
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1125 2023-08-07 07:00:10.000000 mnzipcode-0.1.2/README.md
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:05:07.949367 mnzipcode-0.1.2/mnzipcode/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      104 2023-08-07 06:34:57.000000 mnzipcode-0.1.2/mnzipcode/__init__.py
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)    15460 2023-08-07 05:33:10.000000 mnzipcode-0.1.2/mnzipcode/data.json.bz2
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2531 2023-08-07 08:05:05.000000 mnzipcode-0.1.2/mnzipcode/mnzipcode.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 08:05:07.949367 mnzipcode-0.1.2/mnzipcode.egg-info/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1441 2023-08-07 08:05:07.000000 mnzipcode-0.1.2/mnzipcode.egg-info/PKG-INFO
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      219 2023-08-07 08:05:07.000000 mnzipcode-0.1.2/mnzipcode.egg-info/SOURCES.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        1 2023-08-07 08:05:07.000000 mnzipcode-0.1.2/mnzipcode.egg-info/dependency_links.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       10 2023-08-07 08:05:07.000000 mnzipcode-0.1.2/mnzipcode.egg-info/top_level.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       38 2023-08-07 08:05:07.949367 mnzipcode-0.1.2/setup.cfg
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      556 2023-08-07 08:05:00.000000 mnzipcode-0.1.2/setup.py
```

### Comparing `mnzipcode-0.1.1/PKG-INFO` & `mnzipcode-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnzipcode
-Version: 0.1.1
+Version: 0.1.2
 Summary: mnzipcode is a simple library for querying Mongolian zip codes.
 Home-page: https://github.com/bekkage/mnzipcode
 Author: Bekkage
 Author-email: bilguunsec@gmail.com
 Keywords: mnzipcode zipcode mongolia mn zip code
 Description-Content-Type: text/markdown
```

### Comparing `mnzipcode-0.1.1/README.md` & `mnzipcode-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mnzipcode-0.1.1/mnzipcode/mnzipcode.py` & `mnzipcode-0.1.2/mnzipcode/mnzipcode.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from os import path 
 from sys import version_info
 
 
 __author__: str = 'Bilguun Ganchuluun'
 __email__: str = 'bilguunsec@gmail.com'
 __package__: str = 'mnzipcode'
-__version__: str = '0.1.1'
+__version__: str = '0.1.2'
 
 VALID_ZIPCODE_LENGTH: int = 5
 
 def get_resource_path(relative_path) -> str:
   try: 
     # for PyInstaller
     from sys import _MEIPASS
```

### Comparing `mnzipcode-0.1.1/mnzipcode.egg-info/PKG-INFO` & `mnzipcode-0.1.2/mnzipcode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnzipcode
-Version: 0.1.1
+Version: 0.1.2
 Summary: mnzipcode is a simple library for querying Mongolian zip codes.
 Home-page: https://github.com/bekkage/mnzipcode
 Author: Bekkage
 Author-email: bilguunsec@gmail.com
 Keywords: mnzipcode zipcode mongolia mn zip code
 Description-Content-Type: text/markdown
```

### Comparing `mnzipcode-0.1.1/setup.py` & `mnzipcode-0.1.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools 
 
 with open('README.md') as f: 
   readme = f.read()
 
 setuptools.setup(
   name='mnzipcode',
-  version='0.1.1',
+  version='0.1.2',
   author='Bekkage',
   author_email='bilguunsec@gmail.com',
   url='https://github.com/bekkage/mnzipcode',
   description='mnzipcode is a simple library for querying Mongolian zip codes.',
-  #package_data={
-  #  'mnzipcode': ['data.json.bz2']
-  #},
+  package_data={
+    'mnzipcode': ['data.json.bz2']
+  },
   long_description_content_type= 'text/markdown',
   long_description=readme,
   keywords='mnzipcode zipcode mongolia mn zip code',
   package=['mnzipcode'],
   include_package_data=True,
 )
```

