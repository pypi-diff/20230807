# Comparing `tmp/mnzipcode-0.0.9.tar.gz` & `tmp/mnzipcode-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnzipcode-0.0.9.tar", last modified: Thu Jun 15 10:02:53 2023, max compression
+gzip compressed data, was "mnzipcode-0.1.0.tar", last modified: Mon Aug  7 07:20:53 2023, max compression
```

## Comparing `mnzipcode-0.0.9.tar` & `mnzipcode-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,14 @@
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 10:02:53.185593 mnzipcode-0.0.9/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1033 2023-06-15 10:02:53.185593 mnzipcode-0.0.9/PKG-INFO
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1000 2023-06-15 09:22:59.000000 mnzipcode-0.0.9/README.md
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 10:02:53.181593 mnzipcode-0.0.9/mnzipcode/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       25 2023-05-07 07:52:13.000000 mnzipcode-0.0.9/mnzipcode/__init__.py
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 10:02:53.185593 mnzipcode-0.0.9/mnzipcode/data/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2107 2023-06-15 09:46:17.000000 mnzipcode-0.0.9/mnzipcode/data/duureg_info.json
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     2981 2023-05-07 07:22:37.000000 mnzipcode-0.0.9/mnzipcode/data/province_info.json
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        0 2023-05-07 06:16:51.000000 mnzipcode-0.0.9/mnzipcode/data/sum_info.json
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)   140107 2023-05-07 07:07:44.000000 mnzipcode-0.0.9/mnzipcode/data/zip.json
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     4275 2023-06-15 09:58:58.000000 mnzipcode-0.0.9/mnzipcode/mnZipCodes.py
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-06-15 10:02:53.181593 mnzipcode-0.0.9/mnzipcode.egg-info/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1033 2023-06-15 10:02:53.000000 mnzipcode-0.0.9/mnzipcode.egg-info/PKG-INFO
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      315 2023-06-15 10:02:53.000000 mnzipcode-0.0.9/mnzipcode.egg-info/SOURCES.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        1 2023-06-15 10:02:53.000000 mnzipcode-0.0.9/mnzipcode.egg-info/dependency_links.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       10 2023-06-15 10:02:53.000000 mnzipcode-0.0.9/mnzipcode.egg-info/top_level.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       38 2023-06-15 10:02:53.185593 mnzipcode-0.0.9/setup.cfg
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1184 2023-06-15 09:59:31.000000 mnzipcode-0.0.9/setup.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 07:20:53.330335 mnzipcode-0.1.0/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1442 2023-08-07 07:20:53.330335 mnzipcode-0.1.0/PKG-INFO
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1125 2023-08-07 07:00:10.000000 mnzipcode-0.1.0/README.md
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 07:20:53.330335 mnzipcode-0.1.0/mnzipcode/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      104 2023-08-07 06:34:57.000000 mnzipcode-0.1.0/mnzipcode/__init__.py
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)    15460 2023-08-07 05:33:10.000000 mnzipcode-0.1.0/mnzipcode/data.json.bz2
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1948 2023-08-07 06:34:30.000000 mnzipcode-0.1.0/mnzipcode/mnzipcode.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-08-07 07:20:53.330335 mnzipcode-0.1.0/mnzipcode.egg-info/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1442 2023-08-07 07:20:53.000000 mnzipcode-0.1.0/mnzipcode.egg-info/PKG-INFO
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      219 2023-08-07 07:20:53.000000 mnzipcode-0.1.0/mnzipcode.egg-info/SOURCES.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        1 2023-08-07 07:20:53.000000 mnzipcode-0.1.0/mnzipcode.egg-info/dependency_links.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       10 2023-08-07 07:20:53.000000 mnzipcode-0.1.0/mnzipcode.egg-info/top_level.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       38 2023-08-07 07:20:53.330335 mnzipcode-0.1.0/setup.cfg
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      560 2023-08-07 06:49:23.000000 mnzipcode-0.1.0/setup.py
```

### Comparing `mnzipcode-0.0.9/README.md` & `mnzipcode-0.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,68 @@
-# mnzipcodes
-mnzipcodes is a simple library for querying Mongolian zip codes.
+Metadata-Version: 2.1
+Name: mnzipcode
+Version: 0.1.0
+Summary: mnzipcodes is a simple library for querying Mongolian zip codes.
+Home-page: https://github.com/bekkage/mnzipcode
+Author: Bekkage
+Author-email: bilguunsec@gmail.com
+Keywords: mnzipcode zipcode mongolia mn zip code
+Description-Content-Type: text/markdown
+
+# mnzipcode
+mnzipcode is a simple library for querying Mongolian zip codes.
 
   - Video introduction: [YOUTUBE](https://www.youtube.com/watch?v=vml3CxglLko)
   - PYPI: [MNZIPCODE](https://pypi.org/project/mnzipcode/)
 
 ### Installation
 
 mnzipcode is available on PyPi:
 ```
 # python -m pip install mnzipcode
 ```
 
 ### Example usage:
 
 ```python
->>> import mnzipcode
->>> 
->>> obj = mnzipcode.ZipCode()
->>> 
->>> obj.matching_by_zipcode(11000)
-{'name': 'Ulaanbaatar', 'stat': 'province', 'mnname': 'Улаанбаатар', 'year_established': 1942, 'area': 4704.4, 'population': 1539810, 'density': 327}
->>> 
->>> obj.matching_by_name('Дархан-Уул')
-[{'name': 'Darkhan-Uul', 'zipcode': '45000', 'stat': 'province', 'mnname': 'Дархан-Уул', 'year_established': 1994, 'area': 3275.0, 'population': 107018, 'density': 33}, {'name': 'Дархан-Уул', 'zipcode': '81041', 'stat': 'bag'}, {'name': 'Дархан-Уул', 'zipcode': '81063', 'stat': 'bag'}]
->>> 
->>> obj.isReal(11000)
+>>> import mnzipcode 
+
+
+>>> mnzipcode.matching_by_zipcode(11000)
+{
+  'stat': 'capital', 
+  'mnname': 'Улаанбаатар', 
+  'name': 'Ulaanbaatar', 
+  'year_established': 1942, 
+  'area': 4704.4, 
+  'population': 1539810, 
+  'density': 327, 
+  'zipcode': '11000'
+}
+
+
+>>> mnzipcode.filter(mnname='Дархан-Уул')
+[
+  {
+    'stat': 'province', 
+    'mnname': 'Дархан-Уул', 
+    'name': 'Darkhan-Uul', 
+    'year_established': 1994, 
+    'area': 3275.0, 
+    'population': 107018, 
+    'density': 33, 
+    'zipcode': '45000', 
+    'capital': 'Darkhan', 
+    'capitalmn': 'Дархан'}, 
+  {
+    'mnname': 'Дархан-Уул', 
+    'zipcode': '81041'
+  }, 
+  {
+    'mnname': 'Дархан-Уул', 
+    'zipcode': '81063'
+  }
+]
+
+>>> mnzipcode.is_real(11000)
 True
-```
+```
```

### Comparing `mnzipcode-0.0.9/setup.py` & `mnzipcode-0.1.0/mnzipcode.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,68 @@
-import setuptools 
+Metadata-Version: 2.1
+Name: mnzipcode
+Version: 0.1.0
+Summary: mnzipcodes is a simple library for querying Mongolian zip codes.
+Home-page: https://github.com/bekkage/mnzipcode
+Author: Bekkage
+Author-email: bilguunsec@gmail.com
+Keywords: mnzipcode zipcode mongolia mn zip code
+Description-Content-Type: text/markdown
 
-setuptools.setup(
-  name='mnzipcode',
-  version='0.0.9',
-  author='Bekkage',
-  description='mnzipcodes is a simple library for querying Mongolian zip codes.',
-  package_data={
-    'mnzipcode': ['data/*.json']
-  },
-  long_description_content_type= 'text/markdown',
-  long_description="""
+# mnzipcode
 mnzipcode is a simple library for querying Mongolian zip codes.
 
+  - Video introduction: [YOUTUBE](https://www.youtube.com/watch?v=vml3CxglLko)
+  - PYPI: [MNZIPCODE](https://pypi.org/project/mnzipcode/)
+
 ### Installation
 
 mnzipcode is available on PyPi:
 ```
 # python -m pip install mnzipcode
 ```
 
-Example usage:
+### Example usage:
 
 ```python
->>> import mnzipcode
->>> 
->>> obj = mnzipcode.ZipCode()
->>> 
->>> obj.matching_by_zipcode(11000)
-{'name': 'Ulaanbaatar', 'stat': 'province', 'mnname': 'Улаанбаатар', 'year_established': 1942, 'area': 4704.4, 'population': 1539810, 'density': 327}
->>> 
->>> obj.matching_by_name('Дархан-Уул')
-[{'name': 'Darkhan-Uul', 'zipcode': '45000', 'stat': 'province', 'mnname': 'Дархан-Уул', 'year_established': 1994, 'area': 3275.0, 'population': 107018, 'density': 33}, {'name': 'Дархан-Уул', 'zipcode': '81041', 'stat': 'bag'}, {'name': 'Дархан-Уул', 'zipcode': '81063', 'stat': 'bag'}]
->>> 
->>> obj.isReal(11000)
+>>> import mnzipcode 
+
+
+>>> mnzipcode.matching_by_zipcode(11000)
+{
+  'stat': 'capital', 
+  'mnname': 'Улаанбаатар', 
+  'name': 'Ulaanbaatar', 
+  'year_established': 1942, 
+  'area': 4704.4, 
+  'population': 1539810, 
+  'density': 327, 
+  'zipcode': '11000'
+}
+
+
+>>> mnzipcode.filter(mnname='Дархан-Уул')
+[
+  {
+    'stat': 'province', 
+    'mnname': 'Дархан-Уул', 
+    'name': 'Darkhan-Uul', 
+    'year_established': 1994, 
+    'area': 3275.0, 
+    'population': 107018, 
+    'density': 33, 
+    'zipcode': '45000', 
+    'capital': 'Darkhan', 
+    'capitalmn': 'Дархан'}, 
+  {
+    'mnname': 'Дархан-Уул', 
+    'zipcode': '81041'
+  }, 
+  {
+    'mnname': 'Дархан-Уул', 
+    'zipcode': '81063'
+  }
+]
+
+>>> mnzipcode.is_real(11000)
 True
 ```
-
-  """,
-  package=['mnzipcode']
-)
```

