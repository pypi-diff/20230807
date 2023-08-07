# Comparing `tmp/osmnet-0.1.6.tar.gz` & `tmp/osmnet-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/osmnet-0.1.6.tar", last modified: Mon Jul 13 23:17:46 2020, max compression
+gzip compressed data, was "osmnet-0.1.7.tar", last modified: Mon Aug  7 16:44:15 2023, max compression
```

## Comparing `osmnet-0.1.6.tar` & `osmnet-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2020-07-13 23:17:46.013821 osmnet-0.1.6/
--rw-r--r--   0 maurer     (501) staff       (20)      909 2020-07-13 23:15:15.000000 osmnet-0.1.6/CHANGELOG.rst
--rw-r--r--   0 maurer     (501) staff       (20)    34486 2020-07-13 23:15:15.000000 osmnet-0.1.6/LICENSE.txt
--rw-r--r--   0 maurer     (501) staff       (20)      143 2020-07-13 23:15:15.000000 osmnet-0.1.6/MANIFEST.in
--rw-r--r--   0 maurer     (501) staff       (20)     4220 2020-07-13 23:17:46.013431 osmnet-0.1.6/PKG-INFO
--rw-r--r--   0 maurer     (501) staff       (20)     2679 2020-07-13 23:15:15.000000 osmnet-0.1.6/README.rst
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2020-07-13 23:17:46.010669 osmnet-0.1.6/osmnet/
--rw-r--r--   0 maurer     (501) staff       (20)       66 2020-07-13 23:15:15.000000 osmnet-0.1.6/osmnet/__init__.py
--rw-r--r--   0 maurer     (501) staff       (20)     2920 2020-07-08 21:00:27.000000 osmnet-0.1.6/osmnet/config.py
--rw-r--r--   0 maurer     (501) staff       (20)    32234 2020-07-13 23:15:15.000000 osmnet-0.1.6/osmnet/load.py
--rw-r--r--   0 maurer     (501) staff       (20)     4462 2020-07-08 21:00:27.000000 osmnet-0.1.6/osmnet/utils.py
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2020-07-13 23:17:46.012877 osmnet-0.1.6/osmnet.egg-info/
--rw-r--r--   0 maurer     (501) staff       (20)     4220 2020-07-13 23:17:45.000000 osmnet-0.1.6/osmnet.egg-info/PKG-INFO
--rw-r--r--   0 maurer     (501) staff       (20)      273 2020-07-13 23:17:45.000000 osmnet-0.1.6/osmnet.egg-info/SOURCES.txt
--rw-r--r--   0 maurer     (501) staff       (20)        1 2020-07-13 23:17:45.000000 osmnet-0.1.6/osmnet.egg-info/dependency_links.txt
--rw-r--r--   0 maurer     (501) staff       (20)       69 2020-07-13 23:17:45.000000 osmnet-0.1.6/osmnet.egg-info/requires.txt
--rw-r--r--   0 maurer     (501) staff       (20)        7 2020-07-13 23:17:45.000000 osmnet-0.1.6/osmnet.egg-info/top_level.txt
--rw-r--r--   0 maurer     (501) staff       (20)       38 2020-07-13 23:17:46.013929 osmnet-0.1.6/setup.cfg
--rw-r--r--   0 maurer     (501) staff       (20)     1214 2020-07-13 23:15:15.000000 osmnet-0.1.6/setup.py
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-08-07 16:44:15.997265 osmnet-0.1.7/
+-rw-r--r--   0 maurer     (501) staff       (20)      966 2023-08-07 16:43:11.000000 osmnet-0.1.7/CHANGELOG.rst
+-rw-r--r--   0 maurer     (501) staff       (20)    34486 2023-08-02 19:37:21.000000 osmnet-0.1.7/LICENSE.txt
+-rw-r--r--   0 maurer     (501) staff       (20)      143 2023-08-02 19:37:21.000000 osmnet-0.1.7/MANIFEST.in
+-rw-r--r--   0 maurer     (501) staff       (20)     3454 2023-08-07 16:44:15.997147 osmnet-0.1.7/PKG-INFO
+-rw-r--r--   0 maurer     (501) staff       (20)     2675 2023-08-02 19:37:21.000000 osmnet-0.1.7/README.rst
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-08-07 16:44:15.996318 osmnet-0.1.7/osmnet/
+-rw-r--r--   0 maurer     (501) staff       (20)       66 2023-08-02 19:41:30.000000 osmnet-0.1.7/osmnet/__init__.py
+-rw-r--r--   0 maurer     (501) staff       (20)     2920 2023-08-02 19:37:21.000000 osmnet-0.1.7/osmnet/config.py
+-rw-r--r--   0 maurer     (501) staff       (20)    32245 2023-08-02 19:37:21.000000 osmnet-0.1.7/osmnet/load.py
+-rw-r--r--   0 maurer     (501) staff       (20)     4462 2023-08-02 19:37:21.000000 osmnet-0.1.7/osmnet/utils.py
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-08-07 16:44:15.996988 osmnet-0.1.7/osmnet.egg-info/
+-rw-r--r--   0 maurer     (501) staff       (20)     3454 2023-08-07 16:44:15.000000 osmnet-0.1.7/osmnet.egg-info/PKG-INFO
+-rw-r--r--   0 maurer     (501) staff       (20)      273 2023-08-07 16:44:15.000000 osmnet-0.1.7/osmnet.egg-info/SOURCES.txt
+-rw-r--r--   0 maurer     (501) staff       (20)        1 2023-08-07 16:44:15.000000 osmnet-0.1.7/osmnet.egg-info/dependency_links.txt
+-rw-r--r--   0 maurer     (501) staff       (20)       70 2023-08-07 16:44:15.000000 osmnet-0.1.7/osmnet.egg-info/requires.txt
+-rw-r--r--   0 maurer     (501) staff       (20)        7 2023-08-07 16:44:15.000000 osmnet-0.1.7/osmnet.egg-info/top_level.txt
+-rw-r--r--   0 maurer     (501) staff       (20)       38 2023-08-07 16:44:15.997298 osmnet-0.1.7/setup.cfg
+-rw-r--r--   0 maurer     (501) staff       (20)     1217 2023-08-02 19:45:52.000000 osmnet-0.1.7/setup.py
```

### Comparing `osmnet-0.1.6/CHANGELOG.rst` & `osmnet-0.1.7/CHANGELOG.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+v0.1.7
+======
+
+2023/8/7
+
+* adds support for Shapely 2.0
+
 v0.1.6
 ======
 
 2020/7/13
 
 * adds support for GeoPandas v0.7 and later
 * ends support for Python 2.7 and Win32
```

### Comparing `osmnet-0.1.6/LICENSE.txt` & `osmnet-0.1.7/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
                     GNU AFFERO GENERAL PUBLIC LICENSE
                        Version 3, 19 November 2007
 
- Copyright (C) 2020 UrbanSim Inc.
+ Copyright (C) 2022 UrbanSim Inc.
 
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
 
   The GNU Affero General Public License is a free, copyleft license for
```

### Comparing `osmnet-0.1.6/README.rst` & `osmnet-0.1.7/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 extract street network nodes and edges.
 
 Overview
 ========
 
 OSMnet offers tools to download street network data from OpenStreetMap
 and extract a graph network comprised of nodes and edges to be used in
-`Pandana`_ street network accessibility calculations.
+`Pandana`_ street network accessibility calculations and or `UrbanAccess`_
+to connect GTFS transit networks to road networks.
 
 Let us know what you are working on or if you think you have a great use case
-by tweeting us at ``@urbansim`` or post on the UrbanSim `forum`_.
+by tweeting us at ``@urbansim``.
 
 Library Status
 --------------
 
 *Forthcoming improvements:*
 
 * Tutorial/demo
@@ -80,15 +81,14 @@
 -  `UrbanAccess`_
 
 .. _Pandana: https://github.com/UDST/pandana
 .. _GitHub issues: https://github.com/UDST/osmnet/issues
 .. _OSMnet repo: https://github.com/udst/osmnet
 .. _here: https://udst.github.io/osmnet/index.html
 .. _UrbanAccess: https://github.com/UDST/urbanaccess
-.. _forum: http://discussion.urbansim.com/
 
 .. |Build Status| image:: https://travis-ci.org/UDST/osmnet.svg?branch=master
    :target: https://travis-ci.org/UDST/osmnet
 
 .. |Appveyor Build Status| image:: https://ci.appveyor.com/api/projects/status/acuoygyy3l0lqnpv/branch/master?svg=true
    :target: https://ci.appveyor.com/project/pksohn/osmnet
```

### Comparing `osmnet-0.1.6/osmnet/config.py` & `osmnet-0.1.7/osmnet/config.py`

 * *Files identical despite different names*

### Comparing `osmnet-0.1.6/osmnet/load.py` & `osmnet-0.1.7/osmnet/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,28 +131,28 @@
     # ways with the requested key/value. the '>' makes it recurse so we get
     # ways and way nodes. maxsize is in bytes.
 
     # turn bbox into a polygon and project to local UTM
     polygon = Polygon([(lng_max, lat_min), (lng_min, lat_min),
                        (lng_min, lat_max), (lng_max, lat_max)])
     geometry_proj, crs_proj = project_geometry(polygon,
-                                               crs={'init': 'epsg:4326'})
+                                               crs="EPSG:4326")
 
     # subdivide the bbox area poly if it exceeds the max area size
     # (in meters), then project back to WGS84
     geometry_proj_consolidated_subdivided = consolidate_subdivide_geometry(
         geometry_proj, max_query_area_size=max_query_area_size)
     geometry, crs = project_geometry(geometry_proj_consolidated_subdivided,
                                      crs=crs_proj, to_latlong=True)
     log('Requesting network data within bounding box from Overpass API '
-        'in {:,} request(s)'.format(len(geometry)))
+        'in {:,} request(s)'.format(len(geometry.geoms)))
     start_time = time.time()
 
     # loop through each polygon in the geometry
-    for poly in geometry:
+    for poly in geometry.geoms:
         # represent bbox as lng_max, lat_min, lng_min, lat_max and round
         # lat-longs to 8 decimal places to create
         # consistent URL strings
         lng_max, lat_min, lng_min, lat_max = poly.bounds
         query_template = '[out:json][timeout:{timeout}]{maxsize};' \
                          '(way["highway"]' \
                          '{filters}({lat_min:.8f},{lng_max:.8f},' \
@@ -164,15 +164,15 @@
         response_json = overpass_request(data={'data': query_str},
                                          timeout=timeout)
 
         response_jsons_list.append(response_json)
 
     log('Downloaded OSM network data within bounding box from Overpass '
         'API in {:,} request(s) and'
-        ' {:,.2f} seconds'.format(len(geometry), time.time()-start_time))
+        ' {:,.2f} seconds'.format(len(geometry.geoms), time.time()-start_time))
 
     # stitch together individual json results
     for json in response_jsons_list:
         try:
             response_jsons.extend(json['elements'])
         except KeyError:
             pass
@@ -230,15 +230,15 @@
 
     start_time = time.time()
     log('Posting to {} with timeout={}, "{}"'.format(url, timeout, data))
     response = requests.post(url, data=data, timeout=timeout)
 
     # get the response size and the domain, log result
     size_kb = len(response.content) / 1000.
-    domain = re.findall(r'//(?s)(.*?)/', url)[0]
+    domain = re.findall(r'(?s)//(.*?)/', url)[0]
     log('Downloaded {:,.1f}KB from {} in {:,.2f} seconds'
         .format(size_kb, domain, time.time()-start_time))
 
     try:
         response_json = response.json()
         if 'remark' in response_json:
             log('Server remark: "{}"'.format(response_json['remark'],
@@ -424,32 +424,29 @@
 
 def project_geometry(geometry, crs, to_latlong=False):
     """
     Project a shapely Polygon or MultiPolygon from WGS84 to UTM, or vice-versa
 
     Parameters
     ----------
-    geometry : shapely Polygon or MultiPolygon
+    geometry : shapely.geometry.Polygon or shapely.geometry.MultiPolygon
         the geometry to project
-    crs : int
+    crs : string or pyproj.CRS
         the starting coordinate reference system of the passed-in geometry
+        such as "EPSG:4326"
     to_latlong : bool, optional
         if True, project from crs to WGS84, if False, project
         from crs to local UTM zone
 
     Returns
     -------
     geometry_proj, crs : tuple (projected Shapely geometry, crs of the
     projected geometry)
     """
-    gdf = gpd.GeoDataFrame()
-    gdf.crs = crs
-    gdf.name = 'geometry to project'
-    gdf['geometry'] = None
-    gdf.loc[0, 'geometry'] = geometry
+    gdf = gpd.GeoDataFrame(geometry=[geometry], crs=crs)
     gdf_proj = project_gdf(gdf, to_latlong=to_latlong)
     geometry_proj = gdf_proj['geometry'].iloc[0]
     return geometry_proj, gdf_proj.crs
 
 
 def project_gdf(gdf, to_crs=None, to_latlong=False):
     """
@@ -461,48 +458,50 @@
     Svalbard or far northern Norway. If the GeoDataFrame is already in UTM, it
     will be returned untouched.
 
     Parameters
     ----------
     gdf : geopandas.GeoDataFrame
         the GeoDataFrame to be projected
-    to_crs : dict or string or pyproj.CRS
+    to_crs : string or pyproj.CRS
         if None, project to UTM zone in which gdf's centroid lies, otherwise
         project to this CRS
     to_latlong : bool
         if True, project to epsg:4326 and ignore to_crs
 
     Returns
     -------
     gdf_proj : geopandas.GeoDataFrame
         the projected GeoDataFrame
     """
     if gdf.crs is None or len(gdf) < 1:
-        raise ValueError("GeoDataFrame must have a valid CRS and cannot be empty")
+        raise ValueError(
+            "GeoDataFrame must have a valid CRS and cannot be empty")
 
     # if to_latlong is True, project the gdf to latlong
     if to_latlong:
         gdf_proj = gdf.to_crs(4326)
 
     # else if to_crs was passed-in, project gdf to this CRS
     elif to_crs is not None:
         gdf_proj = gdf.to_crs(to_crs)
 
     # otherwise, automatically project the gdf to UTM
     else:
         if gdf.crs.is_projected:
-            raise ValueError("Geometry must be unprojected to calculate UTM zone")
+            raise ValueError(
+                "Geometry must be unprojected to calculate UTM zone")
 
         # calculate longitude of centroid of union of all geometries in gdf
         avg_lng = gdf["geometry"].unary_union.centroid.x
 
         # calculate UTM zone from avg longitude to define CRS to project to
         utm_zone = int(math.floor((avg_lng + 180) / 6.0) + 1)
-        utm_crs = ('+proj=utm +zone={} +ellps=WGS84 +datum=WGS84 +units=m +no_defs'
-                   .format(utm_zone))
+        utm_crs = ('+proj=utm +zone={} +ellps=WGS84 '
+                   '+datum=WGS84 +units=m +no_defs'.format(utm_zone))
 
         # project the GeoDataFrame to the UTM CRS
         gdf_proj = gdf.to_crs(utm_crs)
 
     return gdf_proj
```

### Comparing `osmnet-0.1.6/osmnet/utils.py` & `osmnet-0.1.7/osmnet/utils.py`

 * *Files identical despite different names*

### Comparing `osmnet-0.1.6/setup.py` & `osmnet-0.1.7/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 
 # read README as the long description
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(
     name='osmnet',
-    version='0.1.6',
+    version='0.1.7',
     license='AGPL',
     description=('Tools for the extraction of OpenStreetMap street network '
                  'data for use in Pandana accessibility analyses.'),
     long_description=long_description,
     author='UrbanSim Inc.',
     url='https://github.com/UDST/osmnet',
     classifiers=[
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: GNU Affero General Public License v3'
     ],
     packages=find_packages(exclude=['*.tests']),
     python_requires='>=3',
     install_requires=[
-        'geopandas >= 0.7',
+        'geopandas >= 0.11',
         'numpy >= 1.10',
         'pandas >= 0.23',
         'requests >= 2.9.1',
-        'shapely >= 1.5'
+        'shapely >= 1.8'
     ]
 )
```

