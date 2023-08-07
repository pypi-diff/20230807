# Comparing `tmp/image2layout_computer_vision-0.1.2.tar.gz` & `tmp/image2layout_computer_vision-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2layout_computer_vision-0.1.2.tar", last modified: Mon Aug  7 07:01:58 2023, max compression
+gzip compressed data, was "image2layout_computer_vision-0.1.3.tar", last modified: Mon Aug  7 07:29:37 2023, max compression
```

## Comparing `image2layout_computer_vision-0.1.2.tar` & `image2layout_computer_vision-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:01:58.914640 image2layout_computer_vision-0.1.2/
--rw-rw-r--   0 test      (1001) test      (1001)     1073 2023-07-20 04:03:09.000000 image2layout_computer_vision-0.1.2/LICENSE
--rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 07:01:58.914640 image2layout_computer_vision-0.1.2/PKG-INFO
--rw-rw-r--   0 test      (1001) test      (1001)     2224 2023-08-07 06:13:00.000000 image2layout_computer_vision-0.1.2/README.md
--rw-rw-r--   0 test      (1001) test      (1001)      637 2023-08-07 06:41:56.000000 image2layout_computer_vision-0.1.2/pyproject.toml
--rw-rw-r--   0 test      (1001) test      (1001)       38 2023-08-07 07:01:58.914640 image2layout_computer_vision-0.1.2/setup.cfg
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:01:58.910640 image2layout_computer_vision-0.1.2/src/
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:01:58.910640 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/
--rw-rw-r--   0 test      (1001) test      (1001)      613 2023-08-04 08:58:07.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/__init__.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:01:58.910640 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/color_extract/
--rw-rw-r--   0 test      (1001) test      (1001)       95 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/color_extract/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)    14464 2023-08-03 04:42:22.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/color_extract/main.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:01:58.914640 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/
--rw-rw-r--   0 test      (1001) test      (1001)      251 2023-08-04 08:48:54.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)    16347 2023-08-07 06:50:31.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/imagebox.py
--rw-rw-r--   0 test      (1001) test      (1001)     3748 2023-08-07 07:00:33.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/main.py
--rw-rw-r--   0 test      (1001) test      (1001)     6286 2023-07-26 05:47:05.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
--rw-rw-r--   0 test      (1001) test      (1001)     2331 2023-08-07 06:43:03.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/model_paddle.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:01:58.914640 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/
--rw-rw-r--   0 test      (1001) test      (1001)      457 2023-08-04 08:57:51.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)     7186 2023-08-04 09:09:14.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/annotation.py
--rw-rw-r--   0 test      (1001) test      (1001)     4896 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/color_system.py
--rw-rw-r--   0 test      (1001) test      (1001)     3820 2023-08-03 10:44:05.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/imaging.py
--rw-rw-r--   0 test      (1001) test      (1001)     2402 2023-08-02 09:28:26.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/pixel_mask.py
--rw-rw-r--   0 test      (1001) test      (1001)     5469 2023-08-03 03:51:23.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/timing.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:01:58.910640 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision.egg-info/
--rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 07:01:58.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision.egg-info/PKG-INFO
--rw-rw-r--   0 test      (1001) test      (1001)     1052 2023-08-07 07:01:58.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision.egg-info/SOURCES.txt
--rw-rw-r--   0 test      (1001) test      (1001)        1 2023-08-07 07:01:58.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision.egg-info/dependency_links.txt
--rw-rw-r--   0 test      (1001) test      (1001)       74 2023-08-07 07:01:58.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision.egg-info/top_level.txt
--rw-rw-r--   0 test      (1001) test      (1001)    11005 2023-07-26 06:47:33.000000 image2layout_computer_vision-0.1.2/src/sandbox.py
--rw-rw-r--   0 test      (1001) test      (1001)    11193 2023-08-03 04:03:51.000000 image2layout_computer_vision-0.1.2/src/sandbox_color.py
--rw-rw-r--   0 test      (1001) test      (1001)     1246 2023-08-04 09:11:31.000000 image2layout_computer_vision-0.1.2/src/sandbox_ocr.py
--rw-rw-r--   0 test      (1001) test      (1001)      812 2023-08-03 04:47:50.000000 image2layout_computer_vision-0.1.2/src/test_color.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/
+-rw-rw-r--   0 test      (1001) test      (1001)     1073 2023-07-20 04:03:09.000000 image2layout_computer_vision-0.1.3/LICENSE
+-rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/PKG-INFO
+-rw-rw-r--   0 test      (1001) test      (1001)     2224 2023-08-07 06:13:00.000000 image2layout_computer_vision-0.1.3/README.md
+-rw-rw-r--   0 test      (1001) test      (1001)      637 2023-08-07 07:29:17.000000 image2layout_computer_vision-0.1.3/pyproject.toml
+-rw-rw-r--   0 test      (1001) test      (1001)       38 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/setup.cfg
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/src/
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/
+-rw-rw-r--   0 test      (1001) test      (1001)      573 2023-08-07 07:13:24.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/__init__.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/color_extract/
+-rw-rw-r--   0 test      (1001) test      (1001)       95 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/color_extract/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)    14464 2023-08-03 04:42:22.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/color_extract/main.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/
+-rw-rw-r--   0 test      (1001) test      (1001)      211 2023-08-07 07:13:29.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)    16366 2023-08-07 07:23:41.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/imagebox.py
+-rw-rw-r--   0 test      (1001) test      (1001)     3080 2023-08-07 07:13:37.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/main.py
+-rw-rw-r--   0 test      (1001) test      (1001)     6286 2023-07-26 05:47:05.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
+-rw-rw-r--   0 test      (1001) test      (1001)     2291 2023-08-07 07:23:57.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/model_paddle.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/
+-rw-rw-r--   0 test      (1001) test      (1001)      333 2023-08-07 07:24:03.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)     7645 2023-08-07 07:20:31.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/annotation.py
+-rw-rw-r--   0 test      (1001) test      (1001)     4896 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/color_system.py
+-rw-rw-r--   0 test      (1001) test      (1001)     3820 2023-08-03 10:44:05.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/imaging.py
+-rw-rw-r--   0 test      (1001) test      (1001)     2402 2023-08-02 09:28:26.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/pixel_mask.py
+-rw-rw-r--   0 test      (1001) test      (1001)     5469 2023-08-03 03:51:23.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/timing.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision.egg-info/
+-rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 07:29:37.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision.egg-info/PKG-INFO
+-rw-rw-r--   0 test      (1001) test      (1001)     1052 2023-08-07 07:29:37.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision.egg-info/SOURCES.txt
+-rw-rw-r--   0 test      (1001) test      (1001)        1 2023-08-07 07:29:37.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision.egg-info/dependency_links.txt
+-rw-rw-r--   0 test      (1001) test      (1001)       74 2023-08-07 07:29:37.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision.egg-info/top_level.txt
+-rw-rw-r--   0 test      (1001) test      (1001)    11005 2023-07-26 06:47:33.000000 image2layout_computer_vision-0.1.3/src/sandbox.py
+-rw-rw-r--   0 test      (1001) test      (1001)    11193 2023-08-03 04:03:51.000000 image2layout_computer_vision-0.1.3/src/sandbox_color.py
+-rw-rw-r--   0 test      (1001) test      (1001)     1246 2023-08-04 09:11:31.000000 image2layout_computer_vision-0.1.3/src/sandbox_ocr.py
+-rw-rw-r--   0 test      (1001) test      (1001)      812 2023-08-03 04:47:50.000000 image2layout_computer_vision-0.1.3/src/test_color.py
```

### Comparing `image2layout_computer_vision-0.1.2/LICENSE` & `image2layout_computer_vision-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.2/PKG-INFO` & `image2layout_computer_vision-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2layout_computer_vision
-Version: 0.1.2
+Version: 0.1.3
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `image2layout_computer_vision-0.1.2/README.md` & `image2layout_computer_vision-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.2/pyproject.toml` & `image2layout_computer_vision-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "Pillow",
   "numpy",
   "pandas",
 ]
 
 [project]
 name = "image2layout_computer_vision"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Felix Do", email="felix.do.1030@gmail.com" },
 ]
 description = "image processing and stuff"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/__init__.py` & `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from . import ocr, color_extract, utils
 
-from .ocr import detect_text, detect_text_boxes, ImageBoxes, BoxMerge, model_dispatch, detect_text_full
+from .ocr import detect_text, detect_text_full, ImageBoxes, BoxMerge, model_dispatch
 from .color_extract import ColorExtractor, extract_colors
 from .utils import get_image, ImageConvert, COLOR, PixelMask, ImageTransform, Chrono, Timer, AnnoDraw
 
 __all__ = [
     'ocr', 'color_extract', 'utils',
-    'detect_text', 'detect_text_boxes', 'detect_text_full',
+    'detect_text', 'detect_text_full',
     'ImageBoxes', 'BoxMerge', 'model_dispatch', 
     'ColorExtractor', 'extract_colors',
     'get_image', 'ImageConvert', 'COLOR', 'PixelMask', 'ImageTransform',
     'Chrono', 'Timer', 'AnnoDraw',
 ]
```

### Comparing `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/color_extract/main.py` & `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/color_extract/main.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/imagebox.py` & `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/imagebox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # %%
 import os
 import json
 import colorsys
 import numpy as np
 import pandas as pd
 from PIL import Image, ImageDraw, ImageFont
-from ..utils import get_image, draw_anno_box
+from ..utils import get_image, AnnoDraw
 from typing import Union, Dict, Tuple, List, Any
 
 # %%
 class BoxMerge:
     
     @classmethod
     def same_column_match(cls,
@@ -346,22 +346,22 @@
                 draw_level_0=False,
                 img_base=None,
                 draw_size=True,
                 color=None,
                 ):
         assert mode in ['box', 'mask', 'all']
         
-        overlay_anno_bottom = draw_anno_box(
+        overlay_anno_bottom = AnnoDraw.draw_anno_box(
             self.size,
             boxes=self.boxes,
             color='#00FF00',
             color_text='#000000',
         )
         
-        overlay_anno_top = draw_anno_box(
+        overlay_anno_top = AnnoDraw.draw_anno_box(
             self.size,
             boxes=self.boxes_top,
             color='#FF00FF',
             color_text='#000000',
         )
         overlay_anno = Image.alpha_composite(
             overlay_anno_bottom,
@@ -375,24 +375,24 @@
         return img_anno
     
     def to_grouped_imageboxes(self, **kwargs):
         '''group boxes with `grouped_boxes` from self and return an ImageBoxes with grouped boxes
         '''
         
         if len(self.boxes) > 0:
-            boxes_nested_final = self.group_boxes(self.boxes, **kwargs)
+            boxes_grouped_final = self.group_boxes(self.boxes, **kwargs)
         else:
-            boxes_nested_final = np.array(self.boxes)
+            boxes_grouped_final = np.array(self.boxes)
         
-        imageboxes_nested = ImageBoxes(
-            boxes=boxes_nested_final,
+        imageboxes_grouped = ImageBoxes(
+            boxes=boxes_grouped_final,
             image=self.image.copy(),
         )
-        imageboxes_nested.set_texts(self.texts)
-        return imageboxes_nested
+        imageboxes_grouped.set_texts(self.texts)
+        return imageboxes_grouped
     
     @classmethod
     def group_boxes(cls,
                 boxes:Union[np.ndarray, list],
                 line_dist_max:float=1.0,
                 line_dist_min:float=-0.1,
                 line_iou_min:float=0.4,
```

### Comparing `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/main.py` & `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,87 +17,64 @@
 debug_logger.setLevel(logging.WARNING)
 
 # %%
 # from .model_layoutmlv2 import ModelDispatch_LayoutMLv2
 # model_dispatch_layout = ModelDispatch_LayoutMLv2(
 #     device='cpu',
 # )
+# model_dispatch = model_dispatch_layout
 
 # %%
 from .model_paddle import ModelDispatch_Paddle
 model_dispatch_paddle = ModelDispatch_Paddle(
     device='cpu',
 )
-
-# %%
 model_dispatch = model_dispatch_paddle
 
 # %%
-def detect_text(image: Union[Image.Image, np.ndarray], merge_boxes=True, **kwargs) -> ImageBoxes:
+def detect_text(image: Union[Image.Image, np.ndarray], **kwargs) -> Tuple[ImageBoxes]:
     '''predict boxes for text in the image
     Parameters:
         image: (PIL.Image.Image, np.ndarray) RGB image
         **kwargs:
             line_dist_max:          max distance between boxes to be in the same sentence (as a ratio of line height)
             line_dist_min:          min (negative) distance between boxes to be in the same sentence (as a ratio of line height)
             line_iou_min:           min vertical iou between boxes to be on the same line
             row_hdist_max:          max horizontal offset between rows to aligned as a column (as a ratio of line height)
             row_vdist_max:          max vertical distance between rows to be in the same column (as a ratio of line height)
             row_height_ratio_min:   min ratio between heights of rows to be in the same column
     Returns:
-        imageboxes: (ImageBoxes) object containing prediction boxes
+        imageboxes_merged: (ImageBoxes) object containing merged prediction boxes
+        imageboxes_raw:    (ImageBoxes) object containing raw prediction boxes
     '''
     _image = get_image(image).convert('RGB')
     debug_logger.debug(msg=f'detect_text | input[{_image.size}]')
     
     result_df = model_dispatch_paddle(_image)
     
     imageboxes_raw = ImageBoxes(
         image=_image,
         boxes=result_df['box'].tolist(),
     )
-    if merge_boxes:
-        imageboxes = imageboxes_raw.to_grouped_imageboxes(**kwargs)
-        debug_logger.debug(msg=f'detect_text | merged[{len(imageboxes_raw.boxes_top)} -> {len(imageboxes.boxes_top)}]')
-        return imageboxes
+    imageboxes_raw.set_texts(result_df['text'].tolist())
     
-    return imageboxes_raw
-
-# %%
-def detect_text_boxes(image: Union[Image.Image, np.ndarray], **kwargs) -> Tuple[np.ndarray, np.ndarray]:
-    '''predict boxes for text in the image
-    Parameters: (same as detect_text)
-    Returns:
-        boxes_merged: (np.ndarray) [M, 4] text boxes detected, merged boxes
-        boxes_raw:    (np.ndarray) [N, 4] text boxes detected, all individual boxes (N >= M)
-    '''
-    imageboxes = detect_text(image, **kwargs)
+    imageboxes_merged = imageboxes_raw.to_grouped_imageboxes(**kwargs)
+    debug_logger.debug(msg=f'detect_text | merged[{len(imageboxes_raw.boxes_top)} -> {len(imageboxes_merged.boxes_top)}]')
     
-    boxes_merged = np.array(imageboxes.boxes_top, int)
-    boxes_raw = np.array(imageboxes.boxes, int)
-    return boxes_merged, boxes_raw
+    return imageboxes_merged, imageboxes_raw
 
 # %%
-def detect_text_full(image: Union[Image.Image, np.ndarray], **kwargs) -> List[Dict]:
+def detect_text_full(image: Union[Image.Image, np.ndarray], **kwargs) -> Tuple[List[Dict]]:
     '''detect and recognize text in the image and merge them, returning raw and merged data
     Parameters: (same as detect_text)
     Returns:
         data_merged: (list of dicts) merged result texts, boxes and scores
         data_raw:    (list of dicts) raw result texts, boxes and scores
     '''
-    _image = get_image(image).convert('RGB')
-    result_df = model_dispatch_paddle(_image)
-    
-    imageboxes_raw = ImageBoxes(
-        image=_image,
-        boxes=result_df['box'].tolist(),
-    )
-    imageboxes_raw.set_texts(result_df['text'].tolist())
-    
-    imageboxes_merged = imageboxes_raw.to_grouped_imageboxes(**kwargs)
+    imageboxes_merged, imageboxes_raw = detect_text(image, **kwargs)
     
     return imageboxes_merged.df_top.to_dict('records'), imageboxes_raw.df_top.to_dict('records')
 
 # %%
 if __name__ == '__main__':
     data_merged, data_raw = detect_text_full('path/to/the/image.png')
```

### Comparing `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/model_layoutmlv2.py` & `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/model_layoutmlv2.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/model_paddle.py` & `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/model_paddle.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time, os
 import numpy as np
 import pandas as pd
 import string
 import colorsys
 from PIL import Image, ImageDraw, ImageFont
 
-from ..utils import draw_anno_text_overlay
+from ..utils import AnnoDraw
 
 # %%
 class ModelDispatch_Paddle:
     def __init__(self,
                 device='cpu',
                 auto_load=False,
                 log_telemetry=False,
@@ -30,19 +30,20 @@
             self._load()
     
     
     def __call__(self, *args, **kwargs):
         return self.forward(*args, **kwargs)
     
     def _load(self):
-        from paddleocr import PaddleOCR, draw_ocr
+        from paddleocr import PaddleOCR
         self.paddle_ocr = PaddleOCR(
             lang=self.lang,
             use_gpu=self.device in ['cuda'],
             use_angle_cls=True,
+            show_log=False,
         )
         self.loaded = True
     
     def _unload(self):
         del self.paddle_ocr
         self.paddle_ocr = None
         self.loaded = False
@@ -61,16 +62,14 @@
             time_elapsed = time.perf_counter() - time_start
             self.telemetry['forward_time'].append(time_elapsed)
             self.telemetry['forward_time'] = self.telemetry['forward_time'][-20:]
         
         return _output
     
     def _forward(self, image:Image.Image) -> pd.DataFrame:
-        width, height = image.size
-        
         result = self.paddle_ocr.ocr(np.array(image.convert('RGB')), cls=True)
         
         result_df = pd.DataFrame(
             data=[
                 {
                     'text': d[1][0],
                     'score': d[1][1],
```

### Comparing `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/annotation.py` & `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/annotation.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,231 +2,226 @@
 import os, time, string, json
 import numpy as np
 import pandas as pd
 import colorsys
 from PIL import Image, ImageFont, ImageDraw
 from typing import Union, Any, List, Dict, Tuple
 from .color_system import COLOR
+from .imaging import ImageConvert, get_image
 
 # %%
-# FONT_PATH = 'utils/OpenSans_Condensed-Medium.ttf'
-# FONT_PATH = 'OpenSans_Condensed-Medium.ttf'
 FONT_PATH = os.path.join(os.path.split(__file__)[0], 'OpenSans_Condensed-Medium.ttf')
 
 # %%
-def draw_anno_box(
-            img=(10, 10),
-            boxes:Union[np.ndarray, list]=[],
-            texts=None,
-            width=None,
-            text_pad=None,
-            color='#00FF00',
-            color_text='#000000',
-            font=FONT_PATH,
-            opacity=1.0,
-            ):
-    
-    if isinstance(img, (tuple, list)):
-        size = tuple(img)
-    else:
-        size = img.size
-    
-    img_anno = Image.new('RGBA', size)
-    
-    size_min = (min(size) + np.linalg.norm(size)) / 2
-    if isinstance(font, str) and os.path.isfile(font):
-        font = ImageFont.truetype(font, int(size_min // 60))
-    else:
-        font = ImageFont.load_default()
-    
-    width = int(max(size_min // 600 if width is None else width, 1))
-    text_pad = int(max(size_min // 400 if text_pad is None else text_pad, 1))
-    
-    draw = ImageDraw.Draw(img_anno)
-    drawing_texts = isinstance(texts, list) and len(texts) == len(boxes)
-    for i, box in enumerate(boxes):
-        _box = np.array(box)
-        draw.rectangle(
-            tuple(_box),
-            outline=color,
-            width=width,
-        )
+class AnnoDraw:
+    
+    @classmethod
+    def draw_anno_box(cls,
+                img=(10, 10),
+                boxes:Union[np.ndarray, list]=[],
+                texts=None,
+                width=None,
+                text_pad=None,
+                color='#00FF00',
+                color_text='#000000',
+                font=FONT_PATH,
+                opacity=1.0,
+                ):
+    
+        if isinstance(img, (tuple, list)):
+            size = tuple(img)
+        else:
+            size = img.size
         
-        if drawing_texts:
-            _size = _box[2:] - _box[:2]
-            # _text = f'{_size[0]}•{_size[1]}'
-            _text = texts[i]
-            _text_box = np.array(font.getbbox(_text))
-            _text_size = _text_box[2:] - _text_box[:2] + [text_pad * 2] * 2
-            _text_box_padded = np.tile(_text_size, 2) * [-.5, -1, .5, 0]
-            _text_offset = _text_box_padded[:2] + [text_pad, 0]
-            _anchor = [(_box[0] + _box[2]) / 2, _box[1]]
-            
+        img_anno = Image.new('RGBA', size)
+        
+        size_min = (min(size) + np.linalg.norm(size)) / 2
+        if isinstance(font, str) and os.path.isfile(font):
+            font = ImageFont.truetype(font, int(size_min // 60))
+        else:
+            font = ImageFont.load_default()
+        
+        width = int(max(size_min // 600 if width is None else width, 1))
+        text_pad = int(max(size_min // 400 if text_pad is None else text_pad, 1))
+        
+        draw = ImageDraw.Draw(img_anno)
+        drawing_texts = isinstance(texts, list) and len(texts) == len(boxes)
+        for i, box in enumerate(boxes):
+            _box = np.array(box)
             draw.rectangle(
-                tuple(_text_box_padded + np.tile(_anchor, 2)),
-                fill=color,
+                tuple(_box),
+                outline=color,
+                width=width,
             )
-            draw.text(
-                tuple(_text_offset + _anchor),
-                text=_text,
-                fill=color_text,
-                font=font,
+            
+            if drawing_texts:
+                _size = _box[2:] - _box[:2]
+                # _text = f'{_size[0]}•{_size[1]}'
+                _text = texts[i]
+                _text_box = np.array(font.getbbox(_text))
+                _text_size = _text_box[2:] - _text_box[:2] + [text_pad * 2] * 2
+                _text_box_padded = np.tile(_text_size, 2) * [-.5, -1, .5, 0]
+                _text_offset = _text_box_padded[:2] + [text_pad, 0]
+                _anchor = [(_box[0] + _box[2]) / 2, _box[1]]
+                
+                draw.rectangle(
+                    tuple(_text_box_padded + np.tile(_anchor, 2)),
+                    fill=color,
+                )
+                draw.text(
+                    tuple(_text_offset + _anchor),
+                    text=_text,
+                    fill=color_text,
+                    font=font,
+                )
+        
+        if isinstance(img, Image.Image):
+            if opacity < 1:
+                assert opacity > 0, f'opacity[{opacity}]'
+                img_anno.putalpha(img_anno.getchannel('A').point(lambda x: x * opacity))
+            
+            img_anno = Image.alpha_composite(
+                img.convert('RGBA'),
+                img_anno,
             )
+        return img_anno
+    
     
-    if isinstance(img, Image.Image):
+    @classmethod
+    def draw_anno_text_overlay(cls,
+                img=(10, 10),
+                boxes=[],
+                texts=None,
+                width=None,
+                text_pad=None,
+                color=None,
+                color_text='#000000',
+                bg_saturation=0.8,
+                bg_value=0.8,
+                font=FONT_PATH,
+                opacity=0.65,
+                ):
+        
+        if isinstance(img, (tuple, list)):
+            size = tuple(img)
+        else:
+            img = get_image(img).convert('RGBA')
+            size = img.size
+        
+        img_box = Image.new('RGBA', size)
+        img_text = Image.new('RGBA', size)
+        
+        size_min = (min(size) + np.linalg.norm(size)) / 2
+        
+        is_loading_font_from_file = isinstance(font, str) and os.path.isfile(font)
+        # assert is_loading_font_from_file, f'cwd[{os.getcwd()}] font[{font}] __file__[{__file__}]'
+        _font = None
+        if not is_loading_font_from_file:
+            _font = ImageFont.load_default()
+        
+        if width is True:
+            width = int(max(size_min // 600, 1))
+        assert width is None or isinstance(width, int)
+        text_pad = int(max(size_min // 400 if text_pad is None else text_pad, 1))
+        
+        draw_box = ImageDraw.Draw(img_box)
+        draw_text = ImageDraw.Draw(img_text)
+        drawing_texts = isinstance(texts, list) and len(texts) == len(boxes)
+        
+        for i, box in enumerate(boxes):
+            _box = np.array(box)
+            _box_size = _box[2:] - _box[:2]
+            _box_xy_center = (_box[:2] + _box[2:]) / 2
+            
+            _color = color if color is not None else tuple([int(v * 255) for v in colorsys.hsv_to_rgb(
+                i * max(1 / len(boxes), 1/12),
+                bg_saturation,
+                bg_value,
+            )])
+            
+            draw_box.rectangle(
+                tuple(_box),
+                fill=_color,
+            )
+            if width is not None:
+                draw_box.rectangle(
+                    tuple(_box),
+                    outline=color_text,
+                    width=width,
+                )
+            
+            if drawing_texts:
+                _text = texts[i]
+                _text_size = np.min(_box_size * [2.5 / len(_text), 1.1])
+                
+                if is_loading_font_from_file:
+                    _font_size = int(max(np.floor(_text_size), 8))
+                    _font = ImageFont.truetype(font, size=_font_size)
+                
+                cls.draw_text_center(
+                    draw_text,
+                    _text,
+                    font=_font,
+                    pos=tuple(_box_xy_center),
+                    color_text=color_text,
+                )
+        
+        # TODO: move custom alpha_composite to its own method
         if opacity < 1:
             assert opacity > 0, f'opacity[{opacity}]'
-            img_anno.putalpha(img_anno.getchannel('A').point(lambda x: x * opacity))
+            img_box.putalpha(img_box.getchannel('A').point(lambda x: x * opacity))
         
         img_anno = Image.alpha_composite(
-            img.convert('RGBA'),
-            img_anno,
+            img_box,
+            img_text,
         )
-    return img_anno
-
-# %%
-STRING_CHARS = string.ascii_letters + string.digits
-def draw_text_center(draw, text, font, pos=(0, 0), color_text=(0, 0, 0), color_bg=None):
-    ascent, descent = font.getmetrics()
-    (width, baseline), (offset_x, offset_y) = font.font.getsize(STRING_CHARS)
-    
-    text_heights = [offset_y, ascent - offset_y, descent]
-    text_ys = np.cumsum([0, *text_heights])
-    
-    (text_width, _), (_, _) = font.font.getsize(text)
-    
-    _pos = np.array(pos)
-    
-    text_box = np.array([
-        0, text_ys[1],
-        text_width, text_ys[3],
-    ])
-    text_size = text_box[2:] - text_box[:2]
-    text_offset = - (text_size / 2 + [0, text_ys[1] * 0.6])
-    text_box_ex = text_box + np.repeat([-1, 1], 2) * 3 + np.array([-1, -1/2, 1, 0]) * descent
-    # text_box_ex = text_box + np.repeat([-1, 1], 2) * 3 + np.array([-1, -1, 1, 0]) * descent
-    
-    if color_bg is not None:
-        draw.rectangle(
-            tuple(np.tile(_pos + text_offset, 2) + text_box_ex),
-            fill=color_bg,
-        )
-    draw.text(
-        tuple(_pos + text_offset + [0, 0]),
-        text=text,
-        fill=color_text,
-        font=font,
-    )
-    return draw
-
-# %%
-def draw_anno_text_overlay(
-            img=(10, 10),
-            boxes=[],
-            texts=None,
-            width=None,
-            text_pad=None,
-            color=None,
-            color_text='#000000',
-            bg_saturation=0.8,
-            bg_value=0.8,
-            font=FONT_PATH,
-            opacity=0.65,
-            ):
-    
-    if isinstance(img, (tuple, list)):
-        size = tuple(img)
-    else:
-        size = img.size
-    
-    img_box = Image.new('RGBA', size)
-    img_text = Image.new('RGBA', size)
-    
-    size_min = (min(size) + np.linalg.norm(size)) / 2
-    
-    is_loading_font_from_file = isinstance(font, str) and os.path.isfile(font)
-    assert is_loading_font_from_file, f'cwd[{os.getcwd()}] font[{font}] __file__[{__file__}]'
-    _font = None
-    if not is_loading_font_from_file:
-        _font = ImageFont.load_default()
-    
-    if width is True:
-        width = int(max(size_min // 600, 1))
-    assert width is None or isinstance(width, int)
-    text_pad = int(max(size_min // 400 if text_pad is None else text_pad, 1))
-    
-    draw_box = ImageDraw.Draw(img_box)
-    draw_text = ImageDraw.Draw(img_text)
-    drawing_texts = isinstance(texts, list) and len(texts) == len(boxes)
-    
-    for i, box in enumerate(boxes):
-        _box = np.array(box)
-        _box_size = _box[2:] - _box[:2]
-        _box_xy_center = (_box[:2] + _box[2:]) / 2
-        
-        _color = color if color is not None else tuple([int(v * 255) for v in colorsys.hsv_to_rgb(
-            i * max(1 / len(boxes), 1/12),
-            bg_saturation,
-            bg_value,
-        )])
-        
-        draw_box.rectangle(
-            tuple(_box),
-            fill=_color,
-        )
-        if width is not None:
-            draw_box.rectangle(
-                tuple(_box),
-                outline=color_text,
-                width=width,
-            )
         
-        if drawing_texts:
-            _text = texts[i]
-            _text_size = np.min(_box_size * [2.5 / len(_text), 1.1])
-            
-            if is_loading_font_from_file:
-                _font_size = int(max(np.floor(_text_size), 8))
-                _font = ImageFont.truetype(font, size=_font_size)
-            
-            draw_text_center(
-                draw_text,
-                _text,
-                font=_font,
-                pos=tuple(_box_xy_center),
-                # pos=(_box_xy_center[0], _box_xy_center[1]),
-                color_text=color_text,
-                # color_bg=_color,
+        if isinstance(img, Image.Image):
+            img_anno = Image.alpha_composite(
+                img,
+                img_anno,
             )
+        return img_anno
     
-    # TODO: move custom alpha_composite to its own method
-    if opacity < 1:
-        assert opacity > 0, f'opacity[{opacity}]'
-        img_box.putalpha(img_box.getchannel('A').point(lambda x: x * opacity))
-    
-    img_anno = Image.alpha_composite(
-        img_box,
-        img_text,
-    )
     
-    if isinstance(img, Image.Image):
-        img_anno = Image.alpha_composite(
-            img.convert('RGBA'),
-            img_anno,
-        )
-    return img_anno
-
-
-# %%
-# TODO: put functions into class methods
-class AnnoDraw:
+    STRING_CHARS = string.ascii_letters + string.digits
     @classmethod
-    def draw_anno_box(cls, *args, **kwargs):
-        return draw_anno_box(*args, **kwargs)
-    
-    @classmethod
-    def draw_anno_text_overlay(cls, *args, **kwargs):
-        return draw_anno_text_overlay(*args, **kwargs)
+    def draw_text_center(cls,
+                draw,
+                text,
+                font,
+                pos=(0, 0),
+                color_text=(0, 0, 0),
+                color_bg=None,
+                ):
+        ascent, descent = font.getmetrics()
+        (width, baseline), (offset_x, offset_y) = font.font.getsize(cls.STRING_CHARS)
+        
+        text_heights = [offset_y, ascent - offset_y, descent]
+        text_ys = np.cumsum([0, *text_heights])
+        
+        (text_width, _), (_, _) = font.font.getsize(text)
+        
+        _pos = np.array(pos)
+        
+        text_box = np.array([
+            0, text_ys[1],
+            text_width, text_ys[3],
+        ])
+        text_size = text_box[2:] - text_box[:2]
+        text_offset = - (text_size / 2 + [0, text_ys[1] * 0.6])
+        text_box_ex = text_box + np.repeat([-1, 1], 2) * 3 + np.array([-1, -1/2, 1, 0]) * descent
+        # text_box_ex = text_box + np.repeat([-1, 1], 2) * 3 + np.array([-1, -1, 1, 0]) * descent
+        
+        if color_bg is not None:
+            draw.rectangle(
+                tuple(np.tile(_pos + text_offset, 2) + text_box_ex),
+                fill=color_bg,
+            )
+        draw.text(
+            tuple(_pos + text_offset + [0, 0]),
+            text=text,
+            fill=color_text,
+            font=font,
+        )
+        return draw
     
-    @classmethod
-    def draw_text_center(cls, *args, **kwargs):
-        return draw_text_center(*args, **kwargs)
```

### Comparing `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/color_system.py` & `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/color_system.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/imaging.py` & `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/pixel_mask.py` & `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/pixel_mask.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/timing.py` & `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/timing.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision.egg-info/PKG-INFO` & `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2layout-computer-vision
-Version: 0.1.2
+Version: 0.1.3
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision.egg-info/SOURCES.txt` & `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.2/src/sandbox.py` & `image2layout_computer_vision-0.1.3/src/sandbox.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.2/src/sandbox_color.py` & `image2layout_computer_vision-0.1.3/src/sandbox_color.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.2/src/sandbox_ocr.py` & `image2layout_computer_vision-0.1.3/src/sandbox_ocr.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.2/src/test_color.py` & `image2layout_computer_vision-0.1.3/src/test_color.py`

 * *Files identical despite different names*

