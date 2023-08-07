# Comparing `tmp/imephu-0.5.0.tar.gz` & `tmp/imephu-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imephu-0.5.0.tar", max compression
+gzip compressed data, was "imephu-0.6.0.tar", max compression
```

## Comparing `imephu-0.5.0.tar` & `imephu-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1102 2023-07-10 14:47:42.674953 imephu-0.5.0/LICENSE
--rw-r--r--   0        0        0     1015 2023-07-10 14:47:42.675169 imephu-0.5.0/README.md
--rw-r--r--   0        0        0      991 2023-07-18 15:32:46.998895 imephu-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      235 2023-07-12 17:32:34.546165 imephu-0.5.0/src/imephu/__init__.py
--rw-r--r--   0        0        0     1550 2023-07-10 14:47:42.735797 imephu-0.5.0/src/imephu/annotation/__init__.py
--rw-r--r--   0        0        0      746 2023-07-10 14:47:42.736360 imephu-0.5.0/src/imephu/annotation/general/__init__.py
--rw-r--r--   0        0        0     4480 2023-07-10 14:47:42.736748 imephu-0.5.0/src/imephu/annotation/general/arrow.py
--rw-r--r--   0        0        0     3879 2023-07-10 14:47:42.737079 imephu-0.5.0/src/imephu/annotation/general/circle.py
--rw-r--r--   0        0        0     2581 2023-07-10 14:47:42.737385 imephu-0.5.0/src/imephu/annotation/general/crosshairs.py
--rw-r--r--   0        0        0     1646 2023-07-10 14:47:42.737673 imephu-0.5.0/src/imephu/annotation/general/empty.py
--rw-r--r--   0        0        0     3021 2023-07-10 14:47:42.738079 imephu-0.5.0/src/imephu/annotation/general/group.py
--rw-r--r--   0        0        0     4428 2023-07-10 14:47:42.738417 imephu-0.5.0/src/imephu/annotation/general/line_path.py
--rw-r--r--   0        0        0     4425 2023-07-10 14:47:42.738680 imephu-0.5.0/src/imephu/annotation/general/rectangle.py
--rw-r--r--   0        0        0     5316 2023-07-10 14:47:42.738939 imephu-0.5.0/src/imephu/annotation/general/text.py
--rw-r--r--   0        0        0     9170 2023-07-10 14:47:42.739226 imephu-0.5.0/src/imephu/annotation/motion.py
--rw-r--r--   0        0        0    12400 2023-07-14 17:06:28.689624 imephu-0.5.0/src/imephu/cli.py
--rw-r--r--   0        0        0    12907 2023-07-10 14:47:42.739791 imephu-0.5.0/src/imephu/finder_chart.py
--rw-r--r--   0        0        0     9710 2023-07-10 14:47:42.740083 imephu-0.5.0/src/imephu/geometry.py
--rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740215 imephu-0.5.0/src/imephu/py.typed
--rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740669 imephu-0.5.0/src/imephu/salt/annotation/__init__.py
--rw-r--r--   0        0        0    12623 2023-07-12 17:32:34.547738 imephu-0.5.0/src/imephu/salt/annotation/nir.py
--rw-r--r--   0        0        0     4365 2023-07-14 17:06:28.691527 imephu-0.5.0/src/imephu/salt/annotation/rss.py
--rw-r--r--   0        0        0     1195 2023-07-10 14:47:42.741408 imephu-0.5.0/src/imephu/salt/annotation/salticam.py
--rw-r--r--   0        0        0     9004 2023-07-10 14:47:42.741632 imephu-0.5.0/src/imephu/salt/annotation/telescope.py
--rw-r--r--   0        0        0    15615 2023-07-14 17:06:28.692233 imephu-0.5.0/src/imephu/salt/finder_chart.py
--rw-r--r--   0        0        0     4859 2023-07-10 14:47:42.742110 imephu-0.5.0/src/imephu/salt/utils.py
--rw-r--r--   0        0        0    10500 2023-07-14 17:06:28.692870 imephu-0.5.0/src/imephu/schema.json
--rw-r--r--   0        0        0     9716 2023-07-18 15:32:47.000288 imephu-0.5.0/src/imephu/service/horizons.py
--rw-r--r--   0        0        0    15225 2023-07-10 14:47:42.742998 imephu-0.5.0/src/imephu/service/survey.py
--rw-r--r--   0        0        0     4149 2023-07-18 15:32:47.001155 imephu-0.5.0/src/imephu/utils.py
--rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 imephu-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-07-10 14:47:42.674953 imephu-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1015 2023-07-10 14:47:42.675169 imephu-0.6.0/README.md
+-rw-r--r--   0        0        0      991 2023-08-07 08:19:38.842172 imephu-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      235 2023-07-12 17:32:34.546165 imephu-0.6.0/src/imephu/__init__.py
+-rw-r--r--   0        0        0     1550 2023-07-10 14:47:42.735797 imephu-0.6.0/src/imephu/annotation/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-10 14:47:42.736360 imephu-0.6.0/src/imephu/annotation/general/__init__.py
+-rw-r--r--   0        0        0     4480 2023-07-10 14:47:42.736748 imephu-0.6.0/src/imephu/annotation/general/arrow.py
+-rw-r--r--   0        0        0     3879 2023-07-10 14:47:42.737079 imephu-0.6.0/src/imephu/annotation/general/circle.py
+-rw-r--r--   0        0        0     2581 2023-07-10 14:47:42.737385 imephu-0.6.0/src/imephu/annotation/general/crosshairs.py
+-rw-r--r--   0        0        0     1646 2023-07-10 14:47:42.737673 imephu-0.6.0/src/imephu/annotation/general/empty.py
+-rw-r--r--   0        0        0     3021 2023-07-10 14:47:42.738079 imephu-0.6.0/src/imephu/annotation/general/group.py
+-rw-r--r--   0        0        0     4425 2023-08-07 08:19:38.844259 imephu-0.6.0/src/imephu/annotation/general/line_path.py
+-rw-r--r--   0        0        0     4425 2023-07-10 14:47:42.738680 imephu-0.6.0/src/imephu/annotation/general/rectangle.py
+-rw-r--r--   0        0        0     6905 2023-08-07 08:19:38.844755 imephu-0.6.0/src/imephu/annotation/general/scale_bar.py
+-rw-r--r--   0        0        0     5330 2023-08-07 08:19:38.845255 imephu-0.6.0/src/imephu/annotation/general/text.py
+-rw-r--r--   0        0        0     9170 2023-07-10 14:47:42.739226 imephu-0.6.0/src/imephu/annotation/motion.py
+-rw-r--r--   0        0        0    12400 2023-07-14 17:06:28.689624 imephu-0.6.0/src/imephu/cli.py
+-rw-r--r--   0        0        0    12907 2023-07-10 14:47:42.739791 imephu-0.6.0/src/imephu/finder_chart.py
+-rw-r--r--   0        0        0     9710 2023-07-10 14:47:42.740083 imephu-0.6.0/src/imephu/geometry.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740215 imephu-0.6.0/src/imephu/py.typed
+-rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740669 imephu-0.6.0/src/imephu/salt/annotation/__init__.py
+-rw-r--r--   0        0        0    12623 2023-07-12 17:32:34.547738 imephu-0.6.0/src/imephu/salt/annotation/nir.py
+-rw-r--r--   0        0        0     4365 2023-07-14 17:06:28.691527 imephu-0.6.0/src/imephu/salt/annotation/rss.py
+-rw-r--r--   0        0        0     1195 2023-07-10 14:47:42.741408 imephu-0.6.0/src/imephu/salt/annotation/salticam.py
+-rw-r--r--   0        0        0     9160 2023-08-07 08:19:38.845769 imephu-0.6.0/src/imephu/salt/annotation/telescope.py
+-rw-r--r--   0        0        0    15615 2023-07-14 17:06:28.692233 imephu-0.6.0/src/imephu/salt/finder_chart.py
+-rw-r--r--   0        0        0     4859 2023-07-10 14:47:42.742110 imephu-0.6.0/src/imephu/salt/utils.py
+-rw-r--r--   0        0        0    10500 2023-07-14 17:06:28.692870 imephu-0.6.0/src/imephu/schema.json
+-rw-r--r--   0        0        0     9716 2023-07-18 15:32:47.000288 imephu-0.6.0/src/imephu/service/horizons.py
+-rw-r--r--   0        0        0    15225 2023-07-10 14:47:42.742998 imephu-0.6.0/src/imephu/service/survey.py
+-rw-r--r--   0        0        0     4149 2023-07-18 15:32:47.001155 imephu-0.6.0/src/imephu/utils.py
+-rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 imephu-0.6.0/PKG-INFO
```

### Comparing `imephu-0.5.0/LICENSE` & `imephu-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/README.md` & `imephu-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/pyproject.toml` & `imephu-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imephu"
-version = "0.5.0"
+version = "0.6.0"
 description = "Generate finder charts for astronomical observations."
 authors = ["Southern African Large Telescope"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `imephu-0.5.0/src/imephu/annotation/__init__.py` & `imephu-0.6.0/src/imephu/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/annotation/general/__init__.py` & `imephu-0.6.0/src/imephu/annotation/general/__init__.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/annotation/general/arrow.py` & `imephu-0.6.0/src/imephu/annotation/general/arrow.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/annotation/general/circle.py` & `imephu-0.6.0/src/imephu/annotation/general/circle.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/annotation/general/crosshairs.py` & `imephu-0.6.0/src/imephu/annotation/general/crosshairs.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/annotation/general/empty.py` & `imephu-0.6.0/src/imephu/annotation/general/empty.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/annotation/general/group.py` & `imephu-0.6.0/src/imephu/annotation/general/group.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/annotation/general/line_path.py` & `imephu-0.6.0/src/imephu/annotation/general/line_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 class LinePathAnnotation(Annotation):
     """An annotation consisting of straight lines between vertices.
 
     The path displayed by this annotation is defined by a set of vertices, which are
     connected by straight lines on the finder chart. (The connecting lines in general
     will refer to curved lines on the sky.)
 
-    By default the path is assumed to be closed, i.e. the last vertex is connected to
+    By default, the path is assumed to be closed, i.e. the last vertex is connected to
     the first by a line. This behavior may be changed with the ``closed`` parameter.
 
     Parameters
     ----------
     vertices: sequence of `~astropy.coordinates.SkyCoord`
         The path vertices, as an array or sequence of sky coordinates (with right
-        ascension abd declination).
+        ascension and declination).
     wcs: `~astropy.wcs.WCS`
         WCS object.
     closed: bool, default: True
-        Whether the the path is closed, i.e. whether the last vertex is connected to the
+        Whether the path is closed, i.e. whether the last vertex is connected to the
         first by a line.
     edgecolor: color, default: "black"
         The edge color.
     facecolor: color, default: "none"
         The filling color.
     **kwargs: dict, optional
         Additional keyword arguments, which will be passed to Matplotlib's
```

### Comparing `imephu-0.5.0/src/imephu/annotation/general/rectangle.py` & `imephu-0.6.0/src/imephu/annotation/general/rectangle.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/annotation/general/text.py` & `imephu-0.6.0/src/imephu/annotation/general/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         The `rotate` method rotates the text position, but not the text itself. If you
         want to rotate the text rather than the text position, you should use the
         ``rotation`` parameter with the angle in degrees.
 
 
     Parameters
     ----------
-    position: `~astropy.coordinates.SkyCoord` or
+    position: `~astropy.coordinates.SkyCoord` or list of float
         The right ascension and declination of the point where to put the text.
     s: str
         The text.
     wcs: `~astropy.wcs.WCS`
         WCS object.
     color: color, default: "black"
         The text color.
```

### Comparing `imephu-0.5.0/src/imephu/annotation/motion.py` & `imephu-0.6.0/src/imephu/annotation/motion.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/cli.py` & `imephu-0.6.0/src/imephu/cli.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/finder_chart.py` & `imephu-0.6.0/src/imephu/finder_chart.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/geometry.py` & `imephu-0.6.0/src/imephu/geometry.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/salt/annotation/nir.py` & `imephu-0.6.0/src/imephu/salt/annotation/nir.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/salt/annotation/rss.py` & `imephu-0.6.0/src/imephu/salt/annotation/rss.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/salt/annotation/salticam.py` & `imephu-0.6.0/src/imephu/salt/annotation/salticam.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/salt/annotation/telescope.py` & `imephu-0.6.0/src/imephu/salt/annotation/telescope.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from imephu.annotation.general import (
     CrosshairsAnnotation,
     EmptyAnnotation,
     GroupAnnotation,
     RectangleAnnotation,
     TextAnnotation,
 )
+from imephu.annotation.general.scale_bar import ScaleBarLineAnnotation
 from imephu.salt.annotation import rss, salticam
 
 
 def title_annotation(
     target: str, proposal_code: str, pi_family_name: str, wcs: WCS
 ) -> TextAnnotation:
     """Return a text annotation with the title to the finder chart.
@@ -288,14 +289,15 @@
                 automated_position_angle=automated_position_angle,
                 wcs=wcs,
             ),
             directions_annotation(fits_center=fits_center, wcs=wcs),
             _crosshairs_annotation(fits_center=fits_center, wcs=wcs),
             salticam.field_of_view_annotation(fits_center=fits_center, wcs=wcs),
             rss.field_of_view_annotation(fits_center=fits_center, wcs=wcs),
+            ScaleBarLineAnnotation(left_edge=(50, 50), minimum_length=100, wcs=wcs),
         ]
     )
 
 
 def _crosshairs_annotation(fits_center: SkyCoord, wcs: WCS) -> CrosshairsAnnotation:
     return CrosshairsAnnotation(
         center=fits_center, size=8 * u.arcmin, wcs=wcs, color="green"
```

### Comparing `imephu-0.5.0/src/imephu/salt/finder_chart.py` & `imephu-0.6.0/src/imephu/salt/finder_chart.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/salt/utils.py` & `imephu-0.6.0/src/imephu/salt/utils.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/schema.json` & `imephu-0.6.0/src/imephu/schema.json`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/service/horizons.py` & `imephu-0.6.0/src/imephu/service/horizons.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/service/survey.py` & `imephu-0.6.0/src/imephu/service/survey.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/src/imephu/utils.py` & `imephu-0.6.0/src/imephu/utils.py`

 * *Files identical despite different names*

### Comparing `imephu-0.5.0/PKG-INFO` & `imephu-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imephu
-Version: 0.5.0
+Version: 0.6.0
 Summary: Generate finder charts for astronomical observations.
 License: MIT
 Author: Southern African Large Telescope
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

