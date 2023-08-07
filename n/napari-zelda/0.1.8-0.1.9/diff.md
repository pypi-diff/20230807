# Comparing `tmp/napari-zelda-0.1.8.tar.gz` & `tmp/napari-zelda-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\napari-zelda-0.1.8.tar", last modified: Mon Nov  8 23:39:10 2021, max compression
+gzip compressed data, was "dist\napari-zelda-0.1.9.tar", last modified: Tue Jan 25 22:34:06 2022, max compression
```

## Comparing `napari-zelda-0.1.8.tar` & `napari-zelda-0.1.9.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxrwx   0        0        0        0 2021-11-08 23:39:10.105375 napari-zelda-0.1.8/
-drwxrwxrwx   0        0        0        0 2021-11-08 23:39:09.850839 napari-zelda-0.1.8/.github/
-drwxrwxrwx   0        0        0        0 2021-11-08 23:39:09.900159 napari-zelda-0.1.8/.github/workflows/
--rw-rw-rw-   0        0        0     3168 2021-09-10 13:26:27.000000 napari-zelda-0.1.8/.github/workflows/test_and_deploy.yml
--rw-rw-rw-   0        0        0     1026 2021-09-10 13:26:27.000000 napari-zelda-0.1.8/.gitignore
-drwxrwxrwx   0        0        0        0 2021-11-08 23:39:09.917108 napari-zelda-0.1.8/.napari/
--rw-rw-rw-   0        0        0   148070 2021-11-07 08:48:39.000000 napari-zelda-0.1.8/.napari/DESCRIPTION.html
--rw-rw-rw-   0        0        0     5579 2021-11-07 08:48:39.000000 napari-zelda-0.1.8/.napari/DESCRIPTION.md
--rw-rw-rw-   0        0        0      169 2021-10-18 09:49:37.000000 napari-zelda-0.1.8/.napari/config.yml
--rw-rw-rw-   0        0        0     1514 2021-09-10 13:26:27.000000 napari-zelda-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      204 2021-10-18 15:45:00.000000 napari-zelda-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     8467 2021-11-08 23:39:10.106327 napari-zelda-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0   150579 2021-11-08 16:13:12.000000 napari-zelda-0.1.8/README.html
--rw-rw-rw-   0        0        0     7509 2021-11-08 16:13:11.000000 napari-zelda-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2021-11-08 23:39:10.030526 napari-zelda-0.1.8/docs/
--rw-rw-rw-   0        0        0    52373 2021-10-22 13:38:46.000000 napari-zelda-0.1.8/docs/2D-AF488.png
--rw-rw-rw-   0        0        0    90489 2021-10-22 13:38:46.000000 napari-zelda-0.1.8/docs/2D-AF488_MT.png
--rw-rw-rw-   0        0        0    57949 2021-10-22 13:38:46.000000 napari-zelda-0.1.8/docs/2D-AF488_parents.png
--rw-rw-rw-   0        0        0    54196 2021-10-22 13:38:46.000000 napari-zelda-0.1.8/docs/2D-MT.png
--rw-rw-rw-   0        0        0    56461 2021-10-22 13:38:46.000000 napari-zelda-0.1.8/docs/2D-MT_children.png
--rw-rw-rw-   0        0        0    54796 2021-10-22 13:38:46.000000 napari-zelda-0.1.8/docs/2D-MT_childrenbyParent.png
--rw-rw-rw-   0        0        0   526073 2021-09-14 18:42:30.000000 napari-zelda-0.1.8/docs/3ch_DNA_Actin_Mitochondria-AF488.tif
--rw-rw-rw-   0        0        0   526075 2021-09-14 18:42:04.000000 napari-zelda-0.1.8/docs/3ch_DNA_Actin_Mitochondria-MitoTracker.tif
--rw-rw-rw-   0        0        0    10054 2021-11-07 00:13:20.000000 napari-zelda-0.1.8/docs/Clipboard_Import_and_Export_Protocols.png
--rw-rw-rw-   0        0        0     2900 2021-10-22 22:04:45.000000 napari-zelda-0.1.8/docs/Clipboard_ZELDA_Launch_ZELDA.png
--rw-rw-rw-   0        0        0     4935 2021-11-07 22:48:14.000000 napari-zelda-0.1.8/docs/Clipboard_ZELDA_Plugin-set_panel_to_float.png
--rw-rw-rw-   0        0        0    81227 2021-10-22 22:04:45.000000 napari-zelda-0.1.8/docs/Clipboard_ZELDA_Plugin_install_ZELDA_in_napari_Arrow.png
--rw-rw-rw-   0        0        0     1911 2021-10-22 22:04:45.000000 napari-zelda-0.1.8/docs/Clipboard_ZELDA_Plugin_install_in_napari.png
--rw-rw-rw-   0        0        0    23896 2021-10-22 22:04:45.000000 napari-zelda-0.1.8/docs/Clipboard_ZELDA_Plugin_installed_ZELDA_in_napari_Arrow.png
--rw-rw-rw-   0        0        0     6647 2021-10-22 13:38:46.000000 napari-zelda-0.1.8/docs/CustomProtocol.png
--rw-rw-rw-   0        0        0    12415 2021-10-22 13:38:46.000000 napari-zelda-0.1.8/docs/Plot_hist_Area.png
--rw-rw-rw-   0        0        0    18878 2021-10-22 13:38:46.000000 napari-zelda-0.1.8/docs/Plot_scatter_Area-EqDiam.png
--rw-rw-rw-   0        0        0     1166 2021-10-27 21:11:18.000000 napari-zelda-0.1.8/docs/ZELDA_icon.png
--rw-rw-rw-   0        0        0      137 2021-09-10 13:26:27.000000 napari-zelda-0.1.8/docs/index.md
--rw-rw-rw-   0        0        0      252 2021-10-18 11:28:17.000000 napari-zelda-0.1.8/mkdocs.yml
-drwxrwxrwx   0        0        0        0 2021-11-08 23:39:10.067437 napari-zelda-0.1.8/napari_zelda/
--rw-rw-rw-   0        0        0      325 2021-10-23 15:30:12.000000 napari-zelda-0.1.8/napari_zelda/__init__.py
--rw-rw-rw-   0        0        0      166 2021-09-11 22:17:25.000000 napari-zelda-0.1.8/napari_zelda/_reader.py
-drwxrwxrwx   0        0        0        0 2021-11-08 23:39:10.102528 napari-zelda-0.1.8/napari_zelda/_tests/
--rw-rw-rw-   0        0        0        0 2021-09-14 10:39:39.000000 napari-zelda-0.1.8/napari_zelda/_tests/test_dock_widget.py
--rw-rw-rw-   0        0        0      483 2021-09-11 19:06:13.000000 napari-zelda-0.1.8/napari_zelda/_writer.py
--rw-rw-rw-   0        0        0      255 2021-09-12 00:15:37.000000 napari-zelda-0.1.8/napari_zelda/main.py
--rw-rw-rw-   0        0        0    38404 2021-11-08 23:35:04.000000 napari-zelda-0.1.8/napari_zelda/napari_zelda.py
--rw-rw-rw-   0        0        0      251 2021-10-22 21:18:48.000000 napari-zelda-0.1.8/napari_zelda/plugin.py
--rw-rw-rw-   0        0        0     2047 2021-11-07 08:36:07.000000 napari-zelda-0.1.8/napari_zelda/protocols_description.txt
--rw-rw-rw-   0        0        0      958 2021-11-06 23:40:55.000000 napari-zelda-0.1.8/napari_zelda/protocols_dict.json
--rw-rw-rw-   0        0        0      131 2021-11-07 08:36:41.000000 napari-zelda-0.1.8/napari_zelda/protocols_history.txt
-drwxrwxrwx   0        0        0        0 2021-11-08 23:39:10.098348 napari-zelda-0.1.8/napari_zelda.egg-info/
--rw-rw-rw-   0        0        0     8467 2021-11-08 23:39:09.000000 napari-zelda-0.1.8/napari_zelda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1377 2021-11-08 23:39:09.000000 napari-zelda-0.1.8/napari_zelda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-08 23:39:09.000000 napari-zelda-0.1.8/napari_zelda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2021-11-08 23:39:09.000000 napari-zelda-0.1.8/napari_zelda.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      118 2021-11-08 23:39:09.000000 napari-zelda-0.1.8/napari_zelda.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2021-11-08 23:39:09.000000 napari-zelda-0.1.8/napari_zelda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      197 2021-10-27 22:09:03.000000 napari-zelda-0.1.8/requirements.txt
--rw-rw-rw-   0        0        0     1173 2021-11-08 23:39:10.109365 napari-zelda-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      538 2021-11-08 22:31:37.000000 napari-zelda-0.1.8/setup.py
--rw-rw-rw-   0        0        0      981 2021-11-07 08:39:26.000000 napari-zelda-0.1.8/tox.ini
+drwxrwxrwx   0        0        0        0 2022-01-25 22:34:06.351697 napari-zelda-0.1.9/
+drwxrwxrwx   0        0        0        0 2022-01-25 22:34:06.272221 napari-zelda-0.1.9/.github/
+drwxrwxrwx   0        0        0        0 2022-01-25 22:34:06.290151 napari-zelda-0.1.9/.github/workflows/
+-rw-rw-rw-   0        0        0      594 2022-01-11 16:23:02.000000 napari-zelda-0.1.9/.github/workflows/plugin_preview.yml
+-rw-rw-rw-   0        0        0     3168 2021-09-10 13:26:27.000000 napari-zelda-0.1.9/.github/workflows/test_and_deploy.yml
+-rw-rw-rw-   0        0        0     1026 2021-09-10 13:26:27.000000 napari-zelda-0.1.9/.gitignore
+drwxrwxrwx   0        0        0        0 2022-01-25 22:34:06.295070 napari-zelda-0.1.9/.napari/
+-rw-rw-rw-   0        0        0   148070 2021-11-07 08:48:39.000000 napari-zelda-0.1.9/.napari/DESCRIPTION.html
+-rw-rw-rw-   0        0        0     5579 2021-11-07 08:48:39.000000 napari-zelda-0.1.9/.napari/DESCRIPTION.md
+-rw-rw-rw-   0        0        0      319 2022-01-11 16:23:02.000000 napari-zelda-0.1.9/.napari/config.yml
+-rw-rw-rw-   0        0        0     1514 2021-09-10 13:26:27.000000 napari-zelda-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      204 2021-10-18 15:45:00.000000 napari-zelda-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     8442 2022-01-25 22:34:06.351697 napari-zelda-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0   150591 2021-11-09 00:01:37.000000 napari-zelda-0.1.9/README.html
+-rw-rw-rw-   0        0        0     7484 2022-01-11 16:23:02.000000 napari-zelda-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2022-01-25 22:34:06.333709 napari-zelda-0.1.9/docs/
+-rw-rw-rw-   0        0        0    52373 2021-10-22 13:38:46.000000 napari-zelda-0.1.9/docs/2D-AF488.png
+-rw-rw-rw-   0        0        0    90489 2021-10-22 13:38:46.000000 napari-zelda-0.1.9/docs/2D-AF488_MT.png
+-rw-rw-rw-   0        0        0    57949 2021-10-22 13:38:46.000000 napari-zelda-0.1.9/docs/2D-AF488_parents.png
+-rw-rw-rw-   0        0        0    54196 2021-10-22 13:38:46.000000 napari-zelda-0.1.9/docs/2D-MT.png
+-rw-rw-rw-   0        0        0    56461 2021-10-22 13:38:46.000000 napari-zelda-0.1.9/docs/2D-MT_children.png
+-rw-rw-rw-   0        0        0    54796 2021-10-22 13:38:46.000000 napari-zelda-0.1.9/docs/2D-MT_childrenbyParent.png
+-rw-rw-rw-   0        0        0   526073 2021-09-14 18:42:30.000000 napari-zelda-0.1.9/docs/3ch_DNA_Actin_Mitochondria-AF488.tif
+-rw-rw-rw-   0        0        0   526075 2021-09-14 18:42:04.000000 napari-zelda-0.1.9/docs/3ch_DNA_Actin_Mitochondria-MitoTracker.tif
+-rw-rw-rw-   0        0        0    10054 2021-11-07 00:13:20.000000 napari-zelda-0.1.9/docs/Clipboard_Import_and_Export_Protocols.png
+-rw-rw-rw-   0        0        0     2900 2021-10-22 22:04:45.000000 napari-zelda-0.1.9/docs/Clipboard_ZELDA_Launch_ZELDA.png
+-rw-rw-rw-   0        0        0     4935 2021-11-07 22:48:14.000000 napari-zelda-0.1.9/docs/Clipboard_ZELDA_Plugin-set_panel_to_float.png
+-rw-rw-rw-   0        0        0    81227 2021-10-22 22:04:45.000000 napari-zelda-0.1.9/docs/Clipboard_ZELDA_Plugin_install_ZELDA_in_napari_Arrow.png
+-rw-rw-rw-   0        0        0     1911 2021-10-22 22:04:45.000000 napari-zelda-0.1.9/docs/Clipboard_ZELDA_Plugin_install_in_napari.png
+-rw-rw-rw-   0        0        0    23896 2021-10-22 22:04:45.000000 napari-zelda-0.1.9/docs/Clipboard_ZELDA_Plugin_installed_ZELDA_in_napari_Arrow.png
+-rw-rw-rw-   0        0        0     6647 2021-10-22 13:38:46.000000 napari-zelda-0.1.9/docs/CustomProtocol.png
+-rw-rw-rw-   0        0        0    12415 2021-10-22 13:38:46.000000 napari-zelda-0.1.9/docs/Plot_hist_Area.png
+-rw-rw-rw-   0        0        0    18878 2021-10-22 13:38:46.000000 napari-zelda-0.1.9/docs/Plot_scatter_Area-EqDiam.png
+-rw-rw-rw-   0        0        0     1166 2021-10-27 21:11:18.000000 napari-zelda-0.1.9/docs/ZELDA_icon.png
+-rw-rw-rw-   0        0        0      137 2021-09-10 13:26:27.000000 napari-zelda-0.1.9/docs/index.md
+-rw-rw-rw-   0        0        0      252 2021-10-18 11:28:17.000000 napari-zelda-0.1.9/mkdocs.yml
+drwxrwxrwx   0        0        0        0 2022-01-25 22:34:06.344701 napari-zelda-0.1.9/napari_zelda/
+-rw-rw-rw-   0        0        0      325 2021-10-23 15:30:12.000000 napari-zelda-0.1.9/napari_zelda/__init__.py
+-rw-rw-rw-   0        0        0      166 2021-09-11 22:17:25.000000 napari-zelda-0.1.9/napari_zelda/_reader.py
+drwxrwxrwx   0        0        0        0 2022-01-25 22:34:06.350701 napari-zelda-0.1.9/napari_zelda/_tests/
+-rw-rw-rw-   0        0        0      711 2022-01-25 21:50:26.000000 napari-zelda-0.1.9/napari_zelda/_tests/test_dock_widget.py
+-rw-rw-rw-   0        0        0      483 2021-09-11 19:06:13.000000 napari-zelda-0.1.9/napari_zelda/_writer.py
+-rw-rw-rw-   0        0        0      255 2021-09-12 00:15:37.000000 napari-zelda-0.1.9/napari_zelda/main.py
+-rw-rw-rw-   0        0        0    38432 2022-01-22 20:40:02.000000 napari-zelda-0.1.9/napari_zelda/napari_zelda.py
+-rw-rw-rw-   0        0        0      251 2021-10-22 21:18:48.000000 napari-zelda-0.1.9/napari_zelda/plugin.py
+-rw-rw-rw-   0        0        0     2047 2021-11-07 08:36:07.000000 napari-zelda-0.1.9/napari_zelda/protocols_description.txt
+-rw-rw-rw-   0        0        0      958 2021-11-06 23:40:55.000000 napari-zelda-0.1.9/napari_zelda/protocols_dict.json
+-rw-rw-rw-   0        0        0      131 2021-11-07 08:36:41.000000 napari-zelda-0.1.9/napari_zelda/protocols_history.txt
+drwxrwxrwx   0        0        0        0 2022-01-25 22:34:06.349667 napari-zelda-0.1.9/napari_zelda.egg-info/
+-rw-rw-rw-   0        0        0     8442 2022-01-25 22:34:05.000000 napari-zelda-0.1.9/napari_zelda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2022-01-25 22:34:06.000000 napari-zelda-0.1.9/napari_zelda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-25 22:34:05.000000 napari-zelda-0.1.9/napari_zelda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2022-01-25 22:34:05.000000 napari-zelda-0.1.9/napari_zelda.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      126 2022-01-25 22:34:05.000000 napari-zelda-0.1.9/napari_zelda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2022-01-25 22:34:05.000000 napari-zelda-0.1.9/napari_zelda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      197 2021-10-27 22:09:03.000000 napari-zelda-0.1.9/requirements.txt
+-rw-rw-rw-   0        0        0     1181 2022-01-25 22:34:06.353410 napari-zelda-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      538 2022-01-25 22:09:00.000000 napari-zelda-0.1.9/setup.py
+-rw-rw-rw-   0        0        0      883 2022-01-25 21:56:03.000000 napari-zelda-0.1.9/tox.ini
```

### Comparing `napari-zelda-0.1.8/.github/workflows/test_and_deploy.yml` & `napari-zelda-0.1.9/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/.gitignore` & `napari-zelda-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/.napari/DESCRIPTION.html` & `napari-zelda-0.1.9/.napari/DESCRIPTION.html`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/.napari/DESCRIPTION.md` & `napari-zelda-0.1.9/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/LICENSE` & `napari-zelda-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/PKG-INFO` & `napari-zelda-0.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,20 @@
-Metadata-Version: 2.1
-Name: napari-zelda
-Version: 0.1.8
-Summary: ZELDA: a 3D Image Segmentation and Parent-Child relation plugin for microscopy image analysis in napari
-Home-page: https://github.com/RoccoDAnt/napari-zelda
-Author: Rocco D'Antuono, Giuseppina Pisignano
-Author-email: rocco.dantuono@hotmail.it
-License: BSD-3-Clause
-Download-URL: https://github.com/RoccoDAnt/napari-zelda/archive/refs/tags/v0.1.8.tar.gz
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Framework :: napari
-Classifier: Topic :: Scientific/Engineering
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # napari-zelda
 
 [![License](https://img.shields.io/pypi/l/napari-zelda.svg?color=green)](https://github.com/RoccoDAnt/napari-zelda/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-zelda.svg?color=green)](https://pypi.org/project/napari-zelda)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-zelda.svg?color=green)](https://python.org)
 [![tests](https://github.com/RoccoDAnt/napari-zelda/workflows/tests/badge.svg)](https://github.com/RoccoDAnt/napari-zelda/actions)
 [![codecov](https://codecov.io/gh/RoccoDAnt/napari-zelda/branch/master/graph/badge.svg)](https://codecov.io/gh/RoccoDAnt/napari-zelda)
 
 ## ZELDA: a 3D Image Segmentation and Parent-Child relation plugin for microscopy image analysis in napari
 #### Authors: Rocco D'Antuono, Giuseppina Pisignano
 
-###### Preprint: [https://www.biorxiv.org/content/10.1101/2021.10.24.465596v1](https://www.biorxiv.org/content/10.1101/2021.10.24.465596v1)
+###### Article: Front. Comput. Sci., 04 January 2022 | https://doi.org/10.3389/fcomp.2021.796117
+
 ###### Examples of 2D and 3D data sets: [https://doi.org/10.5281/zenodo.5651284](https://zenodo.org/record/5651284#.YYgn_WDP2Ch)
 ----------------------------------
 
 ## What you can do with ZELDA plugin for napari
 The plugin can be used to analyze 2D/3D image data sets.  
 Multidimensional images (each channel corresponding to a napari layer) can be used to:
 
@@ -74,40 +52,42 @@
 5. Import and Export Protocols (image analysis workflows) in graphical mode (share with the community!).
 
     | ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_Import_and_Export_Protocols.png) <br> **Import and Export of ZELDA Protocols** |
     ------ |
 
 ## Installation
 
-**Option A.** You can install `napari-zelda` via [pip]. For the best experience, create a conda environment and use napari!=0.4.11, using the following instructions:
-
-    conda create -y -n napari-env python==3.8  
-    conda activate napari-env  
-    pip install "napari[all]"  
-    pip install napari-zelda  
-
-
-**Option B.** Alternatively, clone the repository and install locally via [pip]:
-
-    pip install -e .
-
-**Option C.** Another option is to use the napari interface to install it (make sure napari!=0.4.11):
+**Option A.** The easiest option is to use the napari interface to install ZELDA (make sure napari!=0.4.11):
 1. Plugins / Install/Uninstall Package(s)
 
   ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Plugin_install_in_napari.png)
 
 2. Choose ZELDA
 ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Plugin_install_ZELDA_in_napari_Arrow.png)
 
 3. ZELDA is installed
 ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Plugin_installed_ZELDA_in_napari_Arrow.png)
 
 4. Launch ZELDA
 ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Launch_ZELDA.png)
 
+
+**Option B.** You can install `napari-zelda` also via [pip]. For the best experience, create a conda environment and use napari!=0.4.11, using the following instructions:
+
+    conda create -y -n napari-env python==3.8  
+    conda activate napari-env  
+    pip install "napari[all]"  
+    pip install napari-zelda  
+
+
+**Option C.** Alternatively, clone the repository and install locally via [pip]:
+
+    pip install -e .
+
+
 ## Specifications
 
 This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
 
 The GUI has been developed using [magicgui](https://github.com/napari/magicgui) widgets, while the image analysis and processing include functions from [scikit-image](https://scikit-image.org/), [SciPy](https://scipy.org/), and [NumPy](https://numpy.org/). Results are handled with [pandas](https://pandas.pydata.org/) and [datatable](https://datatable.readthedocs.io/en/latest/). Plots are obtained with [matplotlib](https://matplotlib.org/).  
 <!--
 Don't miss the full getting started guide to set up your new package:
@@ -160,9 +140,7 @@
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
-
```

### Comparing `napari-zelda-0.1.8/README.html` & `napari-zelda-0.1.9/README.html`

 * *Files 0% similar despite different names*

```diff
@@ -76,35 +76,35 @@
 </li>
 <li><p>Import and Export Protocols (image analysis workflows) in graphical mode (share with the community!).</p>
 <p> | <img src="https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_Import_and_Export_Protocols.png" alt> <br> <strong>Import and Export of ZELDA Protocols</strong> |
  ------ |</p>
 </li>
 </ol>
 <h2 id="installation">Installation</h2>
-<p><strong>Option A.</strong> You can install <code>napari-zelda</code> via <a href="https://pypi.org/project/pip/">pip</a>. For the best experience, create a conda environment and use napari!=0.4.11, using the following instructions:</p>
-<pre><code>conda create -y -n napari-env python==3.8  
-conda activate napari-env  
-pip install &quot;napari[all]&quot;  
-pip install napari-zelda  </code></pre><p><strong>Option B.</strong> Alternatively, clone the repository and install locally via <a href="https://pypi.org/project/pip/">pip</a>:</p>
-<pre><code>pip install -e .</code></pre><p><strong>Option C.</strong> Another option is to use the napari interface to install it (make sure napari!=0.4.11):</p>
+<p><strong>Option A.</strong> The easiest option is to use the napari interface to install ZELDA (make sure napari!=0.4.11):</p>
 <ol>
 <li><p>Plugins / Install/Uninstall Package(s)</p>
 <p><img src="https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Plugin_install_in_napari.png" alt></p>
 </li>
 <li><p>Choose ZELDA
 <img src="https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Plugin_install_ZELDA_in_napari_Arrow.png" alt></p>
 </li>
 <li><p>ZELDA is installed
 <img src="https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Plugin_installed_ZELDA_in_napari_Arrow.png" alt></p>
 </li>
 <li><p>Launch ZELDA
 <img src="https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Launch_ZELDA.png" alt></p>
 </li>
 </ol>
-<h2 id="specifications">Specifications</h2>
+<p><strong>Option B.</strong> You can install <code>napari-zelda</code> also via <a href="https://pypi.org/project/pip/">pip</a>. For the best experience, create a conda environment and use napari!=0.4.11, using the following instructions:</p>
+<pre><code>conda create -y -n napari-env python==3.8  
+conda activate napari-env  
+pip install &quot;napari[all]&quot;  
+pip install napari-zelda  </code></pre><p><strong>Option C.</strong> Alternatively, clone the repository and install locally via <a href="https://pypi.org/project/pip/">pip</a>:</p>
+<pre><code>pip install -e .</code></pre><h2 id="specifications">Specifications</h2>
 <p>This <a href="https://github.com/napari/napari">napari</a> plugin was generated with <a href="https://github.com/audreyr/cookiecutter">Cookiecutter</a> using with <a href="https://github.com/napari">@napari</a>&apos;s <a href="https://github.com/napari/cookiecutter-napari-plugin">cookiecutter-napari-plugin</a> template.</p>
 <p>The GUI has been developed using <a href="https://github.com/napari/magicgui">magicgui</a> widgets, while the image analysis and processing include functions from <a href="https://scikit-image.org/">scikit-image</a>, <a href="https://scipy.org/">SciPy</a>, and <a href="https://numpy.org/">NumPy</a>. Results are handled with <a href="https://pandas.pydata.org/">pandas</a> and <a href="https://datatable.readthedocs.io/en/latest/">datatable</a>. Plots are obtained with <a href="https://matplotlib.org/">matplotlib</a>.  </p>
 <!--
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
 
 and review the napari docs for plugin developers:
```

#### html2text {}

```diff
@@ -43,28 +43,29 @@
       |
       Custom image analysis workflow | ------ |
    3. Import and Export Protocols (image analysis workflows) in graphical mode
       (share with the community!).
       |
       Import and Export of ZELDA Protocols | ------ |
 ***** Installation *****
-Option A. You can install napari-zelda via pip. For the best experience, create
-a conda environment and use napari!=0.4.11, using the following instructions:
+Option A. The easiest option is to use the napari interface to install ZELDA
+(make sure napari!=0.4.11):
+   1. Plugins / Install/Uninstall Package(s)
+   2. Choose ZELDA
+   3. ZELDA is installed
+   4. Launch ZELDA
+Option B. You can install napari-zelda also via pip. For the best experience,
+create a conda environment and use napari!=0.4.11, using the following
+instructions:
 conda create -y -n napari-env python==3.8
 conda activate napari-env
 pip install "napari[all]"
 pip install napari-zelda
-Option B. Alternatively, clone the repository and install locally via pip:
+Option C. Alternatively, clone the repository and install locally via pip:
 pip install -e .
-Option C. Another option is to use the napari interface to install it (make
-sure napari!=0.4.11):
-   1. Plugins / Install/Uninstall Package(s)
-   2. Choose ZELDA
-   3. ZELDA is installed
-   4. Launch ZELDA
 ***** Specifications *****
 This napari plugin was generated with Cookiecutter using with @napari's
 cookiecutter-napari-plugin template.
 The GUI has been developed using magicgui widgets, while the image analysis and
 processing include functions from scikit-image, SciPy, and NumPy. Results are
 handled with pandas and datatable. Plots are obtained with matplotlib.
 ***** Contributing *****
```

### Comparing `napari-zelda-0.1.8/README.md` & `napari-zelda-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,43 @@
+Metadata-Version: 2.1
+Name: napari-zelda
+Version: 0.1.9
+Summary: ZELDA: a 3D Image Segmentation and Parent-Child relation plugin for microscopy image analysis in napari
+Home-page: https://github.com/RoccoDAnt/napari-zelda
+Author: Rocco D'Antuono, Giuseppina Pisignano
+Author-email: rocco.dantuono@hotmail.it
+License: BSD-3-Clause
+Download-URL: https://github.com/RoccoDAnt/napari-zelda/archive/refs/tags/v0.1.9.tar.gz
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Framework :: napari
+Classifier: Topic :: Scientific/Engineering
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # napari-zelda
 
 [![License](https://img.shields.io/pypi/l/napari-zelda.svg?color=green)](https://github.com/RoccoDAnt/napari-zelda/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-zelda.svg?color=green)](https://pypi.org/project/napari-zelda)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-zelda.svg?color=green)](https://python.org)
 [![tests](https://github.com/RoccoDAnt/napari-zelda/workflows/tests/badge.svg)](https://github.com/RoccoDAnt/napari-zelda/actions)
 [![codecov](https://codecov.io/gh/RoccoDAnt/napari-zelda/branch/master/graph/badge.svg)](https://codecov.io/gh/RoccoDAnt/napari-zelda)
 
 ## ZELDA: a 3D Image Segmentation and Parent-Child relation plugin for microscopy image analysis in napari
 #### Authors: Rocco D'Antuono, Giuseppina Pisignano
 
-###### Preprint: [https://www.biorxiv.org/content/10.1101/2021.10.24.465596v1](https://www.biorxiv.org/content/10.1101/2021.10.24.465596v1)
+###### Article: Front. Comput. Sci., 04 January 2022 | https://doi.org/10.3389/fcomp.2021.796117
+
 ###### Examples of 2D and 3D data sets: [https://doi.org/10.5281/zenodo.5651284](https://zenodo.org/record/5651284#.YYgn_WDP2Ch)
 ----------------------------------
 
 ## What you can do with ZELDA plugin for napari
 The plugin can be used to analyze 2D/3D image data sets.  
 Multidimensional images (each channel corresponding to a napari layer) can be used to:
 
@@ -51,40 +75,42 @@
 5. Import and Export Protocols (image analysis workflows) in graphical mode (share with the community!).
 
     | ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_Import_and_Export_Protocols.png) <br> **Import and Export of ZELDA Protocols** |
     ------ |
 
 ## Installation
 
-**Option A.** You can install `napari-zelda` via [pip]. For the best experience, create a conda environment and use napari!=0.4.11, using the following instructions:
-
-    conda create -y -n napari-env python==3.8  
-    conda activate napari-env  
-    pip install "napari[all]"  
-    pip install napari-zelda  
-
-
-**Option B.** Alternatively, clone the repository and install locally via [pip]:
-
-    pip install -e .
-
-**Option C.** Another option is to use the napari interface to install it (make sure napari!=0.4.11):
+**Option A.** The easiest option is to use the napari interface to install ZELDA (make sure napari!=0.4.11):
 1. Plugins / Install/Uninstall Package(s)
 
   ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Plugin_install_in_napari.png)
 
 2. Choose ZELDA
 ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Plugin_install_ZELDA_in_napari_Arrow.png)
 
 3. ZELDA is installed
 ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Plugin_installed_ZELDA_in_napari_Arrow.png)
 
 4. Launch ZELDA
 ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Launch_ZELDA.png)
 
+
+**Option B.** You can install `napari-zelda` also via [pip]. For the best experience, create a conda environment and use napari!=0.4.11, using the following instructions:
+
+    conda create -y -n napari-env python==3.8  
+    conda activate napari-env  
+    pip install "napari[all]"  
+    pip install napari-zelda  
+
+
+**Option C.** Alternatively, clone the repository and install locally via [pip]:
+
+    pip install -e .
+
+
 ## Specifications
 
 This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
 
 The GUI has been developed using [magicgui](https://github.com/napari/magicgui) widgets, while the image analysis and processing include functions from [scikit-image](https://scikit-image.org/), [SciPy](https://scipy.org/), and [NumPy](https://numpy.org/). Results are handled with [pandas](https://pandas.pydata.org/) and [datatable](https://datatable.readthedocs.io/en/latest/). Plots are obtained with [matplotlib](https://matplotlib.org/).  
 <!--
 Don't miss the full getting started guide to set up your new package:
@@ -137,7 +163,9 @@
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
+
+
```

### Comparing `napari-zelda-0.1.8/docs/2D-AF488.png` & `napari-zelda-0.1.9/docs/2D-AF488.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/2D-AF488_MT.png` & `napari-zelda-0.1.9/docs/2D-AF488_MT.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/2D-AF488_parents.png` & `napari-zelda-0.1.9/docs/2D-AF488_parents.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/2D-MT.png` & `napari-zelda-0.1.9/docs/2D-MT.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/2D-MT_children.png` & `napari-zelda-0.1.9/docs/2D-MT_children.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/2D-MT_childrenbyParent.png` & `napari-zelda-0.1.9/docs/2D-MT_childrenbyParent.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/3ch_DNA_Actin_Mitochondria-AF488.tif` & `napari-zelda-0.1.9/docs/3ch_DNA_Actin_Mitochondria-AF488.tif`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/3ch_DNA_Actin_Mitochondria-MitoTracker.tif` & `napari-zelda-0.1.9/docs/3ch_DNA_Actin_Mitochondria-MitoTracker.tif`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/Clipboard_Import_and_Export_Protocols.png` & `napari-zelda-0.1.9/docs/Clipboard_Import_and_Export_Protocols.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/Clipboard_ZELDA_Launch_ZELDA.png` & `napari-zelda-0.1.9/docs/Clipboard_ZELDA_Launch_ZELDA.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/Clipboard_ZELDA_Plugin-set_panel_to_float.png` & `napari-zelda-0.1.9/docs/Clipboard_ZELDA_Plugin-set_panel_to_float.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/Clipboard_ZELDA_Plugin_install_ZELDA_in_napari_Arrow.png` & `napari-zelda-0.1.9/docs/Clipboard_ZELDA_Plugin_install_ZELDA_in_napari_Arrow.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/Clipboard_ZELDA_Plugin_install_in_napari.png` & `napari-zelda-0.1.9/docs/Clipboard_ZELDA_Plugin_install_in_napari.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/Clipboard_ZELDA_Plugin_installed_ZELDA_in_napari_Arrow.png` & `napari-zelda-0.1.9/docs/Clipboard_ZELDA_Plugin_installed_ZELDA_in_napari_Arrow.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/CustomProtocol.png` & `napari-zelda-0.1.9/docs/CustomProtocol.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/Plot_hist_Area.png` & `napari-zelda-0.1.9/docs/Plot_hist_Area.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/Plot_scatter_Area-EqDiam.png` & `napari-zelda-0.1.9/docs/Plot_scatter_Area-EqDiam.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/docs/ZELDA_icon.png` & `napari-zelda-0.1.9/docs/ZELDA_icon.png`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/napari_zelda/napari_zelda.py` & `napari-zelda-0.1.9/napari_zelda/napari_zelda.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,31 +199,32 @@
         mask[tuple((seeds).T)] = True
         markers, _ = ndimage.label(mask)
         labels = skimage.segmentation.watershed(-DistanceMap.data, markers, mask=binary.data)
         viewer.add_image(labels, scale=DistanceMap.scale, rgb=False, name='Labelled Children objects', opacity=0.6, rendering='mip', blending='additive', colormap='inferno')
 
 @magicgui(label={'widget_type':'Label', 'label':"Measure segmented objects"}, call_button="Measure objects",
           save_log={'widget_type':'CheckBox','name':'Save_Log','text':'Save Log'},
-          save_to={'widget_type': 'FileEdit', 'value':'\Documents', 'mode':'d','tooltip':'Save results to this folder path','label':False},
+          save_to={'widget_type': 'FileEdit', 'value':'\Documents', 'mode':'d','tooltip':'Save results to this folder path'},
           persist=True
             )
 def measure_one_pop( label, labels: Image, original: Image, save_log, save_to):
     properties=measure.regionprops_table(labels.data, original.data, properties= ['area', 'mean_intensity','min_intensity','max_intensity','equivalent_diameter','major_axis_length','minor_axis_length'])
-    prop={'Area': properties['area']*np.prod(original.scale),'Equivalent_diameter': properties['equivalent_diameter']*original.scale[-1],'MFI': properties['mean_intensity'],
+    prop={'Area': properties['area']*original.scale[-1]*original.scale[-2],'Equivalent_diameter': properties['equivalent_diameter']*original.scale[-1],'MFI': properties['mean_intensity'],
     'Min_Intensity': properties['min_intensity'], 'Max_Intensity': properties['max_intensity'],'MajorAxis_Length': properties['major_axis_length']*original.scale[-1],
     'MinorAxis_Length': properties['minor_axis_length']*original.scale[-1]
     }
     #prop_df=pd.DataFrame(prop)
     prop_df=dt.Frame(prop) #datatable instead of pandas
     prop_df.to_csv(str(save_to)+'\Results.csv')
 
     log=Label(name='Log', tooltip=None)
     log.value="-> GB: sigma="+str(gaussian_blur_one_pop.sigma.value)+"-> Th="+str(threshold_one_pop.threshold.value)+"-> DistMap"
     log.value=log.value+"-> Maxima: min_dist=" + str(show_seeds_one_pop.min_dist.value) + " -> Found n="+str(prop_df.nrows)+ " objects"
-    measure_one_pop.insert(4,log)
+    #measure_one_pop.insert(4,log)
+
 
     if save_log == True:
         Log_file = open(str(save_to)+'\Log_ZELDA_single_population.txt','w')
         Log_file.write(log.value)
         Log_file.close()
 
 @magicgui(label={'widget_type':'Label', 'label':"Relate Parent-to-Child and Measure"}, call_button="Relate and Measure",
@@ -234,15 +235,15 @@
     properties=measure.regionprops_table(Children_labels.data, Original_to_measure.data, properties= ['label','area', 'mean_intensity','min_intensity','max_intensity','equivalent_diameter','major_axis_length','minor_axis_length']
     )
     binary_ch=Children_labels.data>0
     corresponding_parents=Parents_labels.data*binary_ch
     viewer.add_image(corresponding_parents, scale=Parents_labels.scale, rgb=False, name='Labelled children objects by parent', opacity=0.6, rendering='mip', blending='additive', colormap='inferno')
 
     properties_CorrespondingParent=measure.regionprops_table(Children_labels.data, Parents_labels.data, properties=['max_intensity'])
-    prop={'Parent_label': properties_CorrespondingParent['max_intensity'].astype(np.float),'Area': properties['area']*np.prod(Original_to_measure.scale),
+    prop={'Parent_label': properties_CorrespondingParent['max_intensity'].astype(np.float),'Area': properties['area']*Original_to_measure.scale[-1]*Original_to_measure.scale[-2],
     'Equivalent_diameter': properties['equivalent_diameter']*Original_to_measure.scale[-1],'MFI': properties['mean_intensity'],'Min_Intensity': properties['min_intensity'],
     'Max_Intensity': properties['max_intensity'],'MajorAxis_Length': properties['major_axis_length']*Original_to_measure.scale[-1],
     'MinorAxis_Length': properties['minor_axis_length']*Original_to_measure.scale[-1]
     }
     #prop_df=pd.DataFrame(prop)
     prop_df=dt.Frame(prop) #datatable instead of pandas
     prop_df.to_csv(str(save_to_path)+'\Results_parents-children.csv')
```

### Comparing `napari-zelda-0.1.8/napari_zelda/protocols_description.txt` & `napari-zelda-0.1.9/napari_zelda/protocols_description.txt`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/napari_zelda/protocols_dict.json` & `napari-zelda-0.1.9/napari_zelda/protocols_dict.json`

 * *Files identical despite different names*

### Comparing `napari-zelda-0.1.8/napari_zelda.egg-info/PKG-INFO` & `napari-zelda-0.1.9/napari_zelda.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: napari-zelda
-Version: 0.1.8
+Version: 0.1.9
 Summary: ZELDA: a 3D Image Segmentation and Parent-Child relation plugin for microscopy image analysis in napari
 Home-page: https://github.com/RoccoDAnt/napari-zelda
 Author: Rocco D'Antuono, Giuseppina Pisignano
 Author-email: rocco.dantuono@hotmail.it
 License: BSD-3-Clause
-Download-URL: https://github.com/RoccoDAnt/napari-zelda/archive/refs/tags/v0.1.8.tar.gz
+Download-URL: https://github.com/RoccoDAnt/napari-zelda/archive/refs/tags/v0.1.9.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Framework :: napari
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -28,15 +28,16 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-zelda.svg?color=green)](https://python.org)
 [![tests](https://github.com/RoccoDAnt/napari-zelda/workflows/tests/badge.svg)](https://github.com/RoccoDAnt/napari-zelda/actions)
 [![codecov](https://codecov.io/gh/RoccoDAnt/napari-zelda/branch/master/graph/badge.svg)](https://codecov.io/gh/RoccoDAnt/napari-zelda)
 
 ## ZELDA: a 3D Image Segmentation and Parent-Child relation plugin for microscopy image analysis in napari
 #### Authors: Rocco D'Antuono, Giuseppina Pisignano
 
-###### Preprint: [https://www.biorxiv.org/content/10.1101/2021.10.24.465596v1](https://www.biorxiv.org/content/10.1101/2021.10.24.465596v1)
+###### Article: Front. Comput. Sci., 04 January 2022 | https://doi.org/10.3389/fcomp.2021.796117
+
 ###### Examples of 2D and 3D data sets: [https://doi.org/10.5281/zenodo.5651284](https://zenodo.org/record/5651284#.YYgn_WDP2Ch)
 ----------------------------------
 
 ## What you can do with ZELDA plugin for napari
 The plugin can be used to analyze 2D/3D image data sets.  
 Multidimensional images (each channel corresponding to a napari layer) can be used to:
 
@@ -74,40 +75,42 @@
 5. Import and Export Protocols (image analysis workflows) in graphical mode (share with the community!).
 
     | ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_Import_and_Export_Protocols.png) <br> **Import and Export of ZELDA Protocols** |
     ------ |
 
 ## Installation
 
-**Option A.** You can install `napari-zelda` via [pip]. For the best experience, create a conda environment and use napari!=0.4.11, using the following instructions:
-
-    conda create -y -n napari-env python==3.8  
-    conda activate napari-env  
-    pip install "napari[all]"  
-    pip install napari-zelda  
-
-
-**Option B.** Alternatively, clone the repository and install locally via [pip]:
-
-    pip install -e .
-
-**Option C.** Another option is to use the napari interface to install it (make sure napari!=0.4.11):
+**Option A.** The easiest option is to use the napari interface to install ZELDA (make sure napari!=0.4.11):
 1. Plugins / Install/Uninstall Package(s)
 
   ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Plugin_install_in_napari.png)
 
 2. Choose ZELDA
 ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Plugin_install_ZELDA_in_napari_Arrow.png)
 
 3. ZELDA is installed
 ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Plugin_installed_ZELDA_in_napari_Arrow.png)
 
 4. Launch ZELDA
 ![](https://raw.githubusercontent.com/RoccoDAnt/napari-zelda/main/docs/Clipboard_ZELDA_Launch_ZELDA.png)
 
+
+**Option B.** You can install `napari-zelda` also via [pip]. For the best experience, create a conda environment and use napari!=0.4.11, using the following instructions:
+
+    conda create -y -n napari-env python==3.8  
+    conda activate napari-env  
+    pip install "napari[all]"  
+    pip install napari-zelda  
+
+
+**Option C.** Alternatively, clone the repository and install locally via [pip]:
+
+    pip install -e .
+
+
 ## Specifications
 
 This [napari] plugin was generated with [Cookiecutter] using with [@napari]'s [cookiecutter-napari-plugin] template.
 
 The GUI has been developed using [magicgui](https://github.com/napari/magicgui) widgets, while the image analysis and processing include functions from [scikit-image](https://scikit-image.org/), [SciPy](https://scipy.org/), and [NumPy](https://numpy.org/). Results are handled with [pandas](https://pandas.pydata.org/) and [datatable](https://datatable.readthedocs.io/en/latest/). Plots are obtained with [matplotlib](https://matplotlib.org/).  
 <!--
 Don't miss the full getting started guide to set up your new package:
```

### Comparing `napari-zelda-0.1.8/napari_zelda.egg-info/SOURCES.txt` & `napari-zelda-0.1.9/napari_zelda.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 README.html
 README.md
 mkdocs.yml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
+.github/workflows/plugin_preview.yml
 .github/workflows/test_and_deploy.yml
 .napari/DESCRIPTION.html
 .napari/DESCRIPTION.md
 .napari/config.yml
 docs/2D-AF488.png
 docs/2D-AF488_MT.png
 docs/2D-AF488_parents.png
```

### Comparing `napari-zelda-0.1.8/setup.cfg` & `napari-zelda-0.1.9/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 7a65 6c64 610d   = napari-zelda.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e38  .version = 0.1.8
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e39  .version = 0.1.9
 00000030: 0d0a 6175 7468 6f72 203d 2052 6f63 636f  ..author = Rocco
 00000040: 2044 2741 6e74 756f 6e6f 2c20 4769 7573   D'Antuono, Gius
 00000050: 6570 7069 6e61 2050 6973 6967 6e61 6e6f  eppina Pisignano
 00000060: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000070: 2072 6f63 636f 2e64 616e 7475 6f6e 6f40   rocco.dantuono@
 00000080: 686f 746d 6169 6c2e 6974 0d0a 7572 6c20  hotmail.it..url 
 00000090: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
 000000a0: 2e63 6f6d 2f52 6f63 636f 4441 6e74 2f6e  .com/RoccoDAnt/n
 000000b0: 6170 6172 692d 7a65 6c64 610d 0a64 6f77  apari-zelda..dow
 000000c0: 6e6c 6f61 645f 7572 6c20 3d20 6874 7470  nload_url = http
 000000d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f52  s://github.com/R
 000000e0: 6f63 636f 4441 6e74 2f6e 6170 6172 692d  occoDAnt/napari-
 000000f0: 7a65 6c64 612f 6172 6368 6976 652f 7265  zelda/archive/re
-00000100: 6673 2f74 6167 732f 7630 2e31 2e38 2e74  fs/tags/v0.1.8.t
+00000100: 6673 2f74 6167 732f 7630 2e31 2e39 2e74  fs/tags/v0.1.9.t
 00000110: 6172 2e67 7a0d 0a6c 6963 656e 7365 203d  ar.gz..license =
 00000120: 2042 5344 2d33 2d43 6c61 7573 650d 0a64   BSD-3-Clause..d
 00000130: 6573 6372 6970 7469 6f6e 203d 205a 454c  escription = ZEL
 00000140: 4441 3a20 6120 3344 2049 6d61 6765 2053  DA: a 3D Image S
 00000150: 6567 6d65 6e74 6174 696f 6e20 616e 6420  egmentation and 
 00000160: 5061 7265 6e74 2d43 6869 6c64 2072 656c  Parent-Child rel
 00000170: 6174 696f 6e20 706c 7567 696e 2066 6f72  ation plugin for
@@ -59,16 +59,16 @@
 000003a0: 0a09 6a73 6f6e 350d 0a09 6d61 6769 6367  ..json5...magicg
 000003b0: 7569 0d0a 096d 6174 706c 6f74 6c69 623e  ui...matplotlib>
 000003c0: 3d33 2e34 2e33 0d0a 096e 6170 6172 6921  =3.4.3...napari!
 000003d0: 3d30 2e34 2e31 310d 0a09 6e61 7061 7269  =0.4.11...napari
 000003e0: 2d70 6c75 6769 6e2d 656e 6769 6e65 3e3d  -plugin-engine>=
 000003f0: 302e 312e 340d 0a09 6e75 6d70 790d 0a09  0.1.4...numpy...
 00000400: 7061 6e64 6173 0d0a 0973 6369 6b69 742d  pandas...scikit-
-00000410: 696d 6167 650d 0a09 7363 6970 790d 0a0d  image...scipy...
-00000420: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
-00000430: 706f 696e 7473 5d0d 0a6e 6170 6172 692e  points]..napari.
-00000440: 706c 7567 696e 203d 200d 0a09 6e61 7061  plugin = ...napa
-00000450: 7269 2d7a 656c 6461 203d 206e 6170 6172  ri-zelda = napar
-00000460: 695f 7a65 6c64 610d 0a0d 0a5b 6567 675f  i_zelda....[egg_
-00000470: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000480: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000490: 300d 0a0d 0a                             0....
+00000410: 696d 6167 653c 3d30 2e31 382e 330d 0a09  image<=0.18.3...
+00000420: 7363 6970 790d 0a0d 0a5b 6f70 7469 6f6e  scipy....[option
+00000430: 732e 656e 7472 795f 706f 696e 7473 5d0d  s.entry_points].
+00000440: 0a6e 6170 6172 692e 706c 7567 696e 203d  .napari.plugin =
+00000450: 200d 0a09 6e61 7061 7269 2d7a 656c 6461   ...napari-zelda
+00000460: 203d 206e 6170 6172 695f 7a65 6c64 610d   = napari_zelda.
+00000470: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000480: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000490: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `napari-zelda-0.1.8/setup.py` & `napari-zelda-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 use_scm={"write_to": "napari_zelda/_version.py"}
 
 setup(
     name='napari-zelda',
-    version='0.1.8',
+    version='0.1.9',
     author="Rocco D'Antuono, Giuseppina Pisignano",
     description="ZELDA: a 3D Image Segmentation and Parent-Child relation plugin for microscopy image analysis in napari",
-    download_url = 'https://github.com/RoccoDAnt/napari-zelda/archive/refs/tags/v0.1.8.tar.gz',
+    download_url = 'https://github.com/RoccoDAnt/napari-zelda/archive/refs/tags/v0.1.9.tar.gz',
     setup_requires=["setuptools_scm"],
     packages=find_packages(),
     include_package_data=True
     )
```

