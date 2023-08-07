# Comparing `tmp/bia-bob-0.1.1.tar.gz` & `tmp/bia-bob-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bia-bob-0.1.1.tar", last modified: Sat Aug  5 14:14:24 2023, max compression
+gzip compressed data, was "bia-bob-0.1.2.tar", last modified: Mon Aug  7 09:44:33 2023, max compression
```

## Comparing `bia-bob-0.1.1.tar` & `bia-bob-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 14:14:24.584846 bia-bob-0.1.1/
--rw-rw-rw-   0        0        0     1527 2023-08-05 10:23:51.000000 bia-bob-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      101 2023-08-05 10:44:20.000000 bia-bob-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2799 2023-08-05 14:14:24.585849 bia-bob-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1519 2023-08-05 12:15:53.000000 bia-bob-0.1.1/README.md
--rw-rw-rw-   0        0        0     1233 2023-08-05 10:44:20.000000 bia-bob-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1662 2023-08-05 14:14:24.592867 bia-bob-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       89 2023-02-23 17:18:17.000000 bia-bob-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 14:14:24.557775 bia-bob-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-05 14:14:24.568804 bia-bob-0.1.1/src/bia_bob/
--rw-rw-rw-   0        0        0      158 2023-08-05 14:08:29.000000 bia-bob-0.1.1/src/bia_bob/__init__.py
--rw-rw-rw-   0        0        0     1590 2023-08-05 11:28:14.000000 bia-bob-0.1.1/src/bia_bob/_machinery.py
-drwxrwxrwx   0        0        0        0 2023-08-05 14:14:24.584846 bia-bob-0.1.1/src/bia_bob/_tests/
--rw-rw-rw-   0        0        0       31 2023-08-05 10:48:31.000000 bia-bob-0.1.1/src/bia_bob/_tests/__init__.py
--rw-rw-rw-   0        0        0     3349 2023-08-05 11:28:59.000000 bia-bob-0.1.1/src/bia_bob/_tools.py
--rw-rw-rw-   0        0        0     1175 2023-08-05 14:04:46.000000 bia-bob-0.1.1/src/bia_bob/_utilities.py
-drwxrwxrwx   0        0        0        0 2023-08-05 14:14:24.583844 bia-bob-0.1.1/src/bia_bob.egg-info/
--rw-rw-rw-   0        0        0     2799 2023-08-05 14:14:24.000000 bia-bob-0.1.1/src/bia_bob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-08-05 14:14:24.000000 bia-bob-0.1.1/src/bia_bob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 14:14:24.000000 bia-bob-0.1.1/src/bia_bob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-08-05 14:14:24.000000 bia-bob-0.1.1/src/bia_bob.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-05 14:14:24.000000 bia-bob-0.1.1/src/bia_bob.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 09:44:33.091853 bia-bob-0.1.2/
+-rw-rw-rw-   0        0        0     1527 2023-08-05 10:23:51.000000 bia-bob-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-08-05 10:44:20.000000 bia-bob-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3825 2023-08-07 09:44:33.091853 bia-bob-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2545 2023-08-07 09:42:12.000000 bia-bob-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1233 2023-08-05 10:44:20.000000 bia-bob-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1662 2023-08-07 09:44:33.093858 bia-bob-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       89 2023-02-23 17:18:17.000000 bia-bob-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:44:33.044522 bia-bob-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 09:44:33.061094 bia-bob-0.1.2/src/bia_bob/
+-rw-rw-rw-   0        0        0      158 2023-08-07 09:41:27.000000 bia-bob-0.1.2/src/bia_bob/__init__.py
+-rw-rw-rw-   0        0        0     1590 2023-08-05 11:28:14.000000 bia-bob-0.1.2/src/bia_bob/_machinery.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:44:33.090849 bia-bob-0.1.2/src/bia_bob/_tests/
+-rw-rw-rw-   0        0        0       31 2023-08-05 10:48:31.000000 bia-bob-0.1.2/src/bia_bob/_tests/__init__.py
+-rw-rw-rw-   0        0        0     6643 2023-08-07 09:33:59.000000 bia-bob-0.1.2/src/bia_bob/_tools.py
+-rw-rw-rw-   0        0        0     1175 2023-08-05 15:52:07.000000 bia-bob-0.1.2/src/bia_bob/_utilities.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:44:33.085836 bia-bob-0.1.2/src/bia_bob.egg-info/
+-rw-rw-rw-   0        0        0     3825 2023-08-07 09:44:32.000000 bia-bob-0.1.2/src/bia_bob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-08-07 09:44:32.000000 bia-bob-0.1.2/src/bia_bob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 09:44:32.000000 bia-bob-0.1.2/src/bia_bob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-08-07 09:44:32.000000 bia-bob-0.1.2/src/bia_bob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-07 09:44:32.000000 bia-bob-0.1.2/src/bia_bob.egg-info/top_level.txt
```

### Comparing `bia-bob-0.1.1/LICENSE` & `bia-bob-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bia-bob-0.1.1/PKG-INFO` & `bia-bob-0.1.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bia-bob
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Jupyter-based assistant for working on bio-image analysis tasks
 Home-page: https://github.com/haesleinhuepf/bia-bob
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/bia-bob/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/bia-bob#README.md
@@ -36,28 +36,62 @@
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/bia_bob_trailer.gif)
 
 Note: Bob is currently in an early alpha stage. It is not very smart yet. Feedback is very welcome!
 
 ## Usage
 
-Detailed examples of how to interact with Bob are given in [this notebook](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/basic_demo.ipynb)
+Detailed examples of how to interact with Bob are given in these notebooks:
+* [Basic usage](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/basic_demo.ipynb)
+* [Accessing variables](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/globals.ipynb)
+* [Image Filtering](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/image_filtering.ipynb)
+* [Browsing folders](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/browsing_folders.ipynb)
+* [Interactive image stack viewing](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/interactive_stackview.ipynb)
 
+You can initialize Bob like this:
 ```
 from bia_bob import bob
 ```
 
+In case you want it to be aware of all your variables, call this addtionally:
+```
+bob.initialize(globals())
+```
+
+Afterwards, you can ask Bob questions like this:
+```
+%bob Load blobs.tif and show it
+```
+
+You can also ask Bob about available tools:
+```
+%bob list tools
+```
+
+Or like this:
+```
+%%bob
+Please load the image blobs.tif,
+segment bright objects in it, 
+count them and 
+show the segmentation result.
+```
+
+## Example gallery
+
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/load_and_show.png)
 
 ![img_1.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/slice.png)
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/chain_workflows.png)
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/count_blobs.png)
 
+![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/edge_detection.png)
+
 ## Known issues
 
 If you want to ask Bob a question, you need to put a space before the `?`.
 
 ```
 What do you know about blobs.gif?
 ```
```

### Comparing `bia-bob-0.1.1/README.md` & `bia-bob-0.1.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -7,28 +7,62 @@
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/bia_bob_trailer.gif)
 
 Note: Bob is currently in an early alpha stage. It is not very smart yet. Feedback is very welcome!
 
 ## Usage
 
-Detailed examples of how to interact with Bob are given in [this notebook](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/basic_demo.ipynb)
+Detailed examples of how to interact with Bob are given in these notebooks:
+* [Basic usage](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/basic_demo.ipynb)
+* [Accessing variables](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/globals.ipynb)
+* [Image Filtering](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/image_filtering.ipynb)
+* [Browsing folders](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/browsing_folders.ipynb)
+* [Interactive image stack viewing](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/interactive_stackview.ipynb)
 
+You can initialize Bob like this:
 ```
 from bia_bob import bob
 ```
 
+In case you want it to be aware of all your variables, call this addtionally:
+```
+bob.initialize(globals())
+```
+
+Afterwards, you can ask Bob questions like this:
+```
+%bob Load blobs.tif and show it
+```
+
+You can also ask Bob about available tools:
+```
+%bob list tools
+```
+
+Or like this:
+```
+%%bob
+Please load the image blobs.tif,
+segment bright objects in it, 
+count them and 
+show the segmentation result.
+```
+
+## Example gallery
+
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/load_and_show.png)
 
 ![img_1.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/slice.png)
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/chain_workflows.png)
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/count_blobs.png)
 
+![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/edge_detection.png)
+
 ## Known issues
 
 If you want to ask Bob a question, you need to put a space before the `?`.
 
 ```
 What do you know about blobs.gif?
 ```
```

### Comparing `bia-bob-0.1.1/pyproject.toml` & `bia-bob-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bia-bob-0.1.1/setup.cfg` & `bia-bob-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `bia-bob-0.1.1/src/bia_bob/_machinery.py` & `bia-bob-0.1.2/src/bia_bob/_machinery.py`

 * *Files identical despite different names*

### Comparing `bia-bob-0.1.1/src/bia_bob/_utilities.py` & `bia-bob-0.1.2/src/bia_bob/_utilities.py`

 * *Files identical despite different names*

### Comparing `bia-bob-0.1.1/src/bia_bob.egg-info/PKG-INFO` & `bia-bob-0.1.2/src/bia_bob.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bia-bob
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Jupyter-based assistant for working on bio-image analysis tasks
 Home-page: https://github.com/haesleinhuepf/bia-bob
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/bia-bob/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/bia-bob#README.md
@@ -36,28 +36,62 @@
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/bia_bob_trailer.gif)
 
 Note: Bob is currently in an early alpha stage. It is not very smart yet. Feedback is very welcome!
 
 ## Usage
 
-Detailed examples of how to interact with Bob are given in [this notebook](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/basic_demo.ipynb)
+Detailed examples of how to interact with Bob are given in these notebooks:
+* [Basic usage](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/basic_demo.ipynb)
+* [Accessing variables](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/globals.ipynb)
+* [Image Filtering](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/image_filtering.ipynb)
+* [Browsing folders](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/browsing_folders.ipynb)
+* [Interactive image stack viewing](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/interactive_stackview.ipynb)
 
+You can initialize Bob like this:
 ```
 from bia_bob import bob
 ```
 
+In case you want it to be aware of all your variables, call this addtionally:
+```
+bob.initialize(globals())
+```
+
+Afterwards, you can ask Bob questions like this:
+```
+%bob Load blobs.tif and show it
+```
+
+You can also ask Bob about available tools:
+```
+%bob list tools
+```
+
+Or like this:
+```
+%%bob
+Please load the image blobs.tif,
+segment bright objects in it, 
+count them and 
+show the segmentation result.
+```
+
+## Example gallery
+
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/load_and_show.png)
 
 ![img_1.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/slice.png)
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/chain_workflows.png)
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/count_blobs.png)
 
+![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/edge_detection.png)
+
 ## Known issues
 
 If you want to ask Bob a question, you need to put a space before the `?`.
 
 ```
 What do you know about blobs.gif?
 ```
```

