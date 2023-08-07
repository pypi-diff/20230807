# Comparing `tmp/image2layout_computer_vision-0.1.1.tar.gz` & `tmp/image2layout_computer_vision-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2layout_computer_vision-0.1.1.tar", last modified: Mon Aug  7 06:12:59 2023, max compression
+gzip compressed data, was "image2layout_computer_vision-0.1.2.tar", last modified: Mon Aug  7 07:01:58 2023, max compression
```

## Comparing `image2layout_computer_vision-0.1.1.tar` & `image2layout_computer_vision-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 06:12:59.328899 image2layout_computer_vision-0.1.1/
--rw-rw-r--   0 test      (1001) test      (1001)     1073 2023-07-20 04:03:09.000000 image2layout_computer_vision-0.1.1/LICENSE
--rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 06:12:59.328899 image2layout_computer_vision-0.1.1/PKG-INFO
--rw-rw-r--   0 test      (1001) test      (1001)     2224 2023-08-04 10:07:30.000000 image2layout_computer_vision-0.1.1/README.md
--rw-rw-r--   0 test      (1001) test      (1001)      637 2023-08-07 06:08:55.000000 image2layout_computer_vision-0.1.1/pyproject.toml
--rw-rw-r--   0 test      (1001) test      (1001)       38 2023-08-07 06:12:59.328899 image2layout_computer_vision-0.1.1/setup.cfg
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 06:12:59.324899 image2layout_computer_vision-0.1.1/src/
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 06:12:59.324899 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/
--rw-rw-r--   0 test      (1001) test      (1001)      613 2023-08-04 08:58:07.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/__init__.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 06:12:59.328899 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/color_extract/
--rw-rw-r--   0 test      (1001) test      (1001)       95 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/color_extract/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)    14464 2023-08-03 04:42:22.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/color_extract/main.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 06:12:59.328899 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/
--rw-rw-r--   0 test      (1001) test      (1001)      251 2023-08-04 08:48:54.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)    16279 2023-08-04 08:55:20.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/imagebox.py
--rw-rw-r--   0 test      (1001) test      (1001)     3625 2023-08-04 09:10:20.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/main.py
--rw-rw-r--   0 test      (1001) test      (1001)     6286 2023-07-26 05:47:05.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
--rw-rw-r--   0 test      (1001) test      (1001)     2168 2023-08-07 06:07:52.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/model_paddle.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 06:12:59.328899 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/
--rw-rw-r--   0 test      (1001) test      (1001)      457 2023-08-04 08:57:51.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)     7186 2023-08-04 09:09:14.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/annotation.py
--rw-rw-r--   0 test      (1001) test      (1001)     4896 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/color_system.py
--rw-rw-r--   0 test      (1001) test      (1001)     3820 2023-08-03 10:44:05.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/imaging.py
--rw-rw-r--   0 test      (1001) test      (1001)     2402 2023-08-02 09:28:26.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/pixel_mask.py
--rw-rw-r--   0 test      (1001) test      (1001)     5469 2023-08-03 03:51:23.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/timing.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 06:12:59.324899 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision.egg-info/
--rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 06:12:59.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision.egg-info/PKG-INFO
--rw-rw-r--   0 test      (1001) test      (1001)     1052 2023-08-07 06:12:59.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision.egg-info/SOURCES.txt
--rw-rw-r--   0 test      (1001) test      (1001)        1 2023-08-07 06:12:59.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision.egg-info/dependency_links.txt
--rw-rw-r--   0 test      (1001) test      (1001)       74 2023-08-07 06:12:59.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision.egg-info/top_level.txt
--rw-rw-r--   0 test      (1001) test      (1001)    11005 2023-07-26 06:47:33.000000 image2layout_computer_vision-0.1.1/src/sandbox.py
--rw-rw-r--   0 test      (1001) test      (1001)    11193 2023-08-03 04:03:51.000000 image2layout_computer_vision-0.1.1/src/sandbox_color.py
--rw-rw-r--   0 test      (1001) test      (1001)     1246 2023-08-04 09:11:31.000000 image2layout_computer_vision-0.1.1/src/sandbox_ocr.py
--rw-rw-r--   0 test      (1001) test      (1001)      812 2023-08-03 04:47:50.000000 image2layout_computer_vision-0.1.1/src/test_color.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:01:58.914640 image2layout_computer_vision-0.1.2/
+-rw-rw-r--   0 test      (1001) test      (1001)     1073 2023-07-20 04:03:09.000000 image2layout_computer_vision-0.1.2/LICENSE
+-rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 07:01:58.914640 image2layout_computer_vision-0.1.2/PKG-INFO
+-rw-rw-r--   0 test      (1001) test      (1001)     2224 2023-08-07 06:13:00.000000 image2layout_computer_vision-0.1.2/README.md
+-rw-rw-r--   0 test      (1001) test      (1001)      637 2023-08-07 06:41:56.000000 image2layout_computer_vision-0.1.2/pyproject.toml
+-rw-rw-r--   0 test      (1001) test      (1001)       38 2023-08-07 07:01:58.914640 image2layout_computer_vision-0.1.2/setup.cfg
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:01:58.910640 image2layout_computer_vision-0.1.2/src/
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:01:58.910640 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/
+-rw-rw-r--   0 test      (1001) test      (1001)      613 2023-08-04 08:58:07.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/__init__.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:01:58.910640 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/color_extract/
+-rw-rw-r--   0 test      (1001) test      (1001)       95 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/color_extract/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)    14464 2023-08-03 04:42:22.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/color_extract/main.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:01:58.914640 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/
+-rw-rw-r--   0 test      (1001) test      (1001)      251 2023-08-04 08:48:54.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)    16347 2023-08-07 06:50:31.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/imagebox.py
+-rw-rw-r--   0 test      (1001) test      (1001)     3748 2023-08-07 07:00:33.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/main.py
+-rw-rw-r--   0 test      (1001) test      (1001)     6286 2023-07-26 05:47:05.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
+-rw-rw-r--   0 test      (1001) test      (1001)     2331 2023-08-07 06:43:03.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/model_paddle.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:01:58.914640 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/
+-rw-rw-r--   0 test      (1001) test      (1001)      457 2023-08-04 08:57:51.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)     7186 2023-08-04 09:09:14.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/annotation.py
+-rw-rw-r--   0 test      (1001) test      (1001)     4896 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/color_system.py
+-rw-rw-r--   0 test      (1001) test      (1001)     3820 2023-08-03 10:44:05.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/imaging.py
+-rw-rw-r--   0 test      (1001) test      (1001)     2402 2023-08-02 09:28:26.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/pixel_mask.py
+-rw-rw-r--   0 test      (1001) test      (1001)     5469 2023-08-03 03:51:23.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/timing.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 07:01:58.910640 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision.egg-info/
+-rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 07:01:58.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision.egg-info/PKG-INFO
+-rw-rw-r--   0 test      (1001) test      (1001)     1052 2023-08-07 07:01:58.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision.egg-info/SOURCES.txt
+-rw-rw-r--   0 test      (1001) test      (1001)        1 2023-08-07 07:01:58.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision.egg-info/dependency_links.txt
+-rw-rw-r--   0 test      (1001) test      (1001)       74 2023-08-07 07:01:58.000000 image2layout_computer_vision-0.1.2/src/image2layout_computer_vision.egg-info/top_level.txt
+-rw-rw-r--   0 test      (1001) test      (1001)    11005 2023-07-26 06:47:33.000000 image2layout_computer_vision-0.1.2/src/sandbox.py
+-rw-rw-r--   0 test      (1001) test      (1001)    11193 2023-08-03 04:03:51.000000 image2layout_computer_vision-0.1.2/src/sandbox_color.py
+-rw-rw-r--   0 test      (1001) test      (1001)     1246 2023-08-04 09:11:31.000000 image2layout_computer_vision-0.1.2/src/sandbox_ocr.py
+-rw-rw-r--   0 test      (1001) test      (1001)      812 2023-08-03 04:47:50.000000 image2layout_computer_vision-0.1.2/src/test_color.py
```

### Comparing `image2layout_computer_vision-0.1.1/LICENSE` & `image2layout_computer_vision-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.1/PKG-INFO` & `image2layout_computer_vision-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2layout_computer_vision
-Version: 0.1.1
+Version: 0.1.2
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `image2layout_computer_vision-0.1.1/README.md` & `image2layout_computer_vision-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.1/pyproject.toml` & `image2layout_computer_vision-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "Pillow",
   "numpy",
   "pandas",
 ]
 
 [project]
 name = "image2layout_computer_vision"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Felix Do", email="felix.do.1030@gmail.com" },
 ]
 description = "image processing and stuff"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/__init__.py` & `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/__init__.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/color_extract/main.py` & `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/color_extract/main.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/imagebox.py` & `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/imagebox.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
                 {
                     'index': i,
                     'box': _box,
                     'text': _text,
                 }
                 for i, (_box, _text) in enumerate(zip(self.boxes, self.texts))
             ]
-        return pd.DataFrame(data)
+        return pd.DataFrame(data, columns=['index', 'box', 'text'])
     
     @property
     def df_top(self):
         if self.is_single_instance:
             data = [{
                 'index': 0,
                 'box': self.boxes[0],
@@ -333,15 +333,15 @@
                 {
                     'index': i,
                     'box': child.box_outer,
                     'text': child.text,
                 }
                 for i, child in enumerate(self)
             ]
-        return pd.DataFrame(data)
+        return pd.DataFrame(data, columns=['index', 'box', 'text'])
     
     def draw_anno(self,
                 width=2,
                 mode='box',
                 draw_image=True,
                 draw_level_0=False,
                 img_base=None,
```

### Comparing `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/main.py` & `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -74,27 +74,30 @@
     
     boxes_merged = np.array(imageboxes.boxes_top, int)
     boxes_raw = np.array(imageboxes.boxes, int)
     return boxes_merged, boxes_raw
 
 # %%
 def detect_text_full(image: Union[Image.Image, np.ndarray], **kwargs) -> List[Dict]:
+    '''detect and recognize text in the image and merge them, returning raw and merged data
+    Parameters: (same as detect_text)
+    Returns:
+        data_merged: (list of dicts) merged result texts, boxes and scores
+        data_raw:    (list of dicts) raw result texts, boxes and scores
+    '''
     _image = get_image(image).convert('RGB')
-    result_df = model_dispatch_paddle(image)
-    result_data = result_df.to_dict('records')
+    result_df = model_dispatch_paddle(_image)
+    
     imageboxes_raw = ImageBoxes(
         image=_image,
         boxes=result_df['box'].tolist(),
     )
     imageboxes_raw.set_texts(result_df['text'].tolist())
+    
     imageboxes_merged = imageboxes_raw.to_grouped_imageboxes(**kwargs)
     
     return imageboxes_merged.df_top.to_dict('records'), imageboxes_raw.df_top.to_dict('records')
 
 # %%
 if __name__ == '__main__':
-    imageboxes = detect_text('data/inputs/SCR-20230710-ixfw.jpeg')
-    
-    imageboxes.draw_anno(width=3)
+    data_merged, data_raw = detect_text_full('path/to/the/image.png')
     
-    boxes_merged = np.array(imageboxes.boxes_top, int)
-    boxes_raw = np.array(imageboxes.boxes, int)
```

### Comparing `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/model_layoutmlv2.py` & `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/model_layoutmlv2.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/model_paddle.py` & `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/ocr/model_paddle.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 
 # %%
 class ModelDispatch_Paddle:
     def __init__(self,
                 device='cpu',
                 auto_load=False,
                 log_telemetry=False,
+                lang='en',
                 ):
         assert device in ['cpu', 'cuda']
         self.device = device
+        self.lang = lang
         self.paddle_ocr = None
         self.loaded = False
         self.log_telemetry = bool(log_telemetry)
         self.telemetry = {
             'load_time': None,
             'forward_time': [],
         }
@@ -30,15 +32,15 @@
     
     def __call__(self, *args, **kwargs):
         return self.forward(*args, **kwargs)
     
     def _load(self):
         from paddleocr import PaddleOCR, draw_ocr
         self.paddle_ocr = PaddleOCR(
-            lang='en',
+            lang=self.lang,
             use_gpu=self.device in ['cuda'],
             use_angle_cls=True,
         )
         self.loaded = True
     
     def _unload(self):
         del self.paddle_ocr
@@ -63,19 +65,22 @@
         return _output
     
     def _forward(self, image:Image.Image) -> pd.DataFrame:
         width, height = image.size
         
         result = self.paddle_ocr.ocr(np.array(image.convert('RGB')), cls=True)
         
-        result_df = pd.DataFrame([
-            {
-                'text': d[1][0],
-                'score': d[1][1],
-                'box': [int(v) for v in [*d[0][0], *d[0][2]]],
-            }
-            for res in result
-            for d in res
-        ])
+        result_df = pd.DataFrame(
+            data=[
+                {
+                    'text': d[1][0],
+                    'score': d[1][1],
+                    'box': [int(v) for v in [*d[0][0], *d[0][2]]],
+                }
+                for res in result
+                for d in res
+            ],
+            columns=['text', 'score', 'box'],
+        )
         return result_df
 
 # %%
```

### Comparing `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/annotation.py` & `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/color_system.py` & `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/color_system.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/imaging.py` & `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/pixel_mask.py` & `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/pixel_mask.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/timing.py` & `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision/utils/timing.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision.egg-info/PKG-INFO` & `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2layout-computer-vision
-Version: 0.1.1
+Version: 0.1.2
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision.egg-info/SOURCES.txt` & `image2layout_computer_vision-0.1.2/src/image2layout_computer_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.1/src/sandbox.py` & `image2layout_computer_vision-0.1.2/src/sandbox.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.1/src/sandbox_color.py` & `image2layout_computer_vision-0.1.2/src/sandbox_color.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.1/src/sandbox_ocr.py` & `image2layout_computer_vision-0.1.2/src/sandbox_ocr.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.1/src/test_color.py` & `image2layout_computer_vision-0.1.2/src/test_color.py`

 * *Files identical despite different names*

