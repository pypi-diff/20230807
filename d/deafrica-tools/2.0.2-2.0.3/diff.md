# Comparing `tmp/deafrica_tools-2.0.2.tar.gz` & `tmp/deafrica_tools-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deafrica_tools-2.0.2.tar", max compression
+gzip compressed data, was "deafrica_tools-2.0.3.tar", max compression
```

## Comparing `deafrica_tools-2.0.2.tar` & `deafrica_tools-2.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/LICENSE
--rw-r--r--   0        0        0     3097 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/README.md
--rw-r--r--   0        0        0      676 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/__init__.py
--rw-r--r--   0        0        0       22 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/__init__.py
--rw-r--r--   0        0        0    31449 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/animations.py
--rw-r--r--   0        0        0    10984 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/changefilmstrips.py
--rw-r--r--   0        0        0    10494 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/crophealth.py
--rw-r--r--   0        0        0    20287 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/deacoastlines.py
--rw-r--r--   0        0        0    37843 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/forestmonitoring.py
--rw-r--r--   0        0        0     8673 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/geomedian.py
--rw-r--r--   0        0        0    13383 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/imageexport.py
--rw-r--r--   0        0        0    13148 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/wetlandsinsighttool.py
--rw-r--r--   0        0        0     9882 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/app/widgetconstructors.py
--rw-r--r--   0        0        0     2016 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/areaofinterest.py
--rw-r--r--   0        0        0    24548 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/bandindices.py
--rw-r--r--   0        0        0    61473 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/classification.py
--rw-r--r--   0        0        0    23515 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/coastal.py
--rw-r--r--   0        0        0     3404 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/dask.py
--rw-r--r--   0        0        0    35752 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/datahandling.py
--rw-r--r--   0        0        0    14369 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/load_era5.py
--rw-r--r--   0        0        0     2793 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/load_isda.py
--rw-r--r--   0        0        0     2027 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/load_soil_moisture.py
--rw-r--r--   0        0        0     1783 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo
--rw-r--r--   0        0        0     3315 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po
--rw-r--r--   0        0        0    50697 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/plotting.py
--rw-r--r--   0        0        0    36957 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/spatial.py
--rw-r--r--   0        0        0    17245 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/temporal.py
--rw-r--r--   0        0        0    25961 2023-08-01 10:39:16.195908 deafrica_tools-2.0.2/deafrica_tools/wetlands.py
--rw-r--r--   0        0        0     3310 2023-08-01 10:39:16.199908 deafrica_tools-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     5577 1970-01-01 00:00:00.000000 deafrica_tools-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-07 10:32:34.605677 deafrica_tools-2.0.3/LICENSE
+-rw-r--r--   0        0        0     3097 2023-08-07 10:32:34.605677 deafrica_tools-2.0.3/README.md
+-rw-r--r--   0        0        0      676 2023-08-07 10:32:34.605677 deafrica_tools-2.0.3/deafrica_tools/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-07 10:32:34.605677 deafrica_tools-2.0.3/deafrica_tools/app/__init__.py
+-rw-r--r--   0        0        0    31449 2023-08-07 10:32:34.605677 deafrica_tools-2.0.3/deafrica_tools/app/animations.py
+-rw-r--r--   0        0        0    10984 2023-08-07 10:32:34.605677 deafrica_tools-2.0.3/deafrica_tools/app/changefilmstrips.py
+-rw-r--r--   0        0        0    10494 2023-08-07 10:32:34.605677 deafrica_tools-2.0.3/deafrica_tools/app/crophealth.py
+-rw-r--r--   0        0        0    20287 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/app/deacoastlines.py
+-rw-r--r--   0        0        0    37843 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/app/forestmonitoring.py
+-rw-r--r--   0        0        0     8673 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/app/geomedian.py
+-rw-r--r--   0        0        0    13383 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/app/imageexport.py
+-rw-r--r--   0        0        0    13148 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/app/wetlandsinsighttool.py
+-rw-r--r--   0        0        0     9882 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/app/widgetconstructors.py
+-rw-r--r--   0        0        0     2016 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/areaofinterest.py
+-rw-r--r--   0        0        0    24548 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/bandindices.py
+-rw-r--r--   0        0        0    61473 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/classification.py
+-rw-r--r--   0        0        0    23515 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/coastal.py
+-rw-r--r--   0        0        0     3404 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/dask.py
+-rw-r--r--   0        0        0    35752 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/datahandling.py
+-rw-r--r--   0        0        0    14369 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/load_era5.py
+-rw-r--r--   0        0        0     2793 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/load_isda.py
+-rw-r--r--   0        0        0     2027 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/load_soil_moisture.py
+-rw-r--r--   0        0        0     1783 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo
+-rw-r--r--   0        0        0     3315 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po
+-rw-r--r--   0        0        0    50697 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/plotting.py
+-rw-r--r--   0        0        0    36957 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/spatial.py
+-rw-r--r--   0        0        0    17245 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/temporal.py
+-rw-r--r--   0        0        0    25961 2023-08-07 10:32:34.609677 deafrica_tools-2.0.3/deafrica_tools/wetlands.py
+-rw-r--r--   0        0        0     3441 2023-08-07 10:32:34.613677 deafrica_tools-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5545 1970-01-01 00:00:00.000000 deafrica_tools-2.0.3/PKG-INFO
```

### Comparing `deafrica_tools-2.0.2/LICENSE` & `deafrica_tools-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/README.md` & `deafrica_tools-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/__init__.py` & `deafrica_tools-2.0.3/deafrica_tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 
 __locales__ = __path__[0] + '/locales'
 
 
 def set_lang(lang=None):
     if lang is None:
         import os
```

### Comparing `deafrica_tools-2.0.2/deafrica_tools/app/animations.py` & `deafrica_tools-2.0.3/deafrica_tools/app/animations.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/app/changefilmstrips.py` & `deafrica_tools-2.0.3/deafrica_tools/app/changefilmstrips.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/app/crophealth.py` & `deafrica_tools-2.0.3/deafrica_tools/app/crophealth.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/app/deacoastlines.py` & `deafrica_tools-2.0.3/deafrica_tools/app/deacoastlines.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/app/forestmonitoring.py` & `deafrica_tools-2.0.3/deafrica_tools/app/forestmonitoring.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/app/geomedian.py` & `deafrica_tools-2.0.3/deafrica_tools/app/geomedian.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/app/imageexport.py` & `deafrica_tools-2.0.3/deafrica_tools/app/imageexport.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/app/wetlandsinsighttool.py` & `deafrica_tools-2.0.3/deafrica_tools/app/wetlandsinsighttool.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/app/widgetconstructors.py` & `deafrica_tools-2.0.3/deafrica_tools/app/widgetconstructors.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/areaofinterest.py` & `deafrica_tools-2.0.3/deafrica_tools/areaofinterest.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/bandindices.py` & `deafrica_tools-2.0.3/deafrica_tools/bandindices.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/classification.py` & `deafrica_tools-2.0.3/deafrica_tools/classification.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/coastal.py` & `deafrica_tools-2.0.3/deafrica_tools/coastal.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/dask.py` & `deafrica_tools-2.0.3/deafrica_tools/dask.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/datahandling.py` & `deafrica_tools-2.0.3/deafrica_tools/datahandling.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/load_era5.py` & `deafrica_tools-2.0.3/deafrica_tools/load_era5.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/load_isda.py` & `deafrica_tools-2.0.3/deafrica_tools/load_isda.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/load_soil_moisture.py` & `deafrica_tools-2.0.3/deafrica_tools/load_soil_moisture.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo` & `deafrica_tools-2.0.3/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po` & `deafrica_tools-2.0.3/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/plotting.py` & `deafrica_tools-2.0.3/deafrica_tools/plotting.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/spatial.py` & `deafrica_tools-2.0.3/deafrica_tools/spatial.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/temporal.py` & `deafrica_tools-2.0.3/deafrica_tools/temporal.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/deafrica_tools/wetlands.py` & `deafrica_tools-2.0.3/deafrica_tools/wetlands.py`

 * *Files identical despite different names*

### Comparing `deafrica_tools-2.0.2/pyproject.toml` & `deafrica_tools-2.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyproject.toml tells “frontend” build tools like pip and build what “backend” tool to use to create distribution packages for your project.
 
 # Using poetry for dependency management and packaging.
 
 # Package metadata.
 [tool.poetry]
 name = "deafrica-tools"
-version = "2.0.2"
+version = "2.0.3"
 description = "Functions and algorithms for analysing Digital Earth Africa data."
 license = "Apache-2.0"
 authors = ["Digital Earth Africa <systems@digitalearthafrica.org>"]
 readme = "README.md"
 homepage = "https://github.com/digitalearthafrica/deafrica-sandbox-notebooks"
 repository = "https://github.com/digitalearthafrica/deafrica-sandbox-notebooks"
 documentation = "https://docs.digitalearthafrica.org/en/latest/sandbox/notebooks/Tools/index.html"
@@ -18,59 +18,58 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/digitalearthafrica/deafrica-sandbox-notebooks/issues"
 
 # Dependencies and dependency groups
 [tool.poetry.dependencies]
 # declaring the python version for which your package is compatible is mandatory
 python = ">=3.9,<3.12"
-geopandas = "0.13.2"
-shapely = "2.0.1"
-geojson = "3.0.1"
-numpy = "1.23.5"
-dask = {version = "2023.3.1", extras = ["array", "complete", "dataframe"]}
-joblib = "1.2.0"
-pandas = "2.0.2"
-xarray = "2023.5.0"
-dask-ml = "2023.3.24"
-botocore = "1.27.59"
-datacube = {version = "1.8.13", extras = ["celery", "performance", "s3"]}
-scikit-learn = "1.2.2"
-tqdm = "4.65.0"
-requests = "2.31.0"
-matplotlib = "3.7.1"
-otps = {version = "0.3.2", source = "packages.dea.ga.gov.au"}
-owslib = "0.29.2"
-aiohttp = "3.8.4"
+geopandas = ">=0.13.2"
+shapely = ">=2.0.1"
+geojson = ">=3.0.1"
+#numpy = "1.23.5"
+dask = {version = ">=2023.3.1", extras = ["array", "complete", "dataframe"]}
+joblib = ">=1.2.0"
+pandas = ">=2.0.2"
+xarray = ">=2023.5.0"
+dask-ml = ">=2023.3.24"
+botocore = ">=1.27.59"
+datacube = {version = ">=1.8.13", extras = ["celery", "performance", "s3"]}
+scikit-learn = ">=1.2.2"
+tqdm = ">=4.65.0"
+requests = ">=2.31.0"
+matplotlib = ">=3.7.1"
+otps = {version = ">=0.3.2", source = "packages.dea.ga.gov.au"}
+owslib = ">=0.29.2"
+aiohttp = ">=3.8.4"
 gdal = "3.6.3"
-pytz = "2023.3"
-odc-algo = "0.2.3"
-fsspec = "2023.3.0"
-rasterio = "1.3.7"
-pyproj = "3.5.0"
-boto3 = "1.24.59"
-pystac = "1.7.3"
-folium = "0.12.1"
-ipywidgets = "8.0.6"
-branca = "0.6.0"
-ipython = "8.13.1"
-ipyleaflet = "0.17.2"
-scikit-image = "0.21.0"
-odc-ui = {version = "0.2.1.dev3673", source = "packages.dea.ga.gov.au"}
-fiona = "1.9.4.post1"
-rasterstats = "0.19.0"
-geopy = "2.3.0"
-hdstats = "0.2.1"
-packaging = "23.1"
-seaborn = "0.12.2"
-traitlets = "5.9.0"
-rioxarray = "0.14.1"
-numexpr = "2.8.4"
-datetime = "5.1"
-scipy = "1.10.1"
-
+pytz = ">=2023.3"
+odc-algo = {version = ">=0.2.3", source = "packages.dea.ga.gov.au"}
+fsspec = ">=2023.3.0"
+rasterio = ">=1.3.7"
+pyproj = ">=3.5.0"
+boto3 = ">=1.24.59"
+pystac = ">=1.7.3"
+folium = ">=0.12.1"
+ipywidgets = ">=8.0.6"
+branca = ">=0.6.0"
+ipython = ">=8.13.1"
+ipyleaflet = ">=0.17.2"
+scikit-image = ">=0.21.0"
+odc-ui = {version = ">=0.2.1.dev3673", source = "packages.dea.ga.gov.au"}
+fiona = ">=1.9.4.post1"
+rasterstats = ">=0.19.0"
+geopy = ">=2.3.0"
+hdstats = ">=0.2.1"
+packaging = ">=23.1"
+seaborn = ">=0.12.2"
+traitlets = ">=5.9.0"
+rioxarray = ">=0.14.1"
+numexpr = ">=2.8.4"
+datetime = ">=5.1"
+scipy = ">=1.10.1"
 # Package sources for discovery and installation of dependencies.
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "default"
```

### Comparing `deafrica_tools-2.0.2/PKG-INFO` & `deafrica_tools-2.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 Metadata-Version: 2.1
 Name: deafrica-tools
-Version: 2.0.2
+Version: 2.0.3
 Summary: Functions and algorithms for analysing Digital Earth Africa data.
 Home-page: https://github.com/digitalearthafrica/deafrica-sandbox-notebooks
 License: Apache-2.0
 Author: Digital Earth Africa
 Author-email: systems@digitalearthafrica.org
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (==3.8.4)
-Requires-Dist: boto3 (==1.24.59)
-Requires-Dist: botocore (==1.27.59)
-Requires-Dist: branca (==0.6.0)
-Requires-Dist: dask-ml (==2023.3.24)
-Requires-Dist: dask[array,complete,dataframe] (==2023.3.1)
-Requires-Dist: datacube[celery,performance,s3] (==1.8.13)
-Requires-Dist: datetime (==5.1)
-Requires-Dist: fiona (==1.9.4.post1)
-Requires-Dist: folium (==0.12.1)
-Requires-Dist: fsspec (==2023.3.0)
+Requires-Dist: aiohttp (>=3.8.4)
+Requires-Dist: boto3 (>=1.24.59)
+Requires-Dist: botocore (>=1.27.59)
+Requires-Dist: branca (>=0.6.0)
+Requires-Dist: dask-ml (>=2023.3.24)
+Requires-Dist: dask[array,complete,dataframe] (>=2023.3.1)
+Requires-Dist: datacube[celery,performance,s3] (>=1.8.13)
+Requires-Dist: datetime (>=5.1)
+Requires-Dist: fiona (>=1.9.4.post1)
+Requires-Dist: folium (>=0.12.1)
+Requires-Dist: fsspec (>=2023.3.0)
 Requires-Dist: gdal (==3.6.3)
-Requires-Dist: geojson (==3.0.1)
-Requires-Dist: geopandas (==0.13.2)
-Requires-Dist: geopy (==2.3.0)
-Requires-Dist: hdstats (==0.2.1)
-Requires-Dist: ipyleaflet (==0.17.2)
-Requires-Dist: ipython (==8.13.1)
-Requires-Dist: ipywidgets (==8.0.6)
-Requires-Dist: joblib (==1.2.0)
-Requires-Dist: matplotlib (==3.7.1)
-Requires-Dist: numexpr (==2.8.4)
-Requires-Dist: numpy (==1.23.5)
-Requires-Dist: odc-algo (==0.2.3)
-Requires-Dist: odc-ui (==0.2.1.dev3673)
-Requires-Dist: otps (==0.3.2)
-Requires-Dist: owslib (==0.29.2)
-Requires-Dist: packaging (==23.1)
-Requires-Dist: pandas (==2.0.2)
-Requires-Dist: pyproj (==3.5.0)
-Requires-Dist: pystac (==1.7.3)
-Requires-Dist: pytz (==2023.3)
-Requires-Dist: rasterio (==1.3.7)
-Requires-Dist: rasterstats (==0.19.0)
-Requires-Dist: requests (==2.31.0)
-Requires-Dist: rioxarray (==0.14.1)
-Requires-Dist: scikit-image (==0.21.0)
-Requires-Dist: scikit-learn (==1.2.2)
-Requires-Dist: scipy (==1.10.1)
-Requires-Dist: seaborn (==0.12.2)
-Requires-Dist: shapely (==2.0.1)
-Requires-Dist: tqdm (==4.65.0)
-Requires-Dist: traitlets (==5.9.0)
-Requires-Dist: xarray (==2023.5.0)
+Requires-Dist: geojson (>=3.0.1)
+Requires-Dist: geopandas (>=0.13.2)
+Requires-Dist: geopy (>=2.3.0)
+Requires-Dist: hdstats (>=0.2.1)
+Requires-Dist: ipyleaflet (>=0.17.2)
+Requires-Dist: ipython (>=8.13.1)
+Requires-Dist: ipywidgets (>=8.0.6)
+Requires-Dist: joblib (>=1.2.0)
+Requires-Dist: matplotlib (>=3.7.1)
+Requires-Dist: numexpr (>=2.8.4)
+Requires-Dist: odc-algo (>=0.2.3)
+Requires-Dist: odc-ui (>=0.2.1.dev3673)
+Requires-Dist: otps (>=0.3.2)
+Requires-Dist: owslib (>=0.29.2)
+Requires-Dist: packaging (>=23.1)
+Requires-Dist: pandas (>=2.0.2)
+Requires-Dist: pyproj (>=3.5.0)
+Requires-Dist: pystac (>=1.7.3)
+Requires-Dist: pytz (>=2023.3)
+Requires-Dist: rasterio (>=1.3.7)
+Requires-Dist: rasterstats (>=0.19.0)
+Requires-Dist: requests (>=2.31.0)
+Requires-Dist: rioxarray (>=0.14.1)
+Requires-Dist: scikit-image (>=0.21.0)
+Requires-Dist: scikit-learn (>=1.2.2)
+Requires-Dist: scipy (>=1.10.1)
+Requires-Dist: seaborn (>=0.12.2)
+Requires-Dist: shapely (>=2.0.1)
+Requires-Dist: tqdm (>=4.65.0)
+Requires-Dist: traitlets (>=5.9.0)
+Requires-Dist: xarray (>=2023.5.0)
 Project-URL: Bug Tracker, https://github.com/digitalearthafrica/deafrica-sandbox-notebooks/issues
 Project-URL: Documentation, https://docs.digitalearthafrica.org/en/latest/sandbox/notebooks/Tools/index.html
 Project-URL: Repository, https://github.com/digitalearthafrica/deafrica-sandbox-notebooks
 Description-Content-Type: text/markdown
 
 <img align="centre" src="https://github.com/digitalearthafrica/deafrica-sandbox-notebooks/blob/main/Supplementary_data/Github_banner.jpg?raw=true" width="100%">
```

