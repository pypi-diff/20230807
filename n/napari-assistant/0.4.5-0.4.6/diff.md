# Comparing `tmp/napari-assistant-0.4.5.tar.gz` & `tmp/napari-assistant-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-assistant-0.4.5.tar", last modified: Thu Apr  6 14:33:00 2023, max compression
+gzip compressed data, was "napari-assistant-0.4.6.tar", last modified: Mon Aug  7 07:41:57 2023, max compression
```

## Comparing `napari-assistant-0.4.5.tar` & `napari-assistant-0.4.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 14:33:00.852099 napari-assistant-0.4.5/
--rw-rw-rw-   0        0        0     1742 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/LICENSE
--rw-rw-rw-   0        0        0      137 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     7671 2023-04-06 14:33:00.852099 napari-assistant-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     6474 2022-11-19 11:10:40.000000 napari-assistant-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 14:33:00.744852 napari-assistant-0.4.5/napari_assistant/
--rw-rw-rw-   0        0        0      111 2023-04-06 14:32:20.000000 napari-assistant-0.4.5/napari_assistant/__init__.py
--rw-rw-rw-   0        0        0      468 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/__main__.py
--rw-rw-rw-   0        0        0    22183 2022-12-24 20:45:28.000000 napari-assistant-0.4.5/napari_assistant/_categories.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:33:00.788374 napari-assistant-0.4.5/napari_assistant/_gui/
--rw-rw-rw-   0        0        0    23355 2023-04-06 14:30:09.000000 napari-assistant-0.4.5/napari_assistant/_gui/_Assistant.py
--rw-rw-rw-   0        0        0       33 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/__init__.py
--rw-rw-rw-   0        0        0     2438 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/_button_grid.py
--rw-rw-rw-   0        0        0    23415 2022-12-24 21:03:03.000000 napari-assistant-0.4.5/napari_assistant/_gui/_category_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:33:00.851472 napari-assistant-0.4.5/napari_assistant/_gui/icons/
--rw-rw-rw-   0        0        0     1711 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/any_image.png
--rw-rw-rw-   0        0        0    13580 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/binarize.png
--rw-rw-rw-   0        0        0      648 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/binary_image.png
--rw-rw-rw-   0        0        0    15988 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/combine.png
--rw-rw-rw-   0        0        0    14661 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/combine_labels.png
--rw-rw-rw-   0        0        0    15222 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/compare_label_images.png
--rw-rw-rw-   0        0        0    19190 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/filter.png
--rw-rw-rw-   0        0        0     7331 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/generate_code....png
--rw-rw-rw-   0        0        0     2233 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/intensity_image.png
--rw-rw-rw-   0        0        0     5251 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/intensity_image_filtered.png
--rw-rw-rw-   0        0        0     3210 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/intensity_image_with_background.png
--rw-rw-rw-   0        0        0     6725 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/intensity_image_with_noise.png
--rw-rw-rw-   0        0        0    13418 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/label.png
--rw-rw-rw-   0        0        0    14881 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/label_filters.png
--rw-rw-rw-   0        0        0      719 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/label_image.png
--rw-rw-rw-   0        0        0      627 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/label_image_processed.png
--rw-rw-rw-   0        0        0    15193 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/label_neighbor_filters.png
--rw-rw-rw-   0        0        0     1725 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/map.png
--rw-rw-rw-   0        0        0    16008 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/measure_labeled_image.png
--rw-rw-rw-   0        0        0    12364 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/measure_labels.png
--rw-rw-rw-   0        0        0    11105 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/measurement.png
--rw-rw-rw-   0        0        0    13066 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/mesh.png
--rw-rw-rw-   0        0        0      887 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/mesh_image.png
--rw-rw-rw-   0        0        0      735 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/parametric_image.png
--rw-rw-rw-   0        0        0    11460 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/process_labels.png
--rw-rw-rw-   0        0        0     9818 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/projection.png
--rw-rw-rw-   0        0        0    10427 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/redo.png
--rw-rw-rw-   0        0        0    15565 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/remove_background.png
--rw-rw-rw-   0        0        0    25733 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/remove_noise.png
--rw-rw-rw-   0        0        0     9839 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/save_and_load_workflows.png
--rw-rw-rw-   0        0        0    17065 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/search_biii.png
--rw-rw-rw-   0        0        0    12626 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/search_image.sc.png
--rw-rw-rw-   0        0        0     9935 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/search_napari_hub.png
--rw-rw-rw-   0        0        0    10498 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/transform.png
--rw-rw-rw-   0        0        0    10674 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_gui/icons/undo.png
--rw-rw-rw-   0        0        0     1246 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_napari_plugin.py
--rw-rw-rw-   0        0        0     3469 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_undo_redo.py
--rw-rw-rw-   0        0        0      399 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_viewer.py
--rw-rw-rw-   0        0        0    13862 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/napari_assistant/_workflow_io_utility.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:33:00.764375 napari-assistant-0.4.5/napari_assistant.egg-info/
--rw-rw-rw-   0        0        0     7671 2023-04-06 14:33:00.000000 napari-assistant-0.4.5/napari_assistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2295 2023-04-06 14:33:00.000000 napari-assistant-0.4.5/napari_assistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 14:33:00.000000 napari-assistant-0.4.5/napari_assistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2023-04-06 14:33:00.000000 napari-assistant-0.4.5/napari_assistant.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      163 2023-04-06 14:33:00.000000 napari-assistant-0.4.5/napari_assistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-04-06 14:33:00.000000 napari-assistant-0.4.5/napari_assistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1552 2023-04-06 14:33:00.852099 napari-assistant-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0       89 2022-11-08 17:22:49.000000 napari-assistant-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:41:57.003740 napari-assistant-0.4.6/
+-rw-rw-rw-   0        0        0     1742 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0      137 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     7671 2023-08-07 07:41:57.003740 napari-assistant-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6474 2022-11-19 11:10:40.000000 napari-assistant-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 07:41:56.925297 napari-assistant-0.4.6/napari_assistant/
+-rw-rw-rw-   0        0        0      111 2023-08-07 07:40:19.000000 napari-assistant-0.4.6/napari_assistant/__init__.py
+-rw-rw-rw-   0        0        0      468 2023-06-07 17:51:28.000000 napari-assistant-0.4.6/napari_assistant/__main__.py
+-rw-rw-rw-   0        0        0    22183 2022-12-24 20:45:28.000000 napari-assistant-0.4.6/napari_assistant/_categories.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:41:56.961656 napari-assistant-0.4.6/napari_assistant/_gui/
+-rw-rw-rw-   0        0        0    23355 2023-04-06 14:30:09.000000 napari-assistant-0.4.6/napari_assistant/_gui/_Assistant.py
+-rw-rw-rw-   0        0        0       33 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/__init__.py
+-rw-rw-rw-   0        0        0     2412 2023-08-07 07:40:00.000000 napari-assistant-0.4.6/napari_assistant/_gui/_button_grid.py
+-rw-rw-rw-   0        0        0    23415 2022-12-24 21:03:03.000000 napari-assistant-0.4.6/napari_assistant/_gui/_category_widget.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:41:57.001736 napari-assistant-0.4.6/napari_assistant/_gui/icons/
+-rw-rw-rw-   0        0        0     1711 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/any_image.png
+-rw-rw-rw-   0        0        0    13580 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/binarize.png
+-rw-rw-rw-   0        0        0      648 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/binary_image.png
+-rw-rw-rw-   0        0        0    15988 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/combine.png
+-rw-rw-rw-   0        0        0    14661 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/combine_labels.png
+-rw-rw-rw-   0        0        0    15222 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/compare_label_images.png
+-rw-rw-rw-   0        0        0    19190 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/filter.png
+-rw-rw-rw-   0        0        0     7331 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/generate_code....png
+-rw-rw-rw-   0        0        0     2233 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/intensity_image.png
+-rw-rw-rw-   0        0        0     5251 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/intensity_image_filtered.png
+-rw-rw-rw-   0        0        0     3210 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/intensity_image_with_background.png
+-rw-rw-rw-   0        0        0     6725 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/intensity_image_with_noise.png
+-rw-rw-rw-   0        0        0    13418 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/label.png
+-rw-rw-rw-   0        0        0    14881 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/label_filters.png
+-rw-rw-rw-   0        0        0      719 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/label_image.png
+-rw-rw-rw-   0        0        0      627 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/label_image_processed.png
+-rw-rw-rw-   0        0        0    15193 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/label_neighbor_filters.png
+-rw-rw-rw-   0        0        0     1725 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/map.png
+-rw-rw-rw-   0        0        0    16008 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/measure_labeled_image.png
+-rw-rw-rw-   0        0        0    12364 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/measure_labels.png
+-rw-rw-rw-   0        0        0    11105 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/measurement.png
+-rw-rw-rw-   0        0        0    13066 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/mesh.png
+-rw-rw-rw-   0        0        0      887 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/mesh_image.png
+-rw-rw-rw-   0        0        0      735 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/parametric_image.png
+-rw-rw-rw-   0        0        0    11460 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/process_labels.png
+-rw-rw-rw-   0        0        0     9818 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/projection.png
+-rw-rw-rw-   0        0        0    10427 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/redo.png
+-rw-rw-rw-   0        0        0    15565 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/remove_background.png
+-rw-rw-rw-   0        0        0    25733 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/remove_noise.png
+-rw-rw-rw-   0        0        0     9839 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/save_and_load_workflows.png
+-rw-rw-rw-   0        0        0    17065 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/search_biii.png
+-rw-rw-rw-   0        0        0    12626 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/search_image.sc.png
+-rw-rw-rw-   0        0        0     9935 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/search_napari_hub.png
+-rw-rw-rw-   0        0        0    10498 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/transform.png
+-rw-rw-rw-   0        0        0    10674 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_gui/icons/undo.png
+-rw-rw-rw-   0        0        0     1246 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_napari_plugin.py
+-rw-rw-rw-   0        0        0     3469 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_undo_redo.py
+-rw-rw-rw-   0        0        0      399 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_viewer.py
+-rw-rw-rw-   0        0        0    13862 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/napari_assistant/_workflow_io_utility.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:41:56.957644 napari-assistant-0.4.6/napari_assistant.egg-info/
+-rw-rw-rw-   0        0        0     7671 2023-08-07 07:41:56.000000 napari-assistant-0.4.6/napari_assistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2295 2023-08-07 07:41:56.000000 napari-assistant-0.4.6/napari_assistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 07:41:56.000000 napari-assistant-0.4.6/napari_assistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-08-07 07:41:56.000000 napari-assistant-0.4.6/napari_assistant.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      163 2023-08-07 07:41:56.000000 napari-assistant-0.4.6/napari_assistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-08-07 07:41:56.000000 napari-assistant-0.4.6/napari_assistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1552 2023-08-07 07:41:57.005746 napari-assistant-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0       89 2022-11-08 17:22:49.000000 napari-assistant-0.4.6/setup.py
```

### Comparing `napari-assistant-0.4.5/LICENSE` & `napari-assistant-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/PKG-INFO` & `napari-assistant-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-assistant
-Version: 0.4.5
+Version: 0.4.6
 Summary: A pocket calculator like interface to image processing in napari
 Home-page: https://github.com/haesleinhuepf/napari-assistant/
 Author: Robert Haase, Ryan Savill
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/napari-assistant/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/napari-assistant/
```

### Comparing `napari-assistant-0.4.5/README.md` & `napari-assistant-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_categories.py` & `napari-assistant-0.4.6/napari_assistant/_categories.py`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/_Assistant.py` & `napari-assistant-0.4.6/napari_assistant/_gui/_Assistant.py`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/_button_grid.py` & `napari-assistant-0.4.6/napari_assistant/_gui/_button_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from pyrsistent import b
 from qtpy.QtCore import QSize
 from qtpy.QtGui import QIcon, QColor, QBrush
 from qtpy.QtWidgets import QListWidget, QListWidgetItem
 from pathlib import Path
 
 ICON_ROOT = Path(__file__).parent / "icons"
 STYLES = r"""
```

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/_category_widget.py` & `napari-assistant-0.4.6/napari_assistant/_gui/_category_widget.py`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/any_image.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/any_image.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/binarize.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/binarize.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/binary_image.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/binary_image.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/combine.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/combine.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/combine_labels.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/combine_labels.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/compare_label_images.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/compare_label_images.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/filter.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/filter.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/generate_code....png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/generate_code....png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/intensity_image.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/intensity_image.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/intensity_image_filtered.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/intensity_image_filtered.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/intensity_image_with_background.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/intensity_image_with_background.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/intensity_image_with_noise.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/intensity_image_with_noise.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/label.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/label.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/label_filters.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/label_filters.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/label_image.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/label_image.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/label_image_processed.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/label_image_processed.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/label_neighbor_filters.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/label_neighbor_filters.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/map.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/map.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/measure_labeled_image.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/measure_labeled_image.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/measure_labels.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/measure_labels.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/measurement.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/measurement.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/mesh.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/mesh.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/mesh_image.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/mesh_image.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/parametric_image.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/parametric_image.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/process_labels.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/process_labels.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/projection.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/projection.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/redo.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/redo.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/remove_background.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/remove_background.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/remove_noise.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/remove_noise.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/save_and_load_workflows.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/save_and_load_workflows.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/search_biii.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/search_biii.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/search_image.sc.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/search_image.sc.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/search_napari_hub.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/search_napari_hub.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/transform.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/transform.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_gui/icons/undo.png` & `napari-assistant-0.4.6/napari_assistant/_gui/icons/undo.png`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_napari_plugin.py` & `napari-assistant-0.4.6/napari_assistant/_napari_plugin.py`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_undo_redo.py` & `napari-assistant-0.4.6/napari_assistant/_undo_redo.py`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant/_workflow_io_utility.py` & `napari-assistant-0.4.6/napari_assistant/_workflow_io_utility.py`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/napari_assistant.egg-info/PKG-INFO` & `napari-assistant-0.4.6/napari_assistant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-assistant
-Version: 0.4.5
+Version: 0.4.6
 Summary: A pocket calculator like interface to image processing in napari
 Home-page: https://github.com/haesleinhuepf/napari-assistant/
 Author: Robert Haase, Ryan Savill
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/napari-assistant/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/napari-assistant/
```

### Comparing `napari-assistant-0.4.5/napari_assistant.egg-info/SOURCES.txt` & `napari-assistant-0.4.6/napari_assistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-assistant-0.4.5/setup.cfg` & `napari-assistant-0.4.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 6173 7369 7374   = napari-assist
 00000020: 616e 740d 0a76 6572 7369 6f6e 203d 2030  ant..version = 0
-00000030: 2e34 2e35 0d0a 6175 7468 6f72 203d 2052  .4.5..author = R
+00000030: 2e34 2e36 0d0a 6175 7468 6f72 203d 2052  .4.6..author = R
 00000040: 6f62 6572 7420 4861 6173 652c 2052 7961  obert Haase, Rya
 00000050: 6e20 5361 7669 6c6c 0d0a 6175 7468 6f72  n Savill..author
 00000060: 5f65 6d61 696c 203d 2072 6f62 6572 742e  _email = robert.
 00000070: 6861 6173 6540 7475 2d64 7265 7364 656e  haase@tu-dresden
 00000080: 2e64 650d 0a64 6573 6372 6970 7469 6f6e  .de..description
 00000090: 203d 2041 2070 6f63 6b65 7420 6361 6c63   = A pocket calc
 000000a0: 756c 6174 6f72 206c 696b 6520 696e 7465  ulator like inte
```

