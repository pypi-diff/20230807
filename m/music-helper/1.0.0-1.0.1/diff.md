# Comparing `tmp/music-helper-1.0.0.tar.gz` & `tmp/music-helper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "music-helper-1.0.0.tar", last modified: Mon Aug  7 15:26:04 2023, max compression
+gzip compressed data, was "music-helper-1.0.1.tar", last modified: Mon Aug  7 15:31:05 2023, max compression
```

## Comparing `music-helper-1.0.0.tar` & `music-helper-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 15:26:04.276059 music-helper-1.0.0/
--rw-rw-rw-   0        0        0     2591 2023-08-07 15:26:04.272084 music-helper-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2207 2023-08-07 15:18:15.000000 music-helper-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 15:26:04.210237 music-helper-1.0.0/music_helper.egg-info/
--rw-rw-rw-   0        0        0     2591 2023-08-07 15:26:03.000000 music-helper-1.0.0/music_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      625 2023-08-07 15:26:03.000000 music-helper-1.0.0/music_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 15:26:03.000000 music-helper-1.0.0/music_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-08-07 15:26:03.000000 music-helper-1.0.0/music_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-07 15:26:03.000000 music-helper-1.0.0/music_helper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-07 15:26:04.236175 music-helper-1.0.0/musichelper/
--rw-rw-rw-   0        0        0    28180 2023-08-07 14:36:36.000000 music-helper-1.0.0/musichelper/Deezer.py
--rw-rw-rw-   0        0        0     2512 2023-08-07 14:35:14.000000 music-helper-1.0.0/musichelper/MusicHelper.py
--rw-rw-rw-   0        0        0     9135 2023-08-07 14:53:43.000000 music-helper-1.0.0/musichelper/SoundCloud.py
--rw-rw-rw-   0        0        0     9819 2023-08-07 15:13:19.000000 music-helper-1.0.0/musichelper/YTM.py
--rw-rw-rw-   0        0        0       49 2023-08-06 11:27:03.000000 music-helper-1.0.0/musichelper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 15:26:04.269076 music-helper-1.0.0/musichelper/constants/
--rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 music-helper-1.0.0/musichelper/constants/__init__.py
--rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 music-helper-1.0.0/musichelper/constants/api_methods.py
--rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 music-helper-1.0.0/musichelper/constants/api_urls.py
--rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 music-helper-1.0.0/musichelper/constants/image_hosts.py
--rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 music-helper-1.0.0/musichelper/constants/networking_settings.py
--rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 music-helper-1.0.0/musichelper/constants/search_types.py
--rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 music-helper-1.0.0/musichelper/constants/track_formats.py
--rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 music-helper-1.0.0/musichelper/exceptions.py
--rw-rw-rw-   0        0        0     3354 2023-08-07 15:16:58.000000 music-helper-1.0.0/musichelper/util.py
--rw-rw-rw-   0        0        0       42 2023-08-07 15:26:04.276059 music-helper-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      870 2023-08-07 15:24:59.000000 music-helper-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:31:05.580372 music-helper-1.0.1/
+-rw-rw-rw-   0        0        0     2593 2023-08-07 15:31:05.579375 music-helper-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2207 2023-08-07 15:30:15.000000 music-helper-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 15:31:05.528513 music-helper-1.0.1/music_helper.egg-info/
+-rw-rw-rw-   0        0        0     2593 2023-08-07 15:31:05.000000 music-helper-1.0.1/music_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      625 2023-08-07 15:31:05.000000 music-helper-1.0.1/music_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 15:31:05.000000 music-helper-1.0.1/music_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-08-07 15:31:05.000000 music-helper-1.0.1/music_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-07 15:31:05.000000 music-helper-1.0.1/music_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 15:31:05.550453 music-helper-1.0.1/musichelper/
+-rw-rw-rw-   0        0        0    28180 2023-08-07 14:36:36.000000 music-helper-1.0.1/musichelper/Deezer.py
+-rw-rw-rw-   0        0        0     2512 2023-08-07 14:35:14.000000 music-helper-1.0.1/musichelper/MusicHelper.py
+-rw-rw-rw-   0        0        0     9135 2023-08-07 14:53:43.000000 music-helper-1.0.1/musichelper/SoundCloud.py
+-rw-rw-rw-   0        0        0     9819 2023-08-07 15:13:19.000000 music-helper-1.0.1/musichelper/YTM.py
+-rw-rw-rw-   0        0        0       49 2023-08-06 11:27:03.000000 music-helper-1.0.1/musichelper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:31:05.577416 music-helper-1.0.1/musichelper/constants/
+-rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 music-helper-1.0.1/musichelper/constants/__init__.py
+-rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 music-helper-1.0.1/musichelper/constants/api_methods.py
+-rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 music-helper-1.0.1/musichelper/constants/api_urls.py
+-rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 music-helper-1.0.1/musichelper/constants/image_hosts.py
+-rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 music-helper-1.0.1/musichelper/constants/networking_settings.py
+-rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 music-helper-1.0.1/musichelper/constants/search_types.py
+-rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 music-helper-1.0.1/musichelper/constants/track_formats.py
+-rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 music-helper-1.0.1/musichelper/exceptions.py
+-rw-rw-rw-   0        0        0     3354 2023-08-07 15:16:58.000000 music-helper-1.0.1/musichelper/util.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 15:31:05.581369 music-helper-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      872 2023-08-07 15:31:02.000000 music-helper-1.0.1/setup.py
```

### Comparing `music-helper-1.0.0/PKG-INFO` & `music-helper-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: music-helper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Asynchronous library for working with streaming services. Search, download
-Home-page: https://github.com/drhspfn/deezer-asy
+Home-page: https://github.com/drhspfn/music-helper
 Author: drhspfn
 Author-email: drhspfn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-# music-helper | v`1.0.0`
+# music-helper | v`1.0.1`
 
 
 # Installation
 `pip install music-helper`
 
 # Usage
```

### Comparing `music-helper-1.0.0/README.md` & `music-helper-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# music-helper | v`1.0.0`
+# music-helper | v`1.0.1`
 
 
 # Installation
 `pip install music-helper`
 
 # Usage
```

### Comparing `music-helper-1.0.0/music_helper.egg-info/PKG-INFO` & `music-helper-1.0.1/music_helper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: music-helper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Asynchronous library for working with streaming services. Search, download
-Home-page: https://github.com/drhspfn/deezer-asy
+Home-page: https://github.com/drhspfn/music-helper
 Author: drhspfn
 Author-email: drhspfn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-# music-helper | v`1.0.0`
+# music-helper | v`1.0.1`
 
 
 # Installation
 `pip install music-helper`
 
 # Usage
```

### Comparing `music-helper-1.0.0/music_helper.egg-info/SOURCES.txt` & `music-helper-1.0.1/music_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `music-helper-1.0.0/musichelper/Deezer.py` & `music-helper-1.0.1/musichelper/Deezer.py`

 * *Files identical despite different names*

### Comparing `music-helper-1.0.0/musichelper/MusicHelper.py` & `music-helper-1.0.1/musichelper/MusicHelper.py`

 * *Files identical despite different names*

### Comparing `music-helper-1.0.0/musichelper/SoundCloud.py` & `music-helper-1.0.1/musichelper/SoundCloud.py`

 * *Files identical despite different names*

### Comparing `music-helper-1.0.0/musichelper/YTM.py` & `music-helper-1.0.1/musichelper/YTM.py`

 * *Files identical despite different names*

### Comparing `music-helper-1.0.0/musichelper/constants/api_methods.py` & `music-helper-1.0.1/musichelper/constants/api_methods.py`

 * *Files identical despite different names*

### Comparing `music-helper-1.0.0/musichelper/constants/track_formats.py` & `music-helper-1.0.1/musichelper/constants/track_formats.py`

 * *Files identical despite different names*

### Comparing `music-helper-1.0.0/musichelper/util.py` & `music-helper-1.0.1/musichelper/util.py`

 * *Files identical despite different names*

### Comparing `music-helper-1.0.0/setup.py` & `music-helper-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='music-helper',
-    version='1.0.0',
+    version='1.0.1',
     description='Asynchronous library for working with streaming services. Search, download',
     author='drhspfn',
     author_email="drhspfn@gmail.com",
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/drhspfn/deezer-asy",
+    url="https://github.com/drhspfn/music-helper",
     install_requires=[
         "aiofiles",
         "soundcloud-v2",
         "cryptography",
         "mutagen",
         "eyed3",
         "pytube",
```

