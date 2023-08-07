# Comparing `tmp/image2gps-1.2.0.tar.gz` & `tmp/image2gps-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2gps-1.2.0.tar", last modified: Mon Aug  7 13:29:35 2023, max compression
+gzip compressed data, was "image2gps-1.3.0.tar", last modified: Mon Aug  7 14:16:53 2023, max compression
```

## Comparing `image2gps-1.2.0.tar` & `image2gps-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-07 13:29:35.095244 image2gps-1.2.0/
--rw-r--r--   0 abionics   (501) staff       (20)     1068 2023-01-20 20:49:15.000000 image2gps-1.2.0/LICENSE.txt
--rw-r--r--   0 abionics   (501) staff       (20)     1711 2023-08-07 13:29:35.095324 image2gps-1.2.0/PKG-INFO
--rw-r--r--   0 abionics   (501) staff       (20)      811 2023-08-07 13:20:08.000000 image2gps-1.2.0/README.md
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-07 13:29:35.094482 image2gps-1.2.0/image2gps/
--rw-r--r--   0 abionics   (501) staff       (20)      200 2023-08-07 13:29:33.000000 image2gps-1.2.0/image2gps/__init__.py
--rw-r--r--   0 abionics   (501) staff       (20)     1012 2023-08-07 13:25:25.000000 image2gps-1.2.0/image2gps/config.py
--rw-r--r--   0 abionics   (501) staff       (20)      352 2023-08-01 19:16:41.000000 image2gps-1.2.0/image2gps/fix_piexif.py
--rw-r--r--   0 abionics   (501) staff       (20)      674 2023-08-04 16:06:30.000000 image2gps-1.2.0/image2gps/image2gps.py
--rw-r--r--   0 abionics   (501) staff       (20)      844 2023-08-04 15:56:37.000000 image2gps-1.2.0/image2gps/parse_coords.py
--rw-r--r--   0 abionics   (501) staff       (20)     1842 2023-08-07 13:27:43.000000 image2gps-1.2.0/image2gps/parse_time.py
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-07 13:29:35.095147 image2gps-1.2.0/image2gps.egg-info/
--rw-r--r--   0 abionics   (501) staff       (20)     1711 2023-08-07 13:29:35.000000 image2gps-1.2.0/image2gps.egg-info/PKG-INFO
--rw-r--r--   0 abionics   (501) staff       (20)      375 2023-08-07 13:29:35.000000 image2gps-1.2.0/image2gps.egg-info/SOURCES.txt
--rw-r--r--   0 abionics   (501) staff       (20)        1 2023-08-07 13:29:35.000000 image2gps-1.2.0/image2gps.egg-info/dependency_links.txt
--rw-r--r--   0 abionics   (501) staff       (20)        1 2023-08-07 13:29:35.000000 image2gps-1.2.0/image2gps.egg-info/not-zip-safe
--rw-r--r--   0 abionics   (501) staff       (20)       21 2023-08-07 13:29:35.000000 image2gps-1.2.0/image2gps.egg-info/requires.txt
--rw-r--r--   0 abionics   (501) staff       (20)       10 2023-08-07 13:29:35.000000 image2gps-1.2.0/image2gps.egg-info/top_level.txt
--rw-r--r--   0 abionics   (501) staff       (20)       79 2023-08-07 13:29:35.095647 image2gps-1.2.0/setup.cfg
--rw-r--r--   0 abionics   (501) staff       (20)     1558 2023-08-04 15:56:37.000000 image2gps-1.2.0/setup.py
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-07 14:16:53.388413 image2gps-1.3.0/
+-rw-r--r--   0 abionics   (501) staff       (20)     1068 2023-01-20 20:49:15.000000 image2gps-1.3.0/LICENSE.txt
+-rw-r--r--   0 abionics   (501) staff       (20)     1711 2023-08-07 14:16:53.388526 image2gps-1.3.0/PKG-INFO
+-rw-r--r--   0 abionics   (501) staff       (20)      811 2023-08-07 13:20:08.000000 image2gps-1.3.0/README.md
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-07 14:16:53.387518 image2gps-1.3.0/image2gps/
+-rw-r--r--   0 abionics   (501) staff       (20)      200 2023-08-07 14:15:22.000000 image2gps-1.3.0/image2gps/__init__.py
+-rw-r--r--   0 abionics   (501) staff       (20)     1040 2023-08-07 14:08:03.000000 image2gps-1.3.0/image2gps/config.py
+-rw-r--r--   0 abionics   (501) staff       (20)      269 2023-08-07 14:16:39.000000 image2gps-1.3.0/image2gps/failed.py
+-rw-r--r--   0 abionics   (501) staff       (20)      352 2023-08-01 19:16:41.000000 image2gps-1.3.0/image2gps/fix_piexif.py
+-rw-r--r--   0 abionics   (501) staff       (20)      674 2023-08-04 16:06:30.000000 image2gps-1.3.0/image2gps/image2gps.py
+-rw-r--r--   0 abionics   (501) staff       (20)     1009 2023-08-07 14:14:49.000000 image2gps-1.3.0/image2gps/parse_coords.py
+-rw-r--r--   0 abionics   (501) staff       (20)     1951 2023-08-07 14:14:49.000000 image2gps-1.3.0/image2gps/parse_time.py
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-08-07 14:16:53.388230 image2gps-1.3.0/image2gps.egg-info/
+-rw-r--r--   0 abionics   (501) staff       (20)     1711 2023-08-07 14:16:53.000000 image2gps-1.3.0/image2gps.egg-info/PKG-INFO
+-rw-r--r--   0 abionics   (501) staff       (20)      395 2023-08-07 14:16:53.000000 image2gps-1.3.0/image2gps.egg-info/SOURCES.txt
+-rw-r--r--   0 abionics   (501) staff       (20)        1 2023-08-07 14:16:53.000000 image2gps-1.3.0/image2gps.egg-info/dependency_links.txt
+-rw-r--r--   0 abionics   (501) staff       (20)        1 2023-08-07 14:16:53.000000 image2gps-1.3.0/image2gps.egg-info/not-zip-safe
+-rw-r--r--   0 abionics   (501) staff       (20)       32 2023-08-07 14:16:53.000000 image2gps-1.3.0/image2gps.egg-info/requires.txt
+-rw-r--r--   0 abionics   (501) staff       (20)       10 2023-08-07 14:16:53.000000 image2gps-1.3.0/image2gps.egg-info/top_level.txt
+-rw-r--r--   0 abionics   (501) staff       (20)       79 2023-08-07 14:16:53.388788 image2gps-1.3.0/setup.cfg
+-rw-r--r--   0 abionics   (501) staff       (20)     1580 2023-08-07 14:03:59.000000 image2gps-1.3.0/setup.py
```

### Comparing `image2gps-1.2.0/LICENSE.txt` & `image2gps-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `image2gps-1.2.0/PKG-INFO` & `image2gps-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2gps
-Version: 1.2.0
+Version: 1.3.0
 Summary: Extract time and coords from image 🖼📍⏱️
 Home-page: https://github.com/abionics/image2gps
 Author: Alex Ermolaev
 Author-email: abionics.dev@gmail.com
 License: MIT
 Keywords: image gps location extract exif
 Classifier: Intended Audience :: Developers
```

### Comparing `image2gps-1.2.0/README.md` & `image2gps-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `image2gps-1.2.0/image2gps/config.py` & `image2gps-1.3.0/image2gps/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 import loguru
 
 TimeType = datetime.datetime | None
 CoordsType = tuple[float, float] | None
 
 LOGGER = loguru.logger
+FAILED_CACHE_SIZES = 65536
+
 MIN_LOCATION_TIME = datetime.datetime(1960, 1, 1)
 MAX_LOCATION_TIMEDELTA = datetime.timedelta(days=10)
 
 TIME_PATTERN = re.compile(r'\d{2}:\d{2}:\d{2}$')
 DATETIME_PATTENS = {
     re.compile(r'^\d{4}:\d{2}:\d{2} \d{2}:\d{2}:\d{2}$'): '%Y:%m:%d %H:%M:%S',
     re.compile(r'^\d{4}:\d{2}:\d{2}$'): '%Y:%m:%d',
```

### Comparing `image2gps-1.2.0/image2gps/image2gps.py` & `image2gps-1.3.0/image2gps/image2gps.py`

 * *Files identical despite different names*

### Comparing `image2gps-1.2.0/image2gps/parse_coords.py` & `image2gps-1.3.0/image2gps/parse_coords.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import piexif
+from cachetools import LRUCache
 
-from image2gps.config import LOGGER, CoordsType
+from image2gps.config import CoordsType, FAILED_CACHE_SIZES
+from image2gps.failed import on_fail
+
+FAILED_CACHE = LRUCache(FAILED_CACHE_SIZES)
 
 
 def parse_coords(exif: dict) -> CoordsType:
     gps = exif.get('GPS')
     if gps is None or len(gps) == 0:
         return None
     lat = gps.get(piexif.GPSIFD.GPSLatitude)
     lon = gps.get(piexif.GPSIFD.GPSLongitude)
     if lat is None or lon is None:
-        LOGGER.debug(f'Failed to parse GPS "{gps}"')
+        gps_hash = hash(str(gps))
+        on_fail(gps_hash, f'Failed to parse GPS "{gps}"')
         return None
     lat, lon = _value_to_degrees(lat), _value_to_degrees(lon)
     if lat == 0 and lon == 0:
         return None
     return lat, lon
```

### Comparing `image2gps-1.2.0/image2gps/parse_time.py` & `image2gps-1.3.0/image2gps/parse_time.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import datetime
 
 import piexif
 
 from image2gps.config import (
     TimeType,
-    LOGGER,
     MIN_LOCATION_TIME,
     MAX_LOCATION_TIMEDELTA,
     TIME_PATTERN,
     DATETIME_PATTENS,
 )
+from image2gps.failed import on_fail
 
 
 def parse_time(exif: dict) -> TimeType:
     zero_th = exif.get('0th', {})
     time = zero_th.get(piexif.ImageIFD.DateTime)
     if time is None:
         return None
     try:
         time = time.replace(b'\x00', b'').strip().decode().removesuffix('Z').removesuffix(' г.')
         if len(time) == 0 or time.startswith('0000:00:00'):
             return None
         time = _string_to_datetime(time)
     except Exception as e:
-        LOGGER.debug(f'Failed to parse time "{time}" due to {e} ({type(e)})')
+        time_hash = hash(str(time))
+        on_fail(time_hash, f'Failed to parse time "{time}" due to {e} ({type(e)})')
         return None
     max_date = datetime.datetime.now() + MAX_LOCATION_TIMEDELTA
     if time < MIN_LOCATION_TIME or time > max_date:
-        LOGGER.debug(f'Date "{time}" is out of range')
+        time_hash = hash(str(time))
+        on_fail(time_hash, f'Date "{time}" is out of range')
         return None
     return time
 
 
 def _string_to_datetime(value: str) -> datetime.datetime:
     value = _fix_time_overflow(value)
     for pattern, timelike in DATETIME_PATTENS.items():
```

### Comparing `image2gps-1.2.0/image2gps.egg-info/PKG-INFO` & `image2gps-1.3.0/image2gps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2gps
-Version: 1.2.0
+Version: 1.3.0
 Summary: Extract time and coords from image 🖼📍⏱️
 Home-page: https://github.com/abionics/image2gps
 Author: Alex Ermolaev
 Author-email: abionics.dev@gmail.com
 License: MIT
 Keywords: image gps location extract exif
 Classifier: Intended Audience :: Developers
```

### Comparing `image2gps-1.2.0/setup.py` & `image2gps-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     url=URL,
     license='MIT',
     keywords='image gps location extract exif',
     install_requires=[
         'loguru',
         'pillow',
         'piexif',
+        'cachetools',
     ],
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
```

