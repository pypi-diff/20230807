# Comparing `tmp/pyclpu-1.1.2.tar.gz` & `tmp/pyclpu-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclpu-1.1.2.tar", last modified: Wed Jul 12 07:27:30 2023, max compression
+gzip compressed data, was "pyclpu-1.1.3.tar", last modified: Mon Aug  7 14:01:58 2023, max compression
```

## Comparing `pyclpu-1.1.2.tar` & `pyclpu-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 07:27:30.782912 pyclpu-1.1.2/
--rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     8019 2023-07-12 07:27:30.782912 pyclpu-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     7611 2023-07-11 13:30:45.000000 pyclpu-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 07:27:30.773250 pyclpu-1.1.2/pyclpu/
--rw-rw-rw-   0        0        0      629 2023-07-12 07:27:09.000000 pyclpu-1.1.2/pyclpu/__init__.py
--rw-rw-rw-   0        0        0     1878 2023-06-02 09:58:39.000000 pyclpu-1.1.2/pyclpu/constants.py
--rw-rw-rw-   0        0        0      987 2023-07-11 12:56:55.000000 pyclpu-1.1.2/pyclpu/formats.py
--rw-rw-rw-   0        0        0    21605 2023-07-07 18:08:41.000000 pyclpu-1.1.2/pyclpu/image.py
--rw-rw-rw-   0        0        0    30305 2023-06-06 23:27:35.000000 pyclpu-1.1.2/pyclpu/main.py
--rw-rw-rw-   0        0        0    25587 2023-07-07 18:16:16.000000 pyclpu-1.1.2/pyclpu/manager.py
--rw-rw-rw-   0        0        0    28889 2023-07-12 07:19:58.000000 pyclpu-1.1.2/pyclpu/metrology.py
--rw-rw-rw-   0        0        0     7425 2023-06-02 09:58:39.000000 pyclpu-1.1.2/pyclpu/s33293804.py
--rw-rw-rw-   0        0        0    15876 2023-07-11 13:40:42.000000 pyclpu-1.1.2/pyclpu/waveform.py
-drwxrwxrwx   0        0        0        0 2023-07-12 07:27:30.781476 pyclpu-1.1.2/pyclpu.egg-info/
--rw-rw-rw-   0        0        0     8019 2023-07-12 07:27:28.000000 pyclpu-1.1.2/pyclpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-07-12 07:27:28.000000 pyclpu-1.1.2/pyclpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 07:27:28.000000 pyclpu-1.1.2/pyclpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-12 07:27:28.000000 pyclpu-1.1.2/pyclpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 07:27:28.000000 pyclpu-1.1.2/pyclpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       92 2023-07-12 07:27:30.783969 pyclpu-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2437 2023-07-07 18:08:41.000000 pyclpu-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:01:58.225360 pyclpu-1.1.3/
+-rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     8082 2023-08-07 14:01:58.225360 pyclpu-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7674 2023-07-24 09:10:09.000000 pyclpu-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 14:01:58.217665 pyclpu-1.1.3/pyclpu/
+-rw-rw-rw-   0        0        0      629 2023-08-07 14:01:30.000000 pyclpu-1.1.3/pyclpu/__init__.py
+-rw-rw-rw-   0        0        0     1878 2023-06-02 09:58:39.000000 pyclpu-1.1.3/pyclpu/constants.py
+-rw-rw-rw-   0        0        0      987 2023-07-12 07:28:37.000000 pyclpu-1.1.3/pyclpu/formats.py
+-rw-rw-rw-   0        0        0    21605 2023-07-07 18:08:41.000000 pyclpu-1.1.3/pyclpu/image.py
+-rw-rw-rw-   0        0        0    30305 2023-06-06 23:27:35.000000 pyclpu-1.1.3/pyclpu/main.py
+-rw-rw-rw-   0        0        0    25587 2023-07-12 07:28:37.000000 pyclpu-1.1.3/pyclpu/manager.py
+-rw-rw-rw-   0        0        0    37860 2023-08-07 13:52:28.000000 pyclpu-1.1.3/pyclpu/metrology.py
+-rw-rw-rw-   0        0        0     7425 2023-06-02 09:58:39.000000 pyclpu-1.1.3/pyclpu/s33293804.py
+-rw-rw-rw-   0        0        0    21963 2023-07-24 13:06:07.000000 pyclpu-1.1.3/pyclpu/waveform.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:01:58.223529 pyclpu-1.1.3/pyclpu.egg-info/
+-rw-rw-rw-   0        0        0     8082 2023-08-07 14:01:57.000000 pyclpu-1.1.3/pyclpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-08-07 14:01:57.000000 pyclpu-1.1.3/pyclpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 14:01:57.000000 pyclpu-1.1.3/pyclpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-08-07 14:01:57.000000 pyclpu-1.1.3/pyclpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 14:01:57.000000 pyclpu-1.1.3/pyclpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       92 2023-08-07 14:01:58.226729 pyclpu-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2437 2023-07-07 18:08:41.000000 pyclpu-1.1.3/setup.py
```

### Comparing `pyclpu-1.1.2/LICENSE` & `pyclpu-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.2/PKG-INFO` & `pyclpu-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclpu
-Version: 1.1.2
+Version: 1.1.3
 Summary: CLPU Utilities
 Home-page: https://git.clpu.es/mehret/pyclpu
 Author: Michael Ehret
 Author-email: mehret@clpu.es
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -173,15 +173,19 @@
                     manager.strip_extension(new_file)+".spec.dat"
                 ),
                 np.array([tof_detector.Gminus1,tof_detector.dN_dGminus1]).T,
                 header='gamma-1 dN/d(gamma-1)'
             )
 ```
 
-The following sniplet allows to see time-of-flight results from one single waveform file and saves them to a destination.
+### Work with Waveforms
+
+#### ... visualize and dsave data
+
+The following sniplet allows to see results of a channel from one single waveform file, and saves them to a destination.
 
 ```
 from pyclpu import waveform
 
 wfm = waveform.wfmread("C:\\bin\\emp_2023-07-10_44_122214.Wfm.bin")
 waveform.wfmshow(wfm)
```

### Comparing `pyclpu-1.1.2/README.md` & `pyclpu-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,19 @@
                     manager.strip_extension(new_file)+".spec.dat"
                 ),
                 np.array([tof_detector.Gminus1,tof_detector.dN_dGminus1]).T,
                 header='gamma-1 dN/d(gamma-1)'
             )
 ```
 
-The following sniplet allows to see time-of-flight results from one single waveform file and saves them to a destination.
+### Work with Waveforms
+
+#### ... visualize and dsave data
+
+The following sniplet allows to see results of a channel from one single waveform file, and saves them to a destination.
 
 ```
 from pyclpu import waveform
 
 wfm = waveform.wfmread("C:\\bin\\emp_2023-07-10_44_122214.Wfm.bin")
 waveform.wfmshow(wfm)
```

### Comparing `pyclpu-1.1.2/pyclpu/__init__.py` & `pyclpu-1.1.3/pyclpu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 pyclpu.
 
 CLPU Utilities.
 """
 # main attributes
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 __author__ = 'Michael Ehret'
 __credits__ = 'Centro de Laseres Pulsados, Villamayor, Spain'
 
 """
 DEVELOPMENT ZONE
 
 Until the following is not resolved, attributes below __init__.py require manual import as from pyclpu import ATTRIBUTE
```

### Comparing `pyclpu-1.1.2/pyclpu/constants.py` & `pyclpu-1.1.3/pyclpu/constants.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.2/pyclpu/formats.py` & `pyclpu-1.1.3/pyclpu/formats.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.2/pyclpu/image.py` & `pyclpu-1.1.3/pyclpu/image.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.2/pyclpu/main.py` & `pyclpu-1.1.3/pyclpu/main.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.2/pyclpu/manager.py` & `pyclpu-1.1.3/pyclpu/manager.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.2/pyclpu/metrology.py` & `pyclpu-1.1.3/pyclpu/metrology.py`

 * *Files 21% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 from inspect import getsourcefile
 from importlib import reload
 
 import math
 import numpy as np
 
 from scipy import signal
+from scipy import interpolate
+import cv2
 
 import matplotlib.pyplot as plt
 from tkinter import filedialog #not for the function
 from typing import List, Tuple
 
 # INTERNAL
 root = os.path.dirname(os.path.abspath(getsourcefile(lambda:0))) # get environment
@@ -58,93 +60,225 @@
     from waveform import Waveform            # import Waveform from waveform                     waveform.py
     reload(constants)
     reload(formats)
 
 # =============================================================================
 # CLASSES
 # =============================================================================
-class ThomsonParabola:
-    def __init__(self):
-        pass
-    # seleccionar_carpeta_destino(): This function open a folder dialog and allow select a destination folder
-    # inputs: none
-    # outputs; string with the folder path
+class ThomsonParabola():
+    """ Interactive Thomson Parabola diagnostics.
+    The class allows interactive work with data from a 2D particle spectrometer in the scheme of a Thomson Parabola. The interpretation of input waveforms is done relativistically. 
+    
+    Args:
+        dispersion_relation (str, optional) :  Absolute path to dispersion relation. Expect a file with lines ``[energy,space]``.
+        pixel_per_space (float, optional) : Conversion ratio of how many pixels correspond to one unit of space used in the dispersion relation.
+        source_directory (str, optional) : Path to directory with source files. If not given, file dialog will start.
+        source_files (list, optional) : List of filenames within ``source_directory``. If not given, file dialog will start.
+        X_ray_spot (tupple, optional) : Coordinates of the X-ray spot as tupple ``(x,y)``.
+        local_threshold (int, optional) : Threshold for finding local maxima next to local minima, defaults to ``1%`` of difference between minimum and maximum.
+        local_wake (int, optional) : Row-by-row wake, defaults to `10%` of the length of one row.
+        local_quality (int,optinal) : Minimum number of points in a valid trace, discard traces with smaller point lists. Defaults to 100.
+    
+    Attributes:
+        status (bool) : True if processing was successfull, else False.
+            Initializes to False.
+    
+    Returns:
+        filename (str) : Name of input file.
+        Xfiltered (`np.ndarray`) : Input image filtered from X-ray spots.
+        rowmaxs (`np.ndarray`) : Local maxima which were detected in each row.
+        trace (`np.ndarray`) : Detected trace.
+        superposition (`np.ndarray`) : Filtered input image superposed with trace.
+        trace_array (list) : Result list with all detected traces as ``[trace,X,Y]``
+        trace_array_energy (list) : Result list with all converted traces as ``[energy,spectral_count]``.
+        
+    Note:
+        The default trace width is assumed to be 5 pixels. There is currently no build in option to change this.
+        
+    Examples:
+        The class can be used in a functional way
+
+        ```python 
+        from pyclpu import metrology
+        TP = metrology.ThomsonParabola(source_directory = "C:\\bin", source_files = ["shot_426.tiff"])
+        ```
+
+        A more object oriented use case demonstrates how a run can be started after initialization
+
+        ```python
+        import cv2
+        from pyclpu import metrology
+
+        TP = metrology.ThomsonParabola()
+        TP.analyse()
+        ```
+        
+        The following example shows how the results from a single analysis can be saved.
+        
+        ```python
+        import os
+        from pyclpu import manager
+        
+        output_dir = "C:\\bin"
+
+        outA = os.path.join(output_dir, "A_no-X")
+        outB = os.path.join(output_dir, "B_row-by-row-maxs")
+        outC = os.path.join(output_dir, "C_trace")
+        outD = os.path.join(output_dir, "D_superposition")
+
+        if not os.path.exists(outA):
+            os.makedirs(outA)
+        if not os.path.exists(outB):
+            os.makedirs(outB)
+        if not os.path.exists(outC):
+            os.makedirs(outC)    
+        if not os.path.exists(outD):
+            os.makedirs(outD)
+
+        if TP.status:
+            cv2.imwrite(os.path.join(outA, TP.filename), TP.Xfiltered)
+            cv2.imwrite(os.path.join(outB, TP.filename), TP.rowmaxs)
+            cv2.imwrite(os.path.join(outC, TP.filename), TP.trace)
+            cv2.imwrite(os.path.join(outD, TP.filename), TP.superposition)
+            for n in range(len(TP.trace_array)):
+                # coordinates
+                with open(os.path.join(outC,manager.strip_extension(TP.filename) + "_trace_" + str(n) + ".csv"),"w") as f:
+                    f.write("X/[pix], Y/[pix], COUNT\n")
+                    for line in TP.trace_array[n]:
+                        f.write(", ".join(map(str,line))+"\n")
+                # spectrum
+                if hasattr(TP, 'trace_array_energy'):
+                    with open(os.path.join(outC,manager.strip_extension(TP.filename) + "_spectrum_" + str(n) + ".csv"),"w") as f:
+                        f.write("E/[MeV], COUNT*dx/dE\n")
+                        for line in TP.trace_array_energy[n]:
+                            f.write(", ".join(map(str,line))+"\n")
+                    array = np.array(TP.trace_array_energy[n])
+                    plt.plot(array[:,0],array[:,1])
+                    plt.xlabel("Energy / [MeV]")
+                    plt.ylabel("Number-density / [arb.u./MeV]")
+                    plt.savefig(os.path.join(outC,manager.strip_extension(TP.filename) + "_spectrum_" + str(n) + ".png"),dpi=300)
+                    plt.close("all")
+        ```
+        
+        It is also possible to analyse a batch of data in a loop.
+        
+        ```python
+        
+        ```
+    """
+    def __new__(cls, *args, **kwargs):
+        return super().__new__(cls)
+    def __init__(self, *args, **kwargs):
+        self.__dict__.update(kwargs)
+        self.status = False
+        # INTEGRITY
+        if not hasattr(self, 'dispersion_relation'):
+            warning(self.__class__.__name__,"No source file for the dispersion relation ``energy(space)`` defined, expect key `dispersion_relation` as type `str` pointing to a file with lines [energy,space].")
+        if not hasattr(self, 'source_directory'):
+            warning(self.__class__.__name__,"No source directory defined, expect key `source_directory` as type `string`.")
+        if not hasattr(self, 'source_files'):
+            warning(self.__class__.__name__,"No source files defined for data, expect key `source_files` as type `list`.")
+        # IN PLACE
+        if hasattr(self, 'source_directory') and hasattr(self, 'source_files'):
+            self.__run__()
+        return None
+    
     @staticmethod
-    def Seleccionar_carpeta_destino() -> str:
-        carpeta_destino = filedialog.askdirectory(title="Seleccionar carpeta de destino")
-        return carpeta_destino
-
-    # seleccionar_archivos(): This function open a multiple filedialog and allow select a destination folder
-    # inputs: none
-    # outputs: List of string with the files path
+    def Select_source_directory() -> str:
+        """
+        This function open a folder dialog and allow select a destination folder that contains source files.
+        Args: 
+            none
+        Returns: 
+            (unnamed value, string) : path to folder with source files
+        """
+        source_directory = filedialog.askdirectory(title="Select source directory.")
+        return source_directory
+
     @staticmethod
-    def Seleccionar_archivos() -> List[str]:
-        archivos = filedialog.askopenfilenames(title="Seleccionar archivos", filetypes=(
-        ("Archivos TIFF", "*.tiff;*.tif"), ("Todos los archivos", "*.*")))
-        lista = []
-        lista.extend(archivos)
-        return lista
-
-    # _searchpoint(img, a, sea, k): auxiliar function in cas that the trace is lost allow to search forward one pixel more selecting the best value
-    # in the next five pixels adjacent
-    # input img: image that is anlizing
-    #       pointlist  : list of selected point for this trace
-    #       previousvalue: previous value for the Y coordinate
-    #       actualX: actual x value in the scan
-    # output: the previous value of y
+    def Select_files(source_directory = None) -> List[str]:
+        """
+        This function opens a multiple filedialog and allow to select source files.
+        Args: 
+            source_directory (string, optional) : Open file dialogue in this directory, defaults to ``None``.
+        Returns: 
+            (unnamed value, list) : List of string with the file path.
+        Note:
+            Change of ``askopenfilename`` to ``askopenfilenames`` is intended for a future version, such as the organization of the string within a list is hopefully more clear.
+        """
+        file = filedialog.askopenfilename(
+            initialdir = source_directory, 
+            title="Select files", 
+            filetypes = (
+                ("TIFF Files", "*.tiff;*.tif"),
+                ("All files", "*.*")
+            )
+        )
+        source_files = [os.path.basename(file)]
+        #source_files.extend(files)
+        return source_files
+
     @staticmethod
     def _searchpoint(img, pointlist, previousvalue, actualX):
+        """
+        Auxiliar function in cas that the trace is lost allow to search forward one pixel more selecting the best value in the next five pixels adjacent.
+        Args: 
+            (1st positional argument `img`, array) : image that is analysed
+            (2nd positional argument `pointlist`, list) : list of selected point for this trace
+            (3rd positional argument `previousvalue`, float) : previous value for the Y coordinate
+            (4th positional argument `actualX`, float) : actual x value in the scan
+        Returns: 
+            (unnamed value, float) : the previous value of y
+        """
         try:
             # create a dictionary
             asa = {}
             # load the adjacent values
             for l in range(3):
                 asa[l] = img[actualX, int(previousvalue) + l]
-
             # select the maximum values
             max_value = max(asa.values())
-
             # append the best value
             for key, value in asa.items():
                 if value == max_value:
                     pointlist.append((int(key + previousvalue), actualX))
                     previousvalue = key + previousvalue
                     break
-
             return previousvalue
-
         except Exception as ex:
-            raise Exception("searchpoint fail")
+            raise Exception("searchpoint fail!")
 
-    # _rows(img, a, sea, k): auxiliar function search the local maximum in one row
-    # input img: image that is anlizing
-    #       clone  : copy of image where the local maximum are highligthed
-    #       previousvalue: previous value for the Y coordinate
-    #       actualX: actual row
-    #       threshold: the difference between two point in order to be considered a local maximum
     @staticmethod
     def _rows(img, clone, actualX, threshold):
+        """
+        Auxiliar function searches the local maximum in one row
+        Args:
+            (1st positional argument `img`, array) : image that is anlizing
+            (2nd positional argument `clone`, array)  : copy of image, the function will add highlighting of local maximuma
+            (3rd positional argument `previousvalue`, float) : previous value for the Y coordinate
+            (4th positional argument `actualX`, float) : actual row
+            (5th positional argument `threshold`, float) : the difference between two point in order to be considered a local maximum
+        Returns:
+            (unnamed value, float) : Sorted list of local maxima.
+        """
         # initialize variables
-        # set to save the maximum
+        #  set to save the maximum
         localmax = set()
-
-        # row of the image proccesed
+        #  row of the image proccesed
         row = img[actualX:actualX + 1, :]
-
+        #  rest
         localMaxima = []
         oldstatus = 0
         newstatus = 0
         maxvalue = 0
         maxvalex = 0
-
         # scan the row.  Works as a states machine searching for flanks
         for x in range(row.shape[1] - 1):
             centerValue = int(row[0, x])
             rightValue = int(row[0, x + 1])
-
             if rightValue - centerValue > threshold:
                 if newstatus == 0 and oldstatus == 0:
                     minx = x
                     oldstatus = 0
                     newstatus = 1
             elif centerValue - rightValue > threshold:
                 if newstatus == 1 and oldstatus == 1:
@@ -160,116 +294,115 @@
                 elif newstatus == 0 and oldstatus == 1:
                     maxx = x
                     oldstatus = 0
                     newstatus = 0
                     p = (maxvalex, actualX)
                     localMaxima.append(p)
                     localmax.add(maxvalex)
-
                     maxvalue = 0
                     maxvalex = 0
                 elif newstatus == 1 and oldstatus == 1:
                     if maxvalue < centerValue:
                         maxvalue = centerValue
                         maxvalex = x
-
         # highlight the local maximum
         for maxima in localMaxima:
             cv2.circle(clone, maxima, 1, (255, 255, 0))
-
         # return the local maximum ordered
         return sorted(localmax)
 
-    # ThompsomParabolaImageprocessingV2: This function search for the different traces in a Thomson parabola image. produces five folder:
-    # folder input save the original image
-    # folder output save the original image where the traces are painted with different colours
-    # folder mask save the traces with different colours
-    # folfer ouput gray save the traces without discrimination
-    # folder text save the sum of the 5 adjacent values in a csv
-    # input: pathDestinationSelected: output folder
-    #       picturesSelected: List of path for the different pictures
-    #       coluours: List of colours to be used in the different outputs like mask. should be a tuple RGB
-    #       threshold: the difference between two point in order to be considered a local maximum
-    #       wake: The maximum number of points tha can be founded with searchpoint function
-    #       quality: the minimum number of real point admmited in a trace
-    @staticmethod
-    def ThompsomParabolaImageprocessingV2(pathDestinationSelected: str, picturesSelected: List[str],
-                                          colours: List[Tuple[int, int, int]], threshold: int, wake: int, qualit: int):
+    def ThompsomParabolaImageprocessingV2(self, pathDestinationSelected: str, picturesSelected: List[str],
+                                          threshold: int = 0, wake: int = 0, quality_n: int = 100):
+        """
+        This function search for the different traces in a Thomson parabola image. For output, five folders are created:
+        - folder input save the original image
+        - folder output save the original image where the traces are painted with different colours
+        - folder mask save the traces with different colours
+        - folder ouput gray save the traces without discrimination
+        - folder text save the sum of the 5 adjacent values in a csv
+        Args: 
+            pathDestinationSelected (str): output folder
+            picturesSelected (list): List of path for the different pictures
+            threshold (int, optional): the difference between two point in order to be considered a local maximum, initializes to ``0`` and defaults to ``(max(img)-min(img))/100``.
+            wake (int, optional): The maximum number of points tha can be founded with searchpoint function, initializes to ``0`` and defaults to ``size(row)/10``.
+            quality_n: the minimum number of real point admmited in a trace
+        Returns:
+            none
+        """
         # intialize variables
-        pictures = picturesSelected
-        removepictures = []
-        filename = ""
-
-        # output paths
-        pathinputs = os.path.join(pathDestinationSelected, "input")
-        pathoutputsgray = os.path.join(pathDestinationSelected, "output_gray")
-        pathoutputs = os.path.join(pathDestinationSelected, "output")
-        pathoutputsmask = os.path.join(pathDestinationSelected, "mask")
-        pathoutputtext = os.path.join(pathDestinationSelected, "text")
-
-        # create the folder
-        if not os.path.exists(pathinputs):
-            os.makedirs(pathinputs)
-
-        if not os.path.exists(pathoutputs):
-            os.makedirs(pathoutputs)
-
-        if not os.path.exists(pathoutputsgray):
-            os.makedirs(pathoutputsgray)
-
-        if not os.path.exists(pathoutputsmask):
-            os.makedirs(pathoutputsmask)
-
-        if not os.path.exists(pathoutputtext):
-            os.makedirs(pathoutputtext)
+        self.filename = ""
+        
+        # fit dispersion relation if available
+        if hasattr(self, 'dispersion_relation') and hasattr(self, 'pixel_per_space') and hasattr(self, 'X_ray_spot'):
+            conversion = True
+            # build unit conversion for spectrum
+            disprelprot = np.loadtxt(self.dispersion_relation,skiprows=1)[1:]
+            dxde=np.array([[0, 0]])
+            for x in range(0, len(disprelprot)-1):
+               dxde=np.append(dxde, [[(disprelprot[x, 1]-disprelprot[x+1, 1])/(disprelprot[x+1,0]-disprelprot[x,0]),disprelprot[x, 0]]],axis=0)
+            dxde = dxde.T
+            dxde_of_energy = interpolate.interp1d(dxde[1], dxde[0], fill_value="extrapolate")
+            # define funtion energy(space) for lookup of coordinates
+            disrel = disprelprot.T
+            energy_of_y = interpolate.interp1d(disrel[1] * self.pixel_per_space, disrel[0], fill_value="extrapolate")
+        else:
+            conversion = False
 
         # start the proccess
         try:
             # scan each file in the List
             for file in picturesSelected:
 
                 # inicialize variables
                 memory = {}
                 quality = {}
                 trazas = {}
 
                 # get the name of the file
-                filename = os.path.basename(file)
+                self.filename = os.path.basename(file)
 
                 # read the file
-                img = cv2.imread(file, cv2.IMREAD_ANYDEPTH | cv2.IMREAD_GRAYSCALE)
+                img = cv2.imread(os.path.join(pathDestinationSelected,file), cv2.IMREAD_ANYDEPTH | cv2.IMREAD_GRAYSCALE)
 
                 # filter the X ray in the image
                 cv2.medianBlur(img, 5, img)
 
                 # prepare the different output images
-                clone = img.copy()
-                clone = cv2.convertScaleAbs(clone, alpha=(255.0 / 65535.0))
-                clone3 = img.copy()
-                clone3 = cv2.convertScaleAbs(clone3, alpha=(255.0 / 65535.0))
-                original = img.copy()
-                clone2 = np.zeros_like(img, dtype=np.uint8)
-                clone4 = np.zeros_like(img, dtype=np.uint8)
-                clone = cv2.cvtColor(clone, cv2.COLOR_GRAY2RGB)
-                clone3 = cv2.cvtColor(clone3, cv2.COLOR_GRAY2RGB)
+                #  filtered
+                self.Xfiltered = img.copy()
+                #  prepare canvas for image with highlightened maxima
+                self.rowmaxs = np.zeros_like(img, dtype=np.uint8)
+                #  RGB copy canvas for later trace add in
+                self.superposition = img.copy()
+                self.superposition = cv2.convertScaleAbs(self.superposition, alpha=(255.0 / self.superposition.max()))
+                self.superposition = cv2.cvtColor(self.superposition, cv2.COLOR_GRAY2RGB)
+                #  grayscale canvas for later trace add in
+                self.trace = np.zeros_like(img, dtype=np.uint8)
 
                 # range of row scans
                 range_iter = range(1020, -1, -1)
+                
+                # find or fix threshold
+                if threshold == 0:
+                    threshold = max(int((np.nanmax(img)-np.nanmin(img))/100.),1)
 
                 # search the local maximum
                 for i in range_iter:
-                    sort = ThomsonParabola._rows(img, clone2, i, threshold)
+                    sort = self._rows(img, self.rowmaxs, i, threshold)
                     if len(sort) != 0:
                         memory[i] = sort
                 memory = {k: memory[k] for k in sorted(memory.keys())}
-
+                
                 # combinin the different maximum to find the nearest if doesnt exist search with sarchpoint function a point
                 init2 = list(memory.keys())
                 counter = 1
-
+                
+                if wake == 0:
+                    wake = max(int(img.shape[1] / 10.),1)
+                
                 if memory:
                     for j in range(init2[0], init2[-1]):
                         a = []
                         rem = {}
 
                         # check the actual y in memory
                         if j in memory:
@@ -303,38 +436,38 @@
                                                     qul += 1
                                                     flse = 0
                                                     break
                                                 elif sea + 6 >= me and sea <= me:
                                                     meme = sea
                                                     qul += 1
                                                     c1 = 1
-                                                    me = ThomsonParabola._searchpoint(img, a, sea, k)
+                                                    me = self._searchpoint(img, a, sea, k)
                                                     break
                                                 else:
                                                     c1 = 2
                                             if c1 == 1:
                                                 if k in rem:
                                                     rem[k].append(int(meme))
                                                 else:
                                                     aux = []
                                                     aux.append(int(meme))
                                                     rem[k] = aux
                                                 c1 = 0
                                             elif c1 == 2:
-                                                me = ThomsonParabola._searchpoint(img, a, me, k)
+                                                me = self._searchpoint(img, a, me, k)
                                                 flse += 1
                                                 if flse > wake:
                                                     break
                                         else:
-                                            me = ThomsonParabola._searchpoint(img, a, me, k)
+                                            me = self._searchpoint(img, a, me, k)
                                             flse += 1
                                             if flse > wake:
                                                 break
                                     else:
-                                        me = ThomsonParabola._searchpoint(img, a, me, k)
+                                        me = self._searchpoint(img, a, me, k)
                                         flse += 1
                                         if flse > wake:
                                             break
                                     if me > 1200:
                                         break
                                     if flse > wake and len(a) == wake:
                                         for l in range(wake):
@@ -352,58 +485,84 @@
                                 for kk in rem.keys():
                                     for kkk in rem[kk]:
                                         if kkk in memory[kk]:
                                             memory[kk].remove(kkk)
 
                                 # remove the traces with not enough quality
                                 for a in quality.items():
-                                    if a[1] < qualit:
+                                    if a[1] < quality_n:
                                         trazas.pop(a[0], None)
-                # save proccess
+                # image creation proccess and trace array per trace
                 c3 = 0
+                trace_array = []
+                if conversion:
+                    trace_array_energy = []
                 for trazalist in trazas.keys():
                     trazasarray = trazas[trazalist]
-
-                    # save one file for each trace
-                    pathoutputtext2 = os.path.join(pathoutputtext, filename)
-
-                    # create path
-                    if not os.path.exists(pathoutputtext2):
-                        os.makedirs(pathoutputtext2)
-                    nam = "Traza" + str(c3) + ".csv"
-
-                    # write csv and prepare the other outputs
-                    with open(os.path.join(pathoutputtext2, nam), 'w') as writer:
-                        for l in range(len(trazasarray) - 1):
-                            clone3 = cv2.line(clone3, trazasarray[l], trazasarray[l + 1], colours[c3], 4)
-                            clone4 = cv2.line(clone4, trazasarray[l], trazasarray[l + 1], 255, 3)
-                            X = trazasarray[l][0]
-                            Y = trazasarray[l][1]
-
-                            Summa = int(original[Y, X - 2]) + int(original[Y, X - 1]) + int(original[Y, X]) + int(
-                                original[Y, X + 1]) + int(original[Y, X + 2])
-                            towrite = f"{X},{Y},{Summa}"
-                            writer.write(towrite + "\n")
+                    trace_array.append([])
+                    if conversion:
+                        trace_array_energy.append([])
+                    # write trace and prepare the other outputs
+                    for l in range(len(trazasarray) - 1):
+                        self.superposition = cv2.line(self.superposition, trazasarray[l], trazasarray[l + 1], (255, 0, 0), 4)
+                        self.trace = cv2.line(self.trace, trazasarray[l], trazasarray[l + 1], 255, 3)
+                        X = trazasarray[l][0]
+                        Y = trazasarray[l][1]
+
+                        Summa = int(self.Xfiltered[Y, X - 2]) + int(self.Xfiltered[Y, X - 1]) + int(self.Xfiltered[Y, X]) + int(self.Xfiltered[Y, X + 1]) + int(self.Xfiltered[Y, X + 2])
+                        trace_array[-1].append([X,Y,Summa])
+                        
+                        if conversion:
+                            space_var = self.X_ray_spot[1] - Y
+                            energy_var = energy_of_y(space_var)
+                            trace_array_energy[-1].append([energy_var,Summa*dxde_of_energy(energy_var)])
 
                     c3 += 1
                 # save the other files
-                cv2.imwrite(os.path.join(pathinputs, filename), clone)
-                cv2.imwrite(os.path.join(pathoutputs, filename + "out.tiff"), clone3)
-                cv2.imwrite(os.path.join(pathoutputsgray, filename + "out2.tiff"), clone2)
-                cv2.imwrite(os.path.join(pathoutputsmask, filename + "mask.tiff"), clone4)
-                print(filename + "  processed\n")
+                print(" > "+self.filename + " processed\n")
+                self.trace_array = trace_array
+                if conversion:
+                    self.trace_array_energy = trace_array_energy
 
         # in case of fail the processed picturs are removed and the proccess is restarted
         except Exception as ex:
             print(ex)
-            print(filename + "  fail\n")
+            print(" > "+self.filename + " failed\n")
 
-            for f in removepictures:
-                pictures.pop(f)
-            # ThompsomParabolaImageprocessingV2(pathDestinationSelected,pictures,colours,threshold,wake,qualit)
+        return None
+        
+    def __run__(self):
+        # INTEGRITY
+        if not hasattr(self, 'source_directory'):
+            self.source_directory = self.Select_source_directory()
+        if not hasattr(self, 'source_files'):
+            self.source_files = self.Select_files(source_directory = self.source_directory)
+        if not hasattr(self, 'local_threshold'):
+            warning(self.__class__.__name__,"No threshold defined for search of local maxima, expect key `local_threshold` as type `int`. Defaults to `1%` of the difference between maximum and minimum.")
+            self.local_threshold = 0
+        if not hasattr(self, 'local_wake'):
+            warning(self.__class__.__name__,"No row-by-row wake defined, expect key `local_wake` as type `int`. Defaults to `10%` of the length of one row.")
+            self.local_wake = 0
+        if not hasattr(self, 'local_quality'):
+            warning(self.__class__.__name__,"Minimum number of points before a trace is identified as valid, expect key `local_quality` as type `int`. Defaults to ``100``")
+            self.local_quality = 100
+        # MAIN
+        self.ThompsomParabolaImageprocessingV2(
+            pathDestinationSelected = self.source_directory,
+            picturesSelected = self.source_files,
+            threshold = self.local_threshold,
+            wake = self.local_wake, 
+            quality_n = self.local_quality
+        )
+        # housekeeping
+        if hasattr(self, 'trace_array'):
+            self.status = True
+    def analyse(self):
+        # START
+        self.__run__()
             
 class ToF():
     """ Interactive Time-of-Flight diagnostics.
     The class allows interactive work with data from a 1D Time-of-Flight detector. The interpretation of input waveforms is done relativistically. 
     
     Args:
         distance  (float,optional) : Source to detector distance in units of [m].
```

### Comparing `pyclpu-1.1.2/pyclpu/s33293804.py` & `pyclpu-1.1.3/pyclpu/s33293804.py`

 * *Files identical despite different names*

### Comparing `pyclpu-1.1.2/pyclpu/waveform.py` & `pyclpu-1.1.3/pyclpu/waveform.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import os
 import sys
 from inspect import getsourcefile
 from importlib import reload
 
 import math
 import numpy as np
-
+import scipy
 import matplotlib.pyplot as plt
 
 # INTERNAL
 root = os.path.dirname(os.path.abspath(getsourcefile(lambda:0))) # get environment
 sys.path.append(os.path.abspath(root))                           # add environment
 sys.path.append(os.path.abspath(root)+os.path.sep+"LIB")         # add library
 
@@ -200,23 +200,23 @@
                     # known keywords
                     with open(meta_file, 'r') as file:
                         lines = file.readlines()
                     for line in lines:
                         if "resolution" in line.lower():
                             try:
                                 find_increment = line.lower().replace("resolution","").strip().strip(":;,")
-                                horizontal = np.arange(vertical.shape[1]) * np.float(find_increment)
+                                horizontal = np.arange(vertical.shape[1]) * float(find_increment)
                                 timebase_known = True
                                 break
                             except:
                                 continue
                 # unknown exception: manual input
                 if not timebase_known:
                     ask_increment = input("Please enter the increment of timesteps in units of [s]:\n")
-                    horizontal = np.arange(vertical.shape[1]) * np.float(ask_increment)
+                    horizontal = np.arange(vertical.shape[1]) * float(ask_increment)
                 # housekeeping
                 del timebase_known
         return {"horizontal" : horizontal, "vertical" : vertical}
     # EXECUTE
     if iswfm(path):
         wfm = loader(path)
     else:
@@ -304,16 +304,137 @@
         plt.savefig(full_name+".png", dpi = 600)
         plt.close('all')
         return True
     except:
         error(wfmwrite.__name__,"",13)
         return False
         
+# WAVEFORM ANALYSYS
+
+def FastFourierTransform(wfm, *args, **kwargs):
+    """ Executes an FFT. 
+ 
+    The function generates the Fast Fourier Transform of all available channels of a waveform.
+ 
+    Args:
+        wfm (:obj: `numpy.array`) : Wafeform array.
+    
+    Returns:
+        fft (:obj: `numpy.array`) : FFT array.
+    
+    Examples:
+        ```python
+        FastFourierTransform("")
+        ```
+        returns
+        ```
+        None
+        ```
+    """
+    try:
+        fft = {}
+        oneD = False
+        if np.ndim(wfm["vertical"]) == 1:
+            wfm["vertical"] = [wfm["vertical"]]
+            oneD = True
+        fft["timestep"]    = wfm["horizontal"][1] - wfm["horizontal"][0]
+        fft["t_start"]     = wfm["horizontal"][0]
+        fft["t_stop"]      = wfm["horizontal"][-1]
+        fft["samples"]     = wfm["vertical"][0].size
+        fft["frequencies"] = scipy.fft.rfftfreq(fft["samples"], d = fft["timestep"])
+        amplitudes = []
+        for ai,signal in enumerate(wfm["vertical"]):
+            signal_FFT         = scipy.fft.rfft(signal,workers = os.cpu_count())
+            amplitudes.append(signal_FFT)
+        if oneD:
+            amplitudes = amplitudes[0]
+        fft["amplitudes"]  = np.array(amplitudes)
+        return fft
+    except:
+        error(FastFourierTransform.__name__,"",13)
+        return None
+    
+def InverseFastFourierTransform(fft, *args, **kwargs):
+    """ Executes an inverse FFT. 
+ 
+    The function generates the time-domain values of all available channels of a Fourier Transformed sgnal.
+ 
+    Args:
+        fft (:obj: `numpy.array`) : Fourier Transform dictionary ``{"timestep": real, "samples" : integer, "amplitudes" : np.array(), "frequencies" = np.array()}``.
+    
+    Returns:
+        wfm (:obj: `numpy.array`) : Waveform array.
+    
+    Examples:
+        ```python
+        InverseFastFourierTransform("")
+        ```
+        returns
+        ```
+        None
+        ```
+    """
+    try:
+        vertical = []
+        oneD = False
+        if np.ndim(fft["amplitudes"]) == 1:
+            fft["amplitudes"] = [fft["amplitudes"]]
+            oneD = True
+        for ai,amplitude in enumerate(fft["amplitudes"]):
+            ifft = scipy.fft.irfft(amplitude,n=fft["samples"], workers = os.cpu_count())
+            vertical.append(ifft)
+        if oneD:
+            vertical = vertical[0]
+        horizontal = np.linspace(fft["t_start"],fft["t_stop"],num=fft["samples"])
+        return {"horizontal" : horizontal, "vertical" : np.array(vertical)}
+    except:
+        error(InverseFastFourierTransform.__name__,"",13)
+        return None
+        
 # WAVEFORM MANIPULATION
 
+def bandpass(wfm, f_start, f_stop, *args, **kwargs):
+    """ Applies brick-wall bandpass filter to a waveform. 
+ 
+    The function generates the filtered time-domain values of all available channels in a waveform. The frequencies from `f_start` to ´f_stop` pass, others are supressed.
+ 
+    Args:
+        wfm (:obj: `numpy.array`) : Wafeform array.
+        f_start (float) : Lower limit of bandpass.
+        f_stop (float) : High limit of bandpass.
+    
+    Returns:
+        wfm (:obj: `numpy.array`) : Filtered waveform array.
+    
+    Examples:
+        ```python
+        bandpass("")
+        ```
+        returns
+        ```
+        None
+        ```
+    """
+    try:
+        fft = FastFourierTransform(wfm)
+        passed = np.where(np.logical_and(fft["frequencies"]>=f_start, fft["frequencies"]<=f_stop),True,False)
+        amplitudes = []
+        if np.ndim(fft["amplitudes"]) == 1:
+            fft["amplitudes"] = [fft["amplitudes"]]
+            oneD = True
+        for ai,amps in enumerate(fft["amplitudes"]):
+            fft["amplitudes"][ai] = np.where(passed,fft["amplitudes"][ai],0.+0.j)
+        if oneD:
+            fft["amplitudes"] = fft["amplitudes"][0]
+        else:
+            fft["amplitudes"] = np.array(fft["amplitudes"])
+        return InverseFastFourierTransform(fft)
+    except:
+        error(bandpass.__name__,"",13)
+        return None
     
 # =============================================================================
 # CLASSES
 # =============================================================================
 # INTEGRATION AND TESTING
 class Main:
     # https://realpython.com/python-class-constructor/
@@ -342,19 +463,21 @@
         for att in self.__dict__:
             string = string + str(att) + " -> " + str( getattr(self,att) ) + "\n"
         return str(type(self).__name__) + string + ")"
 
 # MAIN OBJECT  
 class Waveform():
     """ Waveform object.
-    The class allows interaction with a waveform object.
+    The class allows interaction with a waveform object. Build-in functions allow to display the data `.show()`; to save the data `.save("path/to/file.csv")`; ...
     
     Args:
         wfm    (dict,optional) : Waveform source as dictionary ``{"horizontal": numpy.array, "vertical": numpy.array(*channels)}`` .
         channel (int,optional) : Channel of interest.
+        lowest_frequency (float,optional) : Lowest frequency that can pass through the circuit, defaults to zero.
+        highest_frequency (float,optional) : Highest frequency that can pass through the circuit, defaults to the maximum allowed by the sampling rate.
     
     Attributes:
         status (bool) : True if processing was successfull, else False.
             Initializes to False.
     
     Returns:
         horizontal (float) : Array with horizontal axis.
@@ -378,14 +501,18 @@
         self.__dict__.update(kwargs)
         self.status = False
         # INTEGRITY
         if not hasattr(self, 'wfm'):
             warning(self.__class__.__name__,"No waveform source defined, expect key `waveform` as `waveform={'horizontal': numpy.array, 'vertical': numpy.array(*channels)}`.")
         if not hasattr(self, 'channel'):
             warning(self.__class__.__name__,"No source channel defined for data, expect key `channel` as type `int`.")
+        if not hasattr(self, 'lowest_frequency'):
+            warning(self.__class__.__name__,"No lowmost frequency defined for circuit, expect key `lowest_frequency` as type `float`.")
+        if not hasattr(self, 'highest_frequency'):
+            warning(self.__class__.__name__,"No highmost frequency defined for circuit, expect key `highest_frequency` as type `float`.")
         # IN PLACE
         if hasattr(self, 'wfm') and hasattr(self, 'channel'):
             self.__run__()
         return None
     def __setattr__(self, name, value):
         super().__setattr__(name, value)
         if hasattr(self, 'wfm') and hasattr(self, 'channel'):
@@ -393,25 +520,40 @@
                 self.__run__()
         return None
     def __run__(self):
         # INTEGRITY
         if not hasattr(self, 'wfm'):
             error(self.__class__.__name__,"No waveform source defined, expect key `waveform` as `waveform={'horizontal': numpy.array, 'vertical': numpy.array(*channels)}`. DO NOTHING.",1169)
             return None
-        if not hasattr(self, 'channel'):
-            warning(self.__class__.__name__,"No source channel defined for data, expect key `channel` as type `int`. Set `channel = 1`.")
-            self.channel = 1
-        # VARIABLES
         if self.wfm is None:
             error(self.__class__.__name__,"No valid waveform source defined, expect key `waveform` as `waveform={'horizontal': numpy.array, 'vertical': numpy.array(*channels)}`. DO NOTHING.",1169)
             return None
+        if not hasattr(self, 'channel'):
+            warning(self.__class__.__name__,"No source channel defined for data, expect key `channel` as type `int`. Set `channel = 1`.")
+            self.channel = 1
+        if not hasattr(self, 'lowest_frequency'):
+            warning(self.__class__.__name__,"No lowmost frequency defined for circuit, expect key `lowest_frequency` as type `float`. Defaults to zero.")
+            self.lowest_frequency = 0.
+        if not hasattr(self, 'highest_frequency'):
+            self.highest_frequency = scipy.fft.rfftfreq(self.wfm["horizontal"].size, d = self.wfm["horizontal"][1] - self.wfm["horizontal"][0])[-1]
+            warning(self.__class__.__name__,"No highmost frequency defined for circuit, expect key `highest_frequency` as type `float`. Defaults to maximum by sampling rate: " +str("%.2E" % self.highest_frequency))
+        # MAIN
         self.horizontal = self.wfm["horizontal"]
         self.vertical = self.wfm["vertical"][self.channel-1]
-        # MAIN
-        # fourier transform etc.
+        # CORRECTIONS
+        # bandpass limited
+        if not( self.highest_frequency == scipy.fft.rfftfreq(self.wfm["horizontal"].size, d = self.wfm["horizontal"][1] - self.wfm["horizontal"][0])[-1] and self.lowest_frequency == 0. ):
+            self.vertical = bandpass(
+                                {
+                                 "horizontal":self.horizontal,
+                                 "vertical"  :self.vertical
+                                },
+                                self.lowest_frequency,
+                                self.highest_frequency
+                            )["vertical"]
         
         # integrity of results
         self.status = True
         # housekeeping
         del self.wfm
         return None
     def show(self):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyclpu-1.1.2/pyclpu.egg-info/PKG-INFO` & `pyclpu-1.1.3/pyclpu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclpu
-Version: 1.1.2
+Version: 1.1.3
 Summary: CLPU Utilities
 Home-page: https://git.clpu.es/mehret/pyclpu
 Author: Michael Ehret
 Author-email: mehret@clpu.es
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -173,15 +173,19 @@
                     manager.strip_extension(new_file)+".spec.dat"
                 ),
                 np.array([tof_detector.Gminus1,tof_detector.dN_dGminus1]).T,
                 header='gamma-1 dN/d(gamma-1)'
             )
 ```
 
-The following sniplet allows to see time-of-flight results from one single waveform file and saves them to a destination.
+### Work with Waveforms
+
+#### ... visualize and dsave data
+
+The following sniplet allows to see results of a channel from one single waveform file, and saves them to a destination.
 
 ```
 from pyclpu import waveform
 
 wfm = waveform.wfmread("C:\\bin\\emp_2023-07-10_44_122214.Wfm.bin")
 waveform.wfmshow(wfm)
```

### Comparing `pyclpu-1.1.2/setup.py` & `pyclpu-1.1.3/setup.py`

 * *Files identical despite different names*

