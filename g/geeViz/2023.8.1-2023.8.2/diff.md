# Comparing `tmp/geeViz-2023.8.1.tar.gz` & `tmp/geeViz-2023.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geeViz-2023.8.1.tar", last modified: Thu Aug  3 19:21:09 2023, max compression
+gzip compressed data, was "geeViz-2023.8.2.tar", last modified: Mon Aug  7 20:53:05 2023, max compression
```

## Comparing `geeViz-2023.8.1.tar` & `geeViz-2023.8.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 19:21:09.915890 geeViz-2023.8.1/
--rw-rw-rw-   0        0        0      574 2023-07-24 21:19:20.000000 geeViz-2023.8.1/LICENSE
--rw-rw-rw-   0        0        0     3851 2023-08-03 19:21:09.914888 geeViz-2023.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     3180 2023-07-18 20:28:01.000000 geeViz-2023.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 19:21:08.893822 geeViz-2023.8.1/geeViz/
--rw-rw-rw-   0        0        0      121 2023-08-03 17:05:51.000000 geeViz-2023.8.1/geeViz/__init__.py
--rw-rw-rw-   0        0        0    24675 2023-08-03 19:18:16.000000 geeViz-2023.8.1/geeViz/assetManagerLib.py
--rw-rw-rw-   0        0        0    96153 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/changeDetectionLib.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:21:09.462829 geeViz-2023.8.1/geeViz/examples/
--rw-rw-rw-   0        0        0     5467 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/CCDCViz.py
--rw-rw-rw-   0        0        0    11883 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/CCDCVizNotebook.ipynb
--rw-rw-rw-   0        0        0     8037 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/CCDCWrapper.py
--rw-rw-rw-   0        0        0     4424 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/GFSTimeLapse.py
--rw-rw-rw-   0        0        0     6284 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/LANDTRENDRViz.py
--rw-rw-rw-   0        0        0     9586 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/LANDTRENDRWrapper.py
--rw-rw-rw-   0        0        0    15557 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
--rw-rw-rw-   0        0        0    12631 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/LCMAP_and_LCMS_Viewer.py
--rw-rw-rw-   0        0        0    19522 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
--rw-rw-rw-   0        0        0      127 2023-08-03 17:05:44.000000 geeViz-2023.8.1/geeViz/examples/__init__.py
--rw-rw-rw-   0        0        0     1972 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/foliumViewerExample.py
--rw-rw-rw-   0        0        0   225731 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/gee2PandasExample.ipynb
--rw-rw-rw-   0        0        0     5771 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/geeViewExample.py
--rw-rw-rw-   0        0        0    16613 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/geeViewExampleNotebook.ipynb
--rw-rw-rw-   0        0        0    43661 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb
--rw-rw-rw-   0        0        0     5779 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/getClimateWrapper.py
--rw-rw-rw-   0        0        0    14302 2023-08-03 17:05:12.000000 geeViz-2023.8.1/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
--rw-rw-rw-   0        0        0    11478 2023-08-03 16:58:50.000000 geeViz-2023.8.1/geeViz/examples/getLandsatWrapper.py
--rw-rw-rw-   0        0        0    18431 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/getLandsatWrapperNotebook.ipynb
--rw-rw-rw-   0        0        0    12128 2023-08-03 17:04:31.000000 geeViz-2023.8.1/geeViz/examples/getSentinel2Wrapper.py
--rw-rw-rw-   0        0        0     9196 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/harmonicRegressionWrapper.py
--rw-rw-rw-   0        0        0     8218 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/lcmsViewerExample.py
--rw-rw-rw-   0        0        0    18777 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/lcmsViewerExampleNotebook.ipynb
--rw-rw-rw-   0        0        0    13051 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/phEEnoVizWrapper.py
--rw-rw-rw-   0        0        0     1063 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/taskTrackerExample.py
--rw-rw-rw-   0        0        0     6317 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/examples/timeLapseExample.py
--rw-rw-rw-   0        0        0     8783 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/foliumView.py
--rw-rw-rw-   0        0        0     1741 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/gcpLib.py
--rw-rw-rw-   0        0        0    10077 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/gee2Pandas.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:21:09.525310 geeViz-2023.8.1/geeViz/geeView/
-drwxrwxrwx   0        0        0        0 2023-08-03 19:21:09.540936 geeViz-2023.8.1/geeViz/geeView/css/
--rw-rw-rw-   0        0        0    30585 2023-07-19 17:12:21.000000 geeViz-2023.8.1/geeViz/geeView/css/style.min.css
--rw-rw-rw-   0        0        0    10024 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/foliumView.html
-drwxrwxrwx   0        0        0        0 2023-08-03 19:21:09.624734 geeViz-2023.8.1/geeViz/geeView/images/
--rw-rw-rw-   0        0        0     7295 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/EE-logo-150.png
--rw-rw-rw-   0        0        0    10301 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/GEE.png
--rw-rw-rw-   0        0        0     5692 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/GEE_logo_transparent.png
--rw-rw-rw-   0        0        0     4551 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/RCR-logo.jpg
--rw-rw-rw-   0        0        0     8352 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/cumulative_icon.png
--rw-rw-rw-   0        0        0     1502 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/layer_icon.png
--rw-rw-rw-   0        0        0   232219 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/logos_usda-fs.svg
--rw-rw-rw-   0        0        0   231399 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg
--rw-rw-rw-   0        0        0      652 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/menu-hamburger_ffffff.svg
--rw-rw-rw-   0        0        0     1489 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/usdalogo.png
--rw-rw-rw-   0        0        0     8174 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/images/usfslogo.png
--rw-rw-rw-   0        0        0     3455 2023-07-19 17:06:25.000000 geeViz-2023.8.1/geeViz/geeView/index.html
-drwxrwxrwx   0        0        0        0 2023-08-03 19:21:09.911203 geeViz-2023.8.1/geeViz/geeView/js/
--rw-rw-rw-   0        0        0    45351 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/js/gena-gee-palettes.js
--rw-rw-rw-   0        0        0   528516 2023-07-19 17:12:21.000000 geeViz-2023.8.1/geeViz/geeView/js/lcms-viewer.min.js
--rw-rw-rw-   0        0        0     1021 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/geeView/js/load.min.js
--rw-rw-rw-   0        0        0   450001 2023-08-03 17:05:30.000000 geeViz-2023.8.1/geeViz/geeView/js/runGeeViz.js
--rw-rw-rw-   0        0        0    16877 2023-07-28 17:13:30.000000 geeViz-2023.8.1/geeViz/geeView.py
--rw-rw-rw-   0        0        0   176095 2023-08-03 16:54:44.000000 geeViz-2023.8.1/geeViz/getImagesLib.py
--rw-rw-rw-   0        0        0     7467 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/migrateGEEAssets.py
--rw-rw-rw-   0        0        0    20743 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/phEEnoViz.py
--rw-rw-rw-   0        0        0     9885 2023-07-18 20:07:28.000000 geeViz-2023.8.1/geeViz/taskManagerLib.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:21:08.934713 geeViz-2023.8.1/geeViz.egg-info/
--rw-rw-rw-   0        0        0     3851 2023-08-03 19:21:08.000000 geeViz-2023.8.1/geeViz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2124 2023-08-03 19:21:08.000000 geeViz-2023.8.1/geeViz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 19:21:08.000000 geeViz-2023.8.1/geeViz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-08-03 19:21:08.000000 geeViz-2023.8.1/geeViz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-03 19:21:08.000000 geeViz-2023.8.1/geeViz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 19:21:09.916889 geeViz-2023.8.1/setup.cfg
--rw-rw-rw-   0        0        0     2173 2023-07-18 20:28:01.000000 geeViz-2023.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:53:05.602232 geeViz-2023.8.2/
+-rw-rw-rw-   0        0        0      574 2023-07-24 21:19:20.000000 geeViz-2023.8.2/LICENSE
+-rw-rw-rw-   0        0        0     3851 2023-08-07 20:53:05.602232 geeViz-2023.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3180 2023-07-18 20:28:01.000000 geeViz-2023.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 20:53:04.798917 geeViz-2023.8.2/geeViz/
+-rw-rw-rw-   0        0        0      121 2023-08-07 18:56:40.000000 geeViz-2023.8.2/geeViz/__init__.py
+-rw-rw-rw-   0        0        0    25661 2023-08-07 20:51:33.000000 geeViz-2023.8.2/geeViz/assetManagerLib.py
+-rw-rw-rw-   0        0        0    96121 2023-08-04 17:04:49.000000 geeViz-2023.8.2/geeViz/changeDetectionLib.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:53:05.167569 geeViz-2023.8.2/geeViz/examples/
+-rw-rw-rw-   0        0        0     5467 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/CCDCViz.py
+-rw-rw-rw-   0        0        0    11883 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/CCDCVizNotebook.ipynb
+-rw-rw-rw-   0        0        0     8037 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/CCDCWrapper.py
+-rw-rw-rw-   0        0        0     4424 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/GFSTimeLapse.py
+-rw-rw-rw-   0        0        0     6284 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/LANDTRENDRViz.py
+-rw-rw-rw-   0        0        0     9586 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/LANDTRENDRWrapper.py
+-rw-rw-rw-   0        0        0    15557 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
+-rw-rw-rw-   0        0        0    12631 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/LCMAP_and_LCMS_Viewer.py
+-rw-rw-rw-   0        0        0    19522 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
+-rw-rw-rw-   0        0        0      127 2023-08-07 20:49:45.000000 geeViz-2023.8.2/geeViz/examples/__init__.py
+-rw-rw-rw-   0        0        0     1972 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/foliumViewerExample.py
+-rw-rw-rw-   0        0        0   225731 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/gee2PandasExample.ipynb
+-rw-rw-rw-   0        0        0     5771 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/geeViewExample.py
+-rw-rw-rw-   0        0        0    16613 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/geeViewExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0    43661 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0     5779 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/getClimateWrapper.py
+-rw-rw-rw-   0        0        0    14302 2023-08-03 17:05:12.000000 geeViz-2023.8.2/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
+-rw-rw-rw-   0        0        0    11478 2023-08-03 16:58:50.000000 geeViz-2023.8.2/geeViz/examples/getLandsatWrapper.py
+-rw-rw-rw-   0        0        0    18431 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/getLandsatWrapperNotebook.ipynb
+-rw-rw-rw-   0        0        0    12128 2023-08-03 17:04:31.000000 geeViz-2023.8.2/geeViz/examples/getSentinel2Wrapper.py
+-rw-rw-rw-   0        0        0     9196 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/harmonicRegressionWrapper.py
+-rw-rw-rw-   0        0        0     8218 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/lcmsViewerExample.py
+-rw-rw-rw-   0        0        0    18777 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/lcmsViewerExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0    13051 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/phEEnoVizWrapper.py
+-rw-rw-rw-   0        0        0     1063 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/taskTrackerExample.py
+-rw-rw-rw-   0        0        0     6317 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/examples/timeLapseExample.py
+-rw-rw-rw-   0        0        0     8783 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/foliumView.py
+-rw-rw-rw-   0        0        0     1741 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/gcpLib.py
+-rw-rw-rw-   0        0        0    11956 2023-08-07 20:52:47.000000 geeViz-2023.8.2/geeViz/gee2Pandas.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:53:05.231952 geeViz-2023.8.2/geeViz/geeView/
+drwxrwxrwx   0        0        0        0 2023-08-07 20:53:05.239975 geeViz-2023.8.2/geeViz/geeView/css/
+-rw-rw-rw-   0        0        0    30585 2023-07-19 17:12:21.000000 geeViz-2023.8.2/geeViz/geeView/css/style.min.css
+-rw-rw-rw-   0        0        0    10024 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/geeView/foliumView.html
+drwxrwxrwx   0        0        0        0 2023-08-07 20:53:05.328278 geeViz-2023.8.2/geeViz/geeView/images/
+-rw-rw-rw-   0        0        0     7295 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/geeView/images/EE-logo-150.png
+-rw-rw-rw-   0        0        0    10301 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/geeView/images/GEE.png
+-rw-rw-rw-   0        0        0     5692 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/geeView/images/GEE_logo_transparent.png
+-rw-rw-rw-   0        0        0     4551 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/geeView/images/RCR-logo.jpg
+-rw-rw-rw-   0        0        0     8352 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/geeView/images/cumulative_icon.png
+-rw-rw-rw-   0        0        0     1502 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/geeView/images/layer_icon.png
+-rw-rw-rw-   0        0        0   232219 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/geeView/images/logos_usda-fs.svg
+-rw-rw-rw-   0        0        0   231399 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg
+-rw-rw-rw-   0        0        0      652 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/geeView/images/menu-hamburger_ffffff.svg
+-rw-rw-rw-   0        0        0     1489 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/geeView/images/usdalogo.png
+-rw-rw-rw-   0        0        0     8174 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/geeView/images/usfslogo.png
+-rw-rw-rw-   0        0        0     3455 2023-07-19 17:06:25.000000 geeViz-2023.8.2/geeViz/geeView/index.html
+drwxrwxrwx   0        0        0        0 2023-08-07 20:53:05.586612 geeViz-2023.8.2/geeViz/geeView/js/
+-rw-rw-rw-   0        0        0    45351 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/geeView/js/gena-gee-palettes.js
+-rw-rw-rw-   0        0        0   528516 2023-07-19 17:12:21.000000 geeViz-2023.8.2/geeViz/geeView/js/lcms-viewer.min.js
+-rw-rw-rw-   0        0        0     1021 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/geeView/js/load.min.js
+-rw-rw-rw-   0        0        0   120725 2023-08-03 20:55:06.000000 geeViz-2023.8.2/geeViz/geeView/js/runGeeViz.js
+-rw-rw-rw-   0        0        0    16877 2023-07-28 17:13:30.000000 geeViz-2023.8.2/geeViz/geeView.py
+-rw-rw-rw-   0        0        0   176095 2023-08-03 16:54:44.000000 geeViz-2023.8.2/geeViz/getImagesLib.py
+-rw-rw-rw-   0        0        0     7467 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/migrateGEEAssets.py
+-rw-rw-rw-   0        0        0    20743 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/phEEnoViz.py
+-rw-rw-rw-   0        0        0     9885 2023-07-18 20:07:28.000000 geeViz-2023.8.2/geeViz/taskManagerLib.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:53:04.854916 geeViz-2023.8.2/geeViz.egg-info/
+-rw-rw-rw-   0        0        0     3851 2023-08-07 20:53:04.000000 geeViz-2023.8.2/geeViz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2124 2023-08-07 20:53:04.000000 geeViz-2023.8.2/geeViz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 20:53:04.000000 geeViz-2023.8.2/geeViz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-08-07 20:53:04.000000 geeViz-2023.8.2/geeViz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 20:53:04.000000 geeViz-2023.8.2/geeViz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 20:53:05.602232 geeViz-2023.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     2173 2023-07-18 20:28:01.000000 geeViz-2023.8.2/setup.py
```

### Comparing `geeViz-2023.8.1/LICENSE` & `geeViz-2023.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/PKG-INFO` & `geeViz-2023.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeViz
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: A package to help with GEE data processing, analysis, and visualization
 Home-page: https://github.com/gee-community/geeViz
 Author: Ian Housman
 Author-email: ian.housman@gmail.com
 License: Apache
 Keywords: earthengine google remote sensing landsat sentinel modis forestry forest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `geeViz-2023.8.1/README.md` & `geeViz-2023.8.2/README.md`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/assetManagerLib.py` & `geeViz-2023.8.2/geeViz/assetManagerLib.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,19 +82,23 @@
         images = walkFolders(fromFolder)
     elif outType == 'tables':
         images = walkFoldersTables(fromFolder)
     #print( images)
 
     for image in images:
         out = toFolder +'/'+ base(image)
-        print( out)
-        try:
-            ee.data.copyAsset(image,out)
-        except:
-            print( out,'Error: May already exist')
+        if not ee_asset_exists(out):
+            print('Copying: ',image)
+            try:
+                ee.data.copyAsset(image,out)
+            except Exception as E:
+                print('Could not copy: ',image)
+                print(E)
+        else:
+            print(out,' already exists')
 
 def copyByName(fromFolder, toFolder, nameIdentifier, outType = 'imageCollection'):
 
     if outType == 'imageCollection':
         create_image_collection(toFolder)
     elif outType == 'tables':
         verify_path(toFolder)
@@ -413,25 +417,40 @@
             print('New collection '+full_path_to_collection+' created')
         except Exception as E:
             print('Could not create: ',full_path_to_collection)
             print(E)
             
 # More general function to create asset collecctions or folders
 # asset_type can be one of ee.data.ASSET_TYPE_FOLDER or ee.data.ASSET_TYPE_IMAGE_COLL
-def create_asset(asset_path,asset_type = ee.data.ASSET_TYPE_FOLDER):
+# If nested folders that do not already exist are provided, they will be created unless recursive = False
+def create_asset(asset_path,asset_type = ee.data.ASSET_TYPE_FOLDER,recursive=True):
+
+    # Find the root and all nested folders
+    project_root = f'{asset_path.split("assets")[0]}assets'
+    sub_directories = f'{asset_path.split("assets/")[1]}'.split('/')
+    
+    # If there is more than 1 level of folder, try to make them
+    if len(sub_directories) > 1 and recursive:
+        print('Found the following sub directories: ',sub_directories)
+        print('Will attempt to create them if they do not exist')
+        path_temp = project_root
+        for sub_directory in sub_directories[:-1]:
+            path_temp = f'{path_temp}/{sub_directory}'
+            create_asset(path_temp,asset_type = ee.data.ASSET_TYPE_FOLDER,recursive = False)
+
     if ee_asset_exists(asset_path):
         print("Asset "+asset_path+" already exists")
     else:
         try:
+            print(asset_path)
             ee.data.createAsset({'type': asset_type}, asset_path)
             print('New asset '+asset_path+' created')
         except Exception as E:
             print('Could not create: ',asset_path)
             print(E)
-
 def verify_path(path):
     response = ee.data.getInfo(path)
     if not response:
         logging.error('%s is not a valid destination. Make sure full path is provided e.g. users/user/nameofcollection '
                       'or projects/myproject/myfolder/newcollection and that you have write access there.', path)
         sys.exit(1)
 ##############################################################################################
```

### Comparing `geeViz-2023.8.1/geeViz/changeDetectionLib.py` & `geeViz-2023.8.2/geeViz/changeDetectionLib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1741,15 +1741,15 @@
   yearStartMonth = 9, yearStartDay = 1, annualizeWithCompositeDates = False, compositeCollection = None):
 
   # Create image collection of images with the proper time stamp as well as a 'year' band with the year fraction.
   if annualizeWithCompositeDates and compositeCollection != None:
     timeImgs = getTimeImageCollectionFromComposites(compositeCollection,startYear,endYear)
   else:
     timeImgs = getTimeImageCollection(startYear, endYear, startJulian ,endJulian, 1, yearStartMonth, yearStartDay)
-  Map.addLayer(timeImgs,{},'time')
+  
   # If selected, add a constant amount of time to last end segment to make sure the last year is annualized correctly.
   # tEndExtrapolationPeriod should be a fraction of a year.
   finalTEnd = ccdcImg.select('tEnd').arraySlice(0,-1,None).rename('tEnd').arrayGet(0).add(tEndExtrapolationPeriod).toArray(0)
   tEnds = ccdcImg.select('tEnd')
   tEnds = tEnds.arraySlice(0,0,-1).arrayCat(finalTEnd,0).rename('tEnd')
   ccdcImg = ccdcImg.addBands(tEnds,None,True)
```

### Comparing `geeViz-2023.8.1/geeViz/examples/CCDCViz.py` & `geeViz-2023.8.2/geeViz/examples/CCDCViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/CCDCVizNotebook.ipynb` & `geeViz-2023.8.2/geeViz/examples/CCDCVizNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/CCDCWrapper.py` & `geeViz-2023.8.2/geeViz/examples/CCDCWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/GFSTimeLapse.py` & `geeViz-2023.8.2/geeViz/examples/GFSTimeLapse.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/LANDTRENDRViz.py` & `geeViz-2023.8.2/geeViz/examples/LANDTRENDRViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/LANDTRENDRWrapper.py` & `geeViz-2023.8.2/geeViz/examples/LANDTRENDRWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb` & `geeViz-2023.8.2/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/LCMAP_and_LCMS_Viewer.py` & `geeViz-2023.8.2/geeViz/examples/LCMAP_and_LCMS_Viewer.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb` & `geeViz-2023.8.2/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/foliumViewerExample.py` & `geeViz-2023.8.2/geeViz/examples/foliumViewerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/gee2PandasExample.ipynb` & `geeViz-2023.8.2/geeViz/examples/gee2PandasExample.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/geeViewExample.py` & `geeViz-2023.8.2/geeViz/examples/geeViewExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/geeViewExampleNotebook.ipynb` & `geeViz-2023.8.2/geeViz/examples/geeViewExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb` & `geeViz-2023.8.2/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/getClimateWrapper.py` & `geeViz-2023.8.2/geeViz/examples/getClimateWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py` & `geeViz-2023.8.2/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/getLandsatWrapper.py` & `geeViz-2023.8.2/geeViz/examples/getLandsatWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/getLandsatWrapperNotebook.ipynb` & `geeViz-2023.8.2/geeViz/examples/getLandsatWrapperNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/getSentinel2Wrapper.py` & `geeViz-2023.8.2/geeViz/examples/getSentinel2Wrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/harmonicRegressionWrapper.py` & `geeViz-2023.8.2/geeViz/examples/harmonicRegressionWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/lcmsViewerExample.py` & `geeViz-2023.8.2/geeViz/examples/lcmsViewerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/lcmsViewerExampleNotebook.ipynb` & `geeViz-2023.8.2/geeViz/examples/lcmsViewerExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/phEEnoVizWrapper.py` & `geeViz-2023.8.2/geeViz/examples/phEEnoVizWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/taskTrackerExample.py` & `geeViz-2023.8.2/geeViz/examples/taskTrackerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/examples/timeLapseExample.py` & `geeViz-2023.8.2/geeViz/examples/timeLapseExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/foliumView.py` & `geeViz-2023.8.2/geeViz/foliumView.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/gcpLib.py` & `geeViz-2023.8.2/geeViz/gcpLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/gee2Pandas.py` & `geeViz-2023.8.2/geeViz/gee2Pandas.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,23 +14,21 @@
    limitations under the License.
 
 """
 
 #--------------------------------------------------------------------------
 #           Module to use GEE's online compute capabilities to take data from GEE into more universal environments such as Pandas
 #--------------------------------------------------------------------------
-
+import geeViz.geeView 
 import sys, ee, os, shutil, subprocess, datetime, calendar, json,glob,numpy,pandas
 import time, logging, pdb
 from simpledbf import Dbf5
-try:
-    z = ee.Number(1).getInfo()
-except:
-    print('Initializing GEE')
-    ee.Initialize()
+
+
+
 #########################################################################
 # Function to convert a featureCollection to json
 # If the output json file already exists, it will read it in
 # Returns the json version of the featureCollection
 # Currently maxNumberOfFeatures > 5000 will error out (need to handle slicing a feature list)
 def featureCollection_to_json(featureCollection,output_json_name,overwrite=False,maxNumberOfFeatures=5000):
     if not os.path.exists(output_json_name) or overwrite:
@@ -45,57 +43,88 @@
         t = json.load(o)
         o.close()
     return t
 #########################################################################
 # Convert featureCollection to csv
 # Can accept geojson or GEE featureCollection as the featureCollection argument
 # Will automatically create geojson version if given a gee FeatureCollection
-def featureCollection_to_csv(featureCollection,output_csv_name,overwrite = False,maxNumberOfFeatures=5000):
+def featureCollection_to_csv(featureCollection,output_csv_name,overwrite = False):
     if not os.path.exists(output_csv_name) or overwrite:
-        
-        # First find out if it is a file pathname or GEE featureCollection
-        # Read in if it's a json file pathname
-        # If it is a GEE featureCollection, convert it to json
-        if isinstance(featureCollection,str) and os.path.splitext(featureCollection)[1].lower().find('json') >-1:
-            o = open(featureCollection,'r')
-            table = json.load(o)
-            o.close()
-        elif isinstance(featureCollection,ee.featurecollection.FeatureCollection):
-            output_json_name = os.path.splitext(output_csv_name)[0]+'.json'
-            table = featureCollection_to_json(featureCollection,output_json_name,overwrite,maxNumberOfFeatures)
-        
-        # Set up the header
-        # Pull in ID and Lng and Lat field names if it's a point
-        if table['features'][0]['geometry']['type'] == 'Point':
-            bands = ['ID','Lng','Lat'] 
-        else:
-            bands = ['ID']
-
-        bands.extend(list(table['features'][0]['properties'].keys()))
-        header = ','.join(bands)+'\n'
-        out = header
-        
-        # Iterate across each feature and pull in the id, and properties
-        for feature in table['features']:
-            props = feature['properties']
-            geo = feature['geometry']
-            geoType = geo['type']
-            ID = str(feature['id'])
-            values = numpy.array(list(props.values()))
+        df = robust_featureCollection_to_df(featureCollection)
+        print('Writing:',output_csv_name)
+        df.to_csv(output_csv_name,index=False)
+    else:
+        print(output_csv_name,' already exists') 
+        # # First find out if it is a file pathname or GEE featureCollection
+        # # Read in if it's a json file pathname
+        # # If it is a GEE featureCollection, convert it to json
+        # if isinstance(featureCollection,str) and os.path.splitext(featureCollection)[1].lower().find('json') >-1:
+        #     o = open(featureCollection,'r')
+        #     table = json.load(o)
+        #     o.close()
+        # elif isinstance(featureCollection,ee.featurecollection.FeatureCollection):
+        #     output_json_name = os.path.splitext(output_csv_name)[0]+'.json'
+        #     table = featureCollection_to_json(featureCollection,output_json_name,overwrite,maxNumberOfFeatures)
+        
+        # # Set up the header
+        # # Pull in ID and Lng and Lat field names if it's a point
+        # if table['features'][0]['geometry']['type'] == 'Point':
+        #     bands = ['ID','Lng','Lat'] 
+        # else:
+        #     bands = ['ID']
+
+        # bands.extend(list(table['features'][0]['properties'].keys()))
+        # header = ','.join(bands)+'\n'
+        # out = header
+        
+        # # Iterate across each feature and pull in the id, and properties
+        # for feature in table['features']:
+        #     props = feature['properties']
+        #     geo = feature['geometry']
+        #     geoType = geo['type']
+        #     ID = str(feature['id'])
+        #     values = numpy.array(list(props.values()))
             
-            if geoType == 'Point':
-                ptCoords = geo['coordinates']
-                values = numpy.concatenate([[ID],geo['coordinates'],values])
-            values = ','.join([str(i) for i in values])+'\n'
-            values = values.replace(',None',',')
-            out+=values
-        
-        o = open(output_csv_name,'w')
-        o.write(out)
-        o.close()
+        #     if geoType == 'Point':
+        #         ptCoords = geo['coordinates']
+        #         values = numpy.concatenate([[ID],geo['coordinates'],values])
+        #     values = ','.join([str(i) for i in values])+'\n'
+        #     values = values.replace(',None',',')
+        #     out+=values
+        
+        # o = open(output_csv_name,'w')
+        # o.write(out)
+        # o.close()
+#########################################################################
+# Function to convert GEE featureCollection to a Pandas Dataframe
+# Handles the 5000 limit
+# This will run into memory errors if any complex operations precede the tables creation
+# In those instances, the featureCollections should first be exported to asset and then brought back in and run through
+# this function
+def robust_featureCollection_to_df(featureCollection):
+    maxFeatures = 5000
+    nFeatures = featureCollection.size().getInfo()
+    featureCollection = featureCollection.toList(1000000,0)
+    out_df = []
+    for start in range(0,nFeatures,maxFeatures):
+        end = start+maxFeatures
+        if end > nFeatures:end = nFeatures
+        print(f'Converting features {start+1}-{end}')
+        fcT = ee.FeatureCollection(featureCollection.slice(start,end))
+        df = pandas.json_normalize(fcT.getInfo()["features"])
+        out_df.append(df)
+       
+    out_df = pandas.concat(out_df)
+
+    properties = out_df.columns
+    properties_out = [prop.replace('properties.','') for prop in properties]
+    prop_dict = dict(zip(properties,properties_out))
+    out_df = out_df.rename(columns=prop_dict)
+
+    return out_df
 #########################################################################
 # Function to compute zonal stats in GEE and download results to a local csv
 def geeToLocalZonalStats(zones,raster,output_csv,reducer=ee.Reducer.first(),scale=None,crs=None,transform=None,tileScale=4,overwrite=False,maxNumberOfFeatures=5000):
     table = raster.reduceRegions(\
       zones,\
       reducer, \
       scale, \
@@ -191,23 +220,31 @@
     o.write(json.dumps(outJson))
     o.close()
     return outJson
 ####################################################################################################
 # Scratch space for testing
 if __name__ == '__main__':
     output_dir = r'C:\tmp\geeToPandasTest' 
-    out_json = os.path.join(output_dir,'test_json.json')
+    if not os.path.exists(output_dir):os.makedirs(output_dir)
+#     out_json = os.path.join(output_dir,'test_json.json')
 
     out_csv = os.path.join(output_dir,'test_json.csv')
-    if not os.path.exists(output_dir):os.makedirs(output_dir)
-    fc = ee.FeatureCollection('projects/lcms-292214/assets/CONUS-LCMS/Training-Tables/Training-Tables-AnnualizedFormat_v2022/LCMS-CONUS-2015').limit(5)
-    composite = ee.ImageCollection('projects/lcms-tcc-shared/assets/Composites/Composite-Collection-yesL7-1984-2020')\
-                    .filter(ee.Filter.calendarRange(2015,2015,'year')).mosaic()
-    # fc = ee.FeatureCollection('projects/lcms-292214/assets/CONUS-Ancillary-Data/FS_District_Boundaries')
-    # print(fc.size().getInfo())
-
-    geeToLocalZonalStats(fc,composite,out_csv,reducer=ee.Reducer.first(),scale=30,crs='EPSG:5070',transform=None,tileScale=4,overwrite=False,maxNumberOfFeatures=500)
-
-    fc_test = tableToFeatureCollection(out_csv,lat='Lat', lon='Lng',properties=[],dateCol=None,groupByColumns = None)
-    print(fc_test.first().getInfo())
-#     # featureCollection_to_json(fc,out_json,overwrite=True,maxNumberOfFeatures=20)
-#     # featureCollection_to_csv(fc,out_csv,overwrite = True,maxNumberOfFeatures=500)
+#     if not os.path.exists(output_dir):os.makedirs(output_dir)
+#     fc = ee.FeatureCollection('projects/lcms-292214/assets/CONUS-LCMS/Training-Tables/Training-Tables-AnnualizedFormat_v2022/LCMS-CONUS-2015').limit(5)
+#     composite = ee.ImageCollection('projects/lcms-tcc-shared/assets/Composites/Composite-Collection-yesL7-1984-2020')\
+#                     .filter(ee.Filter.calendarRange(2015,2015,'year')).mosaic()
+#     # fc = ee.FeatureCollection('projects/lcms-292214/assets/CONUS-Ancillary-Data/FS_District_Boundaries')
+#     # print(fc.size().getInfo())
+
+#     geeToLocalZonalStats(fc,composite,out_csv,reducer=ee.Reducer.first(),scale=30,crs='EPSG:5070',transform=None,tileScale=4,overwrite=False,maxNumberOfFeatures=500)
+
+#     fc_test = tableToFeatureCollection(out_csv,lat='Lat', lon='Lng',properties=[],dateCol=None,groupByColumns = None)
+#     print(fc_test.first().getInfo())
+# #     # featureCollection_to_json(fc,out_json,overwrite=True,maxNumberOfFeatures=20)
+# #     # featureCollection_to_csv(fc,out_csv,overwrite = True,maxNumberOfFeatures=500)
+
+    assets = ee.data.listAssets({'parent': 'projects/rcr-gee/assets/lcms-training/lcms-training_module-4_timeSync'})['assets']
+
+    training_data = ee.FeatureCollection([ee.FeatureCollection(asset['name']) for asset in assets]).flatten()
+   
+    # robust_featureCollection_to_df(training_data.limit(10))
+    featureCollection_to_csv(training_data,out_csv,overwrite = True)
```

### Comparing `geeViz-2023.8.1/geeViz/geeView/css/style.min.css` & `geeViz-2023.8.2/geeViz/geeView/css/style.min.css`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/foliumView.html` & `geeViz-2023.8.2/geeViz/geeView/foliumView.html`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/images/EE-logo-150.png` & `geeViz-2023.8.2/geeViz/geeView/images/EE-logo-150.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/images/GEE.png` & `geeViz-2023.8.2/geeViz/geeView/images/GEE.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/images/GEE_logo_transparent.png` & `geeViz-2023.8.2/geeViz/geeView/images/GEE_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/images/RCR-logo.jpg` & `geeViz-2023.8.2/geeViz/geeView/images/RCR-logo.jpg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/images/cumulative_icon.png` & `geeViz-2023.8.2/geeViz/geeView/images/cumulative_icon.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/images/layer_icon.png` & `geeViz-2023.8.2/geeViz/geeView/images/layer_icon.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/images/logos_usda-fs.svg` & `geeViz-2023.8.2/geeViz/geeView/images/logos_usda-fs.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg` & `geeViz-2023.8.2/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/images/menu-hamburger_ffffff.svg` & `geeViz-2023.8.2/geeViz/geeView/images/menu-hamburger_ffffff.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/images/usdalogo.png` & `geeViz-2023.8.2/geeViz/geeView/images/usdalogo.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/images/usfslogo.png` & `geeViz-2023.8.2/geeViz/geeView/images/usfslogo.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/index.html` & `geeViz-2023.8.2/geeViz/geeView/index.html`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/js/gena-gee-palettes.js` & `geeViz-2023.8.2/geeViz/geeView/js/gena-gee-palettes.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/js/lcms-viewer.min.js` & `geeViz-2023.8.2/geeViz/geeView/js/lcms-viewer.min.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView/js/load.min.js` & `geeViz-2023.8.2/geeViz/geeView/js/load.min.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/geeView.py` & `geeViz-2023.8.2/geeViz/geeView.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/getImagesLib.py` & `geeViz-2023.8.2/geeViz/getImagesLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/migrateGEEAssets.py` & `geeViz-2023.8.2/geeViz/migrateGEEAssets.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/phEEnoViz.py` & `geeViz-2023.8.2/geeViz/phEEnoViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz/taskManagerLib.py` & `geeViz-2023.8.2/geeViz/taskManagerLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/geeViz.egg-info/PKG-INFO` & `geeViz-2023.8.2/geeViz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeViz
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: A package to help with GEE data processing, analysis, and visualization
 Home-page: https://github.com/gee-community/geeViz
 Author: Ian Housman
 Author-email: ian.housman@gmail.com
 License: Apache
 Keywords: earthengine google remote sensing landsat sentinel modis forestry forest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `geeViz-2023.8.1/geeViz.egg-info/SOURCES.txt` & `geeViz-2023.8.2/geeViz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geeViz-2023.8.1/setup.py` & `geeViz-2023.8.2/setup.py`

 * *Files identical despite different names*

