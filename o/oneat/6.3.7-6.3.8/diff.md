# Comparing `tmp/oneat-6.3.7.tar.gz` & `tmp/oneat-6.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneat-6.3.7.tar", last modified: Mon Jul 31 12:14:15 2023, max compression
+gzip compressed data, was "oneat-6.3.8.tar", last modified: Mon Aug  7 11:00:41 2023, max compression
```

## Comparing `oneat-6.3.7.tar` & `oneat-6.3.8.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.677026 oneat-6.3.7/
--rw-r--r--   0 vkapoor    (503) staff       (20)    10244 2023-07-22 10:41:26.000000 oneat-6.3.7/.DS_Store
--rw-r--r--   0 vkapoor    (503) staff       (20)       41 2023-07-21 10:27:28.000000 oneat-6.3.7/.gitattributes
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.654576 oneat-6.3.7/.github/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.658179 oneat-6.3.7/.github/workflows/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2788 2023-07-21 10:27:28.000000 oneat-6.3.7/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 vkapoor    (503) staff       (20)      960 2023-07-22 19:12:40.000000 oneat-6.3.7/.gitignore
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.659316 oneat-6.3.7/.idea/
--rw-r--r--   0 vkapoor    (503) staff       (20)      176 2023-07-21 10:27:28.000000 oneat-6.3.7/.idea/.gitignore
--rw-r--r--   0 vkapoor    (503) staff       (20)      509 2023-07-21 10:27:28.000000 oneat-6.3.7/.idea/Yoloneat.iml
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.659511 oneat-6.3.7/.idea/inspectionProfiles/
--rw-r--r--   0 vkapoor    (503) staff       (20)      174 2023-07-21 10:27:28.000000 oneat-6.3.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      196 2023-07-21 10:27:28.000000 oneat-6.3.7/.idea/misc.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      268 2023-07-21 10:27:28.000000 oneat-6.3.7/.idea/modules.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      233 2023-07-21 10:27:28.000000 oneat-6.3.7/.idea/other.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      180 2023-07-21 10:27:28.000000 oneat-6.3.7/.idea/vcs.xml
--rw-r--r--   0 vkapoor    (503) staff       (20)      854 2023-07-21 10:27:28.000000 oneat-6.3.7/.pre-commit-config.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)      300 2023-07-22 19:11:36.000000 oneat-6.3.7/1
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.3.7/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)       96 2023-07-21 10:27:28.000000 oneat-6.3.7/MANIFEST.in
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-31 12:14:15.677155 oneat-6.3.7/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     7902 2023-07-21 10:27:28.000000 oneat-6.3.7/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.661898 oneat-6.3.7/images/
--rw-r--r--   0 vkapoor    (503) staff       (20)   190057 2023-07-21 10:27:28.000000 oneat-6.3.7/images/Xenopus_example.jpg
--rw-r--r--   0 vkapoor    (503) staff       (20)   752746 2023-07-21 10:27:28.000000 oneat-6.3.7/images/Xenopus_example.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33384 2023-07-21 10:27:28.000000 oneat-6.3.7/images/ch_0_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    34434 2023-07-21 10:27:28.000000 oneat-6.3.7/images/ch_1_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    64858 2023-07-21 10:27:28.000000 oneat-6.3.7/images/ch_2_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    79433 2023-07-21 10:27:28.000000 oneat-6.3.7/images/ch_3_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    50517 2023-07-21 10:27:28.000000 oneat-6.3.7/images/ch_4_crop.png
--rw-r--r--   0 vkapoor    (503) staff       (20)    33211 2023-07-21 10:27:28.000000 oneat-6.3.7/images/ch_5_crop.png
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.663061 oneat-6.3.7/licenses/
--rw-r--r--   0 vkapoor    (503) staff       (20)    11358 2023-07-21 10:27:28.000000 oneat-6.3.7/licenses/Apache-2
--rw-r--r--   0 vkapoor    (503) staff       (20)     1487 2023-07-21 10:27:28.000000 oneat-6.3.7/licenses/BSD-3
--rw-r--r--   0 vkapoor    (503) staff       (20)    35148 2023-07-21 10:27:28.000000 oneat-6.3.7/licenses/GPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     7653 2023-07-21 10:27:28.000000 oneat-6.3.7/licenses/LGPL-3
--rw-r--r--   0 vkapoor    (503) staff       (20)     1080 2023-07-21 10:27:28.000000 oneat-6.3.7/licenses/MIT
--rw-r--r--   0 vkapoor    (503) staff       (20)    16726 2023-07-21 10:27:28.000000 oneat-6.3.7/licenses/MPL-2
--rw-r--r--   0 vkapoor    (503) staff       (20)      255 2023-07-31 09:43:42.000000 oneat-6.3.7/pyproject.toml
--rw-r--r--   0 vkapoor    (503) staff       (20)     1790 2023-07-31 12:14:15.677889 oneat-6.3.7/setup.cfg
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.655275 oneat-6.3.7/src/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.663818 oneat-6.3.7/src/oneat/
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.668317 oneat-6.3.7/src/oneat/NEATModels/
--rw-r--r--   0 vkapoor    (503) staff       (20)    20480 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/.neat_focus.py.swp
--rw-r--r--   0 vkapoor    (503) staff       (20)      554 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/MidogConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     4799 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/Staticconfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      966 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/TrainConfig.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      556 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    11222 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/config.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3642 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/gen_anchors.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13598 2023-07-24 18:11:57.000000 oneat-6.3.7/src/oneat/NEATModels/loss.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38579 2023-07-31 08:35:36.000000 oneat-6.3.7/src/oneat/NEATModels/neat_densevollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40718 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/neat_dynamic_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    27082 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/neat_focus.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21313 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/neat_focus_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    39187 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/neat_lstm.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    15758 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/neat_microscope.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    23305 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/neat_static_resnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    38167 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/neat_vollnet.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    40628 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATModels/nets.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.670095 oneat-6.3.7/src/oneat/NEATUtils/
--rw-r--r--   0 vkapoor    (503) staff       (20)    24298 2023-07-31 12:10:07.000000 oneat-6.3.7/src/oneat/NEATUtils/HolovizNapari.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    51265 2023-07-22 19:11:34.000000 oneat-6.3.7/src/oneat/NEATUtils/MovieCreator.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6795 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATUtils/NMS.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5100 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATUtils/TrainDataMaker.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      590 2023-07-29 13:18:06.000000 oneat-6.3.7/src/oneat/NEATUtils/VisualizeDetections.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2723 2023-07-31 09:43:48.000000 oneat-6.3.7/src/oneat/NEATUtils/Zmapgen.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      228 2023-07-29 13:19:04.000000 oneat-6.3.7/src/oneat/NEATUtils/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.671130 oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/
--rw-r--r--   0 vkapoor    (503) staff       (20)     5400 2023-07-29 13:48:14.000000 oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5167 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25380 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    21393 2023-07-31 11:59:21.000000 oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      296 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.672417 oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/_qt/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2883 2023-07-31 09:20:05.000000 oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2007 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      241 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     2647 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6544 2023-07-31 12:13:47.000000 oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6630 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    25029 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/NEATUtils/plotters.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    70833 2023-07-31 08:33:33.000000 oneat-6.3.7/src/oneat/NEATUtils/utils.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     5002 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/__init__.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.673000 oneat-6.3.7/src/oneat/_tests/
--rw-r--r--   0 vkapoor    (503) staff       (20)        0 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/_tests/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1824 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/_tests/test_nets.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1044 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/_tests/utils.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.676867 oneat-6.3.7/src/oneat/_tests/variables/
--rw-r--r--   0 vkapoor    (503) staff       (20)  5142983 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/_tests/variables/variables.data-00000-of-00001
--rw-r--r--   0 vkapoor    (503) staff       (20)     4787 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/_tests/variables/variables.index
--rw-r--r--   0 vkapoor    (503) staff       (20)      160 2023-07-31 12:14:15.000000 oneat-6.3.7/src/oneat/_version.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       45 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/caped.yaml
--rw-r--r--   0 vkapoor    (503) staff       (20)     5739 2023-07-21 10:27:28.000000 oneat-6.3.7/src/oneat/pretrained.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-31 12:14:15.664904 oneat-6.3.7/src/oneat.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     9169 2023-07-31 12:14:15.000000 oneat-6.3.7/src/oneat.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2632 2023-07-31 12:14:15.000000 oneat-6.3.7/src/oneat.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-31 12:14:15.000000 oneat-6.3.7/src/oneat.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       42 2023-07-31 12:14:15.000000 oneat-6.3.7/src/oneat.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      207 2023-07-31 12:14:15.000000 oneat-6.3.7/src/oneat.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        6 2023-07-31 12:14:15.000000 oneat-6.3.7/src/oneat.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      601 2023-07-21 10:27:28.000000 oneat-6.3.7/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:41.302550 oneat-6.3.8/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    10244 2023-08-06 18:36:23.000000 oneat-6.3.8/.DS_Store
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       41 2023-08-06 18:36:23.000000 oneat-6.3.8/.gitattributes
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:29.678290 oneat-6.3.8/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:37.484597 oneat-6.3.8/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2788 2023-08-06 18:36:23.000000 oneat-6.3.8/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      960 2023-08-06 18:36:23.000000 oneat-6.3.8/.gitignore
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:37.705714 oneat-6.3.8/.idea/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      176 2023-08-06 18:36:23.000000 oneat-6.3.8/.idea/.gitignore
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      509 2023-08-06 18:36:23.000000 oneat-6.3.8/.idea/Yoloneat.iml
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:37.748870 oneat-6.3.8/.idea/inspectionProfiles/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      174 2023-08-06 18:36:23.000000 oneat-6.3.8/.idea/inspectionProfiles/profiles_settings.xml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      196 2023-08-06 18:36:23.000000 oneat-6.3.8/.idea/misc.xml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      268 2023-08-06 18:36:23.000000 oneat-6.3.8/.idea/modules.xml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      233 2023-08-06 18:36:23.000000 oneat-6.3.8/.idea/other.xml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      180 2023-08-06 18:36:23.000000 oneat-6.3.8/.idea/vcs.xml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      854 2023-08-06 18:36:23.000000 oneat-6.3.8/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      300 2023-08-06 18:36:23.000000 oneat-6.3.8/1
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-08-06 18:36:23.000000 oneat-6.3.8/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2023-08-06 18:36:23.000000 oneat-6.3.8/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     9169 2023-08-07 11:00:41.304549 oneat-6.3.8/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     7902 2023-08-06 18:36:23.000000 oneat-6.3.8/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:38.063609 oneat-6.3.8/images/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   190057 2023-08-06 18:36:23.000000 oneat-6.3.8/images/Xenopus_example.jpg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   752746 2023-08-06 18:36:23.000000 oneat-6.3.8/images/Xenopus_example.png
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    33384 2023-08-06 18:36:23.000000 oneat-6.3.8/images/ch_0_crop.png
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    34434 2023-08-06 18:36:23.000000 oneat-6.3.8/images/ch_1_crop.png
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    64858 2023-08-06 18:36:23.000000 oneat-6.3.8/images/ch_2_crop.png
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    79433 2023-08-06 18:36:23.000000 oneat-6.3.8/images/ch_3_crop.png
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    50517 2023-08-06 18:36:23.000000 oneat-6.3.8/images/ch_4_crop.png
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    33211 2023-08-06 18:36:23.000000 oneat-6.3.8/images/ch_5_crop.png
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:38.286439 oneat-6.3.8/licenses/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11358 2023-08-06 18:36:23.000000 oneat-6.3.8/licenses/Apache-2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2023-08-06 18:36:23.000000 oneat-6.3.8/licenses/BSD-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    35148 2023-08-06 18:36:23.000000 oneat-6.3.8/licenses/GPL-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     7653 2023-08-06 18:36:23.000000 oneat-6.3.8/licenses/LGPL-3
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1080 2023-08-06 18:36:23.000000 oneat-6.3.8/licenses/MIT
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16726 2023-08-06 18:36:23.000000 oneat-6.3.8/licenses/MPL-2
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      255 2023-08-06 18:36:23.000000 oneat-6.3.8/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1790 2023-08-07 11:00:41.317691 oneat-6.3.8/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:30.568974 oneat-6.3.8/src/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:38.443205 oneat-6.3.8/src/oneat/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:39.610318 oneat-6.3.8/src/oneat/NEATModels/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    20480 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/.neat_focus.py.swp
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      554 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/MidogConfig.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4799 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/Staticconfig.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      966 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/TrainConfig.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      556 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11222 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/config.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3642 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/gen_anchors.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13598 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/loss.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    38579 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/neat_densevollnet.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    40718 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/neat_dynamic_resnet.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    27082 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/neat_focus.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    21313 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/neat_focus_microscope.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    39187 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/neat_lstm.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    15758 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/neat_microscope.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    23305 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/neat_static_resnet.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    38167 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/neat_vollnet.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    40628 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATModels/nets.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:40.101414 oneat-6.3.8/src/oneat/NEATUtils/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    24298 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/HolovizNapari.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    51232 2023-08-07 10:59:21.000000 oneat-6.3.8/src/oneat/NEATUtils/MovieCreator.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6795 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/NMS.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     5100 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/TrainDataMaker.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      590 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/VisualizeDetections.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2723 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/Zmapgen.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      228 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/__init__.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:40.435458 oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     5400 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     5167 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    25380 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    21393 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      296 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/__init__.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:40.893627 oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/_qt/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2883 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2007 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      241 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/_qt/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2647 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6544 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6630 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    25029 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/plotters.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    70833 2023-08-06 18:36:23.000000 oneat-6.3.8/src/oneat/NEATUtils/utils.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     5002 2023-08-06 18:36:24.000000 oneat-6.3.8/src/oneat/__init__.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:41.064195 oneat-6.3.8/src/oneat/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-06 18:36:24.000000 oneat-6.3.8/src/oneat/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1824 2023-08-06 18:36:24.000000 oneat-6.3.8/src/oneat/_tests/test_nets.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1044 2023-08-06 18:36:24.000000 oneat-6.3.8/src/oneat/_tests/utils.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:41.250654 oneat-6.3.8/src/oneat/_tests/variables/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)  5142983 2023-08-06 18:36:24.000000 oneat-6.3.8/src/oneat/_tests/variables/variables.data-00000-of-00001
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4787 2023-08-06 18:36:24.000000 oneat-6.3.8/src/oneat/_tests/variables/variables.index
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-08-07 11:00:26.000000 oneat-6.3.8/src/oneat/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       45 2023-08-06 18:36:24.000000 oneat-6.3.8/src/oneat/caped.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     5739 2023-08-06 18:36:24.000000 oneat-6.3.8/src/oneat/pretrained.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-08-07 11:00:38.683284 oneat-6.3.8/src/oneat.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     9169 2023-08-07 11:00:26.000000 oneat-6.3.8/src/oneat.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2632 2023-08-07 11:00:29.000000 oneat-6.3.8/src/oneat.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-08-07 11:00:26.000000 oneat-6.3.8/src/oneat.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       42 2023-08-07 11:00:26.000000 oneat-6.3.8/src/oneat.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      207 2023-08-07 11:00:26.000000 oneat-6.3.8/src/oneat.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        6 2023-08-07 11:00:26.000000 oneat-6.3.8/src/oneat.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      601 2023-08-06 18:36:24.000000 oneat-6.3.8/tox.ini
```

### Comparing `oneat-6.3.7/.DS_Store` & `oneat-6.3.8/.DS_Store`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/.github/workflows/test_and_deploy.yml` & `oneat-6.3.8/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/.gitignore` & `oneat-6.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/.pre-commit-config.yaml` & `oneat-6.3.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/LICENSE` & `oneat-6.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/PKG-INFO` & `oneat-6.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.3.7
+Version: 6.3.8
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.3.7/README.md` & `oneat-6.3.8/README.md`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/images/Xenopus_example.jpg` & `oneat-6.3.8/images/Xenopus_example.jpg`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/images/Xenopus_example.png` & `oneat-6.3.8/images/Xenopus_example.png`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/images/ch_0_crop.png` & `oneat-6.3.8/images/ch_0_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/images/ch_1_crop.png` & `oneat-6.3.8/images/ch_1_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/images/ch_2_crop.png` & `oneat-6.3.8/images/ch_2_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/images/ch_3_crop.png` & `oneat-6.3.8/images/ch_3_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/images/ch_4_crop.png` & `oneat-6.3.8/images/ch_4_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/images/ch_5_crop.png` & `oneat-6.3.8/images/ch_5_crop.png`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/licenses/Apache-2` & `oneat-6.3.8/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/licenses/BSD-3` & `oneat-6.3.8/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/licenses/GPL-3` & `oneat-6.3.8/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/licenses/LGPL-3` & `oneat-6.3.8/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/licenses/MIT` & `oneat-6.3.8/licenses/MIT`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/licenses/MPL-2` & `oneat-6.3.8/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/setup.cfg` & `oneat-6.3.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/.neat_focus.py.swp` & `oneat-6.3.8/src/oneat/NEATModels/.neat_focus.py.swp`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/MidogConfig.py` & `oneat-6.3.8/src/oneat/NEATModels/MidogConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/Staticconfig.py` & `oneat-6.3.8/src/oneat/NEATModels/Staticconfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/TrainConfig.py` & `oneat-6.3.8/src/oneat/NEATModels/TrainConfig.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/__init__.py` & `oneat-6.3.8/src/oneat/NEATModels/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/config.py` & `oneat-6.3.8/src/oneat/NEATModels/config.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/gen_anchors.py` & `oneat-6.3.8/src/oneat/NEATModels/gen_anchors.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/loss.py` & `oneat-6.3.8/src/oneat/NEATModels/loss.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/neat_densevollnet.py` & `oneat-6.3.8/src/oneat/NEATModels/neat_densevollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/neat_dynamic_resnet.py` & `oneat-6.3.8/src/oneat/NEATModels/neat_dynamic_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/neat_focus.py` & `oneat-6.3.8/src/oneat/NEATModels/neat_focus.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/neat_focus_microscope.py` & `oneat-6.3.8/src/oneat/NEATModels/neat_focus_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/neat_lstm.py` & `oneat-6.3.8/src/oneat/NEATModels/neat_lstm.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/neat_microscope.py` & `oneat-6.3.8/src/oneat/NEATModels/neat_microscope.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/neat_static_resnet.py` & `oneat-6.3.8/src/oneat/NEATModels/neat_static_resnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/neat_vollnet.py` & `oneat-6.3.8/src/oneat/NEATModels/neat_vollnet.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATModels/nets.py` & `oneat-6.3.8/src/oneat/NEATModels/nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/HolovizNapari.py` & `oneat-6.3.8/src/oneat/NEATUtils/HolovizNapari.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/MovieCreator.py` & `oneat-6.3.8/src/oneat/NEATUtils/MovieCreator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1246,16 +1246,15 @@
         except ValueError:
             pass
     print(dataarr.shape, labelarr.shape)
     traindata, validdata, trainlabel, validlabel = train_test_split(
         dataarr,
         labelarr,
         train_size=train_size,
-        test_size=1 - train_size,
-        shuffle=True,
+        shuffle=False,
     )
     save_full_training_data(save_dir, save_name, traindata, trainlabel, axes)
     save_full_training_data(
         save_dir, save_name_val, validdata, validlabel, axes
     )
```

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/NMS.py` & `oneat-6.3.8/src/oneat/NEATUtils/NMS.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/TrainDataMaker.py` & `oneat-6.3.8/src/oneat/NEATUtils/TrainDataMaker.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/VisualizeDetections.py` & `oneat-6.3.8/src/oneat/NEATUtils/VisualizeDetections.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/Zmapgen.py` & `oneat-6.3.8/src/oneat/NEATUtils/Zmapgen.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py` & `oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/OneatScoreKeeper.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py` & `oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/OneatSimpleVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py` & `oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/OneatVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py` & `oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/OneatVolumeVisualization.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py` & `oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/_qt/OneatFrameWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py` & `oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/_qt/OneatVisWidget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py` & `oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/_qt/oneat_visualize_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py` & `oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/_qt/oneat_volume_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py` & `oneat-6.3.8/src/oneat/NEATUtils/oneat_animation/_qt/oneat_widget.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/plotters.py` & `oneat-6.3.8/src/oneat/NEATUtils/plotters.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/NEATUtils/utils.py` & `oneat-6.3.8/src/oneat/NEATUtils/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/__init__.py` & `oneat-6.3.8/src/oneat/__init__.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/_tests/test_nets.py` & `oneat-6.3.8/src/oneat/_tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/_tests/utils.py` & `oneat-6.3.8/src/oneat/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/_tests/variables/variables.data-00000-of-00001` & `oneat-6.3.8/src/oneat/_tests/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/_tests/variables/variables.index` & `oneat-6.3.8/src/oneat/_tests/variables/variables.index`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat/pretrained.py` & `oneat-6.3.8/src/oneat/pretrained.py`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/src/oneat.egg-info/PKG-INFO` & `oneat-6.3.8/src/oneat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oneat
-Version: 6.3.7
+Version: 6.3.8
 Summary: Action classification for TZYX/TYX shaped images, Static classification for TYX/YX shaped images
 Home-page: https://github.com/Kapoorlabs-CAPED/oneat
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/oneat/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/oneat#README.md
```

### Comparing `oneat-6.3.7/src/oneat.egg-info/SOURCES.txt` & `oneat-6.3.8/src/oneat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oneat-6.3.7/tox.ini` & `oneat-6.3.8/tox.ini`

 * *Files identical despite different names*

