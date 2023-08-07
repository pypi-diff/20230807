# Comparing `tmp/dream_river-0.0.7.tar.gz` & `tmp/dream_river-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dream_river-0.0.7.tar", last modified: Wed Jul  5 02:14:41 2023, max compression
+gzip compressed data, was "dream_river-0.0.8.tar", last modified: Mon Aug  7 06:38:10 2023, max compression
```

## Comparing `dream_river-0.0.7.tar` & `dream_river-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 02:14:41.079277 dream_river-0.0.7/
--rw-rw-rw-   0        0        0     1069 2023-06-09 04:31:46.000000 dream_river-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1090 2023-06-09 04:31:50.000000 dream_river-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0     1392 2023-07-05 02:14:41.080277 dream_river-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      866 2023-06-09 08:10:52.000000 dream_river-0.0.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 02:14:41.058275 dream_river-0.0.7/dream_river/
--rw-rw-rw-   0        0        0     8528 2023-07-05 02:11:46.000000 dream_river-0.0.7/dream_river/ML.py
--rw-rw-rw-   0        0        0      226 2023-06-09 04:57:22.000000 dream_river-0.0.7/dream_river/__init__.py
--rw-rw-rw-   0        0        0     7139 2023-06-13 08:17:08.000000 dream_river-0.0.7/dream_river/convertools.py
--rw-rw-rw-   0        0        0     4967 2023-06-09 04:20:55.000000 dream_river-0.0.7/dream_river/geobox.py
--rw-rw-rw-   0        0        0     7648 2023-06-09 08:30:08.000000 dream_river-0.0.7/dream_river/indices.py
--rw-rw-rw-   0        0        0    15124 2023-06-09 04:21:55.000000 dream_river-0.0.7/dream_river/plotimg.py
-drwxrwxrwx   0        0        0        0 2023-07-05 02:14:41.078277 dream_river-0.0.7/dream_river.egg-info/
--rw-rw-rw-   0        0        0     1392 2023-07-05 02:14:41.000000 dream_river-0.0.7/dream_river.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-07-05 02:14:41.000000 dream_river-0.0.7/dream_river.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 02:14:41.000000 dream_river-0.0.7/dream_river.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-07-05 02:14:41.000000 dream_river-0.0.7/dream_river.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-05 02:14:41.000000 dream_river-0.0.7/dream_river.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-05 02:14:41.082277 dream_river-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1773 2023-07-05 02:12:31.000000 dream_river-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:38:10.883727 dream_river-0.0.8/
+-rw-rw-rw-   0        0        0     1069 2023-06-09 04:31:46.000000 dream_river-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1090 2023-06-09 04:31:50.000000 dream_river-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     1392 2023-08-07 06:38:10.884728 dream_river-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      866 2023-06-09 08:10:52.000000 dream_river-0.0.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-07 06:38:10.865117 dream_river-0.0.8/dream_river/
+-rw-rw-rw-   0        0        0     8528 2023-07-05 02:11:46.000000 dream_river-0.0.8/dream_river/ML.py
+-rw-rw-rw-   0        0        0      226 2023-06-09 04:57:22.000000 dream_river-0.0.8/dream_river/__init__.py
+-rw-rw-rw-   0        0        0     7139 2023-06-13 08:17:08.000000 dream_river-0.0.8/dream_river/convertools.py
+-rw-rw-rw-   0        0        0     4967 2023-06-09 04:20:55.000000 dream_river-0.0.8/dream_river/geobox.py
+-rw-rw-rw-   0        0        0     7648 2023-06-09 08:30:08.000000 dream_river-0.0.8/dream_river/indices.py
+-rw-rw-rw-   0        0        0    17975 2023-08-07 06:17:22.000000 dream_river-0.0.8/dream_river/plotimg.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:38:10.882730 dream_river-0.0.8/dream_river.egg-info/
+-rw-rw-rw-   0        0        0     1392 2023-08-07 06:38:10.000000 dream_river-0.0.8/dream_river.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-08-07 06:38:10.000000 dream_river-0.0.8/dream_river.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 06:38:10.000000 dream_river-0.0.8/dream_river.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-08-07 06:38:10.000000 dream_river-0.0.8/dream_river.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-07 06:38:10.000000 dream_river-0.0.8/dream_river.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-07 06:38:10.890728 dream_river-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1773 2023-08-07 06:31:43.000000 dream_river-0.0.8/setup.py
```

### Comparing `dream_river-0.0.7/LICENSE` & `dream_river-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.7/LICENSE.txt` & `dream_river-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.7/PKG-INFO` & `dream_river-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dream_river
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is a library contained rice detection tools and other geospatial tools for jupyter environment on sphere.gistda.or.th in part of Data Cube
 Home-page: https://github.com/Pathakorn40/rice-detection
 Download-URL: https://pypi.org/project/dream_river/
 Author: Pathakorn Usaha
 Author-email: dreamusaha@gmail.com
 License: MIT
 Keywords: geography,geospatiol,gis,rice detection
```

### Comparing `dream_river-0.0.7/README.rst` & `dream_river-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.7/dream_river/ML.py` & `dream_river-0.0.8/dream_river/ML.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.7/dream_river/convertools.py` & `dream_river-0.0.8/dream_river/convertools.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.7/dream_river/geobox.py` & `dream_river-0.0.8/dream_river/geobox.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.7/dream_river/indices.py` & `dream_river-0.0.8/dream_river/indices.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.7/dream_river/plotimg.py` & `dream_river-0.0.8/dream_river/plotimg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 '''
 ploting tools for creating the interactive map
 for Open Data Cube 
 
-The some function reference from dea_tools library(https://www.dea.ga.gov.au/)
+The reference from dea_tools library(https://www.dea.ga.gov.au/)
 
 '''
 
 # Import required packages
 import math
 import folium
 import numpy as np
 import geopandas as gpd
 import json
 import os
 import datacube 
 import xarray as xr
 import matplotlib.pyplot as plt 
 import odc.ui
+import ipyleaflet
 
-
+from ipyleaflet import Map, TileLayer
+from ipywidgets import widgets as w
+from IPython.display import display
+from odc.ui import with_ui_cbk
 from pyproj import Transformer
 from odc.ui import image_aspect
 from folium.plugins import Draw, Geocoder, Fullscreen, LocateControl
 from datacube.utils.cog import write_cog 
 
+
+
 # This function is used to plot rgb image from dataset
 def rgb(ds,
         bands=['red', 'green', 'blue'],
         index=None,
         index_dim='time',
         robust=True,
         percentile_stretch=None,
@@ -428,7 +434,74 @@
     # perform func
     result = gdf.centroid
     
         #save to output
     result.to_file(output)
     
     
+# ADD Image layer on interactive map
+def img_OnMap(dss, rgb, with_draw_tools=True,zoom=None):
+    
+    polygons, bbox = odc.ui.dss_to_geojson(dss, bbox=True)
+    zoom = odc.ui.zoom_from_bbox(bbox)
+    center = (bbox.bottom + bbox.top) * 0.5, (bbox.right + bbox.left) * 0.5
+
+    
+    """Create a map using ipyleaflet."""
+         
+    m = ipyleaflet.Map(
+    center=center,
+    zoom=zoom,
+    scroll_wheel_zoom=True,  
+    layout=w.Layout(
+        width='600px',   
+        height='600px',  
+    ))
+
+    # Add full-screen and layer visibility controls
+    m.add_control(ipyleaflet.FullScreenControl())
+    m.add_control(ipyleaflet.LayersControl())
+    
+    m.add_layer(ipyleaflet.GeoJSON( data={'type': 'FeatureCollection',
+                                          'features': polygons},
+                                    style={
+                                          'opacity': 0.3,      
+                                          'fillOpacity': 0 },    
+                                    hover_style={'color': 'tomato'},  
+                                    name="Footprints"))
+    
+    img_layer = odc.ui.mk_image_overlay( rgb,
+                                         clamp=3000,  
+                                         fmt='png')   
+
+    # Add image layer to a map we created earlier
+    m.add_layer(img_layer)
+    
+    slider = w.FloatSlider(min=0, max=1, value=1,        
+                       orientation='vertical',       
+                       readout=False,                
+                       layout=w.Layout(width='2em')) 
+
+    # Connect slider value to opacity property of the Image Layer
+    w.jslink((slider, 'value'),         
+         (img_layer, 'opacity') )
+    m.add_control(ipyleaflet.WidgetControl(widget=slider))
+    
+
+    # Add a tile map layer 
+    tile_layer_gistda_sat = TileLayer(url='https://basemap.sphere.gistda.or.th/tiles/thailand_images/EPSG3857/{z}/{x}/{y}.jpeg?key=42B90819583344A789DA424BE70CDB61', name='Gistda Satellite')
+    m.add_layer(tile_layer_gistda_sat)
+    
+    tile_layer_gistda = TileLayer(url='https://basemap.sphere.gistda.or.th/tiles/sphere_hybrid/EPSG3857/{z}/{x}/{y}.jpeg?key=42B90819583344A789DA424BE70CDB61', name='Gistda Hybrid')
+    m.add_layer(tile_layer_gistda)
+    
+    tile_layer_gg_sat = TileLayer(url='https://mt1.google.com/vt/lyrs=s&x={x}&y={y}&z={z}', name='Google Satellite')
+    m.add_layer(tile_layer_gg_sat)
+    
+    tile_layer_gg = TileLayer(url='https://mt1.google.com/vt/lyrs=y&x={x}&y={y}&z={z}', name='Hybrid')
+    m.add_layer(tile_layer_gg)
+    
+    tile_layer_terrain = TileLayer(url='https://mt1.google.com/vt/lyrs=p&x={x}&y={y}&z={z}', name='Terrain')
+    m.add_layer(tile_layer_terrain)
+
+    return m
+
```

### Comparing `dream_river-0.0.7/dream_river.egg-info/PKG-INFO` & `dream_river-0.0.8/dream_river.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dream-river
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is a library contained rice detection tools and other geospatial tools for jupyter environment on sphere.gistda.or.th in part of Data Cube
 Home-page: https://github.com/Pathakorn40/rice-detection
 Download-URL: https://pypi.org/project/dream_river/
 Author: Pathakorn Usaha
 Author-email: dreamusaha@gmail.com
 License: MIT
 Keywords: geography,geospatiol,gis,rice detection
```

### Comparing `dream_river-0.0.7/setup.py` & `dream_river-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 DESC ='This is a library that contain rice cultivated area detection tools and other geospatial tools for jupyter environment on https://sphere.gistda.or.th/ in part of Data Cube. Thus, you needs go to sphere.gistda (https://sphere.gistda.or.th/) and register the account to access jupyter lab environment interactively from a browser.'
 
 setup(
     name='dream_river',
     packages=['dream_river'],
-    version='0.0.7',
+    version='0.0.8',
     license='MIT',
     author_email='dreamusaha@gmail.com',
     description= 'This is a library contained rice detection tools and other geospatial tools for jupyter environment on sphere.gistda.or.th in part of Data Cube',
     long_description= DESC,
     author='Pathakorn Usaha',
     url= 'https://github.com/Pathakorn40/rice-detection',
     download_url= 'https://pypi.org/project/dream_river/',
```

