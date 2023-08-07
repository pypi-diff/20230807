# Comparing `tmp/YeaZ-1.0.1.tar.gz` & `tmp/YeaZ-1.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YeaZ-1.0.1.tar", last modified: Wed Jul 26 13:52:50 2023, max compression
+gzip compressed data, was "YeaZ-1.0.2rc1.tar", last modified: Mon Aug  7 15:31:44 2023, max compression
```

## Comparing `YeaZ-1.0.1.tar` & `YeaZ-1.0.2rc1.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.722675 YeaZ-1.0.1/
--rw-r--r--   0 farzanehwork   (502) staff       (20)   573440 2023-07-26 13:51:44.000000 YeaZ-1.0.1/.coverage
--rw-r--r--   0 farzanehwork   (502) staff       (20)     2091 2023-07-26 13:51:44.000000 YeaZ-1.0.1/.gitignore
--rw-r--r--   0 farzanehwork   (502) staff       (20)     1074 2023-07-26 13:51:44.000000 YeaZ-1.0.1/LICENSE
--rw-r--r--   0 farzanehwork   (502) staff       (20)    16986 2023-07-26 13:52:50.722850 YeaZ-1.0.1/PKG-INFO
--rw-r--r--   0 farzanehwork   (502) staff       (20)    15602 2023-07-26 13:51:44.000000 YeaZ-1.0.1/README.md
-drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.712077 YeaZ-1.0.1/YeaZ.egg-info/
--rw-r--r--   0 farzanehwork   (502) staff       (20)    16986 2023-07-26 13:52:50.000000 YeaZ-1.0.1/YeaZ.egg-info/PKG-INFO
--rw-r--r--   0 farzanehwork   (502) staff       (20)     1188 2023-07-26 13:52:50.000000 YeaZ-1.0.1/YeaZ.egg-info/SOURCES.txt
--rw-r--r--   0 farzanehwork   (502) staff       (20)        1 2023-07-26 13:52:50.000000 YeaZ-1.0.1/YeaZ.egg-info/dependency_links.txt
--rw-r--r--   0 farzanehwork   (502) staff       (20)       43 2023-07-26 13:52:50.000000 YeaZ-1.0.1/YeaZ.egg-info/entry_points.txt
--rw-r--r--   0 farzanehwork   (502) staff       (20)      274 2023-07-26 13:52:50.000000 YeaZ-1.0.1/YeaZ.egg-info/requires.txt
--rw-r--r--   0 farzanehwork   (502) staff       (20)        5 2023-07-26 13:52:50.000000 YeaZ-1.0.1/YeaZ.egg-info/top_level.txt
-drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.714470 YeaZ-1.0.1/example_data/
--rw-r--r--   0 farzanehwork   (502) staff       (20)  1490384 2023-07-26 13:51:44.000000 YeaZ-1.0.1/example_data/2020_3_19_frame_100_cropped.tif
--rw-r--r--   0 farzanehwork   (502) staff       (20)       67 2023-07-26 13:51:44.000000 YeaZ-1.0.1/example_data/readme.md
--rw-r--r--   0 farzanehwork   (502) staff       (20)      311 2023-07-26 13:51:44.000000 YeaZ-1.0.1/pyproject.toml
--rw-r--r--   0 farzanehwork   (502) staff       (20)      253 2023-07-26 13:51:44.000000 YeaZ-1.0.1/requirements.txt
--rw-r--r--   0 farzanehwork   (502) staff       (20)     1641 2023-07-26 13:52:50.723527 YeaZ-1.0.1/setup.cfg
-drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.715845 YeaZ-1.0.1/yeaz/
--rw-r--r--   0 farzanehwork   (502) staff       (20)    76187 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/GUI_main.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)     5521 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/Launch_NN_command_line.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/__init__.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)     2354 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/__main__.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)      160 2023-07-26 13:52:50.000000 YeaZ-1.0.1/yeaz/_version.py
-drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.716702 YeaZ-1.0.1/yeaz/disk/
--rw-r--r--   0 farzanehwork   (502) staff       (20)     5495 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/disk/DialogFileBrowser.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)    17565 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/disk/Reader.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/disk/__init__.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)     1623 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/disk/image_loader.py
-drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.718222 YeaZ-1.0.1/yeaz/icons/
--rw-r--r--   0 farzanehwork   (502) staff       (20)     3988 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/HomeIcon.png
--rw-r--r--   0 farzanehwork   (502) staff       (20)      403 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/LeftArrowIcon.png
--rw-r--r--   0 farzanehwork   (502) staff       (20)      533 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/MoveArrowsIcon.png
--rw-r--r--   0 farzanehwork   (502) staff       (20)      399 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/RightArrowIcon.png
--rw-r--r--   0 farzanehwork   (502) staff       (20)      418 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/ZoomIcon.png
--rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/__init__.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)     1201 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/brush2.png
--rw-r--r--   0 farzanehwork   (502) staff       (20)      884 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/eraser.png
-drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.718778 YeaZ-1.0.1/yeaz/init/
--rw-r--r--   0 farzanehwork   (502) staff       (20)    11215 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/init/InitButtons.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)     2505 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/init/InitLayout.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/init/__init__.py
-drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.720524 YeaZ-1.0.1/yeaz/misc/
--rw-r--r--   0 farzanehwork   (502) staff       (20)     1418 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/misc/BatchRetrack.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)     1655 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/misc/ChangeOneCellValue.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)     1650 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/misc/ExchangeCellValues.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)    15475 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/misc/Extract.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)    23157 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/misc/PlotCanvas.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)     1239 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/misc/ProgressBar.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/misc/__init__.py
-drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.722483 YeaZ-1.0.1/yeaz/unet/
--rw-r--r--   0 farzanehwork   (502) staff       (20)     2991 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/LaunchBatchPrediction.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/__init__.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)     4114 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/hungarian.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)     4586 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/model_pytorch.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)     3819 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/model_tensorflow.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)     4088 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/neural_network.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)     6163 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/segment.py
--rw-r--r--   0 farzanehwork   (502) staff       (20)     1537 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/utils.py
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-08-07 15:31:44.875760 YeaZ-1.0.2rc1/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)   573440 2023-06-12 14:11:09.000000 YeaZ-1.0.2rc1/.coverage
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     2091 2023-08-07 13:35:50.000000 YeaZ-1.0.2rc1/.gitignore
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1074 2023-06-12 14:11:09.000000 YeaZ-1.0.2rc1/LICENSE
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    17683 2023-08-07 15:31:44.875924 YeaZ-1.0.2rc1/PKG-INFO
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    16296 2023-08-07 13:42:47.000000 YeaZ-1.0.2rc1/README.md
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-08-07 15:31:44.865780 YeaZ-1.0.2rc1/YeaZ.egg-info/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    17683 2023-08-07 15:31:44.000000 YeaZ-1.0.2rc1/YeaZ.egg-info/PKG-INFO
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1218 2023-08-07 15:31:44.000000 YeaZ-1.0.2rc1/YeaZ.egg-info/SOURCES.txt
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        1 2023-08-07 15:31:44.000000 YeaZ-1.0.2rc1/YeaZ.egg-info/dependency_links.txt
+-rw-r--r--   0 farzanehwork   (502) staff       (20)       43 2023-08-07 15:31:44.000000 YeaZ-1.0.2rc1/YeaZ.egg-info/entry_points.txt
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      274 2023-08-07 15:31:44.000000 YeaZ-1.0.2rc1/YeaZ.egg-info/requires.txt
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        5 2023-08-07 15:31:44.000000 YeaZ-1.0.2rc1/YeaZ.egg-info/top_level.txt
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-08-07 15:31:44.867533 YeaZ-1.0.2rc1/example_data/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)  1490384 2023-06-12 14:11:09.000000 YeaZ-1.0.2rc1/example_data/2020_3_19_frame_100_cropped.tif
+-rw-r--r--   0 farzanehwork   (502) staff       (20)       67 2023-06-12 14:11:09.000000 YeaZ-1.0.2rc1/example_data/readme.md
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      311 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/pyproject.toml
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      253 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/requirements.txt
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1641 2023-08-07 15:31:44.876509 YeaZ-1.0.2rc1/setup.cfg
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-08-07 15:31:44.868724 YeaZ-1.0.2rc1/yeaz/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    76187 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/GUI_main.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     5521 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/Launch_NN_command_line.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/__init__.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     2354 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/__main__.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      163 2023-08-07 15:31:44.000000 YeaZ-1.0.2rc1/yeaz/_version.py
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-08-07 15:31:44.869480 YeaZ-1.0.2rc1/yeaz/disk/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     5495 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/disk/DialogFileBrowser.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    17565 2023-07-26 09:10:18.000000 YeaZ-1.0.2rc1/yeaz/disk/Reader.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/disk/__init__.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1623 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/disk/image_loader.py
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-08-07 15:31:44.871354 YeaZ-1.0.2rc1/yeaz/icons/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     3988 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/icons/HomeIcon.png
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      403 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/icons/LeftArrowIcon.png
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      533 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/icons/MoveArrowsIcon.png
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      399 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/icons/RightArrowIcon.png
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      418 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/icons/ZoomIcon.png
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/icons/__init__.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1201 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/icons/brush2.png
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      884 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/icons/eraser.png
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-08-07 15:31:44.871978 YeaZ-1.0.2rc1/yeaz/init/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    11160 2023-08-07 09:25:01.000000 YeaZ-1.0.2rc1/yeaz/init/InitButtons.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     2505 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/init/InitLayout.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/init/__init__.py
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-08-07 15:31:44.873739 YeaZ-1.0.2rc1/yeaz/misc/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1418 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/misc/BatchRetrack.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1655 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/misc/ChangeOneCellValue.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1650 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/misc/ExchangeCellValues.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    15475 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/misc/Extract.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    23157 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/misc/PlotCanvas.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1239 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/misc/ProgressBar.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/misc/__init__.py
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-08-07 15:31:44.875409 YeaZ-1.0.2rc1/yeaz/unet/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     2991 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/unet/LaunchBatchPrediction.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/unet/__init__.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     4114 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/unet/hungarian.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     4586 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/unet/model_pytorch.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     3819 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/unet/model_tensorflow.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     4104 2023-08-07 10:07:56.000000 YeaZ-1.0.2rc1/yeaz/unet/neural_network.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     6163 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/unet/segment.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1537 2023-07-26 08:51:04.000000 YeaZ-1.0.2rc1/yeaz/unet/utils.py
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-08-07 15:31:44.875601 YeaZ-1.0.2rc1/yeaz/unet/weights/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-08-07 09:26:06.000000 YeaZ-1.0.2rc1/yeaz/unet/weights/__init__.py
```

### Comparing `YeaZ-1.0.1/.coverage` & `YeaZ-1.0.2rc1/.coverage`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/.gitignore` & `YeaZ-1.0.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/LICENSE` & `YeaZ-1.0.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/PKG-INFO` & `YeaZ-1.0.2rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,7 @@
-Metadata-Version: 2.1
-Name: YeaZ
-Version: 1.0.1
-Summary: Deep-learning based yeast cell segmentation
-Home-page: https://github.com/rahi-lab/YeaZ-GUI
-Author: Sahand Jamal Rahi
-Author-email: sahand.rahi@epfl.ch
-Project-URL: Rahi lab, https://www.epfl.ch/labs/lpbs/
-Keywords: live-cell imaging,cell segmentation,cell tracking,image analysis
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Utilities
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: gui
-Provides-Extra: tensorflow
-Provides-Extra: torch
-License-File: LICENSE
-
 # YeaZ
 
 This is the user manual for the graphical interface for segmenting yeast images using the YeaZ convolutional neural network. You can find the training set with the segmented training images here: https://www.quantsysbio.com/data-and-software/. 
 
 Want to try out the neural network without installing any software? Check out our online segmentation tool at https://lpbs-nn.epfl.ch/.
 
 ## Latest updates
@@ -53,55 +19,69 @@
 6. Improve the overall speed and performance of the application
 7. Add the ability to segment fission images
 8. Fix minor bugs and improve overall stability
 9. enable the option to run on GPU (windows and linux only)
 
 
 ## Installation
+You can either use pip to install YeaZ or install from the source.
 
 ### System requirements
 
 The software requires a standard computer with enough RAM to apply the neural network. 8 GB RAM is enough to predict the 700 x 500 px image provided as the test data. The RAM requirements scale linearly with the number of image pixels.
 
 It was tested on macOS Ventura (13.4.1), Windows 10 Education, and Ubuntu 20.04.4.
 
 Package dependencies: The convolutional neural network relies on Pytorch. The Hungarian algorithm is implemented in the munkres package. In addition, standard image processing and scientific computing libraries are used. 
 
 Installation time is less than 5 minutes. 
 
-### Download weight files for neural network
-
-1. Download the parameters for the neural network:<br>
-    1.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b. Put the file in the folder `yeaz/unet`.  <br>
-    1.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0. Put the file in the folder `yeaz/unet`.  <br>
-    1.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/1h_Wz2d3UY0jkGtMrhl32iEqbOQVXsmKS. Put the file in the folder `yeaz/unet`.  
 
 ### Install from PyPi
 
 1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
 2. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`. 
-3. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+3. Install PyTorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+    
     3.1. for more information visit https://pytorch.org/get-started/locally/
 4. Install YeaZ with the command `pip install yeaz`.
+5. Download weight files for neural network and put them in the yeaz/unet/weights folder which locates in yeaz installation directory.
+   
+    5.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b.
+   
+   5.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0
+   
+   5.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/1h_Wz2d3UY0jkGtMrhl32iEqbOQVXsmKS.
+   
 
 ### Install from source
 
 1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
 2. Clone this repository (`git clone https://github.com/rahi-lab/YeaZ-GUI`).
 3. In the command line, navigate to the folder where you cloned YeaZ-GUI (command `cd YeaZ-GUI`).
 4. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`.   
 5. Activate the environment using `conda activate YeaZ`. 
 6. Install with the command `pip install -e .`.
 7. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+    
     7.1. for more information visit https://pytorch.org/get-started/locally/
+8. Download weight files for neural network and put them in the yeaz/unet/weights folder which locates in yeaz installation directory.
+
+    8.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b.
+    
+    8.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0
+    
+    8.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/1h_Wz2d3UY0jkGtMrhl32iEqbOQVXsmKS.
+
 
 ## Runnig the GUI
 
-1. Open a terminal and activate the environment using `conda activate YeaZ`. 
-2. Run the program with the command `yeaz`.
+1. Open a terminal and activate the environment using `conda activate YeaZ`.
+2. Navigate to the directory where you installed YeaZ using `cd path/to/yeaz` (the easiest way is to search for yeaz folder in your files)
+3. Run the program with the command `yeaz`.
 
 ## Troubleshooting / FAQ 
 
 ### Memory error when running on GPU (cuda). Also might happen on CPU.
 
 Unlike CPU, GPU memory is very limited. If you get a memory error when running on GPU, try the following steps:
 1. Crop the images to smaller sizes. Memory usage depends on number of pixels in your images. You may try cropping your images into several smaller images or removing empty space around cells.
```

### Comparing `YeaZ-1.0.1/README.md` & `YeaZ-1.0.2rc1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+Metadata-Version: 2.1
+Name: YeaZ
+Version: 1.0.2rc1
+Summary: Deep-learning based yeast cell segmentation
+Home-page: https://github.com/rahi-lab/YeaZ-GUI
+Author: Sahand Jamal Rahi
+Author-email: sahand.rahi@epfl.ch
+Project-URL: Rahi lab, https://www.epfl.ch/labs/lpbs/
+Keywords: live-cell imaging,cell segmentation,cell tracking,image analysis
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Utilities
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: gui
+Provides-Extra: tensorflow
+Provides-Extra: torch
+License-File: LICENSE
+
 # YeaZ
 
 This is the user manual for the graphical interface for segmenting yeast images using the YeaZ convolutional neural network. You can find the training set with the segmented training images here: https://www.quantsysbio.com/data-and-software/. 
 
 Want to try out the neural network without installing any software? Check out our online segmentation tool at https://lpbs-nn.epfl.ch/.
 
 ## Latest updates
@@ -19,55 +53,69 @@
 6. Improve the overall speed and performance of the application
 7. Add the ability to segment fission images
 8. Fix minor bugs and improve overall stability
 9. enable the option to run on GPU (windows and linux only)
 
 
 ## Installation
+You can either use pip to install YeaZ or install from the source.
 
 ### System requirements
 
 The software requires a standard computer with enough RAM to apply the neural network. 8 GB RAM is enough to predict the 700 x 500 px image provided as the test data. The RAM requirements scale linearly with the number of image pixels.
 
 It was tested on macOS Ventura (13.4.1), Windows 10 Education, and Ubuntu 20.04.4.
 
 Package dependencies: The convolutional neural network relies on Pytorch. The Hungarian algorithm is implemented in the munkres package. In addition, standard image processing and scientific computing libraries are used. 
 
 Installation time is less than 5 minutes. 
 
-### Download weight files for neural network
-
-1. Download the parameters for the neural network:<br>
-    1.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b. Put the file in the folder `yeaz/unet`.  <br>
-    1.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0. Put the file in the folder `yeaz/unet`.  <br>
-    1.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/1h_Wz2d3UY0jkGtMrhl32iEqbOQVXsmKS. Put the file in the folder `yeaz/unet`.  
 
 ### Install from PyPi
 
 1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
 2. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`. 
-3. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+3. Install PyTorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+    
     3.1. for more information visit https://pytorch.org/get-started/locally/
 4. Install YeaZ with the command `pip install yeaz`.
+5. Download weight files for neural network and put them in the yeaz/unet/weights folder which locates in yeaz installation directory.
+   
+    5.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b.
+   
+   5.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0
+   
+   5.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/1h_Wz2d3UY0jkGtMrhl32iEqbOQVXsmKS.
+   
 
 ### Install from source
 
 1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
 2. Clone this repository (`git clone https://github.com/rahi-lab/YeaZ-GUI`).
 3. In the command line, navigate to the folder where you cloned YeaZ-GUI (command `cd YeaZ-GUI`).
 4. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`.   
 5. Activate the environment using `conda activate YeaZ`. 
 6. Install with the command `pip install -e .`.
 7. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+    
     7.1. for more information visit https://pytorch.org/get-started/locally/
+8. Download weight files for neural network and put them in the yeaz/unet/weights folder which locates in yeaz installation directory.
+
+    8.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b.
+    
+    8.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0
+    
+    8.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/1h_Wz2d3UY0jkGtMrhl32iEqbOQVXsmKS.
+
 
 ## Runnig the GUI
 
-1. Open a terminal and activate the environment using `conda activate YeaZ`. 
-2. Run the program with the command `yeaz`.
+1. Open a terminal and activate the environment using `conda activate YeaZ`.
+2. Navigate to the directory where you installed YeaZ using `cd path/to/yeaz` (the easiest way is to search for yeaz folder in your files)
+3. Run the program with the command `yeaz`.
 
 ## Troubleshooting / FAQ 
 
 ### Memory error when running on GPU (cuda). Also might happen on CPU.
 
 Unlike CPU, GPU memory is very limited. If you get a memory error when running on GPU, try the following steps:
 1. Crop the images to smaller sizes. Memory usage depends on number of pixels in your images. You may try cropping your images into several smaller images or removing empty space around cells.
```

### Comparing `YeaZ-1.0.1/YeaZ.egg-info/PKG-INFO` & `YeaZ-1.0.2rc1/YeaZ.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YeaZ
-Version: 1.0.1
+Version: 1.0.2rc1
 Summary: Deep-learning based yeast cell segmentation
 Home-page: https://github.com/rahi-lab/YeaZ-GUI
 Author: Sahand Jamal Rahi
 Author-email: sahand.rahi@epfl.ch
 Project-URL: Rahi lab, https://www.epfl.ch/labs/lpbs/
 Keywords: live-cell imaging,cell segmentation,cell tracking,image analysis
 Classifier: Development Status :: 4 - Beta
@@ -53,55 +53,69 @@
 6. Improve the overall speed and performance of the application
 7. Add the ability to segment fission images
 8. Fix minor bugs and improve overall stability
 9. enable the option to run on GPU (windows and linux only)
 
 
 ## Installation
+You can either use pip to install YeaZ or install from the source.
 
 ### System requirements
 
 The software requires a standard computer with enough RAM to apply the neural network. 8 GB RAM is enough to predict the 700 x 500 px image provided as the test data. The RAM requirements scale linearly with the number of image pixels.
 
 It was tested on macOS Ventura (13.4.1), Windows 10 Education, and Ubuntu 20.04.4.
 
 Package dependencies: The convolutional neural network relies on Pytorch. The Hungarian algorithm is implemented in the munkres package. In addition, standard image processing and scientific computing libraries are used. 
 
 Installation time is less than 5 minutes. 
 
-### Download weight files for neural network
-
-1. Download the parameters for the neural network:<br>
-    1.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b. Put the file in the folder `yeaz/unet`.  <br>
-    1.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0. Put the file in the folder `yeaz/unet`.  <br>
-    1.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/1h_Wz2d3UY0jkGtMrhl32iEqbOQVXsmKS. Put the file in the folder `yeaz/unet`.  
 
 ### Install from PyPi
 
 1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
 2. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`. 
-3. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+3. Install PyTorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+    
     3.1. for more information visit https://pytorch.org/get-started/locally/
 4. Install YeaZ with the command `pip install yeaz`.
+5. Download weight files for neural network and put them in the yeaz/unet/weights folder which locates in yeaz installation directory.
+   
+    5.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b.
+   
+   5.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0
+   
+   5.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/1h_Wz2d3UY0jkGtMrhl32iEqbOQVXsmKS.
+   
 
 ### Install from source
 
 1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
 2. Clone this repository (`git clone https://github.com/rahi-lab/YeaZ-GUI`).
 3. In the command line, navigate to the folder where you cloned YeaZ-GUI (command `cd YeaZ-GUI`).
 4. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`.   
 5. Activate the environment using `conda activate YeaZ`. 
 6. Install with the command `pip install -e .`.
 7. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+    
     7.1. for more information visit https://pytorch.org/get-started/locally/
+8. Download weight files for neural network and put them in the yeaz/unet/weights folder which locates in yeaz installation directory.
+
+    8.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b.
+    
+    8.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0
+    
+    8.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/1h_Wz2d3UY0jkGtMrhl32iEqbOQVXsmKS.
+
 
 ## Runnig the GUI
 
-1. Open a terminal and activate the environment using `conda activate YeaZ`. 
-2. Run the program with the command `yeaz`.
+1. Open a terminal and activate the environment using `conda activate YeaZ`.
+2. Navigate to the directory where you installed YeaZ using `cd path/to/yeaz` (the easiest way is to search for yeaz folder in your files)
+3. Run the program with the command `yeaz`.
 
 ## Troubleshooting / FAQ 
 
 ### Memory error when running on GPU (cuda). Also might happen on CPU.
 
 Unlike CPU, GPU memory is very limited. If you get a memory error when running on GPU, try the following steps:
 1. Crop the images to smaller sizes. Memory usage depends on number of pixels in your images. You may try cropping your images into several smaller images or removing empty space around cells.
```

### Comparing `YeaZ-1.0.1/YeaZ.egg-info/SOURCES.txt` & `YeaZ-1.0.2rc1/YeaZ.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,8 +44,9 @@
 yeaz/unet/LaunchBatchPrediction.py
 yeaz/unet/__init__.py
 yeaz/unet/hungarian.py
 yeaz/unet/model_pytorch.py
 yeaz/unet/model_tensorflow.py
 yeaz/unet/neural_network.py
 yeaz/unet/segment.py
-yeaz/unet/utils.py
+yeaz/unet/utils.py
+yeaz/unet/weights/__init__.py
```

### Comparing `YeaZ-1.0.1/example_data/2020_3_19_frame_100_cropped.tif` & `YeaZ-1.0.2rc1/example_data/2020_3_19_frame_100_cropped.tif`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/setup.cfg` & `YeaZ-1.0.2rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/GUI_main.py` & `YeaZ-1.0.2rc1/yeaz/GUI_main.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/Launch_NN_command_line.py` & `YeaZ-1.0.2rc1/yeaz/Launch_NN_command_line.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/__main__.py` & `YeaZ-1.0.2rc1/yeaz/__main__.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/disk/DialogFileBrowser.py` & `YeaZ-1.0.2rc1/yeaz/disk/DialogFileBrowser.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/disk/Reader.py` & `YeaZ-1.0.2rc1/yeaz/disk/Reader.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/disk/image_loader.py` & `YeaZ-1.0.2rc1/yeaz/disk/image_loader.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/icons/HomeIcon.png` & `YeaZ-1.0.2rc1/yeaz/icons/HomeIcon.png`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/icons/MoveArrowsIcon.png` & `YeaZ-1.0.2rc1/yeaz/icons/MoveArrowsIcon.png`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/icons/brush2.png` & `YeaZ-1.0.2rc1/yeaz/icons/brush2.png`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/icons/eraser.png` & `YeaZ-1.0.2rc1/yeaz/icons/eraser.png`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/init/InitButtons.py` & `YeaZ-1.0.2rc1/yeaz/init/InitButtons.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,18 @@
 from PyQt6 import QtGui
 from PyQt6.QtCore import Qt
 from PyQt6.QtGui import QKeySequence
 
 import numpy as np
 import os
 import sys
-#in case the app is frozen, the original path cannot find the icons.
-if getattr(sys, 'frozen', False):
-    path_icons = os.path.join(sys._MEIPASS, "icons/")
-    
-else:
-    path_icons = './icons/'
 
+import importlib.resources as resources
+# Access icon file
+path_icons = resources.files('yeaz.icons')
 
 def Init(parent):
     """
     configuration of all the buttons, some buttons just need to be toggled
     meaning that they need just to be clicked and the function associated 
     to the button is called and executed. Other buttons are checkable 
     meaning that until the user has not finished to use the function
@@ -70,60 +67,60 @@
     parent.button_previousframe.setMaximumWidth(150)
     parent.button_previousframe.setShortcut(Qt.Key.Key_Left)
     parent.button_previousframe.move(100,100)
         
     # ZOOM
     parent.button_zoom = QPushButton()
     parent.button_zoom.clicked.connect(parent.ZoomTlbar)
-    parent.button_zoom.setIcon(QtGui.QIcon(path_icons+'ZoomIcon.png'))
+    parent.button_zoom.setIcon(QtGui.QIcon(str(path_icons) + '/ZoomIcon.png'))
     parent.button_zoom.setMaximumWidth(30)
     parent.button_zoom.setMaximumHeight(30)
     parent.button_zoom.setStyleSheet("QPushButton:hover { background-color: blue }" )
     parent.button_zoom.setCheckable(True)
     parent.button_zoom.setShortcut("Z")
     parent.button_zoom.setToolTip("Shortcut: Z")
     parent.button_zoom.setStatusTip('Zoom (draw rectangle with right mouse button to zoom out)')
     parent.buttonlist.append(parent.button_zoom)
     
     # HOME
     parent.button_home = QPushButton()
     parent.button_home.clicked.connect(parent.HomeTlbar)
-    parent.button_home.setIcon(QtGui.QIcon(path_icons+'HomeIcon.png'))
+    parent.button_home.setIcon(QtGui.QIcon(str(path_icons) + '/HomeIcon.png'))
     parent.button_home.setMaximumWidth(30)
     parent.button_home.setMaximumHeight(30)
     parent.button_home.setStyleSheet("QPushButton:hover { background-color: blue }" )
     parent.button_home.setShortcut("H")
     parent.button_home.setToolTip("Shortcut: H")
     parent.button_home.setStatusTip('Reset zoom')
     parent.buttonlist.append(parent.button_home)
     
     # PREVIOUS SCALE (ZOOM SCALE)
     parent.button_back = QPushButton()
     parent.button_back.clicked.connect(parent.BackTlbar)
-    parent.button_back.setIcon(QtGui.QIcon(path_icons+'LeftArrowIcon.png'))
+    parent.button_back.setIcon(QtGui.QIcon(str(path_icons) +'/LeftArrowIcon.png'))
     parent.button_back.setMaximumWidth(30)
     parent.button_back.setMaximumHeight(30)
     parent.button_back.setStyleSheet("QPushButton:hover { background-color: blue }" )
     parent.button_back.setStatusTip('Go back to previous view (undo).')
     parent.buttonlist.append(parent.button_back)
     
     # NEXT SCALE (ZOOM SCALE)
     parent.button_forward = QPushButton()
     parent.button_forward.clicked.connect(parent.ForwardTlbar)
-    parent.button_forward.setIcon(QtGui.QIcon(path_icons+'RightArrowIcon.png'))
+    parent.button_forward.setIcon(QtGui.QIcon(str(path_icons) + '/RightArrowIcon.png'))
     parent.button_forward.setMaximumWidth(30)
     parent.button_forward.setMaximumHeight(30)
     parent.button_forward.setStyleSheet("QPushButton:hover { background-color: blue }")
     parent.button_forward.setStatusTip('Go to next view (redo).')
     parent.buttonlist.append(parent.button_forward)
     
     # PAN 
     parent.button_pan = QPushButton()
     parent.button_pan.clicked.connect(parent.PanTlbar)
-    parent.button_pan.setIcon(QtGui.QIcon(path_icons+'MoveArrowsIcon.png'))
+    parent.button_pan.setIcon(QtGui.QIcon(str(path_icons) + '/MoveArrowsIcon.png'))
     parent.button_pan.setMaximumWidth(30)
     parent.button_pan.setMaximumHeight(30)
     parent.button_pan.setStyleSheet("QPushButton:hover { background-color: blue }")
     parent.button_pan.setCheckable(True)
     parent.button_pan.setShortcut("P")
     parent.button_pan.setToolTip("Shortcut: P")
     parent.button_pan.setStatusTip('Pan')
```

### Comparing `YeaZ-1.0.1/yeaz/init/InitLayout.py` & `YeaZ-1.0.2rc1/yeaz/init/InitLayout.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/misc/BatchRetrack.py` & `YeaZ-1.0.2rc1/yeaz/misc/BatchRetrack.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/misc/ChangeOneCellValue.py` & `YeaZ-1.0.2rc1/yeaz/misc/ChangeOneCellValue.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/misc/ExchangeCellValues.py` & `YeaZ-1.0.2rc1/yeaz/misc/ExchangeCellValues.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/misc/Extract.py` & `YeaZ-1.0.2rc1/yeaz/misc/Extract.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/misc/PlotCanvas.py` & `YeaZ-1.0.2rc1/yeaz/misc/PlotCanvas.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/misc/ProgressBar.py` & `YeaZ-1.0.2rc1/yeaz/misc/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/unet/LaunchBatchPrediction.py` & `YeaZ-1.0.2rc1/yeaz/unet/LaunchBatchPrediction.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/unet/hungarian.py` & `YeaZ-1.0.2rc1/yeaz/unet/hungarian.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/unet/model_pytorch.py` & `YeaZ-1.0.2rc1/yeaz/unet/model_pytorch.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/unet/model_tensorflow.py` & `YeaZ-1.0.2rc1/yeaz/unet/model_tensorflow.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/unet/neural_network.py` & `YeaZ-1.0.2rc1/yeaz/unet/neural_network.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,17 @@
 # from model_tensorflow import unet
 import numpy as np
 import skimage
 from skimage import io
 import skimage.transform as trans
 import torch
 
-if getattr(sys, 'frozen', False):
-    path_weights  = os.path.join(sys._MEIPASS, 'unet/')
-    
-else:
-    path_weights = './unet/'
+import importlib.resources as resources
+# Access weight file
+path_weights = resources.files('yeaz.unet.weights')
 
 def create_directory_if_not_exists(path):
     """
     Create in the file system a new directory if it doesn't exist yet.
     Param:
         path: the path of the new directory
     """
@@ -65,19 +63,19 @@
     (nrow, ncol) = im.shape
     row_add = 16-nrow%16
     col_add = 16-ncol%16
     padded = np.pad(im, ((0, row_add), (0, col_add)))
     
     if pretrained_weights is None:
         if mic_type == 'pc':
-            pretrained_weights = path_weights + 'weights_budding_PhC_multilab_0_1'
+            pretrained_weights = str(path_weights) + '/' + 'weights_budding_PhC_multilab_0_1'
         elif mic_type == 'bf':
-            pretrained_weights = path_weights + 'weights_budding_BF_multilab_0_1'
+            pretrained_weights = str(path_weights) + '/' + 'weights_budding_BF_multilab_0_1'
         elif mic_type == 'fission':
-            pretrained_weights = path_weights + 'weights_fission_multilab_0_2'
+            pretrained_weights = str(path_weights) + '/' + 'weights_fission_multilab_0_2'
         if model_type == 'tensorflow':
             pretrained_weights = pretrained_weights + '.hdf5'
     
     if not os.path.exists(pretrained_weights):
         raise ValueError('Path does not exist')
 
     # WHOLE CELL PREDICTION
```

### Comparing `YeaZ-1.0.1/yeaz/unet/segment.py` & `YeaZ-1.0.2rc1/yeaz/unet/segment.py`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.1/yeaz/unet/utils.py` & `YeaZ-1.0.2rc1/yeaz/unet/utils.py`

 * *Files identical despite different names*

