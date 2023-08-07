# Comparing `tmp/GeoSAM-Image-Encoder-1.0.0.tar.gz` & `tmp/GeoSAM-Image-Encoder-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeoSAM-Image-Encoder-1.0.0.tar", last modified: Sun Aug  6 20:01:26 2023, max compression
+gzip compressed data, was "GeoSAM-Image-Encoder-1.0.1.tar", last modified: Sun Aug  6 20:09:29 2023, max compression
```

## Comparing `GeoSAM-Image-Encoder-1.0.0.tar` & `GeoSAM-Image-Encoder-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 20:01:26.601725 GeoSAM-Image-Encoder-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-08-06 20:01:26.595077 GeoSAM-Image-Encoder-1.0.0/GeoSAM_Image_Encoder.egg-info/
--rw-rw-rw-   0        0        0     3461 2023-08-06 20:01:26.000000 GeoSAM-Image-Encoder-1.0.0/GeoSAM_Image_Encoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-08-06 20:01:26.000000 GeoSAM-Image-Encoder-1.0.0/GeoSAM_Image_Encoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 20:01:26.000000 GeoSAM-Image-Encoder-1.0.0/GeoSAM_Image_Encoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-08-06 20:01:26.000000 GeoSAM-Image-Encoder-1.0.0/GeoSAM_Image_Encoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-06 20:01:26.000000 GeoSAM-Image-Encoder-1.0.0/GeoSAM_Image_Encoder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35090 2023-04-22 12:24:31.000000 GeoSAM-Image-Encoder-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3461 2023-08-06 20:01:26.600723 GeoSAM-Image-Encoder-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2867 2023-08-06 19:50:37.000000 GeoSAM-Image-Encoder-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-06 20:01:26.599724 GeoSAM-Image-Encoder-1.0.0/geosam/
--rw-rw-rw-   0        0        0      126 2023-08-06 19:41:29.000000 GeoSAM-Image-Encoder-1.0.0/geosam/__init__.py
--rw-rw-rw-   0        0        0    20167 2023-08-06 19:49:22.000000 GeoSAM-Image-Encoder-1.0.0/geosam/image_encoder.py
--rw-rw-rw-   0        0        0    25617 2023-08-06 15:57:41.000000 GeoSAM-Image-Encoder-1.0.0/geosam/torchgeo_sam.py
--rw-rw-rw-   0        0        0       42 2023-08-06 20:01:26.601725 GeoSAM-Image-Encoder-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      800 2023-08-06 19:08:40.000000 GeoSAM-Image-Encoder-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:09:29.717398 GeoSAM-Image-Encoder-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-08-06 20:09:29.712140 GeoSAM-Image-Encoder-1.0.1/GeoSAM_Image_Encoder.egg-info/
+-rw-rw-rw-   0        0        0     3466 2023-08-06 20:09:29.000000 GeoSAM-Image-Encoder-1.0.1/GeoSAM_Image_Encoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-08-06 20:09:29.000000 GeoSAM-Image-Encoder-1.0.1/GeoSAM_Image_Encoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 20:09:29.000000 GeoSAM-Image-Encoder-1.0.1/GeoSAM_Image_Encoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-08-06 20:09:29.000000 GeoSAM-Image-Encoder-1.0.1/GeoSAM_Image_Encoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-06 20:09:29.000000 GeoSAM-Image-Encoder-1.0.1/GeoSAM_Image_Encoder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35090 2023-04-22 12:24:31.000000 GeoSAM-Image-Encoder-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3466 2023-08-06 20:09:29.717398 GeoSAM-Image-Encoder-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2867 2023-08-06 19:50:37.000000 GeoSAM-Image-Encoder-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 20:09:29.715878 GeoSAM-Image-Encoder-1.0.1/geosam/
+-rw-rw-rw-   0        0        0      126 2023-08-06 19:41:29.000000 GeoSAM-Image-Encoder-1.0.1/geosam/__init__.py
+-rw-rw-rw-   0        0        0    20167 2023-08-06 19:49:22.000000 GeoSAM-Image-Encoder-1.0.1/geosam/image_encoder.py
+-rw-rw-rw-   0        0        0    25617 2023-08-06 15:57:41.000000 GeoSAM-Image-Encoder-1.0.1/geosam/torchgeo_sam.py
+-rw-rw-rw-   0        0        0       42 2023-08-06 20:09:29.717398 GeoSAM-Image-Encoder-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      805 2023-08-06 20:09:12.000000 GeoSAM-Image-Encoder-1.0.1/setup.py
```

### Comparing `GeoSAM-Image-Encoder-1.0.0/GeoSAM_Image_Encoder.egg-info/PKG-INFO` & `GeoSAM-Image-Encoder-1.0.1/GeoSAM_Image_Encoder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: GeoSAM-Image-Encoder
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for encoding satellite images into Geo-SAM features.
-Home-page: https://github.com/Fanchengyan/data-downloader
+Home-page: https://github.com/Fanchengyan/GeoSAM-Image-Encoder
 Author: Joey, Fancy
 Author-email: fanchy14@lzu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `GeoSAM-Image-Encoder-1.0.0/LICENSE` & `GeoSAM-Image-Encoder-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GeoSAM-Image-Encoder-1.0.0/PKG-INFO` & `GeoSAM-Image-Encoder-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: GeoSAM-Image-Encoder
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for encoding satellite images into Geo-SAM features.
-Home-page: https://github.com/Fanchengyan/data-downloader
+Home-page: https://github.com/Fanchengyan/GeoSAM-Image-Encoder
 Author: Joey, Fancy
 Author-email: fanchy14@lzu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `GeoSAM-Image-Encoder-1.0.0/README.md` & `GeoSAM-Image-Encoder-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `GeoSAM-Image-Encoder-1.0.0/geosam/image_encoder.py` & `GeoSAM-Image-Encoder-1.0.1/geosam/image_encoder.py`

 * *Files identical despite different names*

### Comparing `GeoSAM-Image-Encoder-1.0.0/geosam/torchgeo_sam.py` & `GeoSAM-Image-Encoder-1.0.1/geosam/torchgeo_sam.py`

 * *Files identical despite different names*

### Comparing `GeoSAM-Image-Encoder-1.0.0/setup.py` & `GeoSAM-Image-Encoder-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="GeoSAM-Image-Encoder",
-    version="1.0.0",
+    version="1.0.1",
     author="Joey, Fancy",
     author_email="fanchy14@lzu.edu.cn",
     description="A package for encoding satellite images into Geo-SAM features.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/Fanchengyan/data-downloader",
+    url="https://github.com/Fanchengyan/GeoSAM-Image-Encoder",
     packages=setuptools.find_packages(),
     install_requires=[
         'pandas',
         'tqdm',
         'setuptools',
     ],
     classifiers=[
```

