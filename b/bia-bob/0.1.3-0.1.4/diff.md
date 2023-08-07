# Comparing `tmp/bia-bob-0.1.3.tar.gz` & `tmp/bia-bob-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bia-bob-0.1.3.tar", last modified: Mon Aug  7 11:02:04 2023, max compression
+gzip compressed data, was "bia-bob-0.1.4.tar", last modified: Mon Aug  7 14:55:42 2023, max compression
```

## Comparing `bia-bob-0.1.3.tar` & `bia-bob-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 11:02:04.453003 bia-bob-0.1.3/
--rw-rw-rw-   0        0        0     1527 2023-08-05 10:23:51.000000 bia-bob-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      101 2023-08-05 10:44:20.000000 bia-bob-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3795 2023-08-07 11:02:04.454005 bia-bob-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2548 2023-08-07 10:58:05.000000 bia-bob-0.1.3/README.md
--rw-rw-rw-   0        0        0     1233 2023-08-05 10:44:20.000000 bia-bob-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0     1640 2023-08-07 11:02:04.460854 bia-bob-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0       89 2023-02-23 17:18:17.000000 bia-bob-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-07 11:02:04.421922 bia-bob-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-08-07 11:02:04.431948 bia-bob-0.1.3/src/bia_bob/
--rw-rw-rw-   0        0        0      158 2023-08-07 11:00:50.000000 bia-bob-0.1.3/src/bia_bob/__init__.py
--rw-rw-rw-   0        0        0     1590 2023-08-05 11:28:14.000000 bia-bob-0.1.3/src/bia_bob/_machinery.py
-drwxrwxrwx   0        0        0        0 2023-08-07 11:02:04.451999 bia-bob-0.1.3/src/bia_bob/_tests/
--rw-rw-rw-   0        0        0       31 2023-08-05 10:48:31.000000 bia-bob-0.1.3/src/bia_bob/_tests/__init__.py
--rw-rw-rw-   0        0        0     6643 2023-08-07 09:33:59.000000 bia-bob-0.1.3/src/bia_bob/_tools.py
--rw-rw-rw-   0        0        0     1175 2023-08-05 15:52:07.000000 bia-bob-0.1.3/src/bia_bob/_utilities.py
-drwxrwxrwx   0        0        0        0 2023-08-07 11:02:04.451999 bia-bob-0.1.3/src/bia_bob.egg-info/
--rw-rw-rw-   0        0        0     3795 2023-08-07 11:02:04.000000 bia-bob-0.1.3/src/bia_bob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-08-07 11:02:04.000000 bia-bob-0.1.3/src/bia_bob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 11:02:04.000000 bia-bob-0.1.3/src/bia_bob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-08-07 11:02:04.000000 bia-bob-0.1.3/src/bia_bob.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-07 11:02:04.000000 bia-bob-0.1.3/src/bia_bob.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 14:55:42.169488 bia-bob-0.1.4/
+-rw-rw-rw-   0        0        0     1527 2023-08-07 14:03:50.000000 bia-bob-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-08-07 14:03:50.000000 bia-bob-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4002 2023-08-07 14:55:42.169488 bia-bob-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2755 2023-08-07 14:44:44.000000 bia-bob-0.1.4/README.md
+-rw-rw-rw-   0        0        0     1233 2023-08-07 14:03:50.000000 bia-bob-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1696 2023-08-07 14:55:42.170488 bia-bob-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0       89 2023-08-07 14:03:50.000000 bia-bob-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:55:42.142488 bia-bob-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 14:55:42.149489 bia-bob-0.1.4/src/bia_bob/
+-rw-rw-rw-   0        0        0      158 2023-08-07 14:51:35.000000 bia-bob-0.1.4/src/bia_bob/__init__.py
+-rw-rw-rw-   0        0        0     1593 2023-08-07 14:03:50.000000 bia-bob-0.1.4/src/bia_bob/_machinery.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:55:42.168488 bia-bob-0.1.4/src/bia_bob/_tests/
+-rw-rw-rw-   0        0        0       31 2023-08-07 14:03:50.000000 bia-bob-0.1.4/src/bia_bob/_tests/__init__.py
+-rw-rw-rw-   0        0        0     8257 2023-08-07 14:46:55.000000 bia-bob-0.1.4/src/bia_bob/_tools.py
+-rw-rw-rw-   0        0        0     1175 2023-08-07 14:03:50.000000 bia-bob-0.1.4/src/bia_bob/_utilities.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:55:42.167488 bia-bob-0.1.4/src/bia_bob.egg-info/
+-rw-rw-rw-   0        0        0     4002 2023-08-07 14:55:41.000000 bia-bob-0.1.4/src/bia_bob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-08-07 14:55:42.000000 bia-bob-0.1.4/src/bia_bob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 14:55:41.000000 bia-bob-0.1.4/src/bia_bob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      177 2023-08-07 14:55:41.000000 bia-bob-0.1.4/src/bia_bob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-07 14:55:41.000000 bia-bob-0.1.4/src/bia_bob.egg-info/top_level.txt
```

### Comparing `bia-bob-0.1.3/LICENSE` & `bia-bob-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bia-bob-0.1.3/PKG-INFO` & `bia-bob-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bia-bob
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Jupyter-based assistant for working on bio-image analysis tasks
 Home-page: https://github.com/haesleinhuepf/bia-bob
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/bia-bob/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/bia-bob#README.md
@@ -31,31 +31,33 @@
 BIA Bob is a Jupyter-based assistant for interacting with image data and for working on Bio-image Analysis tasks.
 It is based on [LangChain](https://python.langchain.com/docs/get_started/introduction.html) and [OpenAI's API](https://openai.com/blog/openai-api). You need an openai API account to use it.
 
 Trailer:
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/bia_bob_trailer.gif)
 
-Note: Bob is currently in an early alpha stage. It is not very smart yet. Feedback is very welcome!
+Note: Bob is currently in an early alpha stage. It is not very smart yet and only knows some basic image processing algorithms. 
+Feedback and contributions are very welcome!
 
 ## Usage
 
 Detailed examples of how to interact with Bob are given in these notebooks:
 * [Basic usage](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/basic_demo.ipynb)
 * [Accessing variables](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/globals.ipynb)
 * [Image Filtering](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/image_filtering.ipynb)
+* [Choosing image segmentation algorithms](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/segmentation_algorithms.ipynb)
 * [Browsing folders](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/browsing_folders.ipynb)
 * [Interactive image stack viewing](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/interactive_stackview.ipynb)
 
 You can initialize Bob like this:
 ```
 from bia_bob import bob
 ```
 
-In case you want it to be aware of all your variables, call this addtionally:
+In case you want it to be aware of all your variables, call this additionally:
 ```
 bob.initialize(globals())
 ```
 
 Afterwards, you can ask Bob questions like this:
 ```
 %bob Load blobs.tif and show it
```

### Comparing `bia-bob-0.1.3/README.md` & `bia-bob-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,31 +3,33 @@
 BIA Bob is a Jupyter-based assistant for interacting with image data and for working on Bio-image Analysis tasks.
 It is based on [LangChain](https://python.langchain.com/docs/get_started/introduction.html) and [OpenAI's API](https://openai.com/blog/openai-api). You need an openai API account to use it.
 
 Trailer:
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/bia_bob_trailer.gif)
 
-Note: Bob is currently in an early alpha stage. It is not very smart yet. Feedback is very welcome!
+Note: Bob is currently in an early alpha stage. It is not very smart yet and only knows some basic image processing algorithms. 
+Feedback and contributions are very welcome!
 
 ## Usage
 
 Detailed examples of how to interact with Bob are given in these notebooks:
 * [Basic usage](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/basic_demo.ipynb)
 * [Accessing variables](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/globals.ipynb)
 * [Image Filtering](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/image_filtering.ipynb)
+* [Choosing image segmentation algorithms](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/segmentation_algorithms.ipynb)
 * [Browsing folders](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/browsing_folders.ipynb)
 * [Interactive image stack viewing](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/interactive_stackview.ipynb)
 
 You can initialize Bob like this:
 ```
 from bia_bob import bob
 ```
 
-In case you want it to be aware of all your variables, call this addtionally:
+In case you want it to be aware of all your variables, call this additionally:
 ```
 bob.initialize(globals())
 ```
 
 Afterwards, you can ask Bob questions like this:
 ```
 %bob Load blobs.tif and show it
```

### Comparing `bia-bob-0.1.3/pyproject.toml` & `bia-bob-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bia-bob-0.1.3/setup.cfg` & `bia-bob-0.1.4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -73,31 +73,34 @@
 00000480: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
 00000490: 7320 3d20 0d0a 096e 756d 7079 0d0a 0970  s = ...numpy...p
 000004a0: 7974 686f 6e2d 4c65 7665 6e73 6874 6569  ython-Levenshtei
 000004b0: 6e3e 3d30 2e32 312e 300d 0a09 7363 696b  n>=0.21.0...scik
 000004c0: 6974 2d69 6d61 6765 3e3d 302e 3139 2e30  it-image>=0.19.0
 000004d0: 0d0a 096c 616e 6763 6861 696e 3e3d 302e  ...langchain>=0.
 000004e0: 302e 3235 310d 0a09 7374 6163 6b76 6965  0.251...stackvie
-000004f0: 773e 3d30 2e36 2e33 0d0a 7079 7468 6f6e  w>=0.6.3..python
-00000500: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000510: 380d 0a69 6e63 6c75 6465 5f70 6163 6b61  8..include_packa
-00000520: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
-00000530: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-00000540: 093d 7372 630d 0a0d 0a5b 6f70 7469 6f6e  .=src....[option
-00000550: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-00000560: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
-00000570: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
-00000580: 5f72 6571 7569 7265 5d0d 0a74 6573 7469  _require]..testi
-00000590: 6e67 203d 200d 0a09 746f 780d 0a09 7079  ng = ...tox...py
-000005a0: 7465 7374 2020 2320 6874 7470 733a 2f2f  test  # https://
-000005b0: 646f 6373 2e70 7974 6573 742e 6f72 672f  docs.pytest.org/
-000005c0: 656e 2f6c 6174 6573 742f 636f 6e74 656e  en/latest/conten
-000005d0: 7473 2e68 746d 6c0d 0a09 7079 7465 7374  ts.html...pytest
-000005e0: 2d63 6f76 2020 2320 6874 7470 733a 2f2f  -cov  # https://
-000005f0: 7079 7465 7374 2d63 6f76 2e72 6561 6474  pytest-cov.readt
-00000600: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00000610: 6573 742f 0d0a 0d0a 5b6f 7074 696f 6e73  est/....[options
-00000620: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
-00000630: 2a20 3d20 2a2e 7961 6d6c 0d0a 0d0a 5b65  * = *.yaml....[e
-00000640: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000650: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000660: 203d 2030 0d0a 0d0a                       = 0....
+000004f0: 773e 3d30 2e36 2e33 0d0a 096e 6170 6172  w>=0.6.3...napar
+00000500: 692d 7365 676d 656e 742d 626c 6f62 732d  i-segment-blobs-
+00000510: 616e 642d 7468 696e 6773 2d77 6974 682d  and-things-with-
+00000520: 6d65 6d62 7261 6e65 733e 3d30 2e33 2e36  membranes>=0.3.6
+00000530: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+00000540: 7320 3d20 3e3d 332e 380d 0a69 6e63 6c75  s = >=3.8..inclu
+00000550: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+00000560: 3d20 5472 7565 0d0a 7061 636b 6167 655f  = True..package_
+00000570: 6469 7220 3d20 0d0a 093d 7372 630d 0a0d  dir = ...=src...
+00000580: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000590: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
+000005a0: 3d20 7372 630d 0a0d 0a5b 6f70 7469 6f6e  = src....[option
+000005b0: 732e 6578 7472 6173 5f72 6571 7569 7265  s.extras_require
+000005c0: 5d0d 0a74 6573 7469 6e67 203d 200d 0a09  ]..testing = ...
+000005d0: 746f 780d 0a09 7079 7465 7374 2020 2320  tox...pytest  # 
+000005e0: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
+000005f0: 6573 742e 6f72 672f 656e 2f6c 6174 6573  est.org/en/lates
+00000600: 742f 636f 6e74 656e 7473 2e68 746d 6c0d  t/contents.html.
+00000610: 0a09 7079 7465 7374 2d63 6f76 2020 2320  ..pytest-cov  # 
+00000620: 6874 7470 733a 2f2f 7079 7465 7374 2d63  https://pytest-c
+00000630: 6f76 2e72 6561 6474 6865 646f 6373 2e69  ov.readthedocs.i
+00000640: 6f2f 656e 2f6c 6174 6573 742f 0d0a 0d0a  o/en/latest/....
+00000650: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000660: 5f64 6174 615d 0d0a 2a20 3d20 2a2e 7961  _data]..* = *.ya
+00000670: 6d6c 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ml....[egg_info]
+00000680: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000690: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `bia-bob-0.1.3/src/bia_bob/_machinery.py` & `bia-bob-0.1.4/src/bia_bob/_machinery.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     if line and cell:
         return _context.agent.run(input=line + "\n" + cell)
     if line:
         return _context.agent.run(input=line)
     elif cell:
         return _context.agent.run(input=cell)
     else:
-        return "Please enter a question behind %ba"
+        return "Please enter a question behind %bob"
 
 
 
 def init_assistant(variables, temperature=0):
     if _context.verbose:
         print("Initializing assistant")
     from langchain.memory import ConversationBufferMemory
@@ -52,8 +52,8 @@
         memory=_context.memory
     )
 
     _context.variables = variables
 
 
 
-init_assistant(globals())
+init_assistant(globals())
```

### Comparing `bia-bob-0.1.3/src/bia_bob/_tools.py` & `bia-bob-0.1.4/src/bia_bob/_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,14 +42,31 @@
 
     denoised_image_name = make_variable_name("denoised_" + image_name)
     _context.variables[denoised_image_name] = denoised_image
 
     return "The denoised image has been stored as " + denoised_image_name
 
 
+@_context.tools.append
+@tool
+def median_filter(image_name):
+    """Useful for removing noise from an image using a simple method: the Gaussian blur."""
+    from napari_segment_blobs_and_things_with_membranes import median_filter as nsbatwm_median_filter
+
+    if _context.verbose:
+        print("denoising (Median filter)", image_name)
+
+    image = find_image(_context.variables, image_name)
+    denoised_image = nsbatwm_median_filter(image, radius=1)
+
+    denoised_image_name = make_variable_name("denoised_" + image_name)
+    _context.variables[denoised_image_name] = denoised_image
+
+    return "The denoised image has been stored as " + denoised_image_name
+
 
 @_context.tools.append
 @tool
 def top_hat(image_name):
     """Useful for removing background from an image using a simple method: the Top-Hat filter."""
     from napari_segment_blobs_and_things_with_membranes import white_tophat
 
@@ -82,31 +99,49 @@
 
     return "The image with the enhanced edges has been stored as " + enhanced_edges_image_name
 
 
 @_context.tools.append
 @tool
 def segment_bright_objects(image_name):
-    """Useful for segmenting bright objects in an image that has been loaded and stored before."""
+    """Useful for segmenting bright objects in an image that has been loaded and stored before using the Voronoi-Otsu-Labeling algorithm."""
     from napari_segment_blobs_and_things_with_membranes import voronoi_otsu_labeling
 
     if _context.verbose:
-        print("segmenting", image_name)
+        print("segmenting (voronoi_otsu_labeling)", image_name)
 
     image = find_image(_context.variables, image_name)
     label_image = voronoi_otsu_labeling(image, spot_sigma=4)
 
     label_image_name = "segmented_" + image_name
     _context.variables[make_variable_name(label_image_name)] = label_image
 
     return "The segmented image has been stored as " + label_image_name
 
 
 @_context.tools.append
 @tool
+def segment_dark_objects_with_bright_borders(image_name):
+    """Useful for segmenting dark objects with bright borders in an image that has been loaded and stored before using the Local-Minima-Seeded-Watershed algorithm. This might be good for segmenting cells in case membranes are in the image."""
+    from napari_segment_blobs_and_things_with_membranes import local_minima_seeded_watershed
+
+    if _context.verbose:
+        print("segmenting (local_minima_seeded_watershed)", image_name)
+
+    image = find_image(_context.variables, image_name)
+    label_image = local_minima_seeded_watershed(image, spot_sigma=10)
+
+    label_image_name = "segmented_" + image_name
+    _context.variables[make_variable_name(label_image_name)] = label_image
+
+    return "The segmented image has been stored as " + label_image_name
+
+
+@_context.tools.append
+@tool
 def show_image(image_name):
     """Useful for showing an image that has been loaded and stored before."""
     import stackview
     from IPython.core.display_functions import display
 
     if _context.verbose:
         print("showing", image_name)
@@ -197,7 +232,10 @@
 @_context.tools.append
 @tool
 def list_files_in_folder(folder):
     """Lists all files in a folder"""
     import os
 
     return "The files in the folder are " + ",".join(os.listdir(folder))
+
+
+
```

### Comparing `bia-bob-0.1.3/src/bia_bob/_utilities.py` & `bia-bob-0.1.4/src/bia_bob/_utilities.py`

 * *Files identical despite different names*

### Comparing `bia-bob-0.1.3/src/bia_bob.egg-info/PKG-INFO` & `bia-bob-0.1.4/src/bia_bob.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bia-bob
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Jupyter-based assistant for working on bio-image analysis tasks
 Home-page: https://github.com/haesleinhuepf/bia-bob
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/bia-bob/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/bia-bob#README.md
@@ -31,31 +31,33 @@
 BIA Bob is a Jupyter-based assistant for interacting with image data and for working on Bio-image Analysis tasks.
 It is based on [LangChain](https://python.langchain.com/docs/get_started/introduction.html) and [OpenAI's API](https://openai.com/blog/openai-api). You need an openai API account to use it.
 
 Trailer:
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/bia_bob_trailer.gif)
 
-Note: Bob is currently in an early alpha stage. It is not very smart yet. Feedback is very welcome!
+Note: Bob is currently in an early alpha stage. It is not very smart yet and only knows some basic image processing algorithms. 
+Feedback and contributions are very welcome!
 
 ## Usage
 
 Detailed examples of how to interact with Bob are given in these notebooks:
 * [Basic usage](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/basic_demo.ipynb)
 * [Accessing variables](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/globals.ipynb)
 * [Image Filtering](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/image_filtering.ipynb)
+* [Choosing image segmentation algorithms](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/segmentation_algorithms.ipynb)
 * [Browsing folders](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/browsing_folders.ipynb)
 * [Interactive image stack viewing](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/interactive_stackview.ipynb)
 
 You can initialize Bob like this:
 ```
 from bia_bob import bob
 ```
 
-In case you want it to be aware of all your variables, call this addtionally:
+In case you want it to be aware of all your variables, call this additionally:
 ```
 bob.initialize(globals())
 ```
 
 Afterwards, you can ask Bob questions like this:
 ```
 %bob Load blobs.tif and show it
```

