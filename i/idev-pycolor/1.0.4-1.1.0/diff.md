# Comparing `tmp/idev-pycolor-1.0.4.tar.gz` & `tmp/idev-pycolor-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idev-pycolor-1.0.4.tar", last modified: Wed Aug  2 05:09:07 2023, max compression
+gzip compressed data, was "idev-pycolor-1.1.0.tar", last modified: Mon Aug  7 08:11:45 2023, max compression
```

## Comparing `idev-pycolor-1.0.4.tar` & `idev-pycolor-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 05:09:07.288792 idev-pycolor-1.0.4/
--rw-rw-rw-   0        0        0     1083 2023-07-28 03:09:18.000000 idev-pycolor-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     8387 2023-08-02 05:09:07.288792 idev-pycolor-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     7641 2023-08-02 05:07:36.000000 idev-pycolor-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 05:09:07.228198 idev-pycolor-1.0.4/idev-pycolor/
-drwxrwxrwx   0        0        0        0 2023-08-02 05:09:07.267770 idev-pycolor-1.0.4/idev-pycolor/PyColor/
--rw-rw-rw-   0        0        0    37388 2023-07-31 07:03:11.000000 idev-pycolor-1.0.4/idev-pycolor/PyColor/Colors.py
--rw-rw-rw-   0        0        0     1587 2023-07-31 07:00:42.000000 idev-pycolor-1.0.4/idev-pycolor/PyColor/Functions.py
--rw-rw-rw-   0        0        0     4292 2023-07-31 06:47:09.000000 idev-pycolor-1.0.4/idev-pycolor/PyColor/Palettes.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:09:18.000000 idev-pycolor-1.0.4/idev-pycolor/PyColor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 05:09:07.287755 idev-pycolor-1.0.4/idev-pycolor/idev_pycolor.egg-info/
--rw-rw-rw-   0        0        0     8387 2023-08-02 05:09:07.000000 idev-pycolor-1.0.4/idev-pycolor/idev_pycolor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-08-02 05:09:07.000000 idev-pycolor-1.0.4/idev-pycolor/idev_pycolor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 05:09:07.000000 idev-pycolor-1.0.4/idev-pycolor/idev_pycolor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 05:09:07.000000 idev-pycolor-1.0.4/idev-pycolor/idev_pycolor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      740 2023-08-02 05:07:44.000000 idev-pycolor-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      893 2023-08-02 05:09:07.290755 idev-pycolor-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      985 2023-08-02 05:08:07.000000 idev-pycolor-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:11:45.147010 idev-pycolor-1.1.0/
+-rw-rw-rw-   0        0        0     1083 2023-07-28 03:09:18.000000 idev-pycolor-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     8346 2023-08-07 08:11:45.147010 idev-pycolor-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7641 2023-08-02 05:07:36.000000 idev-pycolor-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 08:11:45.084523 idev-pycolor-1.1.0/idev-pycolor/
+drwxrwxrwx   0        0        0        0 2023-08-07 08:11:45.131348 idev-pycolor-1.1.0/idev-pycolor/PyColor/
+-rw-rw-rw-   0        0        0    40313 2023-08-05 01:49:48.000000 idev-pycolor-1.1.0/idev-pycolor/PyColor/Colors.py
+-rw-rw-rw-   0        0        0     1587 2023-07-31 07:00:42.000000 idev-pycolor-1.1.0/idev-pycolor/PyColor/Functions.py
+-rw-rw-rw-   0        0        0     4292 2023-07-31 06:47:09.000000 idev-pycolor-1.1.0/idev-pycolor/PyColor/Palettes.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:09:18.000000 idev-pycolor-1.1.0/idev-pycolor/PyColor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:11:45.147010 idev-pycolor-1.1.0/idev-pycolor/idev_pycolor.egg-info/
+-rw-rw-rw-   0        0        0     8346 2023-08-07 08:11:45.000000 idev-pycolor-1.1.0/idev-pycolor/idev_pycolor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-08-07 08:11:45.000000 idev-pycolor-1.1.0/idev-pycolor/idev_pycolor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 08:11:45.000000 idev-pycolor-1.1.0/idev-pycolor/idev_pycolor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-07 08:11:45.000000 idev-pycolor-1.1.0/idev-pycolor/idev_pycolor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      699 2023-08-07 08:10:25.000000 idev-pycolor-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      852 2023-08-07 08:11:45.162635 idev-pycolor-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      944 2023-08-07 08:10:47.000000 idev-pycolor-1.1.0/setup.py
```

### Comparing `idev-pycolor-1.0.4/LICENSE` & `idev-pycolor-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idev-pycolor-1.0.4/PKG-INFO` & `idev-pycolor-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: idev-pycolor
-Version: 1.0.4
-Summary: A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.
+Version: 1.1.0
+Summary: A python collection of classes and functions to convert between multiple color models, generate palettes, and more.
 Home-page: https://github.com/IrtsaDevelopment/PyColor
 Author: IrtsaDevelopment
 Author-email: Irtsa <irtsa.development@gmail.com>
 Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyColor
 Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyColor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `idev-pycolor-1.0.4/README.md` & `idev-pycolor-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `idev-pycolor-1.0.4/idev-pycolor/PyColor/Colors.py` & `idev-pycolor-1.1.0/idev-pycolor/PyColor/Colors.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,40 +16,46 @@
 #Classes
 class RGB:
     """
     RGB color class object. 
     Takes in a red, green, and blue value between 0-255
 
     Attributes:
-        red (int): An integer value between 0-255.
-        green (int): An integer value between 0-255.
-        blue (int): An integer value between 0-255.
+        red (int): An integer value between 0-255 or float value between 0-1.
+        green (int): An integer value between 0-255 or float value between 0-1.
+        blue (int): An integer value between 0-255 or float value between 0-1.
 
     Valid Examples:
      - RGB(100, 100, 100)
      - RGB(30, 30, 30)
      - RGB(50, 34, 200)
 
     Invalid Examples:
      - RGB(234, 300, 100)
      - RGB(249, 29, 290)
      - RGB(365, 265, 100)
     """
     
     @staticmethod
     def __checkIfValid(value):
-        if any([True for i in value if type(i) != int]): return False
+        if any([True for i in value if type(i) not in [int, float]]): return False
+        value = [int(i * 255) if type(i) == float else int(i) for i in value]
         if len([i for i in value if i >= 0 and i <= 256]) != 3: return False
 
         return True
 
 
 
-    def __init__(self, red: int, green: int, blue: int):
+    def __init__(self, red: int | float, green: int | float, blue: int | float, notPercent: bool = False):
         if self.__checkIfValid((red, green, blue)):
+            if not notPercent:
+                if type(red) == float: red = int(red * 255)
+                if type(green) == float: green = int(green * 255)
+                if type(blue) == float: blue = int(blue * 255)
+
             self.red = red
             self.green = green
             self.blue = blue
             self.__valid = True
         
         else: self.__valid = False
     
@@ -392,17 +398,17 @@
 
 class HSV:
     """
     HSV color class object. 
     Takes in hue, saturation, and value values.
 
     Attributes:
-        hue (int): An integer value between 0-360.
-        saturation (int): An integer value between 0-100.
-        value (int): An integer value between 0-100.
+        hue (int | float): An integer value between 0-360 or float value between 0-1.
+        saturation (int | float): An integer value between 0-100 or float value between 0-1.
+        value (int | float): An integer value between 0-100 or float value between 0-1.
 
         
     Valid Examples:
      - HSV(342, 100, 100)
      - HSV(100, 30, 80)
      - HSV(50, 30, 100)
 
@@ -410,26 +416,36 @@
      - HSV(2, 101, 50)
      - HSV(-3, 29, 290)
      - HSV(365, 123, 100)
     """
     
     @staticmethod
     def __checkIfValid(value):
-        if any([True for i in value if type(i) != int]): return False
+        if any([True for i in value if type(i) not in [int, float]]): return False
+        value = list(value)
+
+        if type(value[0]) == float: value[0] *= 360
+        if type(value[1]) == float: value[1] *= 100
+        if type(value[2]) == float: value[2] *= 100
 
         if value[0] < 0 or value[0] > 360: return False
         if value[1] < 0 or value[1] > 100: return False
         if value[2] < 0 or value[2] > 100: return False
 
         return True
 
 
 
-    def __init__(self, hue: int, saturation: int, value: int):
+    def __init__(self, hue: int | float, saturation: int | float, value: int | float, notPercent: bool = False):
         if self.__checkIfValid((hue, saturation, value)):
+            if not notPercent:
+                if type(hue) == float: hue = int(hue * 360)
+                if type(saturation) == float: saturation = int(saturation * 100)
+                if type(value) == float: value = int(value * 100)
+
             self.hue = hue
             self.saturation = saturation
             self.value = value
             self.__valid = True
         
         else: self.__valid = False
     
@@ -576,17 +592,17 @@
 
 class HSL:
     """
     HSL color class object. 
     Takes in hue, saturation, and lightness values.
 
     Attributes:
-        hue (int): An integer value between 0-360.
-        saturation (int): An integer value between 0-100.
-        lightness (int): An integer value between 0-100.
+        hue (int | float): An integer value between 0-360 or float value between 0-1.
+        saturation (int | float): An integer value between 0-100 or float value between 0-1.
+        lightness (int | float): An integer value between 0-100 or float value between 0-1.
 
         
     Valid Examples:
      - HSL(342, 100, 100)
      - HSL(100, 30, 80)
      - HSL(50, 30, 100)
 
@@ -594,26 +610,36 @@
      - HSL(2, 101, 50)
      - HSL(-3, 29, 290)
      - HSL(365, 123, 100)
     """
 
     @staticmethod
     def __checkIfValid(value):
-        if any([True for i in value if type(i) != int]): return False
+        if any([True for i in value if type(i) not in [int, float]]): return False
+        value = list(value)
+
+        if type(value[0]) == float: value[0] *= 360
+        if type(value[1]) == float: value[1] *= 100
+        if type(value[2]) == float: value[2] *= 100
 
         if value[0] < 0 or value[0] > 360: return False
         if value[1] < 0 or value[1] > 100: return False
         if value[2] < 0 or value[2] > 100: return False
 
         return True
 
 
 
-    def __init__(self, hue: int, saturation: int, lightness: int):
+    def __init__(self, hue: int | float, saturation: int | float, lightness: int | float, notPercent: bool = False):
         if self.__checkIfValid((hue, saturation, lightness)):
+            if not notPercent:
+                if type(hue) == float: hue = int(hue * 360)
+                if type(saturation) == float: saturation = int(saturation * 100)
+                if type(lightness) == float: lightness = int(lightness * 100)
+
             self.hue = hue
             self.saturation = saturation
             self.lightness = lightness
             self.__valid = True
         
         else: self.__valid = False
     
@@ -759,17 +785,17 @@
 
 class XYZ:
     """
     XYZ color class object. 
     Takes in cyan, magenta, yellow, and key values.
 
     Attributes:
-        x (float): A float value between 0-95.05.
-        y (float): A float value between 0-100.0.
-        z (float): A float value between 0-108.9.
+        x (float): A float value between 0-95.05 or 0-1.
+        y (float): A float value between 0-100.0 or 0-1.
+        z (float): A float value between 0-108.9 or 0-1.
 
         
     Valid Examples:
      - XYZ(84.0, 100.0, 102.0)
      - XYZ(1.0, 30.0, 106.5)
      - XYZ(53.7, 23.4, 100.0)
 
@@ -784,24 +810,31 @@
     def __checkIfValid(value):
         try: value = [float(i) for i in value if type(i) in [int, float]]
         except: return False
 
         if len(value) != 3: return False
         if any([True for i in value if i < 0]): return False
         if value[0] > 95.05 or value[1] > 100 or value[2] > 108.9: return False
-        
+
         return True
 
 
         
-    def __init__(self, x: float, y: float, z: float):
+    def __init__(self, x: float, y: float, z: float, notPercent: bool = False):
         if self.__checkIfValid((x, y, z)):
-            self.x = float(x)
-            self.y = float(y)
-            self.z = float(z)
+            if all([True if i >= 0 and i <= 1 else False for i in (x, y, z)]) and not notPercent:
+                self.x = round((x * 95.05), 2)
+                self.y = round((y * 100.0), 2)
+                self.z = round((z * 108.9), 2)
+            
+            else:
+                self.x = round(x, 2)
+                self.y = round(y, 2)
+                self.z = round(z, 2)
+            
             self.__valid = True
         
         else: self.__valid = False         
 
 
     @property
     def rgb(self) -> tuple:
@@ -951,17 +984,17 @@
 
 class YCC:
     """
     CMYK color class object. 
     Takes in cyan, magenta, yellow, and key values.
 
     Attributes:
-        y (float): An float value between 0-255
-        cb (float): An float value between 0-255
-        cr (float): An float value between 0-255
+        y (float): An float value between 0-255 or 0-1.
+        cb (float): An float value between 0-255 or 0-1.
+        cr (float): An float value between 0-255 or 0-1.
         
   
     Valid Examples:
      - YCC(50.5, 32.24, 23)
      - YCC(12.34, 34.6. 10)
      - YCC(51.2, 30, 200.34)
 
@@ -970,22 +1003,28 @@
      - YCC(234.34, -34.6. 10)
      - YCC(451.2, 30, 200.34)
     """
 
     @staticmethod
     def __checkIfValid(value):
         if any([True for i in value if type(i) not in [int, float]]): return False
+        value = [int(i * 255) if type(i) == float else i for i in value]
         if len([i for i in value if i >= 0 and i <= 256]) != 3: return False
         
         return True
     
 
 
-    def __init__(self, y: float, cb: float, cr: float):
+    def __init__(self, y: float, cb: float, cr: float, notPercent: bool = False):
         if self.__checkIfValid((y, cb, cr)):
+            if not notPercent:
+                if type(y) == float: y = int(y * 255)
+                if type(cb) == float: cb = int(cb * 255)
+                if type(cr) == float: cr = int(cr * 255)
+
             self.y = float(y)
             self.cb = float(cb)
             self.cr = float(cr)
             self.__valid = True
         
         else: self.__valid = False
 
@@ -1153,18 +1192,18 @@
 
 class CMYK:
     """
     CMYK color class object. 
     Takes in cyan, magenta, yellow, and key values.
 
     Attributes:
-        cyan (int): An integer value between 0-100.
-        magenta (int): An integer value between 0-100.
-        yellow (int): An integer value between 0-100.
-        key (int): An integer value between 0-100.
+        cyan (int | float): An integer value between 0-100 or float value between 0-1.
+        magenta (int | float): An integer value between 0-100 or float value between 0-1.
+        yellow (int | float): An integer value between 0-100 or float value between 0-1.
+        key (int | float): An integer value between 0-100 or float value between 0-1.
 
         
     Valid Examples:
      - CMYK(100, 100, 100, 100)
      - CMYK(100, 30, 80, 30)
      - CMYK(50, 30, 100, 0)
 
@@ -1172,21 +1211,28 @@
      - CMYK(2, 101, 50, 101)
      - CMYK(-3, 29, 290, 0)
      - CMYK(365, 123, 100, -100)
     """
 
     @staticmethod
     def __checkIfValid(value):
-        if any([True for i in value if type(i) != int]): return False
-        return len([i for i in list(value) if i >= 0 and i <= 100]) == 4
+        if any([True for i in value if type(i) not in [int, float]]): return False
+        value = [int(i * 100) if type(i) == float else i for i in value]
+        return len([i for i in value if i >= 0 and i <= 100]) == 4
 
 
 
-    def __init__(self, cyan: int, magenta: int, yellow: int, key: int):
+    def __init__(self, cyan: int | float, magenta: int | float, yellow: int | float, key: int | float, notPercent: bool = False):
         if self.__checkIfValid((cyan, magenta, yellow, key)):
+            if not notPercent:
+                if type(cyan) == float: cyan = int(cyan * 100)
+                if type(magenta) == float: magenta = int(magenta * 100)
+                if type(yellow) == float: yellow = int(yellow * 100)
+                if type(key) == float: key = int(key * 100)
+
             self.cyan = cyan
             self.magenta = magenta
             self.yellow = yellow
             self.key = key
             self.__valid = True
         
         else: self.__valid = False
```

### Comparing `idev-pycolor-1.0.4/idev-pycolor/PyColor/Functions.py` & `idev-pycolor-1.1.0/idev-pycolor/PyColor/Functions.py`

 * *Files identical despite different names*

### Comparing `idev-pycolor-1.0.4/idev-pycolor/PyColor/Palettes.py` & `idev-pycolor-1.1.0/idev-pycolor/PyColor/Palettes.py`

 * *Files identical despite different names*

### Comparing `idev-pycolor-1.0.4/idev-pycolor/idev_pycolor.egg-info/PKG-INFO` & `idev-pycolor-1.1.0/idev-pycolor/idev_pycolor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: idev-pycolor
-Version: 1.0.4
-Summary: A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.
+Version: 1.1.0
+Summary: A python collection of classes and functions to convert between multiple color models, generate palettes, and more.
 Home-page: https://github.com/IrtsaDevelopment/PyColor
 Author: IrtsaDevelopment
 Author-email: Irtsa <irtsa.development@gmail.com>
 Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyColor
 Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyColor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `idev-pycolor-1.0.4/pyproject.toml` & `idev-pycolor-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "idev-pycolor"
-version = "1.0.4"
+version = "1.1.0"
 authors = [
   { name="Irtsa", email="irtsa.development@gmail.com" },
 ]
-description = "A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors."
+description = "A python collection of classes and functions to convert between multiple color models, generate palettes, and more."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `idev-pycolor-1.0.4/setup.cfg` & `idev-pycolor-1.1.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 6465 762d 7079 636f 6c6f 720d   = idev-pycolor.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e34  .version = 1.0.4
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e31 2e30  .version = 1.1.0
 00000030: 0d0a 6175 7468 6f72 203d 2049 7274 7361  ..author = Irtsa
 00000040: 4465 7665 6c6f 706d 656e 740d 0a61 7574  Development..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6972 7473  hor_email = irts
 00000060: 612e 6465 7665 6c6f 706d 656e 7440 676d  a.development@gm
 00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000080: 7469 6f6e 203d 2041 2070 7974 686f 6e20  tion = A python 
 00000090: 636f 6c6c 6563 7469 6f6e 206f 6620 636c  collection of cl
 000000a0: 6173 7365 7320 616e 6420 6675 6e63 7469  asses and functi
 000000b0: 6f6e 7320 746f 2063 6f6e 7665 7274 2062  ons to convert b
-000000c0: 6574 7765 656e 2072 6762 2c20 6873 762c  etween rgb, hsv,
-000000d0: 2068 736c 2c20 7879 7a2c 2079 6363 2c20   hsl, xyz, ycc, 
-000000e0: 636d 796b 2c20 616e 6420 6865 7820 636f  cmyk, and hex co
-000000f0: 6c6f 7220 666f 726d 6174 7320 616e 6420  lor formats and 
-00000100: 6765 6e65 7261 7465 2070 616c 6574 7465  generate palette
-00000110: 7320 6672 6f6d 2073 6169 6420 636f 6c6f  s from said colo
-00000120: 7273 2e0d 0a6c 6f6e 675f 6465 7363 7269  rs...long_descri
-00000130: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
-00000140: 4144 4d45 2e6d 642c 204c 4943 454e 5345  ADME.md, LICENSE
-00000150: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-00000160: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
-00000170: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
-00000180: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
-00000190: 6974 6875 622e 636f 6d2f 4972 7473 6144  ithub.com/IrtsaD
-000001a0: 6576 656c 6f70 6d65 6e74 2f50 7943 6f6c  evelopment/PyCol
-000001b0: 6f72 0d0a 7072 6f6a 6563 745f 7572 6c73  or..project_urls
-000001c0: 203d 200d 0a09 4275 6720 5472 6163 6b65   = ...Bug Tracke
-000001d0: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
-000001e0: 7562 2e63 6f6d 2f49 7274 7361 4465 7665  ub.com/IrtsaDeve
-000001f0: 6c6f 706d 656e 742f 5079 436f 6c6f 722f  lopment/PyColor/
-00000200: 6973 7375 6573 0d0a 0972 6570 6f73 6974  issues...reposit
-00000210: 6f72 7920 3d20 6874 7470 733a 2f2f 6769  ory = https://gi
-00000220: 7468 7562 2e63 6f6d 2f49 7274 7361 4465  thub.com/IrtsaDe
-00000230: 7665 6c6f 706d 656e 742f 5079 436f 6c6f  velopment/PyColo
-00000240: 720d 0a63 6c61 7373 6966 6965 7273 203d  r..classifiers =
-00000250: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
-00000260: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000270: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
-00000280: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000290: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-000002a0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-000002b0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-000002c0: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
-000002d0: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
-000002e0: 3d20 0d0a 093d 2069 6465 762d 7079 636f  = ...= idev-pyco
-000002f0: 6c6f 720d 0a70 6163 6b61 6765 7320 3d20  lor..packages = 
-00000300: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
-00000310: 7175 6972 6573 203d 203e 3d33 2e36 0d0a  quires = >=3.6..
-00000320: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-00000330: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-00000340: 203d 2069 6465 762d 7079 636f 6c6f 720d   = idev-pycolor.
-00000350: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000360: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000370: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+000000c0: 6574 7765 656e 206d 756c 7469 706c 6520  etween multiple 
+000000d0: 636f 6c6f 7220 6d6f 6465 6c73 2c20 6765  color models, ge
+000000e0: 6e65 7261 7465 2070 616c 6574 7465 732c  nerate palettes,
+000000f0: 2061 6e64 206d 6f72 652e 0d0a 6c6f 6e67   and more...long
+00000100: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+00000110: 696c 653a 2052 4541 444d 452e 6d64 2c20  ile: README.md, 
+00000120: 4c49 4345 4e53 450d 0a6c 6f6e 675f 6465  LICENSE..long_de
+00000130: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
+00000140: 745f 7479 7065 203d 2074 6578 742f 6d61  t_type = text/ma
+00000150: 726b 646f 776e 0d0a 7572 6c20 3d20 6874  rkdown..url = ht
+00000160: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000170: 2f49 7274 7361 4465 7665 6c6f 706d 656e  /IrtsaDevelopmen
+00000180: 742f 5079 436f 6c6f 720d 0a70 726f 6a65  t/PyColor..proje
+00000190: 6374 5f75 726c 7320 3d20 0d0a 0942 7567  ct_urls = ...Bug
+000001a0: 2054 7261 636b 6572 203d 2068 7474 7073   Tracker = https
+000001b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4972  ://github.com/Ir
+000001c0: 7473 6144 6576 656c 6f70 6d65 6e74 2f50  tsaDevelopment/P
+000001d0: 7943 6f6c 6f72 2f69 7373 7565 730d 0a09  yColor/issues...
+000001e0: 7265 706f 7369 746f 7279 203d 2068 7474  repository = htt
+000001f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000200: 4972 7473 6144 6576 656c 6f70 6d65 6e74  IrtsaDevelopment
+00000210: 2f50 7943 6f6c 6f72 0d0a 636c 6173 7369  /PyColor..classi
+00000220: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
+00000230: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000240: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
+00000250: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
+00000260: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+00000270: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
+00000280: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+00000290: 2049 6e64 6570 656e 6465 6e74 0d0a 0d0a   Independent....
+000002a0: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
+000002b0: 6765 5f64 6972 203d 200d 0a09 3d20 6964  ge_dir = ...= id
+000002c0: 6576 2d70 7963 6f6c 6f72 0d0a 7061 636b  ev-pycolor..pack
+000002d0: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+000002e0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+000002f0: 3e3d 332e 360d 0a0d 0a5b 6f70 7469 6f6e  >=3.6....[option
+00000300: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000310: 0d0a 7768 6572 6520 3d20 6964 6576 2d70  ..where = idev-p
+00000320: 7963 6f6c 6f72 0d0a 0d0a 5b65 6767 5f69  ycolor....[egg_i
+00000330: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+00000340: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+00000350: 0d0a 0d0a                                ....
```

### Comparing `idev-pycolor-1.0.4/setup.py` & `idev-pycolor-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "idev-pycolor",
-    version = "1.0.4",
+    version = "1.1.0",
     author = "IrtsaDevelopment",
     author_email = "irtsa.development@gmail.com",
-    description = "A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.",
+    description = "A python collection of classes and functions to convert between multiple color models, generate palettes, and more.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/IrtsaDevelopment/PyColor",
     project_urls = {
         "Bug Tracker": "https://github.com/IrtsaDevelopment/PyColor/issues",
     },
     classifiers = [
```

