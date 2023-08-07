# Comparing `tmp/pyppbox-3.1b2.tar.gz` & `tmp/pyppbox-3.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppbox-3.1b2.tar", last modified: Wed Jul 26 21:54:02 2023, max compression
+gzip compressed data, was "pyppbox-3.1b3.tar", last modified: Mon Aug  7 12:09:13 2023, max compression
```

## Comparing `pyppbox-3.1b2.tar` & `pyppbox-3.1b3.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.751511 pyppbox-3.1b2/
--rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-26 21:53:46.000000 pyppbox-3.1b2/GETSTARTED.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 21:53:46.000000 pyppbox-3.1b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-26 21:53:46.000000 pyppbox-3.1b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-26 21:54:02.751511 pyppbox-3.1b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-26 21:53:46.000000 pyppbox-3.1b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-07-26 21:53:46.000000 pyppbox-3.1b2/RELEASENOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.735511 pyppbox-3.1b2/pyppbox/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.735511 pyppbox-3.1b2/pyppbox/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.735511 pyppbox-3.1b2/pyppbox/config/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/cfg/cfg.7z
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/cfg/detectors.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/cfg/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/cfg/reiders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/cfg/trackers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/configtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    65085 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/myconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.735511 pyppbox-3.1b2/pyppbox/config/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/strings/strings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/unifiedstrings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.727511 pyppbox-3.1b2/pyppbox/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.739511 pyppbox-3.1b2/pyppbox/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/data/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.739511 pyppbox-3.1b2/pyppbox/data/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/data/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.739511 pyppbox-3.1b2/pyppbox/data/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/data/modules/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.739511 pyppbox-3.1b2/pyppbox/data/res/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/data/res/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/data/res/idmap.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.739511 pyppbox-3.1b2/pyppbox/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   833181 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/assets/TReID.png
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/assets/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    33692 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/assets/settings.ico
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/guidemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/guihub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/guitools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/gui/tmp/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/tmp/input.tmp
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/tmp/ui.tmp
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_deepsort.py
--rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_facenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_gt.py
--rw-r--r--   0 runner    (1001) docker     (123)    23388 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_torchreid.py
--rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_yolocls.py
--rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_yoloult.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/modules/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/modules/detectors/yolocls/
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/detectors/yolocls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/modules/detectors/yoloult/
--rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/detectors/yoloult/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/modules/reiders/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/modules/reiders/facenet/
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/facenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.747511 pyppbox-3.1b2/pyppbox/modules/reiders/facenet/origin/
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31858 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/facenet/origin/detect_face.py
--rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/facenet/origin/facenet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.747511 pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/model_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/model_dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.747511 pyppbox-3.1b2/pyppbox/modules/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.747511 pyppbox-3.1b2/pyppbox/modules/trackers/centroid/
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/centroid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.747511 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.751511 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.751511 pyppbox-3.1b2/pyppbox/modules/trackers/sort/
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/sort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.751511 pyppbox-3.1b2/pyppbox/modules/trackers/sort/origin/
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/sort/origin/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.751511 pyppbox-3.1b2/pyppbox/standalone/
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/standalone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51191 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/standalone/mt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.751511 pyppbox-3.1b2/pyppbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/commontools.py
--rw-r--r--   0 runner    (1001) docker     (123)    25586 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/evatools.py
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/gttools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/logtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/persontools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/restools.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/visualizetools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.735511 pyppbox-3.1b2/pyppbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-26 21:54:02.000000 pyppbox-3.1b2/pyppbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-26 21:54:02.000000 pyppbox-3.1b2/pyppbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:54:02.000000 pyppbox-3.1b2/pyppbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-26 21:54:02.000000 pyppbox-3.1b2/pyppbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 21:54:02.000000 pyppbox-3.1b2/pyppbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.751511 pyppbox-3.1b2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-26 21:53:46.000000 pyppbox-3.1b2/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-26 21:53:46.000000 pyppbox-3.1b2/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-26 21:53:46.000000 pyppbox-3.1b2/requirements/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 21:54:02.751511 pyppbox-3.1b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-26 21:53:46.000000 pyppbox-3.1b2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-26 21:53:46.000000 pyppbox-3.1b2/setup_extra.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.814988 pyppbox-3.1b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-08-07 12:09:00.000000 pyppbox-3.1b3/GETSTARTED.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 12:09:00.000000 pyppbox-3.1b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-07 12:09:00.000000 pyppbox-3.1b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-08-07 12:09:13.814988 pyppbox-3.1b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-07 12:09:00.000000 pyppbox-3.1b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-08-07 12:09:00.000000 pyppbox-3.1b3/RELEASENOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.806988 pyppbox-3.1b3/pyppbox/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.806988 pyppbox-3.1b3/pyppbox/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.806988 pyppbox-3.1b3/pyppbox/config/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/config/cfg/cfg.7z
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/config/cfg/detectors.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/config/cfg/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/config/cfg/reiders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/config/cfg/trackers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/config/configtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65085 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/config/myconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.806988 pyppbox-3.1b3/pyppbox/config/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/config/strings/strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/config/unifiedstrings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.802988 pyppbox-3.1b3/pyppbox/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.806988 pyppbox-3.1b3/pyppbox/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/data/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.806988 pyppbox-3.1b3/pyppbox/data/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/data/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.806988 pyppbox-3.1b3/pyppbox/data/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/data/modules/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.806988 pyppbox-3.1b3/pyppbox/data/res/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/data/res/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/data/res/idmap.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.810988 pyppbox-3.1b3/pyppbox/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.810988 pyppbox-3.1b3/pyppbox/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   833181 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/assets/TReID.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/assets/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33692 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/assets/settings.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/guidemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/guihub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/guitools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.810988 pyppbox-3.1b3/pyppbox/gui/tmp/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/tmp/input.tmp
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/tmp/ui.tmp
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/ui_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/ui_deepsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/ui_facenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/ui_gt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23388 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/ui_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/ui_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/ui_torchreid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/ui_yolocls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/gui/ui_yoloult.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.810988 pyppbox-3.1b3/pyppbox/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.810988 pyppbox-3.1b3/pyppbox/modules/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.810988 pyppbox-3.1b3/pyppbox/modules/detectors/yolocls/
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/detectors/yolocls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.810988 pyppbox-3.1b3/pyppbox/modules/detectors/yoloult/
+-rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/detectors/yoloult/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.810988 pyppbox-3.1b3/pyppbox/modules/reiders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/reiders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.810988 pyppbox-3.1b3/pyppbox/modules/reiders/facenet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/reiders/facenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.810988 pyppbox-3.1b3/pyppbox/modules/reiders/facenet/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31858 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/reiders/facenet/origin/detect_face.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/reiders/facenet/origin/facenet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.810988 pyppbox-3.1b3/pyppbox/modules/reiders/torchreid/
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/reiders/torchreid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/reiders/torchreid/model_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/reiders/torchreid/model_dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/reiders/torchreid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.810988 pyppbox-3.1b3/pyppbox/modules/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.810988 pyppbox-3.1b3/pyppbox/modules/trackers/centroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/centroid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.810988 pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.814988 pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.814988 pyppbox-3.1b3/pyppbox/modules/trackers/sort/
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/sort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.814988 pyppbox-3.1b3/pyppbox/modules/trackers/sort/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/modules/trackers/sort/origin/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.814988 pyppbox-3.1b3/pyppbox/standalone/
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/standalone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51191 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/standalone/mt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.814988 pyppbox-3.1b3/pyppbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/utils/commontools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25586 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/utils/evatools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/utils/gttools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/utils/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/utils/persontools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/utils/restools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9606 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyppbox/utils/visualizetools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.806988 pyppbox-3.1b3/pyppbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-08-07 12:09:13.000000 pyppbox-3.1b3/pyppbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-08-07 12:09:13.000000 pyppbox-3.1b3/pyppbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:09:13.000000 pyppbox-3.1b3/pyppbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-07 12:09:13.000000 pyppbox-3.1b3/pyppbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-07 12:09:13.000000 pyppbox-3.1b3/pyppbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-07 12:09:00.000000 pyppbox-3.1b3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:09:13.814988 pyppbox-3.1b3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-07 12:09:00.000000 pyppbox-3.1b3/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-07 12:09:00.000000 pyppbox-3.1b3/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-08-07 12:09:00.000000 pyppbox-3.1b3/requirements/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 12:09:13.814988 pyppbox-3.1b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-08-07 12:09:00.000000 pyppbox-3.1b3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-07 12:09:00.000000 pyppbox-3.1b3/setup_extra.yaml
```

### Comparing `pyppbox-3.1b2/GETSTARTED.md` & `pyppbox-3.1b3/GETSTARTED.md`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/LICENSE` & `pyppbox-3.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/PKG-INFO` & `pyppbox-3.1b3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.1b2
+Version: 3.1b3
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
@@ -38,17 +38,20 @@
 
 [![Documentation](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml) [![Build PyPI](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml) [![Test Build](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml)
 
 [![Test Core Windows](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml) [![Test Core Linux](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml) [![Test Core macOS](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_macos.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_macos.yaml)
 
 <img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/pyppbox/pyppbox_new_wide.png"><br />
 
-**[📗 Documentation](https://rathaumons.github.io/pyppbox/) > [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) > [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html)**
+**[📗 Documentation](https://rathaumons.github.io/pyppbox/) | [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) | [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html) | [▶️ Demo](https://github.com/rathaumons/pyppbox-demo)**
 
 </div>
 
+***pyppbox*** is an all-in-one Python toolbox which can be used for detecting, tracking, and re-identifying people with only a few lines of codes. It is originally made for [***PoseTReID framework***](https://github.com/rathaumons/PoseTReID_DATASET) which can effectively track specific/certain people across multiple cameras or video scenes in distributed contexts of people interaction spaces such as malls or amusement parks, etc.
+
 * ` pyppbox = Python + People + Toolbox `
 * Design for both short and long term people detecting, tracking, and re-identifying.
 * Integrate GUI for easy configurations and demo.
 * Support dictionary and YAML/JSON configurations.
 * Support [[GTA_V_Dataset]](https://github.com/rathaumons/PoseTReID_DATASET) -> Real-time online and offline evaluation.
 * Check our papers: 1 [[IEEE]](https://ieeexplore.ieee.org/document/9271712) | 2 [[IEEE]](https://ieeexplore.ieee.org/document/9946587) [[arxiv]](https://doi.org/10.48550/arxiv.2205.10086)
+
```

### Comparing `pyppbox-3.1b2/README.md` & `pyppbox-3.1b3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 
 [![Documentation](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml) [![Build PyPI](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml) [![Test Build](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml)
 
 [![Test Core Windows](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml) [![Test Core Linux](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml) [![Test Core macOS](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_macos.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_macos.yaml)
 
 <img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/pyppbox/pyppbox_new_wide.png"><br />
 
-**[📗 Documentation](https://rathaumons.github.io/pyppbox/) > [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) > [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html)**
+**[📗 Documentation](https://rathaumons.github.io/pyppbox/) | [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) | [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html) | [▶️ Demo](https://github.com/rathaumons/pyppbox-demo)**
 
 </div>
 
+***pyppbox*** is an all-in-one Python toolbox which can be used for detecting, tracking, and re-identifying people with only a few lines of codes. It is originally made for [***PoseTReID framework***](https://github.com/rathaumons/PoseTReID_DATASET) which can effectively track specific/certain people across multiple cameras or video scenes in distributed contexts of people interaction spaces such as malls or amusement parks, etc.
+
 * ` pyppbox = Python + People + Toolbox `
 * Design for both short and long term people detecting, tracking, and re-identifying.
 * Integrate GUI for easy configurations and demo.
 * Support dictionary and YAML/JSON configurations.
 * Support [[GTA_V_Dataset]](https://github.com/rathaumons/PoseTReID_DATASET) -> Real-time online and offline evaluation.
 * Check our papers: 1 [[IEEE]](https://ieeexplore.ieee.org/document/9271712) | 2 [[IEEE]](https://ieeexplore.ieee.org/document/9946587) [[arxiv]](https://doi.org/10.48550/arxiv.2205.10086)
+
```

### Comparing `pyppbox-3.1b2/RELEASENOTES.md` & `pyppbox-3.1b3/RELEASENOTES.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,72 +1,80 @@
 # Release Notes 
 
 ## **pyppbox V3 - Make Simpler and Faster**
 
+* `pyppbox` [v3.1b3](https://github.com/rathaumons/pyppbox/tree/v3.1b2)
+
+  - Update and improve visualizetools for new pyppbox-ultralytics
+  - Update requirements
+  - Improve documentations
+  - **Known issue/limitation**:
+    - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
+
 * `pyppbox` [v3.1b2](https://github.com/rathaumons/pyppbox/tree/v3.1b2)
 
   - Improve all supported trackers
   - Improve evatools
   - Change some default configurations
   - Update and improve examples
   - Improve documentations
-  - **Known issue/limitation**: 
+  - **Known issue/limitation**:
     - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
 
 * `pyppbox` [v3.1b1](https://github.com/rathaumons/pyppbox/tree/v3.1b1)
 
   - Add multithreading support for standalone -> `ppbox.standalone.mt.MT`
   - Add multithreading example -> See example 13
   - Add CPU support for `Torchreid`
   - Implement install requirements/dependencies -> See setup.py
   - Simplify and improve requirements
   - Update default config files
   - Update and improve documentations
   - Update and improve GUI
-  - **Known issue/limitation**: 
+  - **Known issue/limitation**:
     - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
 
 * `pyppbox` [v3.0b5](https://github.com/rathaumons/pyppbox/tree/v3.0b5)
 
   - Fix a critical bug in GUI of FaceNet which can cause missing `train_data` configuration
   - Fix and improve documentation
-  - **Known issue/limitation**: 
+  - **Known issue/limitation**:
     - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
 
 * `pyppbox` [v3.0b4](https://github.com/rathaumons/pyppbox/tree/v3.0b4)
 
   - Add hotfix for command `python` in `subprocess` when running on Linux
   - Update and improve dependencies/requirements for macOS and Linux
   - Update and improve `GETSTARTED.md` for macOS and Linux
   - Add core stability test for macOS
-  - **Known issue/limitation**: 
+  - **Known issue/limitation**:
     - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
 
 * `pyppbox` [v3.0b3](https://github.com/rathaumons/pyppbox/tree/v3.0b3)
 
   - Fix GUI for GT
   - Improve supports for Python [3.8-3.11]
   - Update and improve dependencies/requirements
   - Update and improve `GETSTARTED.md`
   - Update test workflows for Python [3.8-3.11]
-  - **Known issue/limitation**: 
+  - **Known issue/limitation**:
     - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
 
 * `pyppbox` [v3.0b2](https://github.com/rathaumons/pyppbox/tree/v3.0b2)
 
   - Add Linux and macOS supports
   - Add workflow for Windows/Linux core stability tests
   - Add workflow for PyPI build -> `pyppbox` is now available on PyPI
   - Improve independency of the modules
   - Improve supports for CPU-Only
   - Improve setup quality
   - Improve GUI stability
   - Update and normalize dependencies/requirements
   - Update and improve documentations
-  - **Known issue/limitation**: 
+  - **Known issue/limitation**:
     - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
 
 * `pyppbox` [v3.0b1](https://github.com/rathaumons/pyppbox/tree/v3.0b1)
 
   - Introduce new structure of `pyppbox` -> Cleaner and simplier
   - Introduce [`pyppbox-data`](https://github.com/rathaumons/pyppbox-data) and [`pyppbox-data-gta5`](https://github.com/rathaumons/PoseTReID_DATASET#-introducing-pyppbox-data-gta5) -> Size of `pyppbox` is now 99.9% smaller, easier to build and easier to install independently, with the freedom of choice for the modules you need
   - Introduce new standard `Person` class for `pyppbox` -> `pyppbox.utils.persontools.Person`
@@ -84,27 +92,27 @@
   - Introduce new online `Sphinx` documentation -> [https://rathaumons.github.io/pyppbox](https://rathaumons.github.io/pyppbox)
   - Remove unnecessary import from submodules and their `__init__.py` files
   - Remove `input_video` and `force_hd` from main configurations, and other unused parameters from other configuration files -> New defaults `{pyppbox root}/config/cfg`
   - Add and update [examples](https://github.com/rathaumons/pyppbox/tree/main/examples) for `pyppbox` V3+ -> No longer compatible with older versions of `pyppbox`
   - Update and improve all supported modules
   - Update and improve GUI
   - Update ***requirements***
-  - **Known issue/limitation**: 
+  - **Known issue/limitation**:
     - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
 
 
 ## **pyppbox V2 - Hello Ultralytics YOLOv8**
 
 * `pyppbox` [v2.0b2](https://github.com/rathaumons/pyppbox/tree/v2.0b2)
 
   - Fix person's keypoint issue in `PManager` when using YOLO Ultralytics with pose estimation model
   - Add support for the new keypoint data format of YOLO Ultralytics's pose estimation model
   - Remove unnecessary imports
   - Update requirements
-  - **Known issue/limitation**: 
+  - **Known issue/limitation**:
     - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
 
 * `pyppbox` [v2.0b1](https://github.com/rathaumons/pyppbox/tree/v2.0b1)
 
   - Integrate PyTorch Ultralytics YOLOv8 -> `pyppbox-ultralytics` as package name
   - ***`torchreid` for pyppbox*** is changed to `pyppbox-torchreid` as package name
   - ***`opencv-contrib-python` for pyppbox*** is changed to `pyppbox-opencv` as package name
@@ -113,15 +121,15 @@
   - Enhance `PManager` & introduce `__` for private ***classes/methods***
   - Improve all related ***configurators*** & change some default configurations
   - Introduce ***lite*** & ***full*** edition of the extra models/weights
   - Update ***requirements*** & drop supports for ***Python 3.9 & CUDA 11.6/11.7***
   - Update the `FacNet` & `Torchreid` pretrained classifier ***PKLs*** for ***GTA5 dataset***
   - Update examples
   - Change to `pypa/build` for `setup.py`
-  - **Known issue/limitation**: 
+  - **Known issue/limitation**:
     - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
 
 
 ## **pyppbox V1.1 - Multithreading Ready**
 
 * `pyppbox` [v1.1b5](https://github.com/rathaumons/pyppbox/tree/v1.1b5)
 
@@ -156,11 +164,11 @@
   - Make sure the all input files such as pre-trained weights/models and others exist according to your **LOCAL** `cfg`
   - Check the **LOCAL** `cfg` and `example_local_cfg.py` as an example
   - Check pull [#4](https://github.com/rathaumons/pyppbox/pull/4) for more details
 
 
 ## **pyppbox V1**
 
-* This repo was reinitiated from version 1.0b9 where the complete history is available here [33da563](https://github.com/rathaumons/pyppbox/tree/33da56302d27204931337b44d9a6a5adc1eb5257)
+* The GitHub repo was reinitiated from version 1.0b9 where the complete history is available here [33da563](https://github.com/rathaumons/pyppbox/tree/33da56302d27204931337b44d9a6a5adc1eb5257)
 
 * [`OpenPose`](https://github.com/CMU-Perceptual-Computing-Lab/openpose) submodule was removed due to [its complicated license](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/LICENSE) -> Check this repo [`pyppbox-paper`](https://github.com/rathaumons/pyppbox-paper) if you need `OpenPose` or need to reproduce the results in the paper
```

### Comparing `pyppbox-3.1b2/pyppbox/__init__.py` & `pyppbox-3.1b3/pyppbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,13 +43,13 @@
     useInternalConfigDir, 
     useThisConfigDir,
     resetInternalConfig,
     generateConfig
 )
 
 
-__version__ = '3.1b2'
+__version__ = '3.1b3'
 __author__ = 'Ratha SIV'
 __description__ = 'Toolbox for people detecting, tracking, and re-identifying.'
 __homepage__ = 'https://rathaumons.github.io/pyppbox'
 __url__ = 'https://github.com/rathaumons/pyppbox.git'
```

### Comparing `pyppbox-3.1b2/pyppbox/config/__init__.py` & `pyppbox-3.1b3/pyppbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/config/cfg/cfg.7z` & `pyppbox-3.1b3/pyppbox/config/cfg/cfg.7z`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/config/cfg/detectors.yaml` & `pyppbox-3.1b3/pyppbox/config/cfg/detectors.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/config/cfg/reiders.yaml` & `pyppbox-3.1b3/pyppbox/config/cfg/reiders.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/config/cfg/trackers.yaml` & `pyppbox-3.1b3/pyppbox/config/cfg/trackers.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/config/configtools.py` & `pyppbox-3.1b3/pyppbox/config/configtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/config/myconfig.py` & `pyppbox-3.1b3/pyppbox/config/myconfig.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/config/unifiedstrings.py` & `pyppbox-3.1b3/pyppbox/config/unifiedstrings.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/__init__.py` & `pyppbox-3.1b3/pyppbox/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/assets/TReID.png` & `pyppbox-3.1b3/pyppbox/gui/assets/TReID.png`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/assets/icon.ico` & `pyppbox-3.1b3/pyppbox/gui/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/assets/settings.ico` & `pyppbox-3.1b3/pyppbox/gui/assets/settings.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/guidemo.py` & `pyppbox-3.1b3/pyppbox/gui/guidemo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/guihub.py` & `pyppbox-3.1b3/pyppbox/gui/guihub.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/guitools.py` & `pyppbox-3.1b3/pyppbox/gui/guitools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/ui_centroid.py` & `pyppbox-3.1b3/pyppbox/gui/ui_centroid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/ui_deepsort.py` & `pyppbox-3.1b3/pyppbox/gui/ui_deepsort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/ui_facenet.py` & `pyppbox-3.1b3/pyppbox/gui/ui_facenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/ui_gt.py` & `pyppbox-3.1b3/pyppbox/gui/ui_gt.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/ui_launcher.py` & `pyppbox-3.1b3/pyppbox/gui/ui_launcher.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/ui_sort.py` & `pyppbox-3.1b3/pyppbox/gui/ui_sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/ui_torchreid.py` & `pyppbox-3.1b3/pyppbox/gui/ui_torchreid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/ui_yolocls.py` & `pyppbox-3.1b3/pyppbox/gui/ui_yolocls.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/gui/ui_yoloult.py` & `pyppbox-3.1b3/pyppbox/gui/ui_yoloult.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/__init__.py` & `pyppbox-3.1b3/pyppbox/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/detectors/__init__.py` & `pyppbox-3.1b3/pyppbox/modules/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/detectors/yolocls/__init__.py` & `pyppbox-3.1b3/pyppbox/modules/detectors/yolocls/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/detectors/yoloult/__init__.py` & `pyppbox-3.1b3/pyppbox/modules/detectors/yoloult/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/reiders/__init__.py` & `pyppbox-3.1b3/pyppbox/modules/reiders/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/reiders/facenet/__init__.py` & `pyppbox-3.1b3/pyppbox/modules/reiders/facenet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py` & `pyppbox-3.1b3/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/reiders/facenet/origin/detect_face.py` & `pyppbox-3.1b3/pyppbox/modules/reiders/facenet/origin/detect_face.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/reiders/facenet/origin/facenet.py` & `pyppbox-3.1b3/pyppbox/modules/reiders/facenet/origin/facenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/__init__.py` & `pyppbox-3.1b3/pyppbox/modules/reiders/torchreid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/model_dict.py` & `pyppbox-3.1b3/pyppbox/modules/reiders/torchreid/model_dict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/model_dict.yaml` & `pyppbox-3.1b3/pyppbox/modules/reiders/torchreid/model_dict.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/utils.py` & `pyppbox-3.1b3/pyppbox/modules/reiders/torchreid/utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/__init__.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/centroid/__init__.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/centroid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/__init__.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/detection.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/detection.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/generate_detections.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/generate_detections.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/iou_matching.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/iou_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/nn_matching.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/nn_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/preprocessing.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/track.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/track.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/tracker.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/deepsort/origin/tracker.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/sort/__init__.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/modules/trackers/sort/origin/sort.py` & `pyppbox-3.1b3/pyppbox/modules/trackers/sort/origin/sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/standalone/__init__.py` & `pyppbox-3.1b3/pyppbox/standalone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/standalone/mt.py` & `pyppbox-3.1b3/pyppbox/standalone/mt.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/utils/__init__.py` & `pyppbox-3.1b3/pyppbox/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/utils/commontools.py` & `pyppbox-3.1b3/pyppbox/utils/commontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/utils/evatools.py` & `pyppbox-3.1b3/pyppbox/utils/evatools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/utils/gttools.py` & `pyppbox-3.1b3/pyppbox/utils/gttools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/utils/logtools.py` & `pyppbox-3.1b3/pyppbox/utils/logtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/utils/persontools.py` & `pyppbox-3.1b3/pyppbox/utils/persontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/utils/restools.py` & `pyppbox-3.1b3/pyppbox/utils/restools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/pyppbox/utils/visualizetools.py` & `pyppbox-3.1b3/pyppbox/utils/visualizetools.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,30 @@
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 import cv2
 import numpy as np
 
-from ultralytics.yolo.utils.plotting import Colors
-
 from .persontools import Person
 from .commontools import getCVMat
-from .logtools import add_error_log
+from .logtools import add_error_log, add_warning_log
 
+# For ultralytics's skeleton
+has_ultralytics = True
+try:
+    from ultralytics.utils.plotting import Colors
+    colors = Colors()
+    skeleton = [[16, 14], [14, 12], [17, 15], [15, 13], [12, 13], [6, 12], [7, 13], [6, 7], [6, 8], 
+                [7, 9], [8, 10], [9, 11], [2, 3], [1, 2], [1, 3], [2, 4], [3, 5], [4, 6], [5, 7]]
+    limb_color = colors.pose_palette[[9, 9, 9, 9, 7, 7, 7, 0, 0, 0, 0, 0, 16, 16, 16, 16, 16, 16, 16]]
+    kpt_color = colors.pose_palette[[16, 16, 16, 16, 16, 0, 0, 0, 0, 0, 0, 9, 9, 9, 9, 9, 9]]
+except ImportError as e:
+    has_ultralytics = False
+    add_warning_log("visualizetools: ultralytics or pyppbox-ultralytics is not installed.")
 
 # For cid
 cid_col = (0, 0, 255)
 cid_font_thickness = 2
 cid_font = cv2.FONT_HERSHEY_COMPLEX_SMALL
 
 # For faceid
@@ -53,20 +63,14 @@
 
 # For reid
 reid_pos = (125, 30)
 reid_col = (0, 255, 255)
 reid_dup_col = (0, 0, 255)
 reid_status_font = cv2.FONT_HERSHEY_COMPLEX_SMALL
 
-# For skeleton
-colors = Colors()
-skeleton = [[16, 14], [14, 12], [17, 15], [15, 13], [12, 13], [6, 12], [7, 13], [6, 7], [6, 8], 
-            [7, 9], [8, 10], [9, 11], [2, 3], [1, 2], [1, 3], [2, 4], [3, 5], [4, 6], [5, 7]]
-limb_color = colors.pose_palette[[9, 9, 9, 9, 7, 7, 7, 0, 0, 0, 0, 0, 16, 16, 16, 16, 16, 16, 16]]
-kpt_color = colors.pose_palette[[16, 16, 16, 16, 16, 0, 0, 0, 0, 0, 0, 9, 9, 9, 9, 9, 9]]
 
 def __addSKL__(img, kpts, radius=5, kpt_line=True):
     # Ultralytics YOLO
     h, w, c = img.shape
     shape = (h, w)
     nkpt, ndim = kpts.shape
     is_pose = nkpt == 17 and ndim == 3
@@ -149,15 +153,15 @@
                     (x, y) = p.repspoint
                     if show_box:
                         cv2.rectangle(img, (p.box_xyxy[0], p.box_xyxy[1]), 
                                       (p.box_xyxy[2], p.box_xyxy[3]), (255, 255, 0), 2)
                     if show_repspoint:
                         cv2.circle(img, (p.repspoint[0], p.repspoint[1]), radius=5, 
                                    color=(0, 0, 255), thickness=-1)
-                    if (isinstance(show_skl, tuple) and np.asarray(show_skl).shape == (3,) 
+                    if (has_ultralytics and isinstance(show_skl, tuple) and np.asarray(show_skl).shape == (3,) 
                         and len(p.keypoints) >= 15):
                         (s, l, r) = show_skl
                         if s: img = __addSKL__(img, p.keypoints, radius=r, kpt_line=l)
                     if (isinstance(show_ids, tuple) and 
                         np.asarray(show_ids).shape == (3,)):
                         if show_ids[0]:
                             cv2.putText(img, str(p.cid), (x - 10, y - 65), cid_font,
```

### Comparing `pyppbox-3.1b2/pyppbox.egg-info/PKG-INFO` & `pyppbox-3.1b3/pyppbox.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.1b2
+Version: 3.1b3
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
@@ -38,17 +38,20 @@
 
 [![Documentation](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/pyppboxdocs.yaml) [![Build PyPI](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/build_pypi.yaml) [![Test Build](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_build.yaml)
 
 [![Test Core Windows](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_windows.yaml) [![Test Core Linux](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_linux.yaml) [![Test Core macOS](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_macos.yaml/badge.svg)](https://github.com/rathaumons/pyppbox/actions/workflows/test_core_macos.yaml)
 
 <img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/pyppbox/pyppbox_new_wide.png"><br />
 
-**[📗 Documentation](https://rathaumons.github.io/pyppbox/) > [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) > [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html)**
+**[📗 Documentation](https://rathaumons.github.io/pyppbox/) | [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) | [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html) | [▶️ Demo](https://github.com/rathaumons/pyppbox-demo)**
 
 </div>
 
+***pyppbox*** is an all-in-one Python toolbox which can be used for detecting, tracking, and re-identifying people with only a few lines of codes. It is originally made for [***PoseTReID framework***](https://github.com/rathaumons/PoseTReID_DATASET) which can effectively track specific/certain people across multiple cameras or video scenes in distributed contexts of people interaction spaces such as malls or amusement parks, etc.
+
 * ` pyppbox = Python + People + Toolbox `
 * Design for both short and long term people detecting, tracking, and re-identifying.
 * Integrate GUI for easy configurations and demo.
 * Support dictionary and YAML/JSON configurations.
 * Support [[GTA_V_Dataset]](https://github.com/rathaumons/PoseTReID_DATASET) -> Real-time online and offline evaluation.
 * Check our papers: 1 [[IEEE]](https://ieeexplore.ieee.org/document/9271712) | 2 [[IEEE]](https://ieeexplore.ieee.org/document/9946587) [[arxiv]](https://doi.org/10.48550/arxiv.2205.10086)
+
```

### Comparing `pyppbox-3.1b2/pyppbox.egg-info/SOURCES.txt` & `pyppbox-3.1b3/pyppbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/requirements/requirements.txt` & `pyppbox-3.1b3/requirements/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,10 +38,10 @@
 pyunpack
 patool
 ### GUI
 PyQt6
 ### Customized pyppbox-torchreid
 pyppbox-torchreid
 ### Customized pyppbox-ultralytics
-pyppbox-ultralytics
+pyppbox-ultralytics>=8.0.142
 ### Unused
 # shapely
```

### Comparing `pyppbox-3.1b2/requirements/test_gpu.py` & `pyppbox-3.1b3/requirements/test_gpu.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/setup.py` & `pyppbox-3.1b3/setup.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b2/setup_extra.yaml` & `pyppbox-3.1b3/setup_extra.yaml`

 * *Files identical despite different names*

