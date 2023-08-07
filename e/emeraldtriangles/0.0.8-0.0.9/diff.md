# Comparing `tmp/emeraldtriangles-0.0.8.tar.gz` & `tmp/emeraldtriangles-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/emeraldtriangles-0.0.8.tar", last modified: Tue Mar 30 13:15:43 2021, max compression
+gzip compressed data, was "dist/emeraldtriangles-0.0.9.tar", last modified: Wed Apr  7 09:05:31 2021, max compression
```

## Comparing `emeraldtriangles-0.0.8.tar` & `emeraldtriangles-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2021-03-30 13:15:43.000000 emeraldtriangles-0.0.8/
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2021-03-30 13:15:43.000000 emeraldtriangles-0.0.8/emeraldtriangles.egg-info/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       17 2021-03-30 13:15:43.000000 emeraldtriangles-0.0.8/emeraldtriangles.egg-info/top_level.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      370 2021-03-30 13:15:43.000000 emeraldtriangles-0.0.8/emeraldtriangles.egg-info/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      600 2021-03-30 13:15:43.000000 emeraldtriangles-0.0.8/emeraldtriangles.egg-info/SOURCES.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       44 2021-03-30 13:15:43.000000 emeraldtriangles-0.0.8/emeraldtriangles.egg-info/requires.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2021-03-30 13:15:43.000000 emeraldtriangles-0.0.8/emeraldtriangles.egg-info/dependency_links.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1711 2021-03-30 13:15:04.000000 emeraldtriangles-0.0.8/setup.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      370 2021-03-30 13:15:43.000000 emeraldtriangles-0.0.8/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       28 2021-03-30 09:42:56.000000 emeraldtriangles-0.0.8/MANIFEST.in
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2021-03-30 13:15:43.000000 emeraldtriangles-0.0.8/setup.cfg
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1461 2021-01-26 12:07:16.000000 emeraldtriangles-0.0.8/README.md
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2021-03-30 13:15:43.000000 emeraldtriangles-0.0.8/emeraldtriangles/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      129 2020-08-21 08:50:45.000000 emeraldtriangles-0.0.8/emeraldtriangles/__init__.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     2276 2021-01-22 08:44:56.000000 emeraldtriangles-0.0.8/emeraldtriangles/cleanup.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1772 2021-01-20 09:58:59.000000 emeraldtriangles-0.0.8/emeraldtriangles/points_in_mesh.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     6391 2021-01-22 08:24:22.000000 emeraldtriangles-0.0.8/emeraldtriangles/refine_mesh.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     3606 2021-01-20 09:58:59.000000 emeraldtriangles-0.0.8/emeraldtriangles/plotting_bokeh.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     2744 2020-10-05 15:04:43.000000 emeraldtriangles-0.0.8/emeraldtriangles/plotting.py
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2021-03-30 13:15:43.000000 emeraldtriangles-0.0.8/emeraldtriangles/io/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     6655 2021-03-30 13:05:47.000000 emeraldtriangles-0.0.8/emeraldtriangles/io/_landxml.pyx
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     3379 2021-03-25 10:57:15.000000 emeraldtriangles-0.0.8/emeraldtriangles/io/__init__.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     6790 2021-03-30 13:06:50.000000 emeraldtriangles-0.0.8/emeraldtriangles/io/landxml.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1608 2021-03-25 16:26:18.000000 emeraldtriangles-0.0.8/emeraldtriangles/io/vtk.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     2934 2021-03-30 09:41:14.000000 emeraldtriangles-0.0.8/emeraldtriangles/io/libxml.pxd
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     3700 2021-01-25 11:14:28.000000 emeraldtriangles-0.0.8/emeraldtriangles/boundary.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2021-04-07 09:05:31.458942 emeraldtriangles-0.0.9/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       28 2021-03-30 09:42:56.000000 emeraldtriangles-0.0.9/MANIFEST.in
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      370 2021-04-07 09:05:31.458942 emeraldtriangles-0.0.9/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1461 2021-01-26 12:07:16.000000 emeraldtriangles-0.0.9/README.md
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2021-04-07 09:05:31.454942 emeraldtriangles-0.0.9/emeraldtriangles/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      129 2020-08-21 08:50:45.000000 emeraldtriangles-0.0.9/emeraldtriangles/__init__.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     4426 2021-04-07 08:14:58.000000 emeraldtriangles-0.0.9/emeraldtriangles/boundary.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     2276 2021-01-22 08:44:56.000000 emeraldtriangles-0.0.9/emeraldtriangles/cleanup.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2021-04-07 09:05:31.458942 emeraldtriangles-0.0.9/emeraldtriangles/io/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       19 2021-04-06 12:17:37.000000 emeraldtriangles-0.0.9/emeraldtriangles/io/__init__.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     6655 2021-03-30 13:05:47.000000 emeraldtriangles-0.0.9/emeraldtriangles/io/_landxml.pyx
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     6790 2021-03-30 13:06:50.000000 emeraldtriangles-0.0.9/emeraldtriangles/io/landxml.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     2934 2021-03-30 09:41:14.000000 emeraldtriangles-0.0.9/emeraldtriangles/io/libxml.pxd
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     5253 2021-04-07 08:37:12.000000 emeraldtriangles-0.0.9/emeraldtriangles/io/sql.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1608 2021-03-25 16:26:18.000000 emeraldtriangles-0.0.9/emeraldtriangles/io/vtk.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     2882 2021-03-31 12:08:27.000000 emeraldtriangles-0.0.9/emeraldtriangles/plotting.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     3606 2021-01-20 09:58:59.000000 emeraldtriangles-0.0.9/emeraldtriangles/plotting_bokeh.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1772 2021-01-20 09:58:59.000000 emeraldtriangles-0.0.9/emeraldtriangles/points_in_mesh.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     6391 2021-01-22 08:24:22.000000 emeraldtriangles-0.0.9/emeraldtriangles/refine_mesh.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2021-04-07 09:05:31.454942 emeraldtriangles-0.0.9/emeraldtriangles.egg-info/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      370 2021-04-07 09:05:31.000000 emeraldtriangles-0.0.9/emeraldtriangles.egg-info/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      627 2021-04-07 09:05:31.000000 emeraldtriangles-0.0.9/emeraldtriangles.egg-info/SOURCES.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2021-04-07 09:05:31.000000 emeraldtriangles-0.0.9/emeraldtriangles.egg-info/dependency_links.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       80 2021-04-07 09:05:31.000000 emeraldtriangles-0.0.9/emeraldtriangles.egg-info/requires.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       17 2021-04-07 09:05:31.000000 emeraldtriangles-0.0.9/emeraldtriangles.egg-info/top_level.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2021-04-07 09:05:31.458942 emeraldtriangles-0.0.9/setup.cfg
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1828 2021-04-07 09:05:01.000000 emeraldtriangles-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `emeraldtriangles-0.0.8/emeraldtriangles.egg-info/SOURCES.txt` & `emeraldtriangles-0.0.9/emeraldtriangles.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 emeraldtriangles.egg-info/dependency_links.txt
 emeraldtriangles.egg-info/requires.txt
 emeraldtriangles.egg-info/top_level.txt
 emeraldtriangles/io/__init__.py
 emeraldtriangles/io/_landxml.pyx
 emeraldtriangles/io/landxml.py
 emeraldtriangles/io/libxml.pxd
+emeraldtriangles/io/sql.py
 emeraldtriangles/io/vtk.py
```

### Comparing `emeraldtriangles-0.0.8/setup.py` & `emeraldtriangles-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,29 +14,35 @@
 class get_numpy_include(object):
     def __fspath__(self):
         import numpy
         return numpy.get_include()
 
 setuptools.setup(
     name='emeraldtriangles',
-    version='0.0.8',
+    version='0.0.9',
     description='Triangle mesh transforms',
     long_description='Iteratively add points to an existing mesh, calculate mesh bounding polygons etc.',
     long_description_content_type="text/markdown",
     author='Egil Moeller',
     author_email='em@emerld.no',
     url='https://github.com/EMeraldGeo/EmeraldTriangles',
     packages=setuptools.find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "scipy",
         "triangle",
+
+        # Maybe make these optional?
+        "pandasio",
         "lxml",
         "matplotlib",
+        "shapely",
+        "geoalchemy2",
+        "pyproj"
     ],
     setup_requires=[
         'setuptools>=18.0',
         'numpy',
         'cython',
     ],
     package_data={'emeraldtriangles': ['*/*.pyx', '*/*.pxd']},
```

### Comparing `emeraldtriangles-0.0.8/README.md` & `emeraldtriangles-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `emeraldtriangles-0.0.8/emeraldtriangles/cleanup.py` & `emeraldtriangles-0.0.9/emeraldtriangles/cleanup.py`

 * *Files identical despite different names*

### Comparing `emeraldtriangles-0.0.8/emeraldtriangles/points_in_mesh.py` & `emeraldtriangles-0.0.9/emeraldtriangles/points_in_mesh.py`

 * *Files identical despite different names*

### Comparing `emeraldtriangles-0.0.8/emeraldtriangles/refine_mesh.py` & `emeraldtriangles-0.0.9/emeraldtriangles/refine_mesh.py`

 * *Files identical despite different names*

### Comparing `emeraldtriangles-0.0.8/emeraldtriangles/plotting_bokeh.py` & `emeraldtriangles-0.0.9/emeraldtriangles/plotting_bokeh.py`

 * *Files identical despite different names*

### Comparing `emeraldtriangles-0.0.8/emeraldtriangles/plotting.py` & `emeraldtriangles-0.0.9/emeraldtriangles/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 
 # Yeah, module is shadowed by the function...
 plotmod = sys.modules["triangle.plot"]
 
 def triangles(ax, vertices, triangles, zorder=-1, edgecolors="red", facecolors="green", cmap="viridis", **kw):
     args = [vertices["X"], vertices["Y"], triangles[[0, 1, 2]]]
     kwargs = {"zorder": zorder, "edgecolors": edgecolors, "cmap": cmap}
+    kwargs.update(kw.get("triangles_args", {}))
     if "facecolors" in triangles.columns:
         kwargs["facecolors"] = triangles["facecolors"].values
     elif "color" in vertices.columns:
         args.append(vertices["color"].values)
     else:
         kwargs["facecolors"] = np.zeros(len(triangles))
         kwargs["cmap"] = matplotlib.colors.ListedColormap(np.array([matplotlib.colors.to_rgba(facecolors)]))
         
     ax.tripcolor(*args, **kwargs)
 
 def vertices(ax, **kw):
     verts = kw['vertices'][["X", "Y"]].values
 
     args = {}
+    args.update(kw.get("vertices_args", {}))
     if "color" in kw['vertices'].columns:
         args["c"] = kw['vertices']["color"].values
     else:
         args["c"] = np.zeros(len(kw['vertices']))
 
     ax.scatter(kw['vertices']["X"], kw['vertices']["Y"], **args)
     if 'labels' in kw:
@@ -38,14 +40,15 @@
         for i in range(verts.shape[0]):
             ax.text(verts[i, 0], verts[i, 1], str(vm[i]))
 
 def points(ax, **kw):
     verts = kw['points'][["X", "Y"]].values
 
     args = {}
+    kwargs.update(kw.get("points_args", {}))
     if "color" in kw['points'].columns:
         args["c"] = kw['points']["color"].values
     else:
         args["c"] = np.zeros(len(kw['points']))
 
     ax.scatter(kw['points']["X"], kw['points']["Y"], cmap="spring", **args)
```

### Comparing `emeraldtriangles-0.0.8/emeraldtriangles/io/_landxml.pyx` & `emeraldtriangles-0.0.9/emeraldtriangles/io/_landxml.pyx`

 * *Files identical despite different names*

### Comparing `emeraldtriangles-0.0.8/emeraldtriangles/io/landxml.py` & `emeraldtriangles-0.0.9/emeraldtriangles/io/landxml.py`

 * *Files identical despite different names*

### Comparing `emeraldtriangles-0.0.8/emeraldtriangles/io/vtk.py` & `emeraldtriangles-0.0.9/emeraldtriangles/io/vtk.py`

 * *Files identical despite different names*

### Comparing `emeraldtriangles-0.0.8/emeraldtriangles/io/libxml.pxd` & `emeraldtriangles-0.0.9/emeraldtriangles/io/libxml.pxd`

 * *Files identical despite different names*

### Comparing `emeraldtriangles-0.0.8/emeraldtriangles/boundary.py` & `emeraldtriangles-0.0.9/emeraldtriangles/boundary.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import numpy as np
 import pandas as pd
 import scipy.spatial
-
+import shapely.geometry
+import warnings
+    
 from . import cleanup
 
 def mesh_boundary(**tri):
     triangles = tri["triangles"]
 
     if not len(triangles):
         return tri
@@ -71,27 +73,46 @@
 
             pos += 1
             segments.loc[current, "ring"] = ring
             segments.loc[current, "pos"] = pos
             
     return segments
 
-def mesh_boundary_to_pointlists(segments, **tri):
+def _mesh_boundary_to_pointlists(segments, **tri):
     segments = _mesh_boundary_mark_rings(segments)
     
     res = {}
     for ring in segments["ring"].unique():
         ringborders = segments[segments["ring"] == ring]
     
         res[int(ring)] = ringborders[[0, "pos"]].rename(columns={0:"point"}).append(
             ringborders[[1, "pos"]].rename(columns={1:"point"})
         ).sort_values("pos").drop_duplicates("pos")["point"].values
 
     return res
 
+def mesh_boundary_to_pointlists(segments, **tri):
+    warnings.warn("Use mesh_boundary_rings() instead", DeprecationWarning)
+    return _mesh_boundary_to_pointlists(segments, **tri)
+    
+def mesh_boundary_rings(**tri):
+    tri["rings"] = mesh_boundary_to_pointlists(**tri)
+    return tri
+    
+def rings_multipolygon(coord_columns=["X", "Y"], **tri):
+    if "rings" not in tri:
+        tri = mesh_boundary(**tri)
+        tri = mesh_boundary_rings(**tri)
+    return shapely.geometry.MultiPolygon([
+        shapely.geometry.Polygon(
+            shapely.geometry.LineString(
+                tri["vertices"].loc[p][coord_columns].values))
+        for p in tri["rings"].values()])
+
+    
 def vertices_boundary(**tri):
     segments = pd.DataFrame(
         scipy.spatial.ConvexHull(tri["vertices"][["X", "Y"]]).simplices,
         columns=[0,1])
     if "segments" in tri:
         segments = tri["segments"].append(segments)
     tri["segments"] = segments
```

