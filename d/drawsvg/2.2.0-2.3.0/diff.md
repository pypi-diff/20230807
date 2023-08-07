# Comparing `tmp/drawsvg-2.2.0-py3-none-any.whl.zip` & `tmp/drawsvg-2.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 43720 bytes, number of entries: 25
+Zip file size: 43921 bytes, number of entries: 25
 -rw-r--r--  2.0 unx     3138 b- defN 23-Mar-05 09:36 drawsvg/__init__.py
 -rw-r--r--  2.0 unx     6579 b- defN 23-Feb-26 08:59 drawsvg/color.py
 -rw-r--r--  2.0 unx     3801 b- defN 23-Feb-26 08:59 drawsvg/defs.py
 -rw-r--r--  2.0 unx    18852 b- defN 23-Mar-05 11:19 drawsvg/drawing.py
--rw-r--r--  2.0 unx    23503 b- defN 23-Jun-25 22:41 drawsvg/elements.py
+-rw-r--r--  2.0 unx    24425 b- defN 23-Aug-07 03:23 drawsvg/elements.py
 -rw-r--r--  2.0 unx     1663 b- defN 23-Mar-05 11:18 drawsvg/font_embed.py
 -rw-r--r--  2.0 unx     4171 b- defN 23-Mar-05 09:36 drawsvg/frame_animation.py
 -rw-r--r--  2.0 unx     1208 b- defN 23-Feb-26 08:59 drawsvg/jupyter.py
 -rw-r--r--  2.0 unx     3137 b- defN 23-Mar-05 09:37 drawsvg/raster.py
 -rw-r--r--  2.0 unx    15499 b- defN 23-Feb-26 08:59 drawsvg/types.py
 -rw-r--r--  2.0 unx     1625 b- defN 23-Feb-26 08:59 drawsvg/url_encode.py
 -rw-r--r--  2.0 unx     8551 b- defN 23-Mar-05 09:37 drawsvg/video.py
@@ -15,13 +15,13 @@
 -rw-r--r--  2.0 unx     4334 b- defN 23-Feb-26 08:59 drawsvg/native_animation/playback_control_js.py
 -rw-r--r--  2.0 unx     3515 b- defN 23-Feb-26 08:59 drawsvg/native_animation/playback_control_ui.py
 -rw-r--r--  2.0 unx    13377 b- defN 23-Feb-26 08:59 drawsvg/native_animation/synced_animation.py
 -rw-r--r--  2.0 unx       86 b- defN 23-Feb-26 08:59 drawsvg/widgets/__init__.py
 -rw-r--r--  2.0 unx     5179 b- defN 23-Feb-26 08:59 drawsvg/widgets/async_animation.py
 -rw-r--r--  2.0 unx     5606 b- defN 23-Jun-25 22:41 drawsvg/widgets/drawing_javascript.py
 -rw-r--r--  2.0 unx     5612 b- defN 23-Feb-26 08:59 drawsvg/widgets/drawing_widget.py
--rw-r--r--  2.0 unx     1056 b- defN 23-Jun-25 22:43 drawsvg-2.2.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    19605 b- defN 23-Jun-25 22:43 drawsvg-2.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-25 22:43 drawsvg-2.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-25 22:43 drawsvg-2.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2058 b- defN 23-Jun-25 22:43 drawsvg-2.2.0.dist-info/RECORD
-25 files, 152473 bytes uncompressed, 40418 bytes compressed:  73.5%
+-rw-r--r--  2.0 unx     1056 b- defN 23-Aug-07 03:24 drawsvg-2.3.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    19605 b- defN 23-Aug-07 03:24 drawsvg-2.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 03:24 drawsvg-2.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Aug-07 03:24 drawsvg-2.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2058 b- defN 23-Aug-07 03:24 drawsvg-2.3.0.dist-info/RECORD
+25 files, 153395 bytes uncompressed, 40619 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -54,23 +54,23 @@
 
 Filename: drawsvg/widgets/drawing_javascript.py
 Comment: 
 
 Filename: drawsvg/widgets/drawing_widget.py
 Comment: 
 
-Filename: drawsvg-2.2.0.dist-info/LICENSE.txt
+Filename: drawsvg-2.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: drawsvg-2.2.0.dist-info/METADATA
+Filename: drawsvg-2.3.0.dist-info/METADATA
 Comment: 
 
-Filename: drawsvg-2.2.0.dist-info/WHEEL
+Filename: drawsvg-2.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: drawsvg-2.2.0.dist-info/top_level.txt
+Filename: drawsvg-2.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: drawsvg-2.2.0.dist-info/RECORD
+Filename: drawsvg-2.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## drawsvg/elements.py

```diff
@@ -593,7 +593,31 @@
 
     Additional keyword arguments are output as additional arguments to the SVG
     node e.g. fill="red", stroke="#ff4477", stroke_width=2.
     '''
     def __init__(self, cx, cy, r, start_deg, end_deg, cw=False, **kwargs):
         super().__init__(d='', **kwargs)
         self.arc(cx, cy, r, start_deg, end_deg, cw=cw, include_m=True)
+
+class ForeignObject(DrawingBasicElement):
+    '''A foreign object, i.e. for embedding HTML.
+
+    In the context of SVG embedded in an HTML document, the XHTML namespace
+    could be omitted in the foreignObject content, but it is mandatory in the
+    context of an SVG document.
+
+    This element works best when viewing the SVG in a browser. Drawing.rasterize()
+    and Drawing.save_png() are unable to display this element.
+
+    Additional keyword arguments are output as additional arguments to the SVG
+    node e.g. fill="red", stroke="#ff4477", stroke_width=2.
+    '''
+    TAG_NAME = 'foreignObject'
+    has_content = True
+    def __init__(self, content, **kwargs):
+        super().__init__(**kwargs)
+        self.content = content
+    def write_content(self, id_map, is_duplicate, output_file, lcontext,
+                      dry_run):
+        if dry_run:
+            return
+        output_file.write(self.content)
```

## Comparing `drawsvg-2.2.0.dist-info/LICENSE.txt` & `drawsvg-2.3.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `drawsvg-2.2.0.dist-info/METADATA` & `drawsvg-2.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: drawsvg
-Version: 2.2.0
+Version: 2.3.0
 Summary: A Python 3 library for programmatically generating SVG (vector) images and animations.  Drawsvg can also render to PNG, MP4, and display your drawings in Jupyter notebook and Jupyter lab.
 Home-page: https://github.com/cduck/drawsvg
-Download-URL: https://github.com/cduck/drawsvg/archive/2.2.0.tar.gz
+Download-URL: https://github.com/cduck/drawsvg/archive/2.3.0.tar.gz
 Author: Casey Duckering
 Keywords: SVG,draw,graphics,iPython,Jupyter,widget,animation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
 Description-Content-Type: text/markdown
```

## Comparing `drawsvg-2.2.0.dist-info/RECORD` & `drawsvg-2.3.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 drawsvg/__init__.py,sha256=DFTRnzTJfjmmGUiJ-8Z7c0iMa__ocm40Lf5VriYtoPI,3138
 drawsvg/color.py,sha256=vQBQofcfh00l_9uIuLKLQSrgjGrqX-pWIuzgVBwHOAE,6579
 drawsvg/defs.py,sha256=uuttKAY9FXPIJyGqCU8KewS2NEv-iV00t2PtXb96E9s,3801
 drawsvg/drawing.py,sha256=tAooLJbvlkmmo5G_IxcAwOp1rpYFiuuiLFCH2sJlG0Q,18852
-drawsvg/elements.py,sha256=79np8AhWaRlMynOfwmDP79cRRJmKbzX6GYREzVTHCYw,23503
+drawsvg/elements.py,sha256=lFCaMEYBkL26_6WT4aDo0BdENR1aMm416vBkKZ1kXMg,24425
 drawsvg/font_embed.py,sha256=qJCx2o70xIJg6yS75mSN5woNhgze2qs3n1ywxNF7ezw,1663
 drawsvg/frame_animation.py,sha256=zd1uybSRNo2WzXNw2HBFjuo_IdBmgUY07j4p4zsa4xQ,4171
 drawsvg/jupyter.py,sha256=ySYXcTyk9cXuiZ3EK5jUNsBR2Qx09p5IUl_NqIwmKDc,1208
 drawsvg/raster.py,sha256=2B2BSlEGt1hEXdwU0SQ1BQorxpC1_73bqeL4w6IIFcc,3137
 drawsvg/types.py,sha256=WUiw5f35xsV0fHvc25LzmfaEzBKx0nDq__N-cO2eIAo,15499
 drawsvg/url_encode.py,sha256=qIPGrYIntw6oDbQfaR_j5XjBgTt81q0_5NyuDwsSidk,1625
 drawsvg/video.py,sha256=y_mWZcIRfrCelbJhtU6KsK2CjYorzqEXr92hWNWkuQk,8551
@@ -14,12 +14,12 @@
 drawsvg/native_animation/playback_control_js.py,sha256=iFoSN4ML_UMOn7aGcUMkWxBbNbMk1-MksKdtVDVj35U,4334
 drawsvg/native_animation/playback_control_ui.py,sha256=F_Yad3JTZbLNvuoRhm5rwj2Lf82TPBe3OGFZhX258y8,3515
 drawsvg/native_animation/synced_animation.py,sha256=AWraTLsXyw5fZa8j8Qap_1J2o5e9o71vyTt6ccnNRVM,13377
 drawsvg/widgets/__init__.py,sha256=fJ4HrEQAUcw8t8wxU7fC2DZzic82hkVlsxwAnbp9OiA,86
 drawsvg/widgets/async_animation.py,sha256=UQn5yglmX_peFDyTULjAvPAgZpOrx9pdAoC3WaAUyOc,5179
 drawsvg/widgets/drawing_javascript.py,sha256=FisdUR5JPT6VK44lU2zlMW40a3PoK0MYr90C7Ake1DY,5606
 drawsvg/widgets/drawing_widget.py,sha256=7GlrRoUTyCggxYa0pFPpuvt5uDsolt9Alv7JYQCwG_A,5612
-drawsvg-2.2.0.dist-info/LICENSE.txt,sha256=WTZNjuw3IxMpVOJgV10X86n9R_LwSSvLza93_LpuEP0,1056
-drawsvg-2.2.0.dist-info/METADATA,sha256=uHY_-blg5ZrSTnstNwjo2yVm9Njawtk5MaiwmwtPK6w,19605
-drawsvg-2.2.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-drawsvg-2.2.0.dist-info/top_level.txt,sha256=4Y7gx7Sf-uUGFe1Avyu7Pwe43DeluiOhQyyBvMHSFsA,8
-drawsvg-2.2.0.dist-info/RECORD,,
+drawsvg-2.3.0.dist-info/LICENSE.txt,sha256=WTZNjuw3IxMpVOJgV10X86n9R_LwSSvLza93_LpuEP0,1056
+drawsvg-2.3.0.dist-info/METADATA,sha256=BJ6eIXag2p3zQxs7Fu1RzSJg8iAhmIWZOQMCrL3Ge5o,19605
+drawsvg-2.3.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+drawsvg-2.3.0.dist-info/top_level.txt,sha256=4Y7gx7Sf-uUGFe1Avyu7Pwe43DeluiOhQyyBvMHSFsA,8
+drawsvg-2.3.0.dist-info/RECORD,,
```

