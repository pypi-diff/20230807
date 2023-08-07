# Comparing `tmp/fracsuite-0.1.3.tar.gz` & `tmp/fracsuite-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fracsuite-0.1.3.tar", last modified: Sun Aug  6 21:47:56 2023, max compression
+gzip compressed data, was "fracsuite-0.1.4.tar", last modified: Mon Aug  7 09:44:17 2023, max compression
```

## Comparing `fracsuite-0.1.3.tar` & `fracsuite-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:47:56.339513 fracsuite-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-06 21:47:56.335513 fracsuite-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-06 21:47:46.000000 fracsuite-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:47:56.335513 fracsuite-0.1.3/fracsuite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 21:47:46.000000 fracsuite-0.1.3/fracsuite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-06 21:47:46.000000 fracsuite-0.1.3/fracsuite/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-08-06 21:47:46.000000 fracsuite-0.1.3/fracsuite/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-06 21:47:46.000000 fracsuite-0.1.3/fracsuite/splinter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:47:56.335513 fracsuite-0.1.3/fracsuite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-06 21:47:56.000000 fracsuite-0.1.3/fracsuite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-06 21:47:56.000000 fracsuite-0.1.3/fracsuite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 21:47:56.000000 fracsuite-0.1.3/fracsuite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 21:47:56.000000 fracsuite-0.1.3/fracsuite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-06 21:47:56.000000 fracsuite-0.1.3/fracsuite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-06 21:47:46.000000 fracsuite-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 21:47:56.339513 fracsuite-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:44:17.993365 fracsuite-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-08-07 09:44:17.993365 fracsuite-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-08-07 09:44:05.000000 fracsuite-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:44:17.989365 fracsuite-0.1.4/fracsuite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:44:05.000000 fracsuite-0.1.4/fracsuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-07 09:44:05.000000 fracsuite-0.1.4/fracsuite/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-08-07 09:44:05.000000 fracsuite-0.1.4/fracsuite/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-07 09:44:05.000000 fracsuite-0.1.4/fracsuite/splinter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:44:17.993365 fracsuite-0.1.4/fracsuite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-08-07 09:44:17.000000 fracsuite-0.1.4/fracsuite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-07 09:44:17.000000 fracsuite-0.1.4/fracsuite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:44:17.000000 fracsuite-0.1.4/fracsuite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-07 09:44:17.000000 fracsuite-0.1.4/fracsuite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 09:44:17.000000 fracsuite-0.1.4/fracsuite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-07 09:44:05.000000 fracsuite-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 09:44:17.993365 fracsuite-0.1.4/setup.cfg
```

### Comparing `fracsuite-0.1.3/fracsuite/analyzer.py` & `fracsuite-0.1.4/fracsuite/analyzer.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 def crop_perspective(img, size = 4000, dbg = False):
     """
     Crops a given image to its containing pane bounds. Finds smallest pane countour with
     4 corner points and aligns, rotates and scales the pane to fit a resulting image.
 
     Args:
         img (Image): Input image with a clearly visible glass pane.
-
+        size (int): Size of the resulting image after perspective transformation.
+        dbg (bool): Displays debug image outputs during processing.
+        
     Returns:
         img: A cropped image which only contains the glass pane. Size: 1000x1000.
             If no 4 point contour is found, the whole image is returned.
     """
     
     def fourCornersSort(pts):
         """ Sort corners: top-left, bot-left, bot-right, top-right """
@@ -239,36 +241,67 @@
 def closeImg(image, sz = 3, it=1):
     kernel_closing = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (sz, sz))
     return cv2.morphologyEx(image, cv2.MORPH_CLOSE, kernel_closing, iterations=it)
 
 
 class Analyzer(object):
     """
-    Analyzer class that can handle an input image.        
+    Analyzer class that can handle an input image.
     """
     
     file_path: str
     
     original_image: nptyp.ArrayLike
     preprocessed_image: nptyp.ArrayLike
         
     contours: list[nptyp.ArrayLike]
     splinters: list[Splinter]
     
-    axs: list[plt.axes]
+    axs: list[plt.Axes]
     
-    def __init__(self, file_path: str, crop = False, img_size = 4000):
+    def __init__(self, file_path: str, crop = False, img_size = 4000,\
+        img_real_size=None):
+        """Create a new analyzer object.
+
+        Args:
+            file_path (str): Path to image.
+            crop (bool, optional): Specify, if the input has to be cropped first. 
+                Defaults to False.
+            img_size (int, optional): Size of the cropped image. 
+                Defaults to 4000, only needed if crop=True.
+            img_real_size (tuple[int,int], optional):
+                Actual size in mm of the input rectangular ply.
+        """
+        
         # image operations
         self.original_image = cv2.imread(file_path, cv2.IMREAD_GRAYSCALE)
         if crop:
             self.original_image = crop_perspective(self.original_image, size=img_size, dbg=False)
         
         
         self.preprocessed_image = preprocess_image(self.original_image)
         
+        
+        f = 1
+        # calculate scale factors
+        if img_real_size is not None:
+            # fx: mm/px
+            fx = img_real_size[0] / self.preprocessed_image.shape[1]
+            fy = img_real_size[1] / self.preprocessed_image.shape[0] 
+            
+            # the factors must match because pixels are always squared
+            # for landscape image, the img_real_size's aspect ratio must match
+            if fx != fy:
+                raise Exception("The scale factors for x and y must match!" + \
+                    "Check the input image and also the img_real_size parameter.")
+            
+            # f: mm/px
+            f = fx
+            
+            
         # contour operations
         all_contours = detect_fragments(self.preprocessed_image)
         stencil = np.zeros((self.preprocessed_image.shape[1], \
             self.preprocessed_image.shape[0]), dtype=np.uint8)
         for c in tqdm(all_contours):
             cv2.drawContours(stencil, [c], -1, 255, thickness = -1) 
         
@@ -281,15 +314,15 @@
         # second step is to skeletonize the closed skeleton from #1
         print('Skeletonize 2|2')
         skeleton = skeletonize(skeleton)
         skeleton = skeleton.astype(np.uint8)
         
         # detect fragments on the closed skeleton
         self.contours = detect_fragments(skeleton)        
-        self.splinters = [Splinter(x,i) for i,x in enumerate(self.contours)]
+        self.splinters = [Splinter(x,i,f) for i,x in enumerate(self.contours)]
     
     def __onselect(self,eclick, erelease):
         """ Private function, internal use only. """
         x1, y1 = eclick.xdata, eclick.ydata
         x2, y2 = erelease.xdata, erelease.ydata
         selected_region = (x1, y1, x2, y2)
         
@@ -410,15 +443,15 @@
         
         # ascending sort, smallest to largest
         areas.sort()
             
         data = []
         
         area_i = 0
-        for area in range(100,int(np.max(areas)),200):
+        for area in np.linspace(np.min(areas),np.max(areas),50):
             index = next((i for i, value in enumerate(areas) if value > area), None)
             p = index
             data.append((area, p))
 
         data_x, data_y = zip(*data)
         
         fig = plt.figure()
```

### Comparing `fracsuite-0.1.3/fracsuite/splinter.py` & `fracsuite-0.1.4/fracsuite/splinter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import numpy as np
 import cv2
 
 
 class Splinter:    
-    def __init__(self, contour, index):
+    def __init__(self, contour, index, mm_px: float):
+        """Create a splinter from a contour.
+
+        Args:
+            contour (np.array): Input contour.
+            index (int): Index of the splinter.
+            mm_px (float): Scale factor for area. px/mm.
+        """
         self.ID = index
         self.contour = contour
         
-        self.area = cv2.contourArea(self.contour)
-        self.circumfence = cv2.arcLength(self.contour, True)
+        self.area = cv2.contourArea(self.contour) * mm_px ** 2
+        self.circumfence = cv2.arcLength(self.contour, True) * mm_px
         
         # roundness
         self.roundness = 4 * np.pi * self.area / self.circumfence ** 2
         # roughness
         self.roughness = self.calculate_roughness()
         
         # centroid
         try:
             M = cv2.moments(self.contour)
             cX = int(M["m10"] / M["m00"])
             cY = int(M["m01"] / M["m00"])
             
-            self.centroid =  (cX, cY)
+            self.centroid =  (cX * mm_px, cY * mm_px)
         except:
             self.centroid = (np.nan, np.nan)
             
     def calculate_roughness(self) -> float:
         """Calculate the roughness of the contour by comparing the circumfence
         of the contour to the circumfence of its convex hull.
```

### Comparing `fracsuite-0.1.3/pyproject.toml` & `fracsuite-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = ["matplotlib", "opencv-python", "numpy", "tqdm", "scikit-image"]
 name = "fracsuite"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Leon Bohmann", email="mail@leonbohmann.de" },
 ]
 description = "Package to help analyze fracture patterns on broken glass plys."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

