# Comparing `tmp/ExoScanner-0.2.3.tar.gz` & `tmp/ExoScanner-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ExoScanner-0.2.3.tar", last modified: Thu Mar 30 14:56:17 2023, max compression
+gzip compressed data, was "dist/ExoScanner-0.2.4.tar", last modified: Mon Aug  7 06:11:06 2023, max compression
```

## Comparing `ExoScanner-0.2.3.tar` & `ExoScanner-0.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 josia      (501) staff       (20)        0 2023-03-30 14:56:17.076225 ExoScanner-0.2.3/
-drwxr-xr-x   0 josia      (501) staff       (20)        0 2023-03-30 14:56:17.066765 ExoScanner-0.2.3/ExoScanner/
--rw-r--r--   0 josia      (501) staff       (20)    50764 2023-02-03 18:26:09.000000 ExoScanner-0.2.3/ExoScanner/Exoscanner_logo.png
--rw-r--r--   0 josia      (501) staff       (20)        0 2023-02-03 18:25:40.000000 ExoScanner-0.2.3/ExoScanner/__init__.py
--rw-r--r--   0 josia      (501) staff       (20)      885 2023-03-21 19:14:33.000000 ExoScanner-0.2.3/ExoScanner/__main__.py
--rw-r--r--   0 josia      (501) staff       (20)     3035 2023-03-30 08:09:22.000000 ExoScanner-0.2.3/ExoScanner/analyzeLightCurves.py
--rw-r--r--   0 josia      (501) staff       (20)     1160 2023-03-28 08:23:43.000000 ExoScanner-0.2.3/ExoScanner/astrometryNET.py
--rw-r--r--   0 josia      (501) staff       (20)      614 2023-03-30 08:07:01.000000 ExoScanner-0.2.3/ExoScanner/config.py
--rw-r--r--   0 josia      (501) staff       (20)     3412 2023-03-30 08:10:00.000000 ExoScanner-0.2.3/ExoScanner/generateBrightnessOfAllStarsInAllImages.py
--rw-r--r--   0 josia      (501) staff       (20)     1326 2023-03-30 08:10:18.000000 ExoScanner-0.2.3/ExoScanner/generateCatalogs.py
--rw-r--r--   0 josia      (501) staff       (20)     1022 2023-03-21 13:32:04.000000 ExoScanner-0.2.3/ExoScanner/generateField.py
--rw-r--r--   0 josia      (501) staff       (20)     1808 2023-03-23 15:14:23.000000 ExoScanner-0.2.3/ExoScanner/generateLightCurves.py
--rw-r--r--   0 josia      (501) staff       (20)     2085 2023-03-20 08:49:04.000000 ExoScanner-0.2.3/ExoScanner/getBrightnessOfOneStarInField.py
--rw-r--r--   0 josia      (501) staff       (20)      838 2023-03-28 11:44:05.000000 ExoScanner-0.2.3/ExoScanner/getCoordinates.py
--rw-r--r--   0 josia      (501) staff       (20)      509 2023-02-03 18:26:09.000000 ExoScanner-0.2.3/ExoScanner/getFilelist.py
--rw-r--r--   0 josia      (501) staff       (20)      547 2023-02-03 18:25:40.000000 ExoScanner-0.2.3/ExoScanner/getTimeOfObservation.py
--rw-r--r--   0 josia      (501) staff       (20)     6684 2023-03-27 08:27:37.000000 ExoScanner-0.2.3/ExoScanner/gui.py
--rw-r--r--   0 josia      (501) staff       (20)     6904 2023-03-06 16:49:27.000000 ExoScanner-0.2.3/ExoScanner/mergeCatalogs.py
--rw-r--r--   0 josia      (501) staff       (20)      812 2023-03-23 09:56:35.000000 ExoScanner-0.2.3/ExoScanner/myAlgorithms.py
--rw-r--r--   0 josia      (501) staff       (20)     3408 2023-03-26 14:38:54.000000 ExoScanner-0.2.3/ExoScanner/output.py
--rw-r--r--   0 josia      (501) staff       (20)     1168 2023-02-03 18:26:09.000000 ExoScanner-0.2.3/ExoScanner/readImage.py
--rw-r--r--   0 josia      (501) staff       (20)     3311 2023-03-26 15:14:46.000000 ExoScanner-0.2.3/ExoScanner/run.py
-drwxr-xr-x   0 josia      (501) staff       (20)        0 2023-03-30 14:56:17.075245 ExoScanner-0.2.3/ExoScanner.egg-info/
--rw-r--r--   0 josia      (501) staff       (20)      541 2023-03-30 14:56:16.000000 ExoScanner-0.2.3/ExoScanner.egg-info/PKG-INFO
--rw-r--r--   0 josia      (501) staff       (20)      775 2023-03-30 14:56:16.000000 ExoScanner-0.2.3/ExoScanner.egg-info/SOURCES.txt
--rw-r--r--   0 josia      (501) staff       (20)        1 2023-03-30 14:56:16.000000 ExoScanner-0.2.3/ExoScanner.egg-info/dependency_links.txt
--rw-r--r--   0 josia      (501) staff       (20)       62 2023-03-30 14:56:16.000000 ExoScanner-0.2.3/ExoScanner.egg-info/requires.txt
--rw-r--r--   0 josia      (501) staff       (20)       11 2023-03-30 14:56:16.000000 ExoScanner-0.2.3/ExoScanner.egg-info/top_level.txt
--rw-r--r--   0 josia      (501) staff       (20)       38 2023-03-27 08:27:26.000000 ExoScanner-0.2.3/MANIFEST.in
--rw-r--r--   0 josia      (501) staff       (20)      541 2023-03-30 14:56:17.075840 ExoScanner-0.2.3/PKG-INFO
--rw-r--r--   0 josia      (501) staff       (20)     2975 2023-03-27 09:36:20.000000 ExoScanner-0.2.3/README.md
--rw-r--r--   0 josia      (501) staff       (20)       38 2023-03-30 14:56:17.076361 ExoScanner-0.2.3/setup.cfg
--rw-r--r--   0 josia      (501) staff       (20)      901 2023-03-30 14:43:49.000000 ExoScanner-0.2.3/setup.py
+drwxr-xr-x   0 josia      (501) staff       (20)        0 2023-08-07 06:11:06.671294 ExoScanner-0.2.4/
+drwxr-xr-x   0 josia      (501) staff       (20)        0 2023-08-07 06:11:06.664148 ExoScanner-0.2.4/ExoScanner/
+-rw-r--r--   0 josia      (501) staff       (20)    50764 2023-03-31 11:09:25.000000 ExoScanner-0.2.4/ExoScanner/Exoscanner_logo.png
+-rw-r--r--   0 josia      (501) staff       (20)        0 2023-02-03 18:25:40.000000 ExoScanner-0.2.4/ExoScanner/__init__.py
+-rw-r--r--   0 josia      (501) staff       (20)      885 2023-08-04 16:50:27.000000 ExoScanner-0.2.4/ExoScanner/__main__.py
+-rw-r--r--   0 josia      (501) staff       (20)     3035 2023-03-31 11:09:25.000000 ExoScanner-0.2.4/ExoScanner/analyzeLightCurves.py
+-rw-r--r--   0 josia      (501) staff       (20)      743 2023-08-06 06:46:10.000000 ExoScanner-0.2.4/ExoScanner/config.py
+-rw-r--r--   0 josia      (501) staff       (20)       42 2023-04-24 07:58:22.000000 ExoScanner-0.2.4/ExoScanner/data.py
+-rw-r--r--   0 josia      (501) staff       (20)     3404 2023-04-24 07:58:22.000000 ExoScanner-0.2.4/ExoScanner/generateBrightnessOfAllStarsInAllImages.py
+-rw-r--r--   0 josia      (501) staff       (20)     1326 2023-03-31 11:09:25.000000 ExoScanner-0.2.4/ExoScanner/generateCatalogs.py
+-rw-r--r--   0 josia      (501) staff       (20)     1022 2023-03-31 11:09:25.000000 ExoScanner-0.2.4/ExoScanner/generateField.py
+-rw-r--r--   0 josia      (501) staff       (20)     1808 2023-03-31 11:09:25.000000 ExoScanner-0.2.4/ExoScanner/generateLightCurves.py
+-rw-r--r--   0 josia      (501) staff       (20)     2615 2023-04-24 08:03:34.000000 ExoScanner-0.2.4/ExoScanner/getBrightnessOfOneStarInField.py
+-rw-r--r--   0 josia      (501) staff       (20)      628 2023-04-24 11:35:21.000000 ExoScanner-0.2.4/ExoScanner/getCoordinates.py
+-rw-r--r--   0 josia      (501) staff       (20)      509 2023-03-31 11:09:25.000000 ExoScanner-0.2.4/ExoScanner/getFilelist.py
+-rw-r--r--   0 josia      (501) staff       (20)      547 2023-02-03 18:25:40.000000 ExoScanner-0.2.4/ExoScanner/getTimeOfObservation.py
+-rw-r--r--   0 josia      (501) staff       (20)     8468 2023-08-06 07:49:15.000000 ExoScanner-0.2.4/ExoScanner/gui.py
+-rw-r--r--   0 josia      (501) staff       (20)     6904 2023-03-06 16:49:27.000000 ExoScanner-0.2.4/ExoScanner/mergeCatalogs.py
+-rw-r--r--   0 josia      (501) staff       (20)      812 2023-03-31 11:09:25.000000 ExoScanner-0.2.4/ExoScanner/myAlgorithms.py
+-rw-r--r--   0 josia      (501) staff       (20)     4227 2023-08-06 07:58:04.000000 ExoScanner-0.2.4/ExoScanner/output.py
+-rw-r--r--   0 josia      (501) staff       (20)     1295 2023-04-24 08:11:14.000000 ExoScanner-0.2.4/ExoScanner/readImage.py
+-rw-r--r--   0 josia      (501) staff       (20)     5152 2023-08-06 07:58:28.000000 ExoScanner-0.2.4/ExoScanner/run.py
+drwxr-xr-x   0 josia      (501) staff       (20)        0 2023-08-07 06:11:06.669265 ExoScanner-0.2.4/ExoScanner.egg-info/
+-rw-r--r--   0 josia      (501) staff       (20)      541 2023-08-07 06:11:06.000000 ExoScanner-0.2.4/ExoScanner.egg-info/PKG-INFO
+-rw-r--r--   0 josia      (501) staff       (20)      766 2023-08-07 06:11:06.000000 ExoScanner-0.2.4/ExoScanner.egg-info/SOURCES.txt
+-rw-r--r--   0 josia      (501) staff       (20)        1 2023-08-07 06:11:06.000000 ExoScanner-0.2.4/ExoScanner.egg-info/dependency_links.txt
+-rw-r--r--   0 josia      (501) staff       (20)       73 2023-08-07 06:11:06.000000 ExoScanner-0.2.4/ExoScanner.egg-info/requires.txt
+-rw-r--r--   0 josia      (501) staff       (20)       11 2023-08-07 06:11:06.000000 ExoScanner-0.2.4/ExoScanner.egg-info/top_level.txt
+-rw-r--r--   0 josia      (501) staff       (20)       38 2023-03-31 11:09:25.000000 ExoScanner-0.2.4/MANIFEST.in
+-rw-r--r--   0 josia      (501) staff       (20)      541 2023-08-07 06:11:06.670445 ExoScanner-0.2.4/PKG-INFO
+-rw-r--r--   0 josia      (501) staff       (20)     3127 2023-08-06 07:01:09.000000 ExoScanner-0.2.4/README.md
+-rw-r--r--   0 josia      (501) staff       (20)       38 2023-08-07 06:11:06.671539 ExoScanner-0.2.4/setup.cfg
+-rw-r--r--   0 josia      (501) staff       (20)      937 2023-08-06 06:51:46.000000 ExoScanner-0.2.4/setup.py
```

### Comparing `ExoScanner-0.2.3/ExoScanner/Exoscanner_logo.png` & `ExoScanner-0.2.4/ExoScanner/Exoscanner_logo.png`

 * *Files identical despite different names*

### Comparing `ExoScanner-0.2.3/ExoScanner/__main__.py` & `ExoScanner-0.2.4/ExoScanner/__main__.py`

 * *Files identical despite different names*

### Comparing `ExoScanner-0.2.3/ExoScanner/analyzeLightCurves.py` & `ExoScanner-0.2.4/ExoScanner/analyzeLightCurves.py`

 * *Files identical despite different names*

### Comparing `ExoScanner-0.2.3/ExoScanner/config.py` & `ExoScanner-0.2.4/ExoScanner/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 params = {
     "input_path": "",           # input location
     "output_path": "",          # output location
     "FWHM": 4,                  # Full-Width-Half-Maximum for finding stars. (passed to DAOFIND)
     "starThreshold": 15,        # Threshold for finding stars. (passed to DAOFIND)
     "StarImageRatio": 3,        # Higher -> Remove more stars; Lower -> Remove more images
     "boxSize": 8,               # Box Size for determining brightness of a star
-    "analysisMode": "variable"  # search for variable stars ("variable") or transits ("exoplanet")
+    "analysisMode": "variable", # search for variable stars ("variable") or transits ("exoplanet")
+    "saturated": 1,             # Max value for a pixel. If this is reached, the star is thrown away.
+    "astrometryApiKey": ""
 }
 
 
 def setParams(p):
     global params
     params = p
```

### Comparing `ExoScanner-0.2.3/ExoScanner/generateBrightnessOfAllStarsInAllImages.py` & `ExoScanner-0.2.4/ExoScanner/generateBrightnessOfAllStarsInAllImages.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 import ExoScanner.config
 
 def cleanUpData(brightness):
     brightness = np.array(brightness)
     removeStars = []
     removeImages = []
     for star in range(0, len(brightness[0])):
+        percentageStar = np.count_nonzero(brightness[:, star]==0)/len(brightness)
         for i in range(0, len(brightness)):
             if brightness[i][star] == 0:
-                percentageStar = np.count_nonzero(brightness[:, star]==0)/len(brightness)
                 percentageImage = np.count_nonzero(brightness[i]==0)/len(brightness[0])
                 if percentageStar*ExoScanner.config.params["StarImageRatio"] > percentageImage or i == 0:
                     removeStars.append(star)
                 else:
                     removeImages.append(i)
     
     cleanData = []
```

### Comparing `ExoScanner-0.2.3/ExoScanner/generateCatalogs.py` & `ExoScanner-0.2.4/ExoScanner/generateCatalogs.py`

 * *Files identical despite different names*

### Comparing `ExoScanner-0.2.3/ExoScanner/generateField.py` & `ExoScanner-0.2.4/ExoScanner/generateField.py`

 * *Files identical despite different names*

### Comparing `ExoScanner-0.2.3/ExoScanner/generateLightCurves.py` & `ExoScanner-0.2.4/ExoScanner/generateLightCurves.py`

 * *Files identical despite different names*

### Comparing `ExoScanner-0.2.3/ExoScanner/getBrightnessOfOneStarInField.py` & `ExoScanner-0.2.4/ExoScanner/getBrightnessOfOneStarInField.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # calculates the brightness of one star in one image by taking a field of a few
 # times a few pixels as input.
 
 from math import sqrt
 import numpy as np
 
+import ExoScanner.config 
+
 
 def getMeanAndDeviation(starRegion, debug=False):
     mean = [0, 0]
     sum = 0
     for i in range(0, len(starRegion)):
         for j in range(0, len(starRegion[0])):
             mean[0]+=i*starRegion[i][j]
@@ -40,23 +42,43 @@
 
 def backgroundRemoval(starRegion):
     values = []
     for i in starRegion:
         for j in i:
             values.append(j)
     values.sort()
-    background = values[int(len(values)/4)]
+    numbackground = int(len(values)/4)
+    background = 0
+    for k in range(numbackground):
+        background += values[k]
+    background /= numbackground
+    background2 = values[int(len(values)/4)]
+
+    #print("Background:")
+    #print(background)
+    #print(" Background2:")
+    #print(background2)
     for i in range(len(starRegion)):
         for j in range(len(starRegion[0])):
             starRegion[i][j]-=background
 
     return starRegion
 
+def saturationFinder(starRegion):
+    found = False
+    for i in starRegion:
+        for j in i:
+           found = found or j>=ExoScanner.config.params['saturated']*0.99
+    return found
 
 def getBrightnessOfOneStarInField(starRegion, subdivide=3, debug=False):
+
+    if saturationFinder(starRegion):
+        return 0
+
     starRegion = backgroundRemoval(starRegion)
 
     starRegion = subdivideMatrix(starRegion, subdivide)
 
     # print(background)
 
     mean,s = getMeanAndDeviation(starRegion, debug)
@@ -67,10 +89,9 @@
     for i in range(0, len(starRegion)):
         for j in range(0, len(starRegion[0])):
             if sqrt((i-mean[0])**2 + (j-mean[1])**2).real <= s*2.5:
                 res += starRegion[i][j]
             # elif sqrt((i-mean[0])**2 + (j-mean[1])**2).real <= s*2.5+1.5:
             #     res += (1-((sqrt((i-mean[0])**2 + (j-mean[1])**2) - s)/1.5).real) * starRegion[i][j]
 
-
     return res
```

### Comparing `ExoScanner-0.2.3/ExoScanner/getCoordinates.py` & `ExoScanner-0.2.4/ExoScanner/getCoordinates.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,34 +3,21 @@
 
 from astroquery import log
 log.setLevel('ERROR')
 from astroquery.astrometry_net import AstrometryNet
 
 from astroquery.simbad import Simbad
 
-
 class Queries:
     wcs = None
     def initialize(self, path, api_key):
         AstrometryNet.api_key = api_key
-        self.wcs = WCS(AstrometryNet.solve_from_image(path))
-        
+        self.wcs = WCS(AstrometryNet.solve_from_image(path))        
 
     def getCoordinates(self, x, y):
         sky = self.wcs.pixel_to_world(x, y)
         Simbad.add_votable_fields('v*')
         return sky
         
     def querySimbad(self, x, y):
         res = Simbad.query_region(self.getCoordinates(x,y), radius='0d3m0s')
         return res
-
-
-
-
-f='/Users/josia/workspace/ExoScanner/dataForTesting/20200624_Transit_Wasp52b-Gornergrat/light/Wasp52-b-002Light.fit'
-a='sefgjpowjimxjkqo'
-x = Queries()
-x.initialize(f,a)
-
-
-print(x.querySimbad(1483, 1026))
```

### Comparing `ExoScanner-0.2.3/ExoScanner/getTimeOfObservation.py` & `ExoScanner-0.2.4/ExoScanner/getTimeOfObservation.py`

 * *Files identical despite different names*

### Comparing `ExoScanner-0.2.3/ExoScanner/gui.py` & `ExoScanner-0.2.4/ExoScanner/gui.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 import tkinter.ttk as ttk
-from tkinter import PhotoImage, Menu, Frame, filedialog, END
+from tkinter import PhotoImage, Menu, Frame, filedialog, END, StringVar
 from ttkthemes import ThemedTk as tk
 from PIL import Image, ImageTk
 
 from ExoScanner.run import run
 
 import ExoScanner.myAlgorithms 
 import ExoScanner.config 
 
 import sys
+from ExoScanner.data import brightness,files,catalogs
 
 class Window(Frame):
 
     def __init__(self, master=None):
         Frame.__init__(self, master)
         self.master = master
 
@@ -27,41 +28,55 @@
 
         self.master.config(menu=menu)
 
         file_manage_frm = ttk.Frame(self.master)
 
         # initializing fields
         self.path_to_files_label = ttk.Label(wraplength=500, text="Input files directory:")
-        self.path_to_files = ttk.Entry()
+        svvx = StringVar()
+        svvx.trace("w", lambda name, index, mode, sv=svvx: self.on_detect_change())
+        self.path_to_files = ttk.Entry(textvariable=svvx)
         self.browse_input = ttk.Button(self.master, text="browse", command=self.set_input_file_location)
+        self.path_to_files.insert(0,ExoScanner.config.params["input_path"])
 
         self.path_to_output_label = ttk.Label(wraplength=500, text="Destination:")
         self.path_to_output = ttk.Entry()
         self.browse_output = ttk.Button(self.master, text="browse", command=self.set_output_file_location)
+        self.path_to_output.insert(0,ExoScanner.config.params["output_path"])
 
         self.param_FWHM_label = ttk.Label(wraplength=500, text="FWHM (used for finding stars; default (4) should be ok)")
-        self.param_FWHM = ttk.Entry()
-        self.param_FWHM.insert(0, "4")
+        svv = StringVar()
+        svv.trace("w", lambda name, index, mode, sv=svv: self.on_detect_change())
+        self.param_FWHM = ttk.Entry(textvariable=svv)
+        self.param_FWHM.insert(0, ExoScanner.config.params["FWHM"])
 
         self.param_star_threshold_label = ttk.Label(wraplength=500, text="Star threshold (used for finding stars; default (15) should be ok)")
-        self.param_star_threshold = ttk.Entry()
-        self.param_star_threshold.insert(0, "15")
+        svvv = StringVar()
+        svvv.trace("w", lambda name, index, mode, sv=svvv: self.on_detect_change())
+        self.param_star_threshold = ttk.Entry(textvariable=svvv)
+        self.param_star_threshold.insert(0, ExoScanner.config.params["starThreshold"])
 
         self.param_star_image_ratio_label = ttk.Label(wraplength=500, text="Star to image valuing ratio. (determines to throw away more stars (higher) or to throw away more images (lower); default (3) should be ok)")
         self.param_star_image_ratio = ttk.Entry()
-        self.param_star_image_ratio.insert(0, "3")
+        self.param_star_image_ratio.insert(0, ExoScanner.config.params["StarImageRatio"])
 
         self.param_box_size_brightness_calc_label = ttk.Label(wraplength=500, text="brightness calculation box size (determines the size of the box which is used to determine the brightness of a star; default (8) should be ok)")
-        self.param_box_size_brightness_calc = ttk.Entry()
-        self.param_box_size_brightness_calc.insert(0, "8")
+        sv = StringVar()
+        sv.trace("w", lambda name, index, mode, sv=sv: self.on_box_change())
+        self.param_box_size_brightness_calc = ttk.Entry(textvariable=sv)
+        self.param_box_size_brightness_calc.insert(0, ExoScanner.config.params["boxSize"])
 
         self.mode_label = ttk.Label(wraplength=500, text="Search for variable stars ('variable') or transits ('exoplanet'). Default is 'variable'")
         self.mode = ttk.Combobox(values=["variable", "exoplanet"])
         self.mode.insert(0, "variable")
 
+        self.astrometrynet_api_key_label = ttk.Label(wraplength=500, text="API-Key for nova.astrometry.net, used for platesolving. (optional)")
+        self.astrometrynet_api_key = ttk.Entry()
+        self.astrometrynet_api_key.insert(0, ExoScanner.config.params["astrometryApiKey"])
+
         self.submit = ttk.Button(self.master, text="Submit",
                                  command=lambda: self.on_submit())
 
         # positioning fields
         self.path_to_files_label.grid(column=0, row=0, padx=5)
         self.path_to_files.grid(column=0, row=1, padx=5, ipady=5, ipadx=100)
         self.browse_input.grid(column=1, row=1, padx=5)
@@ -69,20 +84,22 @@
         self.path_to_output.grid(column=0, row=3, padx=5, ipady=5, ipadx=100)
         self.browse_output.grid(column=1, row=3, padx=5)
 
         self.param_FWHM_label.grid(column=0, row=5, padx=5)
         self.param_FWHM.grid(column=0, row=6, padx=5, ipady=5, ipadx=100)
         self.param_star_threshold_label.grid(column=0, row=7, padx=5)
         self.param_star_threshold.grid(column=0, row=8, padx=5, ipady=5, ipadx=100)
-        self.param_star_image_ratio_label.grid(column=0, row=9, padx=5)
-        self.param_star_image_ratio.grid(column=0, row=10, padx=5, ipady=5, ipadx=100)
-        self.param_box_size_brightness_calc_label.grid(column=0, row=11, padx=5)
-        self.param_box_size_brightness_calc.grid(column=0, row=12, padx=5, ipady=5, ipadx=100)
+        self.param_box_size_brightness_calc_label.grid(column=0, row=9, padx=5)
+        self.param_box_size_brightness_calc.grid(column=0, row=10, padx=5, ipady=5, ipadx=100)
+        self.param_star_image_ratio_label.grid(column=0, row=11, padx=5)
+        self.param_star_image_ratio.grid(column=0, row=12, padx=5, ipady=5, ipadx=100)
         self.mode_label.grid(column=0, row=13, padx=5)
         self.mode.grid(column=0, row=14, padx=5, ipady=5, ipadx=100)
+        self.astrometrynet_api_key_label.grid(column=0, row=15, padx=5)
+        self.astrometrynet_api_key.grid(column=0, row=16, padx=5, ipady=5, ipadx=100)
         
 
         self.submit.grid(column=1, row=4, padx=5, pady=25)
 
     def on_open(self):
         file = filedialog.askopenfilename()
         ExoScanner.myAlgorithms.open_file(file)
@@ -93,14 +110,22 @@
         self.path_to_files.insert(0, path)
 
     def set_output_file_location(self):
         path = filedialog.askdirectory()
         self.path_to_output.delete(0, END)
         self.path_to_output.insert(0, path)
 
+    def on_box_change(self):
+        ExoScanner.data.brightness = []
+
+    def on_detect_change(self):
+        ExoScanner.data.brightness = []
+        ExoScanner.data.files = []
+        ExoScanner.data.catalogs = []
+
     def on_submit(self):
         if self.path_to_files.get() is None:
             print("no input path provided, can't start ExoScanner!")
             return
         ExoScanner.config.params["input_path"] = self.path_to_files.get()
         if self.path_to_output.get() is None:
             print("no output path provided, can't start ExoScanner!")
@@ -122,22 +147,27 @@
             print("no box size provided, can't start ExoScanner!")
             return
         ExoScanner.config.params["boxSize"] = int(self.param_box_size_brightness_calc.get())
         if self.mode.get() is None:
             print("no mode provided, can't start ExoScanner")
             return
         ExoScanner.config.params["analysisMode"] = self.mode.get()
+        if self.astrometrynet_api_key.get() is None:
+            print("WARNING: no api-key set.")
+        ExoScanner.config.params["astrometryApiKey"] = self.astrometrynet_api_key.get()
         
         self.submit["state"] = "disabled"
         run()
         self.submit["state"] = "normal"
 
     def exitProgram(self):
         sys.exit()
 
+def on_closing():
+    sys.exit()
 
 def start_gui():
     absolute_path = os.path.dirname(__file__)
     relative_path = "Exoscanner_logo.png"
     relative_path2 = "ExoScanner_logo.png"
     full_path = os.path.join(absolute_path, relative_path)
     full_path2 = os.path.join(absolute_path, relative_path2)
@@ -145,8 +175,9 @@
     master = tk(theme="black", themebg=True)
     master.title("ExoScanner")
     try:
         master.iconphoto(False, PhotoImage(file=full_path))
     except:
         master.iconphoto(False, PhotoImage(file=full_path2))
     app = Window(master)
+    master.protocol("WM_DELETE_WINDOW", on_closing)
     master.mainloop()
```

### Comparing `ExoScanner-0.2.3/ExoScanner/mergeCatalogs.py` & `ExoScanner-0.2.4/ExoScanner/mergeCatalogs.py`

 * *Files identical despite different names*

### Comparing `ExoScanner-0.2.3/ExoScanner/myAlgorithms.py` & `ExoScanner-0.2.4/ExoScanner/myAlgorithms.py`

 * *Files identical despite different names*

### Comparing `ExoScanner-0.2.3/ExoScanner/output.py` & `ExoScanner-0.2.4/ExoScanner/output.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # The function output() generates the output.
 
 import matplotlib.pyplot as plt
 from ExoScanner import myAlgorithms
 import os
-
+from astropy.io import ascii
 
 
 def outputVariable(lightcurves, times, imageNumber, analysis, output_location, count=20):
     count = min(count, len(analysis))
-    analysis = sorted(analysis, key=lambda d: d['score'], reverse=True)
 
     print(count, "canditates will be returned. Default is 20.")
 
     try:
         os.makedirs(output_location)
     except:
         print(f"directory {output_location} already exists, continuing anyway...")
@@ -51,15 +50,14 @@
         plt.savefig(f"{output_location}/candidate-" + str(i) + ".png")
 
         plt.clf()
 
 
 def outputExoplanet(lightcurves, times, imageNumber, analysis, output_location, count=20):
     count = min(count, len(analysis))
-    analysis = sorted(analysis, key=lambda d: d['score'], reverse=True)
 
     print(count, "canditates will be returned. Default is 20.")
 
     try:
         os.makedirs(output_location)
     except:
         print(f"directory {output_location} already exists, continuing anyway...")
@@ -90,7 +88,30 @@
         else:
             plt.xlabel("time (julian date)")
         plt.ylabel("brightness (normalized flux)")
 
         plt.savefig(f"{output_location}/candidate-" + str(i) + ".png")
 
         plt.clf()
+
+
+def outputLightcurveToCSV(analysis, times, lightcurves, output_location, count=20):
+    count = min(count, len(analysis))
+
+    for i in range(count):
+        lc = lightcurves[analysis[i]["index"]]
+        f = open(f"{output_location}/candidate-" + str(i) + ".csv", "w")
+        f.write("JD\tMAG\n")
+        for j in range(len(lc)):
+            f.write(str(times[j]) + "\t" + str(lc[j]) + "\n")
+        f.close()
+
+
+def makeQueries(analysis, queryEngine, output_location, count=20):
+    count = min(count, len(analysis))
+    for i in range(count):
+        ascii.write(queryEngine.querySimbad(*analysis[i]["coordinates"]), f"{output_location}/candidate-" + str(i) + "-simbad.csv", format="csv", overwrite=True)
+
+        f = open(f"{output_location}/candidate-" + str(i) + "-coordinates.md", "w")
+        f.write("# Candidate #" + str(i) + ":\n" + str(queryEngine.getCoordinates(*analysis[i]["coordinates"])))
+        f.close()
+
```

### Comparing `ExoScanner-0.2.3/ExoScanner/readImage.py` & `ExoScanner-0.2.4/ExoScanner/readImage.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # The function bin() allows for the data to be binned. That is useful when the
 # image is bayered (color-cameras).
 
 import os
 from astropy.io import fits
 import numpy as np
 
+import ExoScanner.config
+
 def rebin(arr, new_shape):
     """Rebin 2D array arr to shape new_shape by averaging."""
     shape = (new_shape[0], arr.shape[0] // new_shape[0],
              new_shape[1], arr.shape[1] // new_shape[1])
     return arr.reshape(shape).mean(-1).mean(1)
 
 def bin(rgb, size):
@@ -25,8 +27,9 @@
             rgb = list(hdu[0].data)
             # rgb.reverse() <- Use this when you want the coordinates to be in GIMP-format.
 
     else:
         raise ValueError("your file has a not supported type!")
 
     if binning != 1: rgb = bin(rgb, binning)
+    ExoScanner.config.params["saturated"] = max(ExoScanner.config.params["saturated"], np.amax(rgb))
     return rgb
```

### Comparing `ExoScanner-0.2.3/ExoScanner/run.py` & `ExoScanner-0.2.4/ExoScanner/run.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,66 @@
 # The function run() calls all the functions needed in the correct order and
 # combines their returned results.
 
+import sys
+import os
+import warnings
+
 from ExoScanner.getFilelist import getFilelist
 from ExoScanner.generateBrightnessOfAllStarsInAllImages import generateBrightnessOfAllStarsInAllImages
 from ExoScanner.generateBrightnessOfAllStarsInAllImages import cleanUpData
 from ExoScanner.generateCatalogs import generateCatalogs
 from ExoScanner.mergeCatalogs import mergeCatalogs
 from ExoScanner.analyzeLightCurves import analyzeLightCurves
 from ExoScanner.getTimeOfObservation import getTimeOfObservation
 from ExoScanner.generateLightCurves import generateLightCurves
 from ExoScanner.output import outputExoplanet
+from ExoScanner.output import outputLightcurveToCSV
 from ExoScanner.output import outputVariable
-
+from ExoScanner.output import makeQueries
+from ExoScanner import getCoordinates
 
 import ExoScanner.config
 
 from astropy.time import Time
 
 import ExoScanner.myAlgorithms
-
+from ExoScanner.data import brightness,files,catalogs
 
 def run():
     pathToLights = ExoScanner.config.params["input_path"]
     output_location = ExoScanner.config.params["output_path"]
     
-    print("finding files...")
-    files = getFilelist(pathToLights)   # get all files
-    print("found", len(files), "files")
-
+    if len(ExoScanner.data.files) == 0:
+        print("finding files...")
+        files = getFilelist(pathToLights)   # get all files
+        ExoScanner.data.files = files
+        print("found", len(files), "files")
+    else:
+        files = ExoScanner.data.files
     if (len(files)<25):
         print("ERROR: At least 25 files are required.")
         exit(0)
 
-    print("finding stars in all images")
-    catalogs, files = generateCatalogs(files)   # get catalogs and ignore files with less than 20 stars
+    if len(ExoScanner.data.catalogs) == 0:
+        print("finding stars in all images")
+        catalogs, files = generateCatalogs(files)   # get catalogs and ignore files with less than 20 stars
+        ExoScanner.data.catalogs = catalogs
+        ExoScanner.data.files = files
+    else:
+        catalogs = ExoScanner.data.catalogs
+        files = ExoScanner.data.files
+    if len(ExoScanner.data.brightness) == 0:
+        print("calculate brightness of stars")
+        brightness = generateBrightnessOfAllStarsInAllImages(files, catalogs, mergeCatalogs(catalogs))  # get brightness
+        ExoScanner.data.brightness = brightness
+    else:
+        brightness = ExoScanner.data.brightness
 
-    print("calculate brightness of stars")
-    brightness = generateBrightnessOfAllStarsInAllImages(files, catalogs, mergeCatalogs(catalogs))  # get brightness
+    print("cleanup data")
     brightness, axis, stars = cleanUpData(brightness)   # remove bad images and bad stars
 
     print(len(axis), "files are usable. The others will be ignored.")
     print(len(stars), "stars are usable. The others will be ignored.")
 
     if (len(axis)<25):
         print("ERROR: At least 25 files are required. Only", len(axis), "usable files were provided.")
@@ -68,18 +88,47 @@
         times = axis
         imageNumber = 1
 
     for i in range(len(analysis)):  # add index and coordinates in the first image to the analysis of each star
         analysis[i]["index"] = i
         analysis[i]["coordinates"] = (round(catalogs[0]["xcentroid"][stars[i]]),round(catalogs[0]["ycentroid"][stars[i]]))
 
+    analysis = sorted(analysis, key=lambda d: d['score'], reverse=True)
+
     print("writing output files")
 
     if (ExoScanner.config.params["analysisMode"] == "variable"):
         outputVariable(lightCurves, times, imageNumber, analysis, output_location)
     elif (ExoScanner.config.params["analysisMode"] == "exoplanet"):
         outputExoplanet(lightCurves, times, imageNumber, analysis, output_location)
     else:
         outputVariable(lightCurves, times, imageNumber, analysis, output_location)
 
+    print("writing datapoints to CSV")
+    outputLightcurveToCSV(analysis, times, lightCurves, output_location)
+
+    queryEngine = getCoordinates.Queries()
+    try:
+        if (ExoScanner.config.params["astrometryApiKey"]==""): raise Exception
+        print("trying to connect to astrometry.net")
+        f = open(os.devnull, 'w')
+        sys.stdout = f
+        queryEngine.initialize(files[0], ExoScanner.config.params["astrometryApiKey"])
+        f.close()
+        sys.stdout = sys.__stdout__
+        print("success.")
+        print("querying simbad")
+        f = open(os.devnull, 'w')
+        sys.stdout = f
+        warnings.filterwarnings("ignore")
+        makeQueries(analysis, queryEngine, output_location)
+        warnings.filterwarnings("default")
+        f.close()
+        sys.stdout = sys.__stdout__
+    except:
+        sys.stdout = sys.__stdout__
+        print("WARNING: querying astrometry.net failed. (is the API-key set?) sky-coordinates and simbad results will not be available.")
+
+
+
     ExoScanner.myAlgorithms.open_file(output_location)
     print("done")
```

### Comparing `ExoScanner-0.2.3/ExoScanner.egg-info/PKG-INFO` & `ExoScanner-0.2.4/ExoScanner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ExoScanner
-Version: 0.2.3
+Version: 0.2.4
 Summary: A program to analyze an image-series for exoplanet transits.
 Home-page: https://github.com/josia-john/ExoScanner
 Author: Josia John
 Author-email: me@jlabs.anonaddy.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ExoScanner-0.2.3/ExoScanner.egg-info/SOURCES.txt` & `ExoScanner-0.2.4/ExoScanner.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 MANIFEST.in
 README.md
 setup.py
 ExoScanner/Exoscanner_logo.png
 ExoScanner/__init__.py
 ExoScanner/__main__.py
 ExoScanner/analyzeLightCurves.py
-ExoScanner/astrometryNET.py
 ExoScanner/config.py
+ExoScanner/data.py
 ExoScanner/generateBrightnessOfAllStarsInAllImages.py
 ExoScanner/generateCatalogs.py
 ExoScanner/generateField.py
 ExoScanner/generateLightCurves.py
 ExoScanner/getBrightnessOfOneStarInField.py
 ExoScanner/getCoordinates.py
 ExoScanner/getFilelist.py
```

### Comparing `ExoScanner-0.2.3/PKG-INFO` & `ExoScanner-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ExoScanner
-Version: 0.2.3
+Version: 0.2.4
 Summary: A program to analyze an image-series for exoplanet transits.
 Home-page: https://github.com/josia-john/ExoScanner
 Author: Josia John
 Author-email: me@jlabs.anonaddy.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ExoScanner-0.2.3/README.md` & `ExoScanner-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,18 +50,25 @@
 On mac, you can install ExoScanner as a python-package. Then you can run the following command to
 run ExoScanner with a GUI:
 
 ```
 python -m ExoScanner
 ```
 
-## How to compile with pyinstaller?
+## How to compile with pyinstaller? (this is for me, so that I don't forget)
 The program can be "compiled" into a .exe file using pyinstaller: Be sure to replace "\<path>\" with the location to the cli.py file
 ```
 pyinstaller --noconfirm --onefile --console --name "ExoScanner" --hidden-import "photutils.geometry.core" --collect-data "photutils" --hidden-import "ttkthemes" --icon "<path>/images/Exoscanner_logo.ico" --add-data "<path>/ExoScanner/Exoscanner_logo.png;Exoscanner" "<path>/cli.py"
 ```
 
+## Upload to PyPi (this is for me, so that I don't forget)
+
+```
+python setup.py sdist
+twine upload dist/*
+```
+
 ## FAQ
 If you have any questions, feel free to contact me! I can be reached at [me@jlabs.anonaddy.com](mailto:me@jlabs.anonaddy.com)
 
 If you already want a copy of my paper, please also contact me. The final version
 will be uploaded here on January 9th though.
```

### Comparing `ExoScanner-0.2.3/setup.py` & `ExoScanner-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup
 
 setup(
     name='ExoScanner',
-    version='0.2.3',    
+    version='0.2.4',    
     description='A program to analyze an image-series for exoplanet transits.',
     url='https://github.com/josia-john/ExoScanner',
     author='Josia John',
     author_email='me@jlabs.anonaddy.com',
     packages=['ExoScanner'],
     install_requires=['matplotlib',
                       'numpy',                    
                       'astropy',
+                      'astroquery',
                       'statistics',
                       'photutils',
                       'scipy',
                       'ttkthemes'
                       ],
 
     classifiers=[
```

