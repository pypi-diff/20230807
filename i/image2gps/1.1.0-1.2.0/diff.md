# Comparing `tmp/image2gps-1.1.0.tar.gz` & `tmp/image2gps-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2gps-1.1.0.tar", last modified: Fri Aug  4 16:14:28 2023, max compression
+gzip compressed data, was "image2gps-1.2.0.tar", last modified: Mon Aug  7 13:29:35 2023, max compression
```

## Comparing `image2gps-1.1.0.tar` & `image2gps-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-04 16:14:28.062861 image2gps-1.1.0/
--rw-r--r--   0 abionics   (501) staff       (20)     1068 2023-01-20 20:49:15.000000 image2gps-1.1.0/LICENSE.txt
--rw-r--r--   0 abionics   (501) staff       (20)     1622 2023-08-04 16:14:28.062928 image2gps-1.1.0/PKG-INFO
--rw-r--r--   0 abionics   (501) staff       (20)      722 2023-08-04 15:56:37.000000 image2gps-1.1.0/README.md
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-04 16:14:28.062160 image2gps-1.1.0/image2gps/
--rw-r--r--   0 abionics   (501) staff       (20)      200 2023-08-04 16:14:01.000000 image2gps-1.1.0/image2gps/__init__.py
--rw-r--r--   0 abionics   (501) staff       (20)      851 2023-08-04 15:56:37.000000 image2gps-1.1.0/image2gps/config.py
--rw-r--r--   0 abionics   (501) staff       (20)      352 2023-08-01 19:16:41.000000 image2gps-1.1.0/image2gps/fix_piexif.py
--rw-r--r--   0 abionics   (501) staff       (20)      674 2023-08-04 16:06:30.000000 image2gps-1.1.0/image2gps/image2gps.py
--rw-r--r--   0 abionics   (501) staff       (20)      844 2023-08-04 15:56:37.000000 image2gps-1.1.0/image2gps/parse_coords.py
--rw-r--r--   0 abionics   (501) staff       (20)     1166 2023-08-04 16:00:07.000000 image2gps-1.1.0/image2gps/parse_time.py
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-04 16:14:28.062773 image2gps-1.1.0/image2gps.egg-info/
--rw-r--r--   0 abionics   (501) staff       (20)     1622 2023-08-04 16:14:28.000000 image2gps-1.1.0/image2gps.egg-info/PKG-INFO
--rw-r--r--   0 abionics   (501) staff       (20)      375 2023-08-04 16:14:28.000000 image2gps-1.1.0/image2gps.egg-info/SOURCES.txt
--rw-r--r--   0 abionics   (501) staff       (20)        1 2023-08-04 16:14:28.000000 image2gps-1.1.0/image2gps.egg-info/dependency_links.txt
--rw-r--r--   0 abionics   (501) staff       (20)        1 2023-08-04 16:14:28.000000 image2gps-1.1.0/image2gps.egg-info/not-zip-safe
--rw-r--r--   0 abionics   (501) staff       (20)       21 2023-08-04 16:14:28.000000 image2gps-1.1.0/image2gps.egg-info/requires.txt
--rw-r--r--   0 abionics   (501) staff       (20)       10 2023-08-04 16:14:28.000000 image2gps-1.1.0/image2gps.egg-info/top_level.txt
--rw-r--r--   0 abionics   (501) staff       (20)       79 2023-08-04 16:14:28.063281 image2gps-1.1.0/setup.cfg
--rw-r--r--   0 abionics   (501) staff       (20)     1558 2023-08-04 15:56:37.000000 image2gps-1.1.0/setup.py
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-07 13:29:35.095244 image2gps-1.2.0/
+-rw-r--r--   0 abionics   (501) staff       (20)     1068 2023-01-20 20:49:15.000000 image2gps-1.2.0/LICENSE.txt
+-rw-r--r--   0 abionics   (501) staff       (20)     1711 2023-08-07 13:29:35.095324 image2gps-1.2.0/PKG-INFO
+-rw-r--r--   0 abionics   (501) staff       (20)      811 2023-08-07 13:20:08.000000 image2gps-1.2.0/README.md
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-07 13:29:35.094482 image2gps-1.2.0/image2gps/
+-rw-r--r--   0 abionics   (501) staff       (20)      200 2023-08-07 13:29:33.000000 image2gps-1.2.0/image2gps/__init__.py
+-rw-r--r--   0 abionics   (501) staff       (20)     1012 2023-08-07 13:25:25.000000 image2gps-1.2.0/image2gps/config.py
+-rw-r--r--   0 abionics   (501) staff       (20)      352 2023-08-01 19:16:41.000000 image2gps-1.2.0/image2gps/fix_piexif.py
+-rw-r--r--   0 abionics   (501) staff       (20)      674 2023-08-04 16:06:30.000000 image2gps-1.2.0/image2gps/image2gps.py
+-rw-r--r--   0 abionics   (501) staff       (20)      844 2023-08-04 15:56:37.000000 image2gps-1.2.0/image2gps/parse_coords.py
+-rw-r--r--   0 abionics   (501) staff       (20)     1842 2023-08-07 13:27:43.000000 image2gps-1.2.0/image2gps/parse_time.py
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-07 13:29:35.095147 image2gps-1.2.0/image2gps.egg-info/
+-rw-r--r--   0 abionics   (501) staff       (20)     1711 2023-08-07 13:29:35.000000 image2gps-1.2.0/image2gps.egg-info/PKG-INFO
+-rw-r--r--   0 abionics   (501) staff       (20)      375 2023-08-07 13:29:35.000000 image2gps-1.2.0/image2gps.egg-info/SOURCES.txt
+-rw-r--r--   0 abionics   (501) staff       (20)        1 2023-08-07 13:29:35.000000 image2gps-1.2.0/image2gps.egg-info/dependency_links.txt
+-rw-r--r--   0 abionics   (501) staff       (20)        1 2023-08-07 13:29:35.000000 image2gps-1.2.0/image2gps.egg-info/not-zip-safe
+-rw-r--r--   0 abionics   (501) staff       (20)       21 2023-08-07 13:29:35.000000 image2gps-1.2.0/image2gps.egg-info/requires.txt
+-rw-r--r--   0 abionics   (501) staff       (20)       10 2023-08-07 13:29:35.000000 image2gps-1.2.0/image2gps.egg-info/top_level.txt
+-rw-r--r--   0 abionics   (501) staff       (20)       79 2023-08-07 13:29:35.095647 image2gps-1.2.0/setup.cfg
+-rw-r--r--   0 abionics   (501) staff       (20)     1558 2023-08-04 15:56:37.000000 image2gps-1.2.0/setup.py
```

### Comparing `image2gps-1.1.0/LICENSE.txt` & `image2gps-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `image2gps-1.1.0/PKG-INFO` & `image2gps-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2gps
-Version: 1.1.0
+Version: 1.2.0
 Summary: Extract time and coords from image 🖼📍⏱️
 Home-page: https://github.com/abionics/image2gps
 Author: Alex Ermolaev
 Author-email: abionics.dev@gmail.com
 License: MIT
 Keywords: image gps location extract exif
 Classifier: Intended Audience :: Developers
@@ -45,15 +45,19 @@
 pip install image2gps
 ```
 
 
 ## Tests
 
 ```bash
-python -m pytest tests/test.py
+python -m pytest tests
+
+# or only certain tests
+python -m pytest tests/test_main.py
+python -m pytest tests/test_time.py
 ```
 
 
 ## More
 
 PyPI: https://pypi.org/project/image2gps
```

### Comparing `image2gps-1.1.0/image2gps/config.py` & `image2gps-1.2.0/image2gps/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 TimeType = datetime.datetime | None
 CoordsType = tuple[float, float] | None
 
 LOGGER = loguru.logger
 MIN_LOCATION_TIME = datetime.datetime(1960, 1, 1)
 MAX_LOCATION_TIMEDELTA = datetime.timedelta(days=10)
 
-# todo more patterns
+TIME_PATTERN = re.compile(r'\d{2}:\d{2}:\d{2}$')
 DATETIME_PATTENS = {
     re.compile(r'^\d{4}:\d{2}:\d{2} \d{2}:\d{2}:\d{2}$'): '%Y:%m:%d %H:%M:%S',
     re.compile(r'^\d{4}:\d{2}:\d{2}$'): '%Y:%m:%d',
     re.compile(r'^\d{4}:\d{2}:\d{2} \d{2}:\d{2}:\d{2}[-+]\d{2}:\d{2}$'): '%Y:%m:%d %H:%M:%S%z',
     re.compile(r'^\d{4}/\d{2}/\d{2} \d{2}:\d{2}:\d{2}$'): '%Y/%m/%d %H:%M:%S',
     re.compile(r'^\d{4}/\d{2}/\d{2}$'): '%Y/%m/%d',
     re.compile(r'^\d{2}/\d{2}/\d{4}$'): '%d/%m/%Y',
     re.compile(r'^\d{2}/\d{2}/\d{4} \d{1,2}:\d{2}$'): '%d/%m/%Y %H:%M',
     re.compile(r'^\d{2}/\d{2}/\d{4} \d{2}:\d{2}:\d{2}$'): '%d/%m/%Y %H:%M:%S',
+    re.compile(r'^\d{1,2} .{3} \d{4} \d{2}:\d{2}:\d{2}$'): '%d %b %Y %H:%M:%S',
+    re.compile(r'^\d{1,2} .{3} \d{4}$'): '%d %b %Y',
 }
```

### Comparing `image2gps-1.1.0/image2gps/image2gps.py` & `image2gps-1.2.0/image2gps/image2gps.py`

 * *Files identical despite different names*

### Comparing `image2gps-1.1.0/image2gps/parse_coords.py` & `image2gps-1.2.0/image2gps/parse_coords.py`

 * *Files identical despite different names*

### Comparing `image2gps-1.1.0/image2gps.egg-info/PKG-INFO` & `image2gps-1.2.0/image2gps.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2gps
-Version: 1.1.0
+Version: 1.2.0
 Summary: Extract time and coords from image 🖼📍⏱️
 Home-page: https://github.com/abionics/image2gps
 Author: Alex Ermolaev
 Author-email: abionics.dev@gmail.com
 License: MIT
 Keywords: image gps location extract exif
 Classifier: Intended Audience :: Developers
@@ -45,15 +45,19 @@
 pip install image2gps
 ```
 
 
 ## Tests
 
 ```bash
-python -m pytest tests/test.py
+python -m pytest tests
+
+# or only certain tests
+python -m pytest tests/test_main.py
+python -m pytest tests/test_time.py
 ```
 
 
 ## More
 
 PyPI: https://pypi.org/project/image2gps
```

### Comparing `image2gps-1.1.0/setup.py` & `image2gps-1.2.0/setup.py`

 * *Files identical despite different names*

