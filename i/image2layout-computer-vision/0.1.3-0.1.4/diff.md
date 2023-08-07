# Comparing `tmp/image2layout_computer_vision-0.1.3.tar.gz` & `tmp/image2layout_computer_vision-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2layout_computer_vision-0.1.3.tar", last modified: Mon Aug  7 07:29:37 2023, max compression
+gzip compressed data, was "image2layout_computer_vision-0.1.4.tar", last modified: Mon Aug  7 09:24:05 2023, max compression
```

## Comparing `image2layout_computer_vision-0.1.3.tar` & `image2layout_computer_vision-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/
--rw-rw-r--   0 test      (1001) test      (1001)     1073 2023-07-20 04:03:09.000000 image2layout_computer_vision-0.1.3/LICENSE
--rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/PKG-INFO
--rw-rw-r--   0 test      (1001) test      (1001)     2224 2023-08-07 06:13:00.000000 image2layout_computer_vision-0.1.3/README.md
--rw-rw-r--   0 test      (1001) test      (1001)      637 2023-08-07 07:29:17.000000 image2layout_computer_vision-0.1.3/pyproject.toml
--rw-rw-r--   0 test      (1001) test      (1001)       38 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/setup.cfg
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/src/
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/
--rw-rw-r--   0 test      (1001) test      (1001)      573 2023-08-07 07:13:24.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/__init__.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/color_extract/
--rw-rw-r--   0 test      (1001) test      (1001)       95 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/color_extract/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)    14464 2023-08-03 04:42:22.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/color_extract/main.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/
--rw-rw-r--   0 test      (1001) test      (1001)      211 2023-08-07 07:13:29.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)    16366 2023-08-07 07:23:41.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/imagebox.py
--rw-rw-r--   0 test      (1001) test      (1001)     3080 2023-08-07 07:13:37.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/main.py
--rw-rw-r--   0 test      (1001) test      (1001)     6286 2023-07-26 05:47:05.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
--rw-rw-r--   0 test      (1001) test      (1001)     2291 2023-08-07 07:23:57.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/model_paddle.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/
--rw-rw-r--   0 test      (1001) test      (1001)      333 2023-08-07 07:24:03.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)     7645 2023-08-07 07:20:31.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/annotation.py
--rw-rw-r--   0 test      (1001) test      (1001)     4896 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/color_system.py
--rw-rw-r--   0 test      (1001) test      (1001)     3820 2023-08-03 10:44:05.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/imaging.py
--rw-rw-r--   0 test      (1001) test      (1001)     2402 2023-08-02 09:28:26.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/pixel_mask.py
--rw-rw-r--   0 test      (1001) test      (1001)     5469 2023-08-03 03:51:23.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/timing.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:29:37.705422 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision.egg-info/
--rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 07:29:37.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision.egg-info/PKG-INFO
--rw-rw-r--   0 test      (1001) test      (1001)     1052 2023-08-07 07:29:37.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision.egg-info/SOURCES.txt
--rw-rw-r--   0 test      (1001) test      (1001)        1 2023-08-07 07:29:37.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision.egg-info/dependency_links.txt
--rw-rw-r--   0 test      (1001) test      (1001)       74 2023-08-07 07:29:37.000000 image2layout_computer_vision-0.1.3/src/image2layout_computer_vision.egg-info/top_level.txt
--rw-rw-r--   0 test      (1001) test      (1001)    11005 2023-07-26 06:47:33.000000 image2layout_computer_vision-0.1.3/src/sandbox.py
--rw-rw-r--   0 test      (1001) test      (1001)    11193 2023-08-03 04:03:51.000000 image2layout_computer_vision-0.1.3/src/sandbox_color.py
--rw-rw-r--   0 test      (1001) test      (1001)     1246 2023-08-04 09:11:31.000000 image2layout_computer_vision-0.1.3/src/sandbox_ocr.py
--rw-rw-r--   0 test      (1001) test      (1001)      812 2023-08-03 04:47:50.000000 image2layout_computer_vision-0.1.3/src/test_color.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:24:05.779772 image2layout_computer_vision-0.1.4/
+-rw-rw-r--   0 test      (1001) test      (1001)     1073 2023-07-20 04:03:09.000000 image2layout_computer_vision-0.1.4/LICENSE
+-rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 09:24:05.779772 image2layout_computer_vision-0.1.4/PKG-INFO
+-rw-rw-r--   0 test      (1001) test      (1001)     2224 2023-08-07 06:13:00.000000 image2layout_computer_vision-0.1.4/README.md
+-rw-rw-r--   0 test      (1001) test      (1001)      637 2023-08-07 09:23:41.000000 image2layout_computer_vision-0.1.4/pyproject.toml
+-rw-rw-r--   0 test      (1001) test      (1001)       38 2023-08-07 09:24:05.779772 image2layout_computer_vision-0.1.4/setup.cfg
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:24:05.775772 image2layout_computer_vision-0.1.4/src/
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:24:05.775772 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/
+-rw-rw-r--   0 test      (1001) test      (1001)      573 2023-08-07 09:23:20.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/__init__.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:24:05.775772 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/color_extract/
+-rw-rw-r--   0 test      (1001) test      (1001)       95 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/color_extract/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)    14464 2023-08-03 04:42:22.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/color_extract/main.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:24:05.779772 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/
+-rw-rw-r--   0 test      (1001) test      (1001)      211 2023-08-07 07:13:29.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)    17049 2023-08-07 08:43:47.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/imagebox.py
+-rw-rw-r--   0 test      (1001) test      (1001)     3080 2023-08-07 07:13:37.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/main.py
+-rw-rw-r--   0 test      (1001) test      (1001)     6286 2023-07-26 05:47:05.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
+-rw-rw-r--   0 test      (1001) test      (1001)     2261 2023-08-07 07:31:11.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/model_paddle.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:24:05.779772 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/
+-rw-rw-r--   0 test      (1001) test      (1001)      333 2023-08-07 09:23:10.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)     7703 2023-08-07 09:06:09.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/annotation.py
+-rw-rw-r--   0 test      (1001) test      (1001)     4896 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/color_system.py
+-rw-rw-r--   0 test      (1001) test      (1001)     6603 2023-08-07 09:12:59.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/imaging.py
+-rw-rw-r--   0 test      (1001) test      (1001)     2402 2023-08-02 09:28:26.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/pixel_mask.py
+-rw-rw-r--   0 test      (1001) test      (1001)     5469 2023-08-03 03:51:23.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/timing.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:24:05.775772 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision.egg-info/
+-rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 09:24:05.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision.egg-info/PKG-INFO
+-rw-rw-r--   0 test      (1001) test      (1001)     1052 2023-08-07 09:24:05.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision.egg-info/SOURCES.txt
+-rw-rw-r--   0 test      (1001) test      (1001)        1 2023-08-07 09:24:05.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision.egg-info/dependency_links.txt
+-rw-rw-r--   0 test      (1001) test      (1001)       74 2023-08-07 09:24:05.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision.egg-info/top_level.txt
+-rw-rw-r--   0 test      (1001) test      (1001)    11005 2023-07-26 06:47:33.000000 image2layout_computer_vision-0.1.4/src/sandbox.py
+-rw-rw-r--   0 test      (1001) test      (1001)    11193 2023-08-03 04:03:51.000000 image2layout_computer_vision-0.1.4/src/sandbox_color.py
+-rw-rw-r--   0 test      (1001) test      (1001)     1514 2023-08-07 09:18:57.000000 image2layout_computer_vision-0.1.4/src/sandbox_ocr.py
+-rw-rw-r--   0 test      (1001) test      (1001)      812 2023-08-03 04:47:50.000000 image2layout_computer_vision-0.1.4/src/test_color.py
```

### Comparing `image2layout_computer_vision-0.1.3/LICENSE` & `image2layout_computer_vision-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.3/PKG-INFO` & `image2layout_computer_vision-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2layout_computer_vision
-Version: 0.1.3
+Version: 0.1.4
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `image2layout_computer_vision-0.1.3/README.md` & `image2layout_computer_vision-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.3/pyproject.toml` & `image2layout_computer_vision-0.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "Pillow",
   "numpy",
   "pandas",
 ]
 
 [project]
 name = "image2layout_computer_vision"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Felix Do", email="felix.do.1030@gmail.com" },
 ]
 description = "image processing and stuff"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/__init__.py` & `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/__init__.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/color_extract/main.py` & `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/color_extract/main.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/imagebox.py` & `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/imagebox.py`

 * *Files 7% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             original_indices = sorted_indices[indices]
             group_box = cls.merge_boxes(sorted_boxes[indices])
             data_group.append({
                 'indices': original_indices,
                 'box': group_box,
             })
         
-        df_group = pd.DataFrame(data_group)
+        df_group = pd.DataFrame(data_group, columns=['indices', 'box'])
         df_group
         return df_group
     
     @classmethod
     def box_dist(cls, boxa, boxb):
         dists = np.array([
             boxa[:2] - boxb[2:],
@@ -237,14 +237,16 @@
                     self.box_outer = np.array(child_imageboxes.box_outer, int)
                 else:
                     self.box_outer[:2] = np.min([self.box_outer[:2], child_imageboxes.box_outer[:2]], axis=0)
                     self.box_outer[2:] = np.max([self.box_outer[2:], child_imageboxes.box_outer[2:]], axis=0)
                 
             self.box = np.array(self.box_outer, int)
             super().__init__(imageboxes)
+        
+        self.update_texts()
     
     def _repr(self) -> list:
         if self.is_single_instance:
             return [f'Box[{",".join([str(v) for v in self.box])}],']
         else:
             return [
                 f'Boxes[{len(self)}x](',
@@ -255,39 +257,41 @@
                 ],
                 ')',
             ]
         
     def __repr__(self) -> str:
         return '\n'.join(self._repr())
     
-    def set_texts(self, texts:list, update_from_children=True):
+    def set_texts(self, texts:List[str], update:bool=True):
         assert isinstance(texts, list), f''
-        assert len(texts) > 0
         if self.is_single_instance:
-            _text = str(texts[0])
-            self.text = _text
-            self.texts = [_text]
+            if len(texts) > 0:
+                _text = str(texts[0])
+                self.text = _text
+                self.texts = [_text]
         else:
             box_count = len(self.boxes)
-            assert len(texts) == box_count, 'len of texts does not match len of self.boxes'
+            # assert len(texts) == box_count, 'len of texts does not match len of self.boxes'
             _index_offset = 0
             for child in self:
                 child_box_count = len(child.boxes)
                 _texts = texts[_index_offset: _index_offset+child_box_count]
-                child.set_texts(_texts, update_from_children=False)
+                child.set_texts(_texts, update=False)
                 _index_offset += child_box_count
             
-            if update_from_children:
-                self.update_texts_from_children()
+        if update:
+            self.update_texts()
     
-    def update_texts_from_children(self):
-        if not self.is_single_instance:
+    def update_texts(self):
+        if self.is_single_instance:
+            self.texts = [self.text]
+        else:
             self.texts = []
             for child in self:
-                _texts = child.update_texts_from_children()
+                _texts = child.update_texts()
                 self.texts.extend(_texts)
             self.text = ' '.join(self.texts)
         return self.texts
     
     @property
     def images(self):
         return [child.image for child in self]
@@ -344,14 +348,15 @@
                 mode='box',
                 draw_image=True,
                 draw_level_0=False,
                 img_base=None,
                 draw_size=True,
                 color=None,
                 ):
+        # DEPRECATED
         assert mode in ['box', 'mask', 'all']
         
         overlay_anno_bottom = AnnoDraw.draw_anno_box(
             self.size,
             boxes=self.boxes,
             color='#00FF00',
             color_text='#000000',
@@ -389,69 +394,82 @@
         )
         imageboxes_grouped.set_texts(self.texts)
         return imageboxes_grouped
     
     @classmethod
     def group_boxes(cls,
                 boxes:Union[np.ndarray, list],
+                
+                merge_lines:bool=False,
                 line_dist_max:float=1.0,
                 line_dist_min:float=-0.1,
                 line_iou_min:float=0.4,
+                
+                merge_rows:bool=True,
                 row_hdist_max:float=0.4,
                 row_vdist_max:float=1.8,
                 row_height_ratio_min:float=0.8,
+                
+                merge_containing:bool=True,
                 ) -> list:
         '''processes self.boxes and returns a new ImageBoxes object with grouped boxes
         Parameters:
             boxes
+            merge_lines      (bool) False - whether to merge lines
+            merge_rows       (bool) True - whether to merge rows
+            merge_containing (bool) True - whether to merge overlaping boxes
             line_dist_max:          max distance between boxes to be in the same sentence (as a ratio of line height)
             line_dist_min:          min (negative) distance between boxes to be in the same sentence (as a ratio of line height)
             line_iou_min:           min vertical iou between boxes to be on the same line
             row_hdist_max:          max horizontal offset between rows to aligned as a column (as a ratio of line height)
             row_vdist_max:          max vertical distance between rows to be in the same column (as a ratio of line height)
             row_height_ratio_min:   min ratio between heights of rows to be in the same column
         Returns:
             boxes_nested_final (list): nested boxes
         '''
-        
-        # TODO: implement to keep texts, currently discard all given texts
-        # TODO: implement nested boxes
-        
         _boxes = np.array(boxes)
         assert _boxes.ndim == 2
         assert _boxes.shape[-1] == 4
         
-        df_group_0 = BoxMerge.group_texts_by_match_fn(
-            _boxes,
-            fn=BoxMerge.same_line_match,
-            sort_index=0,
-            dist_max=line_dist_max,
-            dist_min=line_dist_min,
-            iou_min=line_iou_min,
-        )
-        df_group_1 = BoxMerge.group_texts_by_match_fn(
-            np.array(list(df_group_0['box'])),
-            fn=BoxMerge.same_column_match,
-            sort_index=1,
-            hdist_max=row_hdist_max,
-            vdist_max=row_vdist_max,
-            height_ratio_min=row_height_ratio_min,
-        )
-        df_group_2 = BoxMerge.group_texts_by_match_fn(
-            np.array(list(df_group_1['box'])),
-            fn=BoxMerge.box_containing_match,
-        )
-        _boxes_out = np.array(df_group_2['box'].to_list(), int)
+        merged_dfs = []
+        merged_boxes = np.array(_boxes)
         
-        indices_original = cls.get_original_nested_indices([
-            df_group_0,
-            df_group_1,
-            df_group_2,
-        ])
-        indices_original
+        if merge_lines:
+            _df_merged = BoxMerge.group_texts_by_match_fn(
+                merged_boxes,
+                fn=BoxMerge.same_line_match,
+                sort_index=0,
+                dist_max=line_dist_max,
+                dist_min=line_dist_min,
+                iou_min=line_iou_min,
+            )
+            merged_dfs.append(_df_merged)
+            merged_boxes = np.array(_df_merged['box'].tolist())
+        
+        if merge_rows:
+            _df_merged = BoxMerge.group_texts_by_match_fn(
+                merged_boxes,
+                fn=BoxMerge.same_column_match,
+                sort_index=1,
+                hdist_max=row_hdist_max,
+                vdist_max=row_vdist_max,
+                height_ratio_min=row_height_ratio_min,
+            )
+            merged_dfs.append(_df_merged)
+            merged_boxes = np.array(_df_merged['box'].tolist())
+        
+        if merge_containing:
+            _df_merged = BoxMerge.group_texts_by_match_fn(
+                merged_boxes,
+                fn=BoxMerge.box_containing_match,
+            )
+            merged_dfs.append(_df_merged)
+            merged_boxes = np.array(_df_merged['box'].tolist())
+        
+        indices_original = cls.get_original_nested_indices(merged_dfs)
         
         boxes_nested_final = [
             [
                 _boxes[i].tolist()
                 for i in _indices
             ]
             for _indices in indices_original
```

### Comparing `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/main.py` & `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/main.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/model_layoutmlv2.py` & `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/model_layoutmlv2.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/ocr/model_paddle.py` & `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/model_paddle.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import time, os
 import numpy as np
 import pandas as pd
 import string
 import colorsys
 from PIL import Image, ImageDraw, ImageFont
 
-from ..utils import AnnoDraw
-
 # %%
 class ModelDispatch_Paddle:
     def __init__(self,
                 device='cpu',
                 auto_load=False,
                 log_telemetry=False,
                 lang='en',
```

### Comparing `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/annotation.py` & `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os, time, string, json
 import numpy as np
 import pandas as pd
 import colorsys
 from PIL import Image, ImageFont, ImageDraw
 from typing import Union, Any, List, Dict, Tuple
 from .color_system import COLOR
-from .imaging import ImageConvert, get_image
+from .imaging import get_image, ImageConvert, ImageTransform
 
 # %%
 FONT_PATH = os.path.join(os.path.split(__file__)[0], 'OpenSans_Condensed-Medium.ttf')
 
 # %%
 class AnnoDraw:
     
@@ -22,15 +22,15 @@
                 width=None,
                 text_pad=None,
                 color='#00FF00',
                 color_text='#000000',
                 font=FONT_PATH,
                 opacity=1.0,
                 ):
-    
+        
         if isinstance(img, (tuple, list)):
             size = tuple(img)
         else:
             size = img.size
         
         img_anno = Image.new('RGBA', size)
         
@@ -82,27 +82,75 @@
             img_anno = Image.alpha_composite(
                 img.convert('RGBA'),
                 img_anno,
             )
         return img_anno
     
     
+    STRING_CHARS = string.ascii_letters + string.digits
+    @classmethod
+    def draw_text_center(cls,
+                draw,
+                text,
+                font,
+                pos=(0, 0),
+                color_text=(0, 0, 0),
+                color_bg=None,
+                ):
+        
+        try:
+            ascent, descent = font.getmetrics()
+            (width, baseline), (offset_x, offset_y) = font.font.getsize(cls.STRING_CHARS)
+            
+            text_ys = np.cumsum([0, offset_y, ascent - offset_y, descent])
+            
+            (text_width, _), (_, _) = font.font.getsize(text)
+        except Exception as e:
+            text_ys = np.cumsum([0, 3, 5, 3])
+            text_width = font.getbbox(text)[2]
+            descent = 3
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
+    
+
     @classmethod
     def draw_anno_text_overlay(cls,
-                img=(10, 10),
-                boxes=[],
-                texts=None,
-                width=None,
-                text_pad=None,
-                color=None,
-                color_text='#000000',
-                bg_saturation=0.8,
-                bg_value=0.8,
-                font=FONT_PATH,
-                opacity=0.65,
+                img:tuple=(10, 10),
+                boxes:list=[],
+                texts:list=None,
+                width:int=None,
+                text_pad:int=None,
+                color:string=None,
+                color_text:string='#000000',
+                bg_saturation:float=0.8,
+                bg_value:float=0.8,
+                font:str=FONT_PATH,
+                opacity:float=0.65,
                 ):
         
         if isinstance(img, (tuple, list)):
             size = tuple(img)
         else:
             img = get_image(img).convert('RGBA')
             size = img.size
@@ -161,67 +209,18 @@
                     draw_text,
                     _text,
                     font=_font,
                     pos=tuple(_box_xy_center),
                     color_text=color_text,
                 )
         
-        # TODO: move custom alpha_composite to its own method
-        if opacity < 1:
-            assert opacity > 0, f'opacity[{opacity}]'
-            img_box.putalpha(img_box.getchannel('A').point(lambda x: x * opacity))
-        
-        img_anno = Image.alpha_composite(
-            img_box,
-            img_text,
-        )
+        if opacity != 1:
+            img_box = ImageTransform.setalpha(img_box, scale=opacity)
         
         if isinstance(img, Image.Image):
-            img_anno = Image.alpha_composite(
-                img,
-                img_anno,
-            )
-        return img_anno
-    
-    
-    STRING_CHARS = string.ascii_letters + string.digits
-    @classmethod
-    def draw_text_center(cls,
-                draw,
-                text,
-                font,
-                pos=(0, 0),
-                color_text=(0, 0, 0),
-                color_bg=None,
-                ):
-        ascent, descent = font.getmetrics()
-        (width, baseline), (offset_x, offset_y) = font.font.getsize(cls.STRING_CHARS)
-        
-        text_heights = [offset_y, ascent - offset_y, descent]
-        text_ys = np.cumsum([0, *text_heights])
-        
-        (text_width, _), (_, _) = font.font.getsize(text)
-        
-        _pos = np.array(pos)
-        
-        text_box = np.array([
-            0, text_ys[1],
-            text_width, text_ys[3],
-        ])
-        text_size = text_box[2:] - text_box[:2]
-        text_offset = - (text_size / 2 + [0, text_ys[1] * 0.6])
-        text_box_ex = text_box + np.repeat([-1, 1], 2) * 3 + np.array([-1, -1/2, 1, 0]) * descent
-        # text_box_ex = text_box + np.repeat([-1, 1], 2) * 3 + np.array([-1, -1, 1, 0]) * descent
+            img_anno = ImageTransform.composite(img, img_box, img_text)
+        else:
+            img_anno = ImageTransform.composite(img_box, img_text)
         
-        if color_bg is not None:
-            draw.rectangle(
-                tuple(np.tile(_pos + text_offset, 2) + text_box_ex),
-                fill=color_bg,
-            )
-        draw.text(
-            tuple(_pos + text_offset + [0, 0]),
-            text=text,
-            fill=color_text,
-            font=font,
-        )
-        return draw
+        return img_anno
     
+
```

### Comparing `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/color_system.py` & `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/color_system.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/pixel_mask.py` & `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/pixel_mask.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision/utils/timing.py` & `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/timing.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision.egg-info/PKG-INFO` & `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2layout-computer-vision
-Version: 0.1.3
+Version: 0.1.4
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `image2layout_computer_vision-0.1.3/src/image2layout_computer_vision.egg-info/SOURCES.txt` & `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.3/src/sandbox.py` & `image2layout_computer_vision-0.1.4/src/sandbox.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.3/src/sandbox_color.py` & `image2layout_computer_vision-0.1.4/src/sandbox_color.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.3/src/sandbox_ocr.py` & `image2layout_computer_vision-0.1.4/src/sandbox_ocr.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,71 +4,68 @@
 from PIL import Image
 from image2layout_computer_vision import (
     ImageBoxes,
     detect_text,
     detect_text_full,
     model_dispatch,
     AnnoDraw,
+    ImageTransform,
 )
 
 # %%
-img = Image.open('/home/test/code/image2layout_computer_vision/data/inputs/Coterie benefits.png').convert('RGB')
+img_fp = '/home/test/code/image2layout_computer_vision/data/inputs/Coterie benefits.png'
+img_fp = '/home/test/code/image2layout_computer_vision/data/inputs/Screenshot 2023-07-13 at 11.03.48.png'
+img = Image.open(img_fp).convert('RGB')
 img
 
 # %%
-data_merged, data_raw = detect_text_full(img)
+data_merged, data_raw = detect_text_full(
+    img,
+    row_hdist_max=0.15,
+    row_vdist_max=1.8,
+    row_height_ratio_min=0.85,
+)
 data_merged, data_raw
 
-# %%
-AnnoDraw.draw_anno_text_overlay(
+img_anno_merged = AnnoDraw.draw_anno_text_overlay(
     img=img,
     boxes=[v['box'] for v in data_merged],
     texts=[v['text'] for v in data_merged],
     width=2,
     text_pad=None,
     # color='#00FF88',
     color_text='#000000',
+    # font=None,
     # font='data/OpenSans_Condensed-Medium.ttf',
     opacity=0.75,
-).convert('RGB')
+)
 
-# %%
-AnnoDraw.draw_anno_text_overlay(
+img_anno_raw = AnnoDraw.draw_anno_text_overlay(
     img=img,
     boxes=[v['box'] for v in data_raw],
     texts=[v['text'] for v in data_raw],
     width=2,
     text_pad=None,
     # color='#00FF88',
     color_text='#000000',
+    # font='OpenSans_Condensed-Medium.ttf',
     # font='data/OpenSans_Condensed-Medium.ttf',
     opacity=0.75,
-).convert('RGB')
-
-# %%
-
-
+)
 
+img_anno_dual = ImageTransform.concatenate(
+    # [img_anno_merged, img_anno_raw],
+    # [img, img_anno_merged],
+    [img, img_anno_raw, img_anno_merged],
+    columns=1,
+    spacing=10,
+)
 
+img_anno_dual.convert('RGB')
 
 # %%
-df = model_dispatch(img)
-df
 
-# %%
-imageboxes = detect_text(img)
-imageboxes
 
-# %%
-imageboxes.set_texts(df['text'].tolist())
-imageboxes
 
-# %%
-imageboxes.df
 
-# %%
-IB = ImageBoxes(
-    image=img,
-    boxes=imageboxes.boxes_top,
-)
 
 # %%
```

### Comparing `image2layout_computer_vision-0.1.3/src/test_color.py` & `image2layout_computer_vision-0.1.4/src/test_color.py`

 * *Files identical despite different names*

