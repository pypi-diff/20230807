# Comparing `tmp/pyppbox-ultralytics-8.0.145.tar.gz` & `tmp/pyppbox-ultralytics-8.0.149.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppbox-ultralytics-8.0.145.tar", last modified: Sun Jul 30 10:05:54 2023, max compression
+gzip compressed data, was "pyppbox-ultralytics-8.0.149.tar", last modified: Mon Aug  7 11:16:52 2023, max compression
```

## Comparing `pyppbox-ultralytics-8.0.145.tar` & `pyppbox-ultralytics-8.0.149.tar`

### file list

```diff
@@ -1,217 +1,218 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.456288 pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-30 10:05:54.000000 pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-07-30 10:05:54.000000 pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:05:54.000000 pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-30 10:05:54.000000 pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-30 10:05:54.000000 pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 10:05:54.000000 pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.456288 pyppbox-ultralytics-8.0.145/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.456288 pyppbox-ultralytics-8.0.145/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.456288 pyppbox-ultralytics-8.0.145/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.456288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.452288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/rt-detr/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v5/
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v6/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v6/yolov6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/cfg/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/trackers/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/cfg/trackers/bytetrack.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.460288 pyppbox-ultralytics-8.0.145/ultralytics/data/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)    37439 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/data/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16521 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    25864 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46161 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    31186 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/models/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/models/nas/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/nas/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/nas/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/nas/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.464288 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/tiny_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/utils/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/val.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26091 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/autobackend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.468288 pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/head.py
--rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36011 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.472288 pyppbox-ultralytics-8.0.145/ultralytics/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.472288 pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.472288 pyppbox-ultralytics-8.0.145/ultralytics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    30232 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.472288 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (123)    19491 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    42325 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    29013 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (123)    23082 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.472288 pyppbox-ultralytics-8.0.145/ultralytics/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/ultralytics/yolo/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/yolo/cfg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/ultralytics/yolo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/yolo/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/ultralytics/yolo/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/yolo/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/ultralytics/yolo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/yolo/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:05:54.476288 pyppbox-ultralytics-8.0.145/ultralytics/yolo/v8/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-30 10:05:40.000000 pyppbox-ultralytics-8.0.145/ultralytics/yolo/v8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.141656 pyppbox-ultralytics-8.0.149/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-08-07 11:16:52.141656 pyppbox-ultralytics-8.0.149/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.097656 pyppbox-ultralytics-8.0.149/pyppbox_ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-08-07 11:16:52.000000 pyppbox-ultralytics-8.0.149/pyppbox_ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-08-07 11:16:52.000000 pyppbox-ultralytics-8.0.149/pyppbox_ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:16:52.000000 pyppbox-ultralytics-8.0.149/pyppbox_ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-07 11:16:52.000000 pyppbox-ultralytics-8.0.149/pyppbox_ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-07 11:16:52.000000 pyppbox-ultralytics-8.0.149/pyppbox_ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 11:16:52.000000 pyppbox-ultralytics-8.0.149/pyppbox_ultralytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-07 11:16:52.141656 pyppbox-ultralytics-8.0.149/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.097656 pyppbox-ultralytics-8.0.149/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.097656 pyppbox-ultralytics-8.0.149/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.097656 pyppbox-ultralytics-8.0.149/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    50427 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.097656 pyppbox-ultralytics-8.0.149/ultralytics/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.101656 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    42439 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12421 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/open-images-v7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.093655 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.101656 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/rt-detr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.105656 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.105656 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.105656 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v6/yolov6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.105656 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.105656 pyppbox-ultralytics-8.0.149/ultralytics/cfg/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/trackers/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/cfg/trackers/bytetrack.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.109656 pyppbox-ultralytics-8.0.149/ultralytics/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37439 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/data/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.109656 pyppbox-ultralytics-8.0.149/ultralytics/data/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/data/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16521 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26128 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.113656 pyppbox-ultralytics-8.0.149/ultralytics/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46340 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24199 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31202 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.113656 pyppbox-ultralytics-8.0.149/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.113656 pyppbox-ultralytics-8.0.149/ultralytics/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.113656 pyppbox-ultralytics-8.0.149/ultralytics/models/fastsam/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/fastsam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/fastsam/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/fastsam/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/fastsam/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/fastsam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/fastsam/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.117656 pyppbox-ultralytics-8.0.149/ultralytics/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/nas/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/nas/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/nas/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.117656 pyppbox-ultralytics-8.0.149/ultralytics/models/rtdetr/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/rtdetr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/rtdetr/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/rtdetr/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/rtdetr/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/rtdetr/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.117656 pyppbox-ultralytics-8.0.149/ultralytics/models/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.121656 pyppbox-ultralytics-8.0.149/ultralytics/models/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/sam/modules/tiny_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.121656 pyppbox-ultralytics-8.0.149/ultralytics/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/utils/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.121656 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.121656 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.121656 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/detect/val.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.125656 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/pose/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.125656 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.125656 pyppbox-ultralytics-8.0.149/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26091 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/nn/autobackend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.129656 pyppbox-ultralytics-8.0.149/ultralytics/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/nn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15990 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/nn/modules/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36187 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.129656 pyppbox-ultralytics-8.0.149/ultralytics/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/trackers/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/trackers/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.129656 pyppbox-ultralytics-8.0.149/ultralytics/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/trackers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/trackers/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/trackers/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.137656 pyppbox-ultralytics-8.0.149/ultralytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    30325 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.137656 pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21017 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42325 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29071 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27483 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23082 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.137656 pyppbox-ultralytics-8.0.149/ultralytics/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.137656 pyppbox-ultralytics-8.0.149/ultralytics/yolo/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/yolo/cfg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.141656 pyppbox-ultralytics-8.0.149/ultralytics/yolo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/yolo/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.141656 pyppbox-ultralytics-8.0.149/ultralytics/yolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/yolo/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.141656 pyppbox-ultralytics-8.0.149/ultralytics/yolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/yolo/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:52.141656 pyppbox-ultralytics-8.0.149/ultralytics/yolo/v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-07 11:16:40.000000 pyppbox-ultralytics-8.0.149/ultralytics/yolo/v8/__init__.py
```

### Comparing `pyppbox-ultralytics-8.0.145/LICENSE` & `pyppbox-ultralytics-8.0.149/LICENSE`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/PKG-INFO` & `pyppbox-ultralytics-8.0.149/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox-ultralytics
-Version: 8.0.145
+Version: 8.0.149
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/rathaumons/ultralytics-for-pyppbox
 Author: rathaROG
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/rathaumons/ultralytics-for-pyppbox/issues
 Project-URL: Funding, https://ultralytics.com
@@ -33,16 +33,16 @@
 Provides-Extra: export
 License-File: LICENSE
 
 [![Build PyPI](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml)
 
 # Customized Ultralytics for [`pyppbox`](https://github.com/rathaumons/pyppbox)
 
-* Updated: **July 30, 2023**
-* Synced with: v8.0.145 -> [[a02b7e6]](https://github.com/ultralytics/ultralytics/commit/a02b7e6273b53f99536f3cefafc159e05bec2428)
+* Updated: **August 07, 2023**
+* Synced with: v8.0.149 -> [[7565210]](https://github.com/ultralytics/ultralytics/commit/756521048434f09f70802c704194d2e0c9266e99) + [[9a2c069]](https://github.com/ultralytics/ultralytics/commit/9a2c0691e3bcb0ae20ec482d25b857ab4c21bfd2)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
 * What customized:
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
```

### Comparing `pyppbox-ultralytics-8.0.145/README.md` & `pyppbox-ultralytics-8.0.149/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![Build PyPI](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml)
 
 # Customized Ultralytics for [`pyppbox`](https://github.com/rathaumons/pyppbox)
 
-* Updated: **July 30, 2023**
-* Synced with: v8.0.145 -> [[a02b7e6]](https://github.com/ultralytics/ultralytics/commit/a02b7e6273b53f99536f3cefafc159e05bec2428)
+* Updated: **August 07, 2023**
+* Synced with: v8.0.149 -> [[7565210]](https://github.com/ultralytics/ultralytics/commit/756521048434f09f70802c704194d2e0c9266e99) + [[9a2c069]](https://github.com/ultralytics/ultralytics/commit/9a2c0691e3bcb0ae20ec482d25b857ab4c21bfd2)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
 * What customized:
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
```

### Comparing `pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/PKG-INFO` & `pyppbox-ultralytics-8.0.149/pyppbox_ultralytics.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox-ultralytics
-Version: 8.0.145
+Version: 8.0.149
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/rathaumons/ultralytics-for-pyppbox
 Author: rathaROG
 Author-email: hello@ultralytics.com
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/rathaumons/ultralytics-for-pyppbox/issues
 Project-URL: Funding, https://ultralytics.com
@@ -33,16 +33,16 @@
 Provides-Extra: export
 License-File: LICENSE
 
 [![Build PyPI](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml)
 
 # Customized Ultralytics for [`pyppbox`](https://github.com/rathaumons/pyppbox)
 
-* Updated: **July 30, 2023**
-* Synced with: v8.0.145 -> [[a02b7e6]](https://github.com/ultralytics/ultralytics/commit/a02b7e6273b53f99536f3cefafc159e05bec2428)
+* Updated: **August 07, 2023**
+* Synced with: v8.0.149 -> [[7565210]](https://github.com/ultralytics/ultralytics/commit/756521048434f09f70802c704194d2e0c9266e99) + [[9a2c069]](https://github.com/ultralytics/ultralytics/commit/9a2c0691e3bcb0ae20ec482d25b857ab4c21bfd2)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
 * What customized:
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
```

### Comparing `pyppbox-ultralytics-8.0.145/pyppbox_ultralytics.egg-info/SOURCES.txt` & `pyppbox-ultralytics-8.0.149/pyppbox_ultralytics.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 ultralytics/cfg/datasets/coco-pose.yaml
 ultralytics/cfg/datasets/coco.yaml
 ultralytics/cfg/datasets/coco128-seg.yaml
 ultralytics/cfg/datasets/coco128.yaml
 ultralytics/cfg/datasets/coco8-pose.yaml
 ultralytics/cfg/datasets/coco8-seg.yaml
 ultralytics/cfg/datasets/coco8.yaml
+ultralytics/cfg/datasets/open-images-v7.yaml
 ultralytics/cfg/datasets/xView.yaml
 ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
 ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
 ultralytics/cfg/models/v3/yolov3-spp.yaml
 ultralytics/cfg/models/v3/yolov3-tiny.yaml
 ultralytics/cfg/models/v3/yolov3.yaml
 ultralytics/cfg/models/v5/yolov5-p6.yaml
```

### Comparing `pyppbox-ultralytics-8.0.145/requirements.txt` & `pyppbox-ultralytics-8.0.149/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/setup.cfg` & `pyppbox-ultralytics-8.0.149/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/setup.py` & `pyppbox-ultralytics-8.0.149/setup.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/tests/test_cli.py` & `pyppbox-ultralytics-8.0.149/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/tests/test_engine.py` & `pyppbox-ultralytics-8.0.149/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/tests/test_python.py` & `pyppbox-ultralytics-8.0.149/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/__init__.py` & `pyppbox-ultralytics-8.0.149/ultralytics/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-__version__ = '8.0.145'
+__version__ = '8.0.149'
 
 from ultralytics.hub import start
 from ultralytics.models import RTDETR, SAM, YOLO
 from ultralytics.models.fastsam import FastSAM
 from ultralytics.models.nas import NAS
 from ultralytics.utils import SETTINGS as settings
 from ultralytics.utils.checks import check_yolo as checks
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/assets/bus.jpg` & `pyppbox-ultralytics-8.0.149/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/assets/zidane.jpg` & `pyppbox-ultralytics-8.0.149/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/__init__.py` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,17 @@
     This function processes Ultralytics HUB CLI commands such as login and logout.
     It should be called when executing a script with arguments related to HUB authentication.
 
     Args:
         args (List[str]): A list of command line arguments
 
     Example:
+        ```bash
         python my_script.py hub login your_api_key
+        ```
     """
     from ultralytics import hub
 
     if args[0] == 'login':
         key = args[1] if len(args) > 1 else ''
         # Log in to Ultralytics HUB using the provided API key
         hub.login(key)
@@ -242,27 +244,34 @@
     This function processes YOLO settings CLI commands such as reset.
     It should be called when executing a script with arguments related to YOLO settings management.
 
     Args:
         args (List[str]): A list of command line arguments for YOLO settings management.
 
     Example:
+        ```bash
         python my_script.py yolo settings reset
+        ```
     """
-    if any(args):
-        if args[0] == 'reset':
-            SETTINGS_YAML.unlink()  # delete the settings file
-            SETTINGS.reset()  # create new settings
-            LOGGER.info('Settings reset successfully')  # inform the user that settings have been reset
-        else:
-            new = dict(parse_key_value_pair(a) for a in args)
-            check_dict_alignment(SETTINGS, new)
-            SETTINGS.update(new)
-
-    yaml_print(SETTINGS_YAML)  # print the current settings
+    url = 'https://docs.ultralytics.com/quickstart/#ultralytics-settings'  # help URL
+    try:
+        if any(args):
+            if args[0] == 'reset':
+                SETTINGS_YAML.unlink()  # delete the settings file
+                SETTINGS.reset()  # create new settings
+                LOGGER.info('Settings reset successfully')  # inform the user that settings have been reset
+            else:  # save a new setting
+                new = dict(parse_key_value_pair(a) for a in args)
+                check_dict_alignment(SETTINGS, new)
+                SETTINGS.update(new)
+
+        LOGGER.info(f'💡 Learn about settings at {url}')
+        yaml_print(SETTINGS_YAML)  # print the current settings
+    except Exception as e:
+        LOGGER.warning(f"WARNING ⚠️ settings error: '{e}'. Please see {url} for help.")
 
 
 def parse_key_value_pair(pair):
     """Parse one 'key=value' pair and return key and value."""
     re.sub(r' *= *', '=', pair)  # remove spaces around equals sign
     k, v = pair.split('=', 1)  # split on first '=' sign
     assert v, f"missing '{k}' value"
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/Argoverse.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/Argoverse.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 # Argoverse-HD dataset (ring-front-center camera) http://www.cs.cmu.edu/~mengtial/proj/streaming/ by Argo AI
 # Example usage: yolo train data=Argoverse.yaml
 # parent
 # ├── ultralytics
 # └── datasets
-#     └── Argoverse  ← downloads here (31.3 GB)
+#     └── Argoverse  ← downloads here (31.5 GB)
 
 
 # Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
 path: ../datasets/Argoverse  # dataset root dir
 train: Argoverse-1.1/images/train/  # train images (relative to 'path') 39384 images
 val: Argoverse-1.1/images/val/  # val images (relative to 'path') 15062 images
 test: Argoverse-1.1/images/test/  # test images (optional) https://eval.ai/web/challenges/challenge-page/800/overview
@@ -57,17 +57,17 @@
           labels[k].append(f"{cls} {x_center} {y_center} {width} {height}\n")
 
       for k in labels:
           with open(k, "w") as f:
               f.writelines(labels[k])
 
 
-  # Download
+  # Download 'https://argoverse-hd.s3.us-east-2.amazonaws.com/Argoverse-HD-Full.zip' (deprecated S3 link)
   dir = Path(yaml['path'])  # dataset root dir
-  urls = ['https://argoverse-hd.s3.us-east-2.amazonaws.com/Argoverse-HD-Full.zip']
+  urls = ['https://drive.google.com/file/d/1st9qW3BeIwQsnR0t8mRpvbsSWIo16ACi/view?usp=drive_link']
   download(urls, dir=dir)
 
   # Convert
   annotations_dir = 'Argoverse-HD/annotations/'
   (dir / 'Argoverse-1.1' / 'tracking').rename(dir / 'Argoverse-1.1' / 'images')  # rename 'tracking' to 'images'
   for d in "train.json", "val.json":
-      argoverse2yolo(dir / annotations_dir / d)  # convert VisDrone annotations to YOLO labels
+      argoverse2yolo(dir / annotations_dir / d)  # convert Argoverse annotations to YOLO labels
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/GlobalWheat2020.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/ImageNet.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/Objects365.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/SKU-110K.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/VOC.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/VisDrone.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco-pose.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco128-seg.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco128.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco8-pose.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco8-seg.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/coco8.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/datasets/xView.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/default.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v3/yolov3-spp.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v3/yolov3-tiny.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v3/yolov3.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v5/yolov5-p6.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v5/yolov5.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v6/yolov6.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-cls.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-p2.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-p6.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-pose.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8-seg.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/models/v8/yolov8.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/trackers/botsort.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/trackers/botsort.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/cfg/trackers/bytetrack.yaml` & `pyppbox-ultralytics-8.0.149/ultralytics/cfg/trackers/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/data/annotator.py` & `pyppbox-ultralytics-8.0.149/ultralytics/data/annotator.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,20 @@
     if not output_dir:
         output_dir = Path(str(data)).parent / 'labels'
     Path(output_dir).mkdir(exist_ok=True, parents=True)
 
     det_results = det_model(data, stream=True, device=device)
 
     for result in det_results:
-        boxes = result.boxes.xyxy  # Boxes object for bbox outputs
         class_ids = result.boxes.cls.int().tolist()  # noqa
         if len(class_ids):
+            boxes = result.boxes.xyxy  # Boxes object for bbox outputs
             sam_results = sam_model(result.orig_img, bboxes=boxes, verbose=False, save=False, device=device)
             segments = sam_results[0].masks.xyn  # noqa
 
-            with open(str(Path(output_dir) / Path(result.path).stem) + '.txt', 'w') as f:
+            with open(f'{str(Path(output_dir) / Path(result.path).stem)}.txt', 'w') as f:
                 for i in range(len(segments)):
                     s = segments[i]
                     if len(s) == 0:
                         continue
                     segment = map(str, segments[i].reshape(-1).tolist())
                     f.write(f'{class_ids[i]} ' + ' '.join(segment) + '\n')
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/data/augment.py` & `pyppbox-ultralytics-8.0.149/ultralytics/data/augment.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/data/base.py` & `pyppbox-ultralytics-8.0.149/ultralytics/data/base.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/data/build.py` & `pyppbox-ultralytics-8.0.149/ultralytics/data/build.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/data/converter.py` & `pyppbox-ultralytics-8.0.149/ultralytics/data/converter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/data/dataset.py` & `pyppbox-ultralytics-8.0.149/ultralytics/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/data/loaders.py` & `pyppbox-ultralytics-8.0.149/ultralytics/data/loaders.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/data/utils.py` & `pyppbox-ultralytics-8.0.149/ultralytics/data/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,16 +205,20 @@
     # Read yaml (optional)
     if isinstance(data, (str, Path)):
         data = yaml_load(data, append_filename=True)  # dictionary
 
     # Checks
     for k in 'train', 'val':
         if k not in data:
-            raise SyntaxError(
-                emojis(f"{dataset} '{k}:' key missing ❌.\n'train' and 'val' are required in all data YAMLs."))
+            if k == 'val' and 'validation' in data:
+                LOGGER.info("WARNING ⚠️ renaming data YAML 'validation' key to 'val' to match YOLO format.")
+                data['val'] = data.pop('validation')  # replace 'validation' key with 'val' key
+            else:
+                raise SyntaxError(
+                    emojis(f"{dataset} '{k}:' key missing ❌.\n'train' and 'val' are required in all data YAMLs."))
     if 'names' not in data and 'nc' not in data:
         raise SyntaxError(emojis(f"{dataset} key missing ❌.\n either 'names' or 'nc' are required in all data YAMLs."))
     if 'names' in data and 'nc' in data and len(data['names']) != data['nc']:
         raise SyntaxError(emojis(f"{dataset} 'names' length {len(data['names'])} and 'nc: {data['nc']}' must match."))
     if 'names' not in data:
         data['names'] = [f'class_{i}' for i in range(data['nc'])]
     else:
@@ -247,22 +251,22 @@
             m = f"\nDataset '{name}' images not found ⚠️, missing path '{[x for x in val if not x.exists()][0]}'"
             if s and autodownload:
                 LOGGER.warning(m)
             else:
                 m += f"\nNote dataset download directory is '{DATASETS_DIR}'. You can update this in '{SETTINGS_YAML}'"
                 raise FileNotFoundError(m)
             t = time.time()
+            r = None  # success
             if s.startswith('http') and s.endswith('.zip'):  # URL
                 safe_download(url=s, dir=DATASETS_DIR, delete=True)
-                r = None  # success
             elif s.startswith('bash '):  # bash script
                 LOGGER.info(f'Running {s} ...')
                 r = os.system(s)
             else:  # python script
-                r = exec(s, {'yaml': data})  # return None
+                exec(s, {'yaml': data})
             dt = f'({round(time.time() - t, 1)}s)'
             s = f"success ✅ {dt}, saved to {colorstr('bold', DATASETS_DIR)}" if r in (0, None) else f'failure {dt} ❌'
             LOGGER.info(f'Dataset download {s}\n')
     check_font('Arial.ttf' if is_ascii(data['names']) else 'Arial.Unicode.ttf')  # download fonts
 
     return data  # dictionary
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/engine/exporter.py` & `pyppbox-ultralytics-8.0.149/ultralytics/engine/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 TensorFlow Lite         | `tflite`                  | yolov8n.tflite
 TensorFlow Edge TPU     | `edgetpu`                 | yolov8n_edgetpu.tflite
 TensorFlow.js           | `tfjs`                    | yolov8n_web_model/
 PaddlePaddle            | `paddle`                  | yolov8n_paddle_model/
 ncnn                    | `ncnn`                    | yolov8n_ncnn_model/
 
 Requirements:
-    $ pip install ultralytics[export]
+    $ pip install "ultralytics[export]"
 
 Python:
     from ultralytics import YOLO
     model = YOLO('yolov8n.pt')
     results = model.export(format='onnx')
 
 CLI:
     $ yolo mode=export model=yolov8n.pt format=onnx
 
 Inference:
     $ yolo predict model=yolov8n.pt                 # PyTorch
                          yolov8n.torchscript        # TorchScript
-                         yolov8n.onnx               # ONNX Runtime or OpenCV DNN with --dnn
+                         yolov8n.onnx               # ONNX Runtime or OpenCV DNN with dnn=True
                          yolov8n_openvino_model     # OpenVINO
                          yolov8n.engine             # TensorRT
                          yolov8n.mlmodel            # CoreML (macOS-only)
                          yolov8n_saved_model        # TensorFlow SavedModel
                          yolov8n.pb                 # TensorFlow GraphDef
                          yolov8n.tflite             # TensorFlow Lite
                          yolov8n_edgetpu.tflite     # TensorFlow Edge TPU
@@ -173,15 +173,15 @@
         if edgetpu and not LINUX:
             raise SystemError('Edge TPU export only supported on Linux. See https://coral.ai/docs/edgetpu/compiler/')
 
         # Input
         im = torch.zeros(self.args.batch, 3, *self.imgsz).to(self.device)
         file = Path(
             getattr(model, 'pt_path', None) or getattr(model, 'yaml_file', None) or model.yaml.get('yaml_file', ''))
-        if file.suffix == '.yaml':
+        if file.suffix in ('.yaml', '.yml'):
             file = Path(file.name)
 
         # Update model
         model = deepcopy(model).to(self.device)
         for p in model.parameters():
             p.requires_grad = False
         model.eval()
@@ -210,16 +210,16 @@
         # Assign
         self.im = im
         self.model = model
         self.file = file
         self.output_shape = tuple(y.shape) if isinstance(y, torch.Tensor) else \
             tuple(tuple(x.shape if isinstance(x, torch.Tensor) else []) for x in y)
         self.pretty_name = Path(self.model.yaml.get('yaml_file', self.file)).stem.replace('yolo', 'YOLO')
-        trained_on = f'trained on {Path(self.args.data).name}' if self.args.data else '(untrained)'
-        description = f'Ultralytics {self.pretty_name} model {trained_on}'
+        data = model.args['data'] if hasattr(model, 'args') and isinstance(model.args, dict) else ''
+        description = f'Ultralytics {self.pretty_name} model {f"trained on {data}" if data else ""}'
         self.metadata = {
             'description': description,
             'author': 'Ultralytics',
             'license': 'AGPL-3.0 https://ultralytics.com/license',
             'date': datetime.now().isoformat(),
             'version': __version__,
             'stride': int(max(model.stride)),
@@ -265,21 +265,20 @@
         f = [str(x) for x in f if x]  # filter out '' and None
         if any(f):
             f = str(Path(f[-1]))
             square = self.imgsz[0] == self.imgsz[1]
             s = '' if square else f"WARNING ⚠️ non-PyTorch val requires square images, 'imgsz={self.imgsz}' will not " \
                                   f"work. Use export 'imgsz={max(self.imgsz)}' if val is required."
             imgsz = self.imgsz[0] if square else str(self.imgsz)[1:-1].replace(' ', '')
-            data = f'data={self.args.data}' if model.task == 'segment' and format == 'pb' else ''
-            LOGGER.info(
-                f'\nExport complete ({time.time() - t:.1f}s)'
-                f"\nResults saved to {colorstr('bold', file.parent.resolve())}"
-                f'\nPredict:         yolo predict task={model.task} model={f} imgsz={imgsz} {data}'
-                f'\nValidate:        yolo val task={model.task} model={f} imgsz={imgsz} data={self.args.data} {s}'
-                f'\nVisualize:       https://netron.app')
+            predict_data = f'data={data}' if model.task == 'segment' and format == 'pb' else ''
+            LOGGER.info(f'\nExport complete ({time.time() - t:.1f}s)'
+                        f"\nResults saved to {colorstr('bold', file.parent.resolve())}"
+                        f'\nPredict:         yolo predict task={model.task} model={f} imgsz={imgsz} {predict_data}'
+                        f'\nValidate:        yolo val task={model.task} model={f} imgsz={imgsz} data={data} {s}'
+                        f'\nVisualize:       https://netron.app')
 
         self.run_callbacks('on_export_end')
         return f  # return list of exported files/dirs
 
     @try_export
     def export_torchscript(self, prefix=colorstr('TorchScript:')):
         """YOLOv8 TorchScript model export."""
@@ -297,15 +296,15 @@
         return f, None
 
     @try_export
     def export_onnx(self, prefix=colorstr('ONNX:')):
         """YOLOv8 ONNX export."""
         requirements = ['onnx>=1.12.0']
         if self.args.simplify:
-            requirements += ['onnxsim>=0.4.17', 'onnxruntime-gpu' if torch.cuda.is_available() else 'onnxruntime']
+            requirements += ['onnxsim>=0.4.33', 'onnxruntime-gpu' if torch.cuda.is_available() else 'onnxruntime']
         check_requirements(requirements)
         import onnx  # noqa
 
         opset_version = self.args.opset or get_latest_opset()
         LOGGER.info(f'\n{prefix} starting export with onnx {onnx.__version__} opset {opset_version}...')
         f = str(self.file.with_suffix('.onnx'))
 
@@ -418,15 +417,15 @@
         elif (ROOT / pnnx_filename).is_file():
             pnnx = ROOT / pnnx_filename
         else:
             LOGGER.warning(
                 f'{prefix} WARNING ⚠️ PNNX not found. Attempting to download binary file from '
                 'https://github.com/pnnx/pnnx/.\nNote PNNX Binary file must be placed in current working directory '
                 f'or in {ROOT}. See PNNX repo for full installation instructions.')
-            _, assets = get_github_assets(repo='pnnx/pnnx')
+            _, assets = get_github_assets(repo='pnnx/pnnx', retry=True)
             asset = [x for x in assets if ('macos' if MACOS else 'ubuntu' if LINUX else 'windows') in x][0]
             attempt_download_asset(asset, repo='pnnx/pnnx', release='latest')
             unzip_dir = Path(asset).with_suffix('')
             pnnx = ROOT / pnnx_filename  # new location
             (unzip_dir / pnnx_filename).rename(pnnx)  # move binary to ROOT
             shutil.rmtree(unzip_dir)  # delete unzip dir
             Path(asset).unlink()  # delete zip
@@ -568,65 +567,69 @@
             t.write(engine.serialize())
 
         return f, None
 
     @try_export
     def export_saved_model(self, prefix=colorstr('TensorFlow SavedModel:')):
         """YOLOv8 TensorFlow SavedModel export."""
+        cuda = torch.cuda.is_available()
         try:
             import tensorflow as tf  # noqa
         except ImportError:
-            cuda = torch.cuda.is_available()
             check_requirements(f"tensorflow{'-macos' if MACOS else '-aarch64' if ARM64 else '' if cuda else '-cpu'}")
             import tensorflow as tf  # noqa
-        check_requirements(('onnx', 'onnx2tf>=1.9.1', 'sng4onnx>=1.0.1', 'onnxsim>=0.4.17', 'onnx_graphsurgeon>=0.3.26',
-                            'tflite_support', 'onnxruntime-gpu' if torch.cuda.is_available() else 'onnxruntime'),
-                           cmds='--extra-index-url https://pypi.ngc.nvidia.com')
+        check_requirements(
+            ('onnx', 'onnx2tf>=1.15.4', 'sng4onnx>=1.0.1', 'onnxsim>=0.4.33', 'onnx_graphsurgeon>=0.3.26',
+             'tflite_support', 'onnxruntime-gpu' if cuda else 'onnxruntime'),
+            cmds='--extra-index-url https://pypi.ngc.nvidia.com')  # onnx_graphsurgeon only on NVIDIA
 
         LOGGER.info(f'\n{prefix} starting export with tensorflow {tf.__version__}...')
         f = Path(str(self.file).replace(self.file.suffix, '_saved_model'))
         if f.is_dir():
             import shutil
             shutil.rmtree(f)  # delete output folder
 
         # Export to ONNX
         self.args.simplify = True
         f_onnx, _ = self.export_onnx()
 
         # Export to TF
         tmp_file = f / 'tmp_tflite_int8_calibration_images.npy'  # int8 calibration images file
         if self.args.int8:
+            verbosity = '--verbosity info'
             if self.args.data:
                 import numpy as np
 
                 from ultralytics.data.dataset import YOLODataset
                 from ultralytics.data.utils import check_det_dataset
 
                 # Generate calibration data for integer quantization
                 LOGGER.info(f"{prefix} collecting INT8 calibration images from 'data={self.args.data}'")
-                dataset = YOLODataset(check_det_dataset(self.args.data)['val'], imgsz=self.imgsz[0], augment=False)
+                data = check_det_dataset(self.args.data)
+                dataset = YOLODataset(data['val'], data=data, imgsz=self.imgsz[0], augment=False)
                 images = []
                 n_images = 100  # maximum number of images
                 for n, batch in enumerate(dataset):
                     if n >= n_images:
                         break
-                    im = batch['img'].permute(1, 2, 0)[None]  # list to nparray, CHW to BHWC,
+                    im = batch['img'].permute(1, 2, 0)[None]  # list to nparray, CHW to BHWC
                     images.append(im)
                 f.mkdir()
                 images = torch.cat(images, 0).float()
                 # mean = images.view(-1, 3).mean(0)  # imagenet mean [123.675, 116.28, 103.53]
                 # std = images.view(-1, 3).std(0)  # imagenet std [58.395, 57.12, 57.375]
                 np.save(str(tmp_file), images.numpy())  # BHWC
                 int8 = f'-oiqt -qt per-tensor -cind images "{tmp_file}" "[[[[0, 0, 0]]]]" "[[[[255, 255, 255]]]]"'
             else:
                 int8 = '-oiqt -qt per-tensor'
         else:
+            verbosity = '--non_verbose'
             int8 = ''
 
-        cmd = f'onnx2tf -i "{f_onnx}" -o "{f}" -nuo --non_verbose {int8}'.strip()
+        cmd = f'onnx2tf -i "{f_onnx}" -o "{f}" -nuo {verbosity} {int8}'.strip()
         LOGGER.info(f"{prefix} running '{cmd}'")
         subprocess.run(cmd, shell=True)
         yaml_save(f / 'metadata.yaml', self.metadata)  # add metadata.yaml
 
         # Remove/rename TFLite models
         if self.args.int8:
             tmp_file.unlink(missing_ok=True)
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/engine/model.py` & `pyppbox-ultralytics-8.0.149/ultralytics/engine/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             self.session = HUBTrainingSession(model)
             model = self.session.model_file
 
         # Load or create new YOLO model
         suffix = Path(model).suffix
         if not suffix and Path(model).stem in GITHUB_ASSET_STEMS:
             model, suffix = Path(model).with_suffix('.pt'), '.pt'  # add suffix, i.e. yolov8n -> yolov8n.pt
-        if suffix == '.yaml':
+        if suffix in ('.yaml', '.yml'):
             self._new(model, task)
         else:
             self._load(model, task)
 
     def __call__(self, source=None, stream=False, **kwargs):
         """Calls the 'predict' function with given arguments to perform object detection."""
         return self.predict(source, stream, **kwargs)
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/engine/predictor.py` & `pyppbox-ultralytics-8.0.149/ultralytics/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/engine/results.py` & `pyppbox-ultralytics-8.0.149/ultralytics/engine/results.py`

 * *Files 11% similar despite different names*

```diff
@@ -78,18 +78,18 @@
 
     Attributes:
         orig_img (numpy.ndarray): The original image as a numpy array.
         orig_shape (tuple): The original image shape in (height, width) format.
         boxes (Boxes, optional): A Boxes object containing the detection bounding boxes.
         masks (Masks, optional): A Masks object containing the detection masks.
         probs (Probs, optional): A Probs object containing probabilities of each class for classification task.
+        keypoints (Keypoints, optional): A Keypoints object containing detected keypoints for each object.
+        speed (dict): A dictionary of preprocess, inference, and postprocess speeds in milliseconds per image.
         names (dict): A dictionary of class names.
         path (str): The path to the image file.
-        keypoints (Keypoints, optional): A Keypoints object containing detected keypoints for each object.
-        speed (dict): A dictionary of preprocess, inference and postprocess speeds in milliseconds per image.
         _keys (tuple): A tuple of attribute names for non-empty attributes.
     """
 
     def __init__(self, orig_img, path, names, boxes=None, masks=None, probs=None, keypoints=None) -> None:
         """Initialize the Results class."""
         self.orig_img = orig_img
         self.orig_shape = orig_img.shape[:2]
@@ -106,14 +106,19 @@
     def __getitem__(self, idx):
         """Return a Results object for the specified index."""
         r = self.new()
         for k in self.keys:
             setattr(r, k, getattr(self, k)[idx])
         return r
 
+    def __len__(self):
+        """Return the number of detections in the Results object."""
+        for k in self.keys:
+            return len(getattr(self, k))
+
     def update(self, boxes=None, masks=None, probs=None):
         """Update the boxes, masks, and probs attributes of the Results object."""
         if boxes is not None:
             ops.clip_boxes(boxes, self.orig_shape)  # clip boxes
             self.boxes = Boxes(boxes, self.orig_shape)
         if masks is not None:
             self.masks = Masks(masks, self.orig_shape)
@@ -144,19 +149,14 @@
     def to(self, *args, **kwargs):
         """Return a copy of the Results object with tensors on the specified device and dtype."""
         r = self.new()
         for k in self.keys:
             setattr(r, k, getattr(self, k).to(*args, **kwargs))
         return r
 
-    def __len__(self):
-        """Return the number of detections in the Results object."""
-        for k in self.keys:
-            return len(getattr(self, k))
-
     def new(self):
         """Return a new Results object with the same image, path, and names."""
         return Results(orig_img=self.orig_img, path=self.path, names=self.names)
 
     @property
     def keys(self):
         """Return a list of non-empty attribute names."""
@@ -195,14 +195,28 @@
             labels (bool): Whether to plot the label of bounding boxes.
             boxes (bool): Whether to plot the bounding boxes.
             masks (bool): Whether to plot the masks.
             probs (bool): Whether to plot classification probability
 
         Returns:
             (numpy.ndarray): A numpy array of the annotated image.
+
+        Example:
+            ```python
+            from PIL import Image
+            from ultralytics import YOLO
+
+            model = YOLO('yolov8n.pt')
+            results = model('bus.jpg')  # results list
+            for r in results:
+                im_array = r.plot()  # plot a BGR numpy array of predictions
+                im = Image.fromarray(im[..., ::-1])  # RGB PIL image
+                im.show()  # show image
+                im.save('results.jpg')  # save image
+            ```
         """
         if img is None and isinstance(self.orig_img, torch.Tensor):
             img = np.ascontiguousarray(self.orig_img[0].permute(1, 2, 0).cpu().detach().numpy()) * 255
 
         # Deprecation warn TODO: remove in 8.2
         if 'show_conf' in kwargs:
             deprecation_warn('show_conf', 'conf')
@@ -324,18 +338,14 @@
             file_name = Path(file_name)
         for d in self.boxes:
             save_one_box(d.xyxy,
                          self.orig_img.copy(),
                          file=save_dir / self.names[int(d.cls)] / f'{file_name.stem}.jpg',
                          BGR=True)
 
-    def pandas(self):
-        """Convert the object to a pandas DataFrame (not yet implemented)."""
-        LOGGER.warning("WARNING ⚠️ 'Results.pandas' method is not yet implemented.")
-
     def tojson(self, normalize=False):
         """Convert the object to JSON format."""
         if self.probs is not None:
             LOGGER.warning('Warning: Classify task do not support `tojson` yet.')
             return
 
         import json
@@ -364,38 +374,33 @@
 
 class Boxes(BaseTensor):
     """
     A class for storing and manipulating detection boxes.
 
     Args:
         boxes (torch.Tensor | numpy.ndarray): A tensor or numpy array containing the detection boxes,
-            with shape (num_boxes, 6). The last two columns should contain confidence and class values.
+            with shape (num_boxes, 6) or (num_boxes, 7). The last two columns contain confidence and class values.
+            If present, the third last column contains track IDs.
         orig_shape (tuple): Original image size, in the format (height, width).
 
     Attributes:
-        boxes (torch.Tensor | numpy.ndarray): The detection boxes with shape (num_boxes, 6).
-        orig_shape (torch.Tensor | numpy.ndarray): Original image size, in the format (height, width).
-        is_track (bool): True if the boxes also include track IDs, False otherwise.
-
-    Properties:
         xyxy (torch.Tensor | numpy.ndarray): The boxes in xyxy format.
         conf (torch.Tensor | numpy.ndarray): The confidence values of the boxes.
         cls (torch.Tensor | numpy.ndarray): The class values of the boxes.
         id (torch.Tensor | numpy.ndarray): The track IDs of the boxes (if available).
         xywh (torch.Tensor | numpy.ndarray): The boxes in xywh format.
         xyxyn (torch.Tensor | numpy.ndarray): The boxes in xyxy format normalized by original image size.
         xywhn (torch.Tensor | numpy.ndarray): The boxes in xywh format normalized by original image size.
-        data (torch.Tensor): The raw bboxes tensor
+        data (torch.Tensor): The raw bboxes tensor (alias for `boxes`).
 
     Methods:
         cpu(): Move the object to CPU memory.
         numpy(): Convert the object to a numpy array.
         cuda(): Move the object to CUDA memory.
         to(*args, **kwargs): Move the object to the specified device.
-        pandas(): Convert the object to a pandas DataFrame (not yet implemented).
     """
 
     def __init__(self, boxes, orig_shape) -> None:
         """Initialize the Boxes class."""
         if boxes.ndim == 1:
             boxes = boxes[None, :]
         n = boxes.shape[-1]
@@ -455,162 +460,145 @@
         return self.data
 
 
 class Masks(BaseTensor):
     """
     A class for storing and manipulating detection masks.
 
-    Args:
-        masks (torch.Tensor | np.ndarray): A tensor containing the detection masks, with shape (num_masks, height, width).
-        orig_shape (tuple): Original image size, in the format (height, width).
-
     Attributes:
-        masks (torch.Tensor | np.ndarray): A tensor containing the detection masks, with shape (num_masks, height, width).
-        orig_shape (tuple): Original image size, in the format (height, width).
-
-    Properties:
-        xy (list): A list of segments (pixels) which includes x, y segments of each detection.
-        xyn (list): A list of segments (normalized) which includes x, y segments of each detection.
+        segments (list): Deprecated property for segments (normalized).
+        xy (list): A list of segments in pixel coordinates.
+        xyn (list): A list of normalized segments.
 
     Methods:
-        cpu(): Returns a copy of the masks tensor on CPU memory.
-        numpy(): Returns a copy of the masks tensor as a numpy array.
-        cuda(): Returns a copy of the masks tensor on GPU memory.
-        to(): Returns a copy of the masks tensor with the specified device and dtype.
+        cpu(): Returns the masks tensor on CPU memory.
+        numpy(): Returns the masks tensor as a numpy array.
+        cuda(): Returns the masks tensor on GPU memory.
+        to(device, dtype): Returns the masks tensor with the specified device and dtype.
     """
 
     def __init__(self, masks, orig_shape) -> None:
-        """Initialize the Masks class."""
+        """Initialize the Masks class with the given masks tensor and original image shape."""
         if masks.ndim == 2:
             masks = masks[None, :]
         super().__init__(masks, orig_shape)
 
     @property
     @lru_cache(maxsize=1)
     def segments(self):
-        """Return segments (deprecated; normalized)."""
-        LOGGER.warning("WARNING ⚠️ 'Masks.segments' is deprecated. Use 'Masks.xyn' for segments (normalized) and "
-                       "'Masks.xy' for segments (pixels) instead.")
+        """Return segments (normalized). Deprecated; use xyn property instead."""
+        LOGGER.warning(
+            "WARNING ⚠️ 'Masks.segments' is deprecated. Use 'Masks.xyn' for segments (normalized) and 'Masks.xy' for segments (pixels) instead."
+        )
         return self.xyn
 
     @property
     @lru_cache(maxsize=1)
     def xyn(self):
-        """Return segments (normalized)."""
+        """Return normalized segments."""
         return [
             ops.scale_coords(self.data.shape[1:], x, self.orig_shape, normalize=True)
             for x in ops.masks2segments(self.data)]
 
     @property
     @lru_cache(maxsize=1)
     def xy(self):
-        """Return segments (pixels)."""
+        """Return segments in pixel coordinates."""
         return [
             ops.scale_coords(self.data.shape[1:], x, self.orig_shape, normalize=False)
             for x in ops.masks2segments(self.data)]
 
     @property
     def masks(self):
-        """Return the raw masks tensor (deprecated)."""
+        """Return the raw masks tensor. Deprecated; use data attribute instead."""
         LOGGER.warning("WARNING ⚠️ 'Masks.masks' is deprecated. Use 'Masks.data' instead.")
         return self.data
 
-    def pandas(self):
-        """Convert the object to a pandas DataFrame (not yet implemented)."""
-        LOGGER.warning("WARNING ⚠️ 'Masks.pandas' method is not yet implemented.")
-
 
 class Keypoints(BaseTensor):
     """
     A class for storing and manipulating detection keypoints.
 
-    Args:
-        keypoints (torch.Tensor | np.ndarray): A tensor containing the detection keypoints, with shape (num_dets, num_kpts, 2/3).
-        orig_shape (tuple): Original image size, in the format (height, width).
-
     Attributes:
-        keypoints (torch.Tensor | np.ndarray): A tensor containing the detection keypoints, with shape (num_dets, num_kpts, 2/3).
-        orig_shape (tuple): Original image size, in the format (height, width).
-
-    Properties:
-        xy (list): A list of keypoints (pixels) which includes x, y keypoints of each detection.
-        xyn (list): A list of keypoints (normalized) which includes x, y keypoints of each detection.
+        xy (torch.Tensor): A collection of keypoints containing x, y coordinates for each detection.
+        xyn (torch.Tensor): A normalized version of xy with coordinates in the range [0, 1].
+        conf (torch.Tensor): Confidence values associated with keypoints if available, otherwise None.
 
     Methods:
         cpu(): Returns a copy of the keypoints tensor on CPU memory.
         numpy(): Returns a copy of the keypoints tensor as a numpy array.
         cuda(): Returns a copy of the keypoints tensor on GPU memory.
-        to(): Returns a copy of the keypoints tensor with the specified device and dtype.
+        to(device, dtype): Returns a copy of the keypoints tensor with the specified device and dtype.
     """
 
     def __init__(self, keypoints, orig_shape) -> None:
+        """Initializes the Keypoints object with detection keypoints and original image size."""
         if keypoints.ndim == 2:
             keypoints = keypoints[None, :]
         super().__init__(keypoints, orig_shape)
         self.has_visible = self.data.shape[-1] == 3
 
     @property
     @lru_cache(maxsize=1)
     def xy(self):
+        """Returns x, y coordinates of keypoints."""
         return self.data[..., :2]
 
     @property
     @lru_cache(maxsize=1)
     def xyn(self):
+        """Returns normalized x, y coordinates of keypoints."""
         xy = self.xy.clone() if isinstance(self.xy, torch.Tensor) else np.copy(self.xy)
         xy[..., 0] /= self.orig_shape[1]
         xy[..., 1] /= self.orig_shape[0]
         return xy
 
     @property
     @lru_cache(maxsize=1)
     def conf(self):
+        """Returns confidence values of keypoints if available, else None."""
         return self.data[..., 2] if self.has_visible else None
 
 
 class Probs(BaseTensor):
     """
-    A class for storing and manipulating classify predictions.
-
-    Args:
-        probs (torch.Tensor | np.ndarray): A tensor containing the detection keypoints, with shape (num_class, ).
+    A class for storing and manipulating classification predictions.
 
     Attributes:
-        probs (torch.Tensor | np.ndarray): A tensor containing the detection keypoints, with shape (num_class).
-
-    Properties:
-        top5 (list[int]): Top 1 indice.
-        top1 (int): Top 5 indices.
+        top1 (int): Index of the top 1 class.
+        top5 (list[int]): Indices of the top 5 classes.
+        top1conf (torch.Tensor): Confidence of the top 1 class.
+        top5conf (torch.Tensor): Confidences of the top 5 classes.
 
     Methods:
         cpu(): Returns a copy of the probs tensor on CPU memory.
         numpy(): Returns a copy of the probs tensor as a numpy array.
         cuda(): Returns a copy of the probs tensor on GPU memory.
         to(): Returns a copy of the probs tensor with the specified device and dtype.
     """
 
     def __init__(self, probs, orig_shape=None) -> None:
         super().__init__(probs, orig_shape)
 
     @property
     @lru_cache(maxsize=1)
+    def top1(self):
+        """Return the index of top 1."""
+        return int(self.data.argmax())
+
+    @property
+    @lru_cache(maxsize=1)
     def top5(self):
         """Return the indices of top 5."""
         return (-self.data).argsort(0)[:5].tolist()  # this way works with both torch and numpy.
 
     @property
     @lru_cache(maxsize=1)
-    def top1(self):
-        """Return the indices of top 1."""
-        return int(self.data.argmax())
+    def top1conf(self):
+        """Return the confidence of top 1."""
+        return self.data[self.top1]
 
     @property
     @lru_cache(maxsize=1)
     def top5conf(self):
         """Return the confidences of top 5."""
         return self.data[self.top5]
-
-    @property
-    @lru_cache(maxsize=1)
-    def top1conf(self):
-        """Return the confidences of top 1."""
-        return self.data[self.top1]
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/engine/trainer.py` & `pyppbox-ultralytics-8.0.149/ultralytics/engine/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             self.args.workers = 0  # faster CPU training as time dominated by inference, not dataloading
 
         # Model and Dataset
         self.model = self.args.model
         try:
             if self.args.task == 'classify':
                 self.data = check_cls_dataset(self.args.data)
-            elif self.args.data.endswith('.yaml') or self.args.task in ('detect', 'segment'):
+            elif self.args.data.split('.')[-1] in ('yaml', 'yml') or self.args.task in ('detect', 'segment'):
                 self.data = check_det_dataset(self.args.data)
                 if 'yaml_file' in self.data:
                     self.args.data = self.data['yaml_file']  # for validating 'yolo train data=url.zip' usage
         except Exception as e:
             raise RuntimeError(emojis(f"Dataset '{clean_url(self.args.data)}' error ❌ {e}")) from e
 
         self.trainset, self.testset = self.get_dataset(self.data)
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/engine/validator.py` & `pyppbox-ultralytics-8.0.149/ultralytics/engine/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             imgsz = check_imgsz(self.args.imgsz, stride=stride)
             if engine:
                 self.args.batch = model.batch_size
             elif not pt and not jit:
                 self.args.batch = 1  # export.py models default to batch-size 1
                 LOGGER.info(f'Forcing batch=1 square inference (1,3,{imgsz},{imgsz}) for non-PyTorch models')
 
-            if isinstance(self.args.data, str) and self.args.data.endswith('.yaml'):
+            if isinstance(self.args.data, str) and self.args.data.split('.')[-1] in ('yaml', 'yml'):
                 self.data = check_det_dataset(self.args.data)
             elif self.args.task == 'classify':
                 self.data = check_cls_dataset(self.args.data, split=self.args.split)
             else:
                 raise FileNotFoundError(emojis(f"Dataset '{self.args.data}' for task={self.args.task} not found ❌"))
 
             if self.device.type == 'cpu':
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/hub/__init__.py` & `pyppbox-ultralytics-8.0.149/ultralytics/hub/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,27 +12,33 @@
     """
     Log in to the Ultralytics HUB API using the provided API key.
 
     Args:
         api_key (str, optional): May be an API key or a combination API key and model ID, i.e. key_id
 
     Example:
+        ```python
         from ultralytics import hub
+
         hub.login('API_KEY')
+        ```
     """
     Auth(api_key, verbose=True)
 
 
 def logout():
     """
     Log out of Ultralytics HUB by removing the API key from the settings file. To log in again, use 'yolo hub login'.
 
     Example:
+        ```python
         from ultralytics import hub
+
         hub.logout()
+        ```
     """
     SETTINGS['api_key'] = ''
     yaml_save(USER_CONFIG_DIR / 'settings.yaml', SETTINGS)
     LOGGER.info(f"{PREFIX}logged out ✅. To log in again, use 'yolo hub login'.")
 
 
 def start(key=''):
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/hub/auth.py` & `pyppbox-ultralytics-8.0.149/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/hub/session.py` & `pyppbox-ultralytics-8.0.149/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/hub/utils.py` & `pyppbox-ultralytics-8.0.149/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/model.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/fastsam/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,13 +19,13 @@
         results = model.predict('ultralytics/assets/bus.jpg')
     """
 
     def __init__(self, model='FastSAM-x.pt'):
         """Call the __init__ method of the parent class (YOLO) with the updated default model"""
         if model == 'FastSAM.pt':
             model = 'FastSAM-x.pt'
-        assert Path(model).suffix != '.yaml', 'FastSAM models only support pre-trained models.'
+        assert Path(model).suffix not in ('.yaml', '.yml'), 'FastSAM models only support pre-trained models.'
         super().__init__(model=model, task='segment')
 
     @property
     def task_map(self):
         return {'segment': {'predictor': FastSAMPredictor, 'validator': FastSAMValidator}}
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/predict.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/fastsam/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/prompt.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/fastsam/prompt.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/utils.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/fastsam/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 def bbox_iou(box1, boxes, iou_thres=0.9, image_shape=(640, 640), raw_output=False):
     """
     Compute the Intersection-Over-Union of a bounding box with respect to an array of other bounding boxes.
 
     Args:
         box1 (torch.Tensor): (4, )
         boxes (torch.Tensor): (n, 4)
+        iou_thres (float): IoU threshold
+        image_shape (tuple): (height, width)
+        raw_output (bool): If True, return the raw IoU values instead of the indices
 
     Returns:
         high_iou_indices (torch.Tensor): Indices of boxes with IoU > thres
     """
     boxes = adjust_bboxes_to_image_border(boxes, image_shape)
     # obtain coordinates for intersections
     x1 = torch.max(box1[0], boxes[:, 0])
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/fastsam/val.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/fastsam/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/nas/model.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/nas/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .predict import NASPredictor
 from .val import NASValidator
 
 
 class NAS(Model):
 
     def __init__(self, model='yolo_nas_s.pt') -> None:
-        assert Path(model).suffix != '.yaml', 'YOLO-NAS models only support pre-trained models.'
+        assert Path(model).suffix not in ('.yaml', '.yml'), 'YOLO-NAS models only support pre-trained models.'
         super().__init__(model, task='detect')
 
     @smart_inference_mode()
     def _load(self, weights: str, task: str):
         # Load or create new NAS model
         import super_gradients
         suffix = Path(weights).suffix
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/nas/predict.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/nas/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/nas/val.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/nas/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/model.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/rtdetr/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 class RTDETR(Model):
     """
     RTDETR model interface.
     """
 
     def __init__(self, model='rtdetr-l.pt') -> None:
-        if model and not model.endswith('.pt') and not model.endswith('.yaml'):
-            raise NotImplementedError('RT-DETR only supports creating from pt file or yaml file.')
+        if model and not model.split('.')[-1] in ('pt', 'yaml', 'yml'):
+            raise NotImplementedError('RT-DETR only supports creating from *.pt file or *.yaml file.')
         super().__init__(model=model, task='detect')
 
     @property
     def task_map(self):
         return {
             'detect': {
                 'predictor': RTDETRPredictor,
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/predict.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/rtdetr/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/train.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/rtdetr/train.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/rtdetr/val.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/rtdetr/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/amg.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/sam/amg.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/build.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/sam/build.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/model.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/sam/model.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/decoders.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/encoders.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/sam.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/tiny_encoder.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/sam/modules/tiny_encoder.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/modules/transformer.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/sam/predict.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/sam/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/utils/loss.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/utils/ops.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/predict.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/classify/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/train.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/classify/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         model = str(self.model)
         # Load a YOLO model locally, from torchvision, or from Ultralytics assets
         if model.endswith('.pt'):
             self.model, _ = attempt_load_one_weight(model, device='cpu')
             for p in self.model.parameters():
                 p.requires_grad = True  # for training
-        elif model.endswith('.yaml'):
+        elif model.split('.')[-1] in ('yaml', 'yml'):
             self.model = self.get_model(cfg=model)
         elif model in torchvision.models.__dict__:
             self.model = torchvision.models.__dict__[model](weights='IMAGENET1K_V1' if self.args.pretrained else None)
         else:
             FileNotFoundError(f'ERROR: model={model} not found locally or online. Please check model name.')
         ClassificationModel.reshape_outputs(self.model, self.data['nc'])
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/classify/val.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/classify/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/predict.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/detect/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/train.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/detect/train.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/detect/val.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/detect/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/model.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/model.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/predict.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/pose/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/train.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/pose/train.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/pose/val.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/pose/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/predict.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/segment/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/train.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/segment/train.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/models/yolo/segment/val.py` & `pyppbox-ultralytics-8.0.149/ultralytics/models/yolo/segment/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/nn/__init__.py` & `pyppbox-ultralytics-8.0.149/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/nn/autobackend.py` & `pyppbox-ultralytics-8.0.149/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/__init__.py` & `pyppbox-ultralytics-8.0.149/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/block.py` & `pyppbox-ultralytics-8.0.149/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/conv.py` & `pyppbox-ultralytics-8.0.149/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/head.py` & `pyppbox-ultralytics-8.0.149/ultralytics/nn/modules/head.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,39 +303,38 @@
     def _get_decoder_input(self, feats, shapes, dn_embed=None, dn_bbox=None):
         bs = len(feats)
         # prepare input for decoder
         anchors, valid_mask = self._generate_anchors(shapes, dtype=feats.dtype, device=feats.device)
         features = self.enc_output(valid_mask * feats)  # bs, h*w, 256
 
         enc_outputs_scores = self.enc_score_head(features)  # (bs, h*w, nc)
-        # dynamic anchors + static content
-        enc_outputs_bboxes = self.enc_bbox_head(features) + anchors  # (bs, h*w, 4)
 
         # query selection
         # (bs, num_queries)
         topk_ind = torch.topk(enc_outputs_scores.max(-1).values, self.num_queries, dim=1).indices.view(-1)
         # (bs, num_queries)
         batch_ind = torch.arange(end=bs, dtype=topk_ind.dtype).unsqueeze(-1).repeat(1, self.num_queries).view(-1)
 
-        # Unsigmoided
-        refer_bbox = enc_outputs_bboxes[batch_ind, topk_ind].view(bs, self.num_queries, -1)
-        # refer_bbox = torch.gather(enc_outputs_bboxes, 1, topk_ind.reshape(bs, self.num_queries).unsqueeze(-1).repeat(1, 1, 4))
+        # (bs, num_queries, 256)
+        top_k_features = features[batch_ind, topk_ind].view(bs, self.num_queries, -1)
+        # (bs, num_queries, 4)
+        top_k_anchors = anchors[:, topk_ind].view(bs, self.num_queries, -1)
+
+        # dynamic anchors + static content
+        refer_bbox = self.enc_bbox_head(top_k_features) + top_k_anchors
 
         enc_bboxes = refer_bbox.sigmoid()
         if dn_bbox is not None:
             refer_bbox = torch.cat([dn_bbox, refer_bbox], 1)
-        if self.training:
-            refer_bbox = refer_bbox.detach()
         enc_scores = enc_outputs_scores[batch_ind, topk_ind].view(bs, self.num_queries, -1)
 
-        if self.learnt_init_query:
-            embeddings = self.tgt_embed.weight.unsqueeze(0).repeat(bs, 1, 1)
-        else:
-            embeddings = features[batch_ind, topk_ind].view(bs, self.num_queries, -1)
-            if self.training:
+        embeddings = self.tgt_embed.weight.unsqueeze(0).repeat(bs, 1, 1) if self.learnt_init_query else top_k_features
+        if self.training:
+            refer_bbox = refer_bbox.detach()
+            if not self.learnt_init_query:
                 embeddings = embeddings.detach()
         if dn_embed is not None:
             embeddings = torch.cat([dn_embed, embeddings], 1)
 
         return embeddings, refer_bbox, enc_bboxes, enc_scores
 
     # TODO
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/transformer.py` & `pyppbox-ultralytics-8.0.149/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/nn/modules/utils.py` & `pyppbox-ultralytics-8.0.149/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/nn/tasks.py` & `pyppbox-ultralytics-8.0.149/ultralytics/nn/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,16 @@
             y.append(x if m.i in self.save else None)  # save output
             if visualize:
                 feature_visualization(x, m.type, m.i, save_dir=visualize)
         return x
 
     def _predict_augment(self, x):
         """Perform augmentations on input image x and return augmented inference."""
-        LOGGER.warning(
-            f'WARNING ⚠️ {self.__class__.__name__} has not supported augment inference yet! Now using single-scale inference instead.'
-        )
+        LOGGER.warning(f'WARNING ⚠️ {self.__class__.__name__} does not support augmented inference yet. '
+                       f'Reverting to single-scale inference instead.')
         return self._predict_once(x)
 
     def _profile_one_layer(self, m, x, dt):
         """
         Profile the computation time and FLOPs of a single layer of the model on a given input.
         Appends the results to the provided list.
 
@@ -101,23 +100,23 @@
             m (nn.Module): The layer to be profiled.
             x (torch.Tensor): The input data to the layer.
             dt (list): A list to store the computation time of the layer.
 
         Returns:
             None
         """
-        c = m == self.model[-1]  # is final layer, copy input as inplace fix
-        o = thop.profile(m, inputs=[x.clone() if c else x], verbose=False)[0] / 1E9 * 2 if thop else 0  # FLOPs
+        c = m == self.model[-1] and isinstance(x, list)  # is final layer list, copy input as inplace fix
+        flops = thop.profile(m, inputs=[x.copy() if c else x], verbose=False)[0] / 1E9 * 2 if thop else 0  # FLOPs
         t = time_sync()
         for _ in range(10):
-            m(x.clone() if c else x)
+            m(x.copy() if c else x)
         dt.append((time_sync() - t) * 100)
         if m == self.model[0]:
             LOGGER.info(f"{'time (ms)':>10s} {'GFLOPs':>10s} {'params':>10s}  module")
-        LOGGER.info(f'{dt[-1]:10.2f} {o:10.2f} {m.np:10.0f}  {m.type}')
+        LOGGER.info(f'{dt[-1]:10.2f} {flops:10.2f} {m.np:10.0f}  {m.type}')
         if c:
             LOGGER.info(f"{sum(dt):10.2f} {'-':>10s} {'-':>10s}  Total")
 
     def fuse(self, verbose=True):
         """
         Fuse the `Conv2d()` and `BatchNorm2d()` layers of the model into a single layer, in order to improve the
         computation efficiency.
@@ -158,40 +157,41 @@
         return sum(isinstance(v, bn) for v in self.modules()) < thresh  # True if < 'thresh' BatchNorm layers in model
 
     def info(self, detailed=False, verbose=True, imgsz=640):
         """
         Prints model information
 
         Args:
+            detailed (bool): if True, prints out detailed information about the model. Defaults to False
             verbose (bool): if True, prints out the model information. Defaults to False
             imgsz (int): the size of the image that the model will be trained on. Defaults to 640
         """
         return model_info(self, detailed=detailed, verbose=verbose, imgsz=imgsz)
 
     def _apply(self, fn):
         """
-        `_apply()` is a function that applies a function to all the tensors in the model that are not
-        parameters or registered buffers
+        Applies a function to all the tensors in the model that are not parameters or registered buffers.
 
         Args:
-            fn: the function to apply to the model
+            fn (function): the function to apply to the model
 
         Returns:
             A model that is a Detect() object.
         """
         self = super()._apply(fn)
         m = self.model[-1]  # Detect()
         if isinstance(m, (Detect, Segment)):
             m.stride = fn(m.stride)
             m.anchors = fn(m.anchors)
             m.strides = fn(m.strides)
         return self
 
     def load(self, weights, verbose=True):
-        """Load the weights into the model.
+        """
+        Load the weights into the model.
 
         Args:
             weights (dict | torch.nn.Module): The pre-trained weights to be loaded.
             verbose (bool, optional): Whether to log the transfer progress. Defaults to True.
         """
         model = weights['model'] if isinstance(weights, dict) else weights  # torchvision models are not dicts
         csd = model.float().state_dict()  # checkpoint state_dict as FP32
@@ -334,15 +334,15 @@
         return self._predict_once(x)
 
 
 class ClassificationModel(BaseModel):
     """YOLOv8 classification model."""
 
     def __init__(self,
-                 cfg=None,
+                 cfg='yolov8n-cls.yaml',
                  model=None,
                  ch=3,
                  nc=None,
                  cutoff=10,
                  verbose=True):  # yaml, model, channels, number of classes, cutoff index, verbose flag
         super().__init__()
         self._from_detection_model(model, nc, cutoff) if model is not None else self._from_yaml(cfg, ch, nc, verbose)
@@ -507,16 +507,18 @@
     where you've moved a module from one location to another, but you still want to support the old import
     paths for backwards compatibility.
 
     Args:
         modules (dict, optional): A dictionary mapping old module paths to new module paths.
 
     Example:
+        ```python
         with temporary_modules({'old.module.path': 'new.module.path'}):
             import old.module.path  # this will now import new.module.path
+        ```
 
     Note:
         The changes are only in effect inside the context manager and are undone once the context manager exits.
         Be aware that directly manipulating `sys.modules` can lead to unpredictable results, especially in larger
         applications or libraries. Use this function with caution.
     """
     if not modules:
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/trackers/basetrack.py` & `pyppbox-ultralytics-8.0.149/ultralytics/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/trackers/bot_sort.py` & `pyppbox-ultralytics-8.0.149/ultralytics/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/trackers/byte_tracker.py` & `pyppbox-ultralytics-8.0.149/ultralytics/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/trackers/track.py` & `pyppbox-ultralytics-8.0.149/ultralytics/trackers/track.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/gmc.py` & `pyppbox-ultralytics-8.0.149/ultralytics/trackers/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/kalman_filter.py` & `pyppbox-ultralytics-8.0.149/ultralytics/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/trackers/utils/matching.py` & `pyppbox-ultralytics-8.0.149/ultralytics/trackers/utils/matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/__init__.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -325,15 +325,18 @@
         s = f.read()  # string
 
         # Remove special characters
         if not s.isprintable():
             s = re.sub(r'[^\x09\x0A\x0D\x20-\x7E\x85\xA0-\uD7FF\uE000-\uFFFD\U00010000-\U0010ffff]+', '', s)
 
         # Add YAML filename to dict and return
-        return {**yaml.safe_load(s), 'yaml_file': str(file)} if append_filename else yaml.safe_load(s)
+        data = yaml.safe_load(s) or {}  # always return a dict (yaml.safe_load() may return None for empty files)
+        if append_filename:
+            data['yaml_file'] = str(file)
+        return data
 
 
 def yaml_print(yaml_file: Union[str, Path, dict]) -> None:
     """
     Pretty prints a yaml file or a yaml-formatted dictionary.
 
     Args:
@@ -352,14 +355,27 @@
 for k, v in DEFAULT_CFG_DICT.items():
     if isinstance(v, str) and v.lower() == 'none':
         DEFAULT_CFG_DICT[k] = None
 DEFAULT_CFG_KEYS = DEFAULT_CFG_DICT.keys()
 DEFAULT_CFG = IterableSimpleNamespace(**DEFAULT_CFG_DICT)
 
 
+def is_ubuntu() -> bool:
+    """
+    Check if the OS is Ubuntu.
+
+    Returns:
+        (bool): True if OS is Ubuntu, False otherwise.
+    """
+    with contextlib.suppress(FileNotFoundError):
+        with open('/etc/os-release') as f:
+            return 'ID=ubuntu' in f.read()
+    return False
+
+
 def is_colab():
     """
     Check if the current script is running inside a Google Colab notebook.
 
     Returns:
         (bool): True if running inside a Colab notebook, False otherwise.
     """
@@ -543,14 +559,27 @@
     Returns:
         (dict): A dictionary where each key is a parameter name, and each value is the default value of that parameter.
     """
     signature = inspect.signature(func)
     return {k: v.default for k, v in signature.parameters.items() if v.default is not inspect.Parameter.empty}
 
 
+def get_ubuntu_version():
+    """
+    Retrieve the Ubuntu version if the OS is Ubuntu.
+
+    Returns:
+        (str): Ubuntu version or None if not an Ubuntu OS.
+    """
+    with contextlib.suppress(FileNotFoundError, AttributeError):
+        with open('/etc/os-release') as f:
+            return re.search(r'VERSION_ID="(\d+\.\d+)"', f.read())[1]
+    return None
+
+
 def get_user_config_dir(sub_dir='Ultralytics'):
     """
     Get the user config directory.
 
     Args:
         sub_dir (str): The name of the subdirectory to create.
 
@@ -564,25 +593,26 @@
         path = Path.home() / 'Library' / 'Application Support' / sub_dir
     elif LINUX:
         path = Path.home() / '.config' / sub_dir
     else:
         raise ValueError(f'Unsupported operating system: {platform.system()}')
 
     # GCP and AWS lambda fix, only /tmp is writeable
-    if not is_dir_writeable(str(path.parent)):
-        path = Path('/tmp') / sub_dir
-        LOGGER.warning(f"WARNING ⚠️ user config directory is not writeable, defaulting to '{path}'.")
+    if not is_dir_writeable(path.parent):
+        LOGGER.warning(f"WARNING ⚠️ user config directory '{path}' is not writeable, defaulting to '/tmp' or CWD."
+                       'Alternatively you can define a YOLO_CONFIG_DIR environment variable for this path.')
+        path = Path('/tmp') / sub_dir if is_dir_writeable('/tmp') else Path().cwd() / sub_dir
 
     # Create the subdirectory if it does not exist
     path.mkdir(parents=True, exist_ok=True)
 
     return path
 
 
-USER_CONFIG_DIR = Path(os.getenv('YOLO_CONFIG_DIR', get_user_config_dir()))  # Ultralytics settings dir
+USER_CONFIG_DIR = Path(os.getenv('YOLO_CONFIG_DIR') or get_user_config_dir())  # Ultralytics settings dir
 SETTINGS_YAML = USER_CONFIG_DIR / 'settings.yaml'
 
 
 def colorstr(*input):
     """Colors a string https://en.wikipedia.org/wiki/ANSI_escape_code, i.e.  colorstr('blue', 'hello world')."""
     *args, string = input if len(input) > 1 else ('blue', 'bold', input[0])  # color arguments, string
     colors = {
@@ -709,32 +739,14 @@
         sentry_sdk.set_user({'id': SETTINGS['uuid']})  # SHA-256 anonymized UUID hash
 
         # Disable all sentry logging
         for logger in 'sentry_sdk', 'sentry_sdk.errors':
             logging.getLogger(logger).setLevel(logging.CRITICAL)
 
 
-def update_dict_recursive(d, u):
-    """
-    Recursively updates the dictionary `d` with the key-value pairs from the dictionary `u` without overwriting
-    entire sub-dictionaries. Note that function recursion is intended and not a problem, as this allows for updating
-    nested dictionaries at any arbitrary depth.
-
-    Args:
-        d (dict): The dictionary to be updated.
-        u (dict): The dictionary to update `d` with.
-
-    Returns:
-        (dict): The recursively updated dictionary.
-    """
-    for k, v in u.items():
-        d[k] = update_dict_recursive(d.get(k, {}), v) if isinstance(v, dict) else v
-    return d
-
-
 class SettingsManager(dict):
     """
     Manages Ultralytics settings stored in a YAML file.
 
     Args:
         file (str | Path): Path to the Ultralytics settings YAML file. Default is USER_CONFIG_DIR / 'settings.yaml'.
         version (str): Settings version. In case of local version mismatch, new default settings will be saved.
@@ -787,28 +799,23 @@
                     'with your settings or a recent ultralytics package update. '
                     f"\nView settings with 'yolo settings' or at '{self.file}'"
                     "\nUpdate settings with 'yolo settings key=value', i.e. 'yolo settings runs_dir=path/to/dir'.")
                 self.reset()
 
     def load(self):
         """Loads settings from the YAML file."""
-        self.update(yaml_load(self.file))
+        super().update(yaml_load(self.file))
 
     def save(self):
         """Saves the current settings to the YAML file."""
         yaml_save(self.file, dict(self))
 
     def update(self, *args, **kwargs):
-        """Updates a setting value in the current settings and saves the settings."""
-        new = dict(*args, **kwargs)
-        if any(isinstance(v, dict) for v in new.values()):
-            update_dict_recursive(self, new)
-        else:
-            # super().update(*args, **kwargs)
-            super().update(new)
+        """Updates a setting value in the current settings."""
+        super().update(*args, **kwargs)
         self.save()
 
     def reset(self):
         """Resets the settings to default and saves them."""
         self.clear()
         self.update(self.defaults)
         self.save()
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/autobatch.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/benchmarks.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/benchmarks.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
             print('No matching *.pt or *.onnx files found.')
             return
 
         table_rows = []
         output = []
         for file in files:
             engine_file = file.with_suffix('.engine')
-            if file.suffix in ('.pt', '.yaml'):
+            if file.suffix in ('.pt', '.yaml', '.yml'):
                 model = YOLO(str(file))
                 model.fuse()  # to report correct params and GFLOPs in model.info()
                 model_info = model.info()
                 if self.trt and self.device.type != 'cpu' and not engine_file.is_file():
                     engine_file = model.export(format='engine',
                                                half=True,
                                                imgsz=self.imgsz,
@@ -225,15 +225,15 @@
     def get_files(self):
         files = []
         for path in self.paths:
             path = Path(path)
             if path.is_dir():
                 extensions = ['*.pt', '*.onnx', '*.yaml']
                 files.extend([file for ext in extensions for file in glob.glob(str(path / ext))])
-            elif path.suffix in {'.pt', '.yaml'}:  # add non-existing
+            elif path.suffix in ('.pt', '.yaml', '.yml'):  # add non-existing
                 files.append(str(path))
             else:
                 files.extend(glob.glob(str(path)))
 
         print(f'Profiling: {sorted(files)}')
         return [Path(file) for file in sorted(files)]
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/base.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/clearml.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/comet.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/dvc.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/dvc.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             live.log_metric(metric, value, plot=False)
 
         _log_plots(trainer.plots, 'val')
         _log_plots(trainer.validator.plots, 'val')
         _log_confusion_matrix(trainer.validator)
 
         if trainer.best.exists():
-            live.log_artifact(trainer.best, copy=True)
+            live.log_artifact(trainer.best, copy=True, type='model')
 
         live.end()
 
 
 callbacks = {
     'on_pretrain_routine_start': on_pretrain_routine_start,
     'on_pretrain_routine_end': on_pretrain_routine_end,
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/hub.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/mlflow.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/mlflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     assert SETTINGS['mlflow'] is True  # verify integration is enabled
 except (ImportError, AssertionError):
     mlflow = None
 
 
 def on_pretrain_routine_end(trainer):
     """Logs training parameters to MLflow."""
-    global mlflow, run, run_id, experiment_name
+    global mlflow, run, experiment_name
 
     if os.environ.get('MLFLOW_TRACKING_URI') is None:
         mlflow = None
 
     if mlflow:
         mlflow_location = os.environ['MLFLOW_TRACKING_URI']  # "http://192.168.xxx.xxx:5000"
         mlflow.set_tracking_uri(mlflow_location)
@@ -35,16 +35,15 @@
         mlflow.set_experiment(experiment_name)
 
         prefix = colorstr('MLFlow: ')
         try:
             run, active_run = mlflow, mlflow.active_run()
             if not active_run:
                 active_run = mlflow.start_run(experiment_id=experiment.experiment_id, run_name=run_name)
-            run_id = active_run.info.run_id
-            LOGGER.info(f'{prefix}Using run_id({run_id}) at {mlflow_location}')
+            LOGGER.info(f'{prefix}Using run_id({active_run.info.run_id}) at {mlflow_location}')
             run.log_params(vars(trainer.model.args))
         except Exception as err:
             LOGGER.error(f'{prefix}Failing init - {repr(err)}')
             LOGGER.warning(f'{prefix}Continuing without Mlflow')
 
 
 def on_fit_epoch_end(trainer):
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/neptune.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/raytune.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/raytune.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/tensorboard.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/callbacks/wb.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/checks.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/checks.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     Verify image size is a multiple of the given stride in each dimension. If the image size is not a multiple of the
     stride, update it to the nearest multiple of the stride that is greater than or equal to the given floor value.
 
     Args:
         imgsz (int | cList[int]): Image size.
         stride (int): Stride value.
         min_dim (int): Minimum number of dimensions.
+        max_dim (int): Maximum number of dimensions.
         floor (int): Minimum allowed value for image size.
 
     Returns:
         (List[int]): Updated image size.
     """
     # Convert stride to integer if it is a tensor
     stride = int(stride.max() if isinstance(stride, torch.Tensor) else stride)
@@ -86,44 +87,73 @@
     # Add missing dimensions if necessary
     sz = [sz[0], sz[0]] if min_dim == 2 and len(sz) == 1 else sz[0] if min_dim == 1 and len(sz) == 1 else sz
 
     return sz
 
 
 def check_version(current: str = '0.0.0',
-                  minimum: str = '0.0.0',
+                  required: str = '0.0.0',
                   name: str = 'version ',
-                  pinned: bool = False,
                   hard: bool = False,
                   verbose: bool = False) -> bool:
     """
-    Check current version against the required minimum version.
+    Check current version against the required version or range.
 
     Args:
         current (str): Current version.
-        minimum (str): Required minimum version.
+        required (str): Required version or range (in pip-style format).
         name (str): Name to be used in warning message.
-        pinned (bool): If True, versions must match exactly. If False, minimum version must be satisfied.
-        hard (bool): If True, raise an AssertionError if the minimum version is not met.
-        verbose (bool): If True, print warning message if minimum version is not met.
+        hard (bool): If True, raise an AssertionError if the requirement is not met.
+        verbose (bool): If True, print warning message if requirement is not met.
 
     Returns:
-        (bool): True if minimum version is met, False otherwise.
-    """
-    current, minimum = (pkg.parse_version(x) for x in (current, minimum))
-    result = (current == minimum) if pinned else (current >= minimum)  # bool
-    warning_message = f'WARNING ⚠️ {name}{minimum} is required by YOLOv8, but {name}{current} is currently installed'
-    if hard:
-        assert result, emojis(warning_message)  # assert min requirements met
-    if verbose and not result:
-        LOGGER.warning(warning_message)
+        (bool): True if requirement is met, False otherwise.
+
+    Example:
+        # check if current version is exactly 22.04
+        check_version(current='22.04', required='==22.04')
+
+        # check if current version is greater than or equal to 22.04
+        check_version(current='22.10', required='22.04')  # assumes '>=' inequality if none passed
+
+        # check if current version is less than or equal to 22.04
+        check_version(current='22.04', required='<=22.04')
+
+        # check if current version is between 20.04 (inclusive) and 22.04 (exclusive)
+        check_version(current='21.10', required='>20.04,<22.04')
+    """
+    current = pkg.parse_version(current)
+    constraints = re.findall(r'([<>!=]{1,2}\s*\d+\.\d+)', required) or [f'>={required}']
+
+    result = True
+    for constraint in constraints:
+        op, version = re.match(r'([<>!=]{1,2})\s*(\d+\.\d+)', constraint).groups()
+        version = pkg.parse_version(version)
+        if op == '==' and current != version:
+            result = False
+        elif op == '!=' and current == version:
+            result = False
+        elif op == '>=' and not (current >= version):
+            result = False
+        elif op == '<=' and not (current <= version):
+            result = False
+        elif op == '>' and not (current > version):
+            result = False
+        elif op == '<' and not (current < version):
+            result = False
+    if not result:
+        warning_message = f'WARNING ⚠️ {name}{required} is required, but {name}{current} is currently installed'
+        if hard:
+            raise ModuleNotFoundError(emojis(warning_message))  # assert version requirements met
+        if verbose:
+            LOGGER.warning(warning_message)
     return result
 
 
-def check_latest_pypi_version(package_name='pyppbox-ultralytics'):
+def check_latest_pypi_version(package_name='ultralytics'):
     """
     Returns the latest version of a PyPI package without downloading or installing it.
 
     Parameters:
         package_name (str): The name of the package to find the latest version for.
 
     Returns:
@@ -210,14 +240,28 @@
 
     Args:
         requirements (Union[Path, str, List[str]]): Path to a requirements.txt file, a single package requirement as a
             string, or a list of package requirements as strings.
         exclude (Tuple[str]): Tuple of package names to exclude from checking.
         install (bool): If True, attempt to auto-update packages that don't meet requirements.
         cmds (str): Additional commands to pass to the pip install command when auto-updating.
+
+    Example:
+        ```python
+        from ultralytics.utils.checks import check_requirements
+
+        # Check a requirements.txt file
+        check_requirements('path/to/requirements.txt')
+
+        # Check a single package
+        check_requirements('ultralytics>=8.0.0')
+
+        # Check multiple packages
+        check_requirements(['numpy', 'ultralytics>=8.0.0'])
+        ```
     """
     prefix = colorstr('red', 'bold', 'requirements:')
     check_python()  # check python version
     check_torchvision()  # check torch-torchvision compatibility
     if isinstance(requirements, Path):  # requirements.txt file
         file = requirements.resolve()
         assert file.exists(), f'{prefix} {file} not found, check failed.'
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/dist.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/dist.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/downloads.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/downloads.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import contextlib
+import re
 import shutil
 import subprocess
 from itertools import repeat
 from multiprocessing.pool import ThreadPool
 from pathlib import Path
 from urllib import parse, request
-from zipfile import BadZipFile, ZipFile, is_zipfile
 
 import requests
 import torch
 from tqdm import tqdm
 
 from ultralytics.utils import LOGGER, checks, clean_url, emojis, is_online, url2file
 
@@ -35,55 +35,103 @@
         if check:
             with request.urlopen(url) as response:
                 return response.getcode() == 200  # check if exists online
         return True
     return False
 
 
-def unzip_file(file, path=None, exclude=('.DS_Store', '__MACOSX'), exist_ok=False):
+def zip_directory(directory, compress=True, exclude=('.DS_Store', '__MACOSX'), progress=True):
+    """
+    Zips the contents of a directory, excluding files containing strings in the exclude list.
+    The resulting zip file is named after the directory and placed alongside it.
+
+    Args:
+        directory (str | Path): The path to the directory to be zipped.
+        compress (bool): Whether to compress the files while zipping. Default is True.
+        exclude (tuple, optional): A tuple of filename strings to be excluded. Defaults to ('.DS_Store', '__MACOSX').
+        progress (bool, optional): Whether to display a progress bar. Defaults to True.
+
+    Returns:
+        (Path): The path to the resulting zip file.
+
+    Example:
+        ```python
+        from ultralytics.utils.downloads import zip_directory
+
+        file = zip_directory('path/to/dir')
+        ```
+    """
+    from zipfile import ZIP_DEFLATED, ZIP_STORED, ZipFile
+
+    directory = Path(directory)
+    if not directory.is_dir():
+        raise FileNotFoundError(f"Directory '{directory}' does not exist.")
+
+    # Unzip with progress bar
+    files_to_zip = [f for f in directory.rglob('*') if f.is_file() and not any(x in f.name for x in exclude)]
+    zip_file = directory.with_suffix('.zip')
+    compression = ZIP_DEFLATED if compress else ZIP_STORED
+    with ZipFile(zip_file, 'w', compression) as f:
+        for file in tqdm(files_to_zip, desc=f'Zipping {directory} to {zip_file}...', unit='file', disable=not progress):
+            f.write(file, file.relative_to(directory))
+
+    return zip_file  # return path to zip file
+
+
+def unzip_file(file, path=None, exclude=('.DS_Store', '__MACOSX'), exist_ok=False, progress=True):
     """
     Unzips a *.zip file to the specified path, excluding files containing strings in the exclude list.
 
     If the zipfile does not contain a single top-level directory, the function will create a new
     directory with the same name as the zipfile (without the extension) to extract its contents.
     If a path is not provided, the function will use the parent directory of the zipfile as the default path.
 
     Args:
         file (str): The path to the zipfile to be extracted.
         path (str, optional): The path to extract the zipfile to. Defaults to None.
         exclude (tuple, optional): A tuple of filename strings to be excluded. Defaults to ('.DS_Store', '__MACOSX').
         exist_ok (bool, optional): Whether to overwrite existing contents if they exist. Defaults to False.
+        progress (bool, optional): Whether to display a progress bar. Defaults to True.
 
     Raises:
         BadZipFile: If the provided file does not exist or is not a valid zipfile.
 
     Returns:
         (Path): The path to the directory where the zipfile was extracted.
+
+    Example:
+        ```python
+        from ultralytics.utils.downloads import unzip_file
+
+        dir = unzip_file('path/to/file.zip')
+        ```
     """
+    from zipfile import BadZipFile, ZipFile, is_zipfile
+
     if not (Path(file).exists() and is_zipfile(file)):
         raise BadZipFile(f"File '{file}' does not exist or is a bad zip file.")
     if path is None:
         path = Path(file).parent  # default path
 
     # Unzip the file contents
     with ZipFile(file) as zipObj:
-        file_list = [f for f in zipObj.namelist() if all(x not in f for x in exclude)]
-        top_level_dirs = {Path(f).parts[0] for f in file_list}
+        files = [f for f in zipObj.namelist() if all(x not in f for x in exclude)]
+        top_level_dirs = {Path(f).parts[0] for f in files}
 
-        if len(top_level_dirs) > 1 or not file_list[0].endswith('/'):
+        if len(top_level_dirs) > 1 or not files[0].endswith('/'):
             path = Path(path) / Path(file).stem  # define new unzip directory
 
         # Check if destination directory already exists and contains files
         extract_path = Path(path) / list(top_level_dirs)[0]
         if extract_path.exists() and any(extract_path.iterdir()) and not exist_ok:
             # If it exists and is not empty, return the path without unzipping
             LOGGER.info(f'Skipping {file} unzip (already unzipped)')
             return path
 
-        for f in file_list:
+        for f in tqdm(files, desc=f'Unzipping {file} to {Path(path).resolve()}...', unit='file', disable=not progress):
             zipObj.extract(f, path=path)
 
     return path  # return unzip dir
 
 
 def check_disk_space(url='https://ultralytics.com/assets/coco128.zip', sf=1.5, hard=True):
     """
@@ -113,14 +161,56 @@
             LOGGER.warning(text)
             return False
 
             # Pass if error
     return True
 
 
+def get_google_drive_file_info(link):
+    """
+    Retrieves the direct download link and filename for a shareable Google Drive file link.
+
+    Args:
+        link (str): The shareable link of the Google Drive file.
+
+    Returns:
+        (str): Direct download URL for the Google Drive file.
+        (str): Original filename of the Google Drive file. If filename extraction fails, returns None.
+
+    Example:
+        ```python
+        from ultralytics.utils.downloads import get_google_drive_file_info
+
+        link = "https://drive.google.com/file/d/1cqT-cJgANNrhIHCrEufUYhQ4RqiWG_lJ/view?usp=drive_link"
+        url, filename = get_google_drive_file_info(link)
+        ```
+    """
+    file_id = link.split('/d/')[1].split('/view')[0]
+    drive_url = f'https://drive.google.com/uc?export=download&id={file_id}'
+
+    # Start session
+    filename = None
+    with requests.Session() as session:
+        response = session.get(drive_url, stream=True)
+        if 'quota exceeded' in str(response.content.lower()):
+            raise ConnectionError(
+                emojis(f'❌  Google Drive file download quota exceeded. '
+                       f'Please try again later or download this file manually at {link}.'))
+        token = None
+        for key, value in response.cookies.items():
+            if key.startswith('download_warning'):
+                token = value
+        if token:
+            drive_url = f'https://drive.google.com/uc?export=download&confirm={token}&id={file_id}'
+        cd = response.headers.get('content-disposition')
+        if cd:
+            filename = re.findall('filename="(.+)"', cd)[0]
+    return drive_url, filename
+
+
 def safe_download(url,
                   file=None,
                   dir=None,
                   unzip=True,
                   delete=False,
                   curl=False,
                   retry=3,
@@ -139,21 +229,26 @@
         delete (bool, optional): Whether to delete the downloaded file after unzipping. Default: False.
         curl (bool, optional): Whether to use curl command line tool for downloading. Default: False.
         retry (int, optional): The number of times to retry the download in case of failure. Default: 3.
         min_bytes (float, optional): The minimum number of bytes that the downloaded file should have, to be considered
             a successful download. Default: 1E0.
         progress (bool, optional): Whether to display a progress bar during the download. Default: True.
     """
-    f = dir / url2file(url) if dir else Path(file)  # URL converted to filename
+
+    # Check if the URL is a Google Drive link
+    gdrive = 'drive.google.com' in url
+    if gdrive:
+        url, file = get_google_drive_file_info(url)
+
+    f = dir / (file if gdrive else url2file(url)) if dir else Path(file)  # URL converted to filename
     if '://' not in str(url) and Path(url).is_file():  # URL exists ('://' check required in Windows Python<3.10)
         f = Path(url)  # filename
     elif not f.is_file():  # URL and file do not exist
         assert dir or file, 'dir or file required for download'
-        f = dir / url2file(url) if dir else Path(file)
-        desc = f"Downloading {clean_url(url)} to '{f}'"
+        desc = f"Downloading {url if gdrive else clean_url(url)} to '{f}'"
         LOGGER.info(f'{desc}...')
         f.parent.mkdir(parents=True, exist_ok=True)  # make directory if missing
         check_disk_space(url)
         for i in range(retry + 1):
             try:
                 if curl or i > 0:  # curl download with retry, continue
                     s = 'sS' * (not progress)  # silent
@@ -185,33 +280,37 @@
                 if i == 0 and not is_online():
                     raise ConnectionError(emojis(f'❌  Download failure for {url}. Environment is not online.')) from e
                 elif i >= retry:
                     raise ConnectionError(emojis(f'❌  Download failure for {url}. Retry limit reached.')) from e
                 LOGGER.warning(f'⚠️ Download failure, retrying {i + 1}/{retry} {url}...')
 
     if unzip and f.exists() and f.suffix in ('', '.zip', '.tar', '.gz'):
+        from zipfile import is_zipfile
+
         unzip_dir = dir or f.parent  # unzip to dir if provided else unzip in place
-        LOGGER.info(f'Unzipping {f} to {unzip_dir.absolute()}...')
         if is_zipfile(f):
             unzip_dir = unzip_file(file=f, path=unzip_dir)  # unzip
-        elif f.suffix == '.tar':
-            subprocess.run(['tar', 'xf', f, '--directory', unzip_dir], check=True)  # unzip
-        elif f.suffix == '.gz':
-            subprocess.run(['tar', 'xfz', f, '--directory', unzip_dir], check=True)  # unzip
+        elif f.suffix in ('.tar', '.gz'):
+            LOGGER.info(f'Unzipping {f} to {unzip_dir.resolve()}...')
+            subprocess.run(['tar', 'xf' if f.suffix == '.tar' else 'xfz', f, '--directory', unzip_dir], check=True)
         if delete:
             f.unlink()  # remove zip
         return unzip_dir
 
 
-def get_github_assets(repo='ultralytics/assets', version='latest'):
+def get_github_assets(repo='ultralytics/assets', version='latest', retry=False):
     """Return GitHub repo tag and assets (i.e. ['yolov8n.pt', 'yolov8s.pt', ...])."""
     if version != 'latest':
         version = f'tags/{version}'  # i.e. tags/v6.2
-    response = requests.get(f'https://api.github.com/repos/{repo}/releases/{version}').json()  # github api
-    return response['tag_name'], [x['name'] for x in response['assets']]  # tag, assets
+    url = f'https://api.github.com/repos/{repo}/releases/{version}'
+    r = requests.get(url)  # github api
+    if r.status_code != 200 and retry:
+        r = requests.get(url)  # try again
+    data = r.json()
+    return data['tag_name'], [x['name'] for x in data['assets']]  # tag, assets
 
 
 def attempt_download_asset(file, repo='ultralytics/assets', release='v0.0.0'):
     """Attempt file download from GitHub release assets if not found locally. release = 'latest', 'v6.2', etc."""
     from ultralytics.utils import SETTINGS  # scoped for circular import
 
     # YOLOv3/5u updates
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/files.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,19 @@
 
     Args:
         path (str | Path): The original path.
 
     Yields:
         (Path): Temporary path with spaces replaced by underscores if spaces were present, otherwise the original path.
 
-    Examples:
+    Example:
+        ```python
         with spaces_in_path('/path/with spaces') as new_path:
             # your code here
+        ```
     """
 
     # If path has spaces, replace them with underscores
     if ' ' in str(path):
         string = isinstance(path, str)  # input type
         path = Path(path)
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/instance.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/instance.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/loss.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/metrics.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/ops.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,18 +57,22 @@
 
 def coco80_to_coco91_class():  #
     """
     Converts 80-index (val2014) to 91-index (paper).
     For details see https://tech.amikelive.com/node-718/what-object-categories-labels-are-in-coco-dataset/.
 
     Example:
+        ```python
+        import numpy as np
+
         a = np.loadtxt('data/coco.names', dtype='str', delimiter='\n')
         b = np.loadtxt('data/coco_paper.names', dtype='str', delimiter='\n')
         x1 = [list(a[i] == b).index(True) + 1 for i in range(80)]  # darknet to coco
         x2 = [list(b[i] == a).index(True) if any(b[i] == a) else None for i in range(91)]  # coco to darknet
+        ```
     """
     return [
         1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 27, 28, 31, 32, 33, 34,
         35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63,
         64, 65, 67, 70, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 84, 85, 86, 87, 88, 89, 90]
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/patches.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/patches.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/plotting.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/plotting.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,53 +7,74 @@
 
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from PIL import Image, ImageDraw, ImageFont
 from PIL import __version__ as pil_version
-from scipy.ndimage import gaussian_filter1d
 
 from ultralytics.utils import LOGGER, TryExcept, plt_settings, threaded
 
 from .checks import check_font, check_version, is_ascii
 from .files import increment_path
 from .ops import clip_boxes, scale_image, xywh2xyxy, xyxy2xywh
 
 
 class Colors:
-    """Ultralytics color palette https://ultralytics.com/."""
+    """
+    Ultralytics default color palette https://ultralytics.com/.
+
+    This class provides methods to work with the Ultralytics color palette, including converting hex color codes to
+    RGB values.
+
+    Attributes:
+        palette (list of tuple): List of RGB color values.
+        n (int): The number of colors in the palette.
+        pose_palette (np.array): A specific color palette array with dtype np.uint8.
+    """
 
     def __init__(self):
         """Initialize colors as hex = matplotlib.colors.TABLEAU_COLORS.values()."""
         hexs = ('FF3838', 'FF9D97', 'FF701F', 'FFB21D', 'CFD231', '48F90A', '92CC17', '3DDB86', '1A9334', '00D4BB',
                 '2C99A8', '00C2FF', '344593', '6473FF', '0018EC', '8438FF', '520085', 'CB38FF', 'FF95C8', 'FF37C7')
         self.palette = [self.hex2rgb(f'#{c}') for c in hexs]
         self.n = len(self.palette)
         self.pose_palette = np.array([[255, 128, 0], [255, 153, 51], [255, 178, 102], [230, 230, 0], [255, 153, 255],
                                       [153, 204, 255], [255, 102, 255], [255, 51, 255], [102, 178, 255], [51, 153, 255],
                                       [255, 153, 153], [255, 102, 102], [255, 51, 51], [153, 255, 153], [102, 255, 102],
                                       [51, 255, 51], [0, 255, 0], [0, 0, 255], [255, 0, 0], [255, 255, 255]],
                                      dtype=np.uint8)
 
     def __call__(self, i, bgr=False):
-        """Converts hex color codes to rgb values."""
+        """Converts hex color codes to RGB values."""
         c = self.palette[int(i) % self.n]
         return (c[2], c[1], c[0]) if bgr else c
 
     @staticmethod
-    def hex2rgb(h):  # rgb order (PIL)
+    def hex2rgb(h):
+        """Converts hex color codes to RGB values (i.e. default PIL order)."""
         return tuple(int(h[1 + i:1 + i + 2], 16) for i in (0, 2, 4))
 
 
 colors = Colors()  # create instance for 'from utils.plots import colors'
 
 
 class Annotator:
-    """YOLOv8 Annotator for train/val mosaics and jpgs and detect/hub inference annotations."""
+    """
+    Ultralytics Annotator for train/val mosaics and JPGs and predictions annotations.
+
+    Attributes:
+        im (Image.Image or numpy array): The image to annotate.
+        pil (bool): Whether to use PIL or cv2 for drawing annotations.
+        font (ImageFont.truetype or ImageFont.load_default): Font used for text annotations.
+        lw (float): Line width for drawing.
+        skeleton (List[List[int]]): Skeleton structure for keypoints.
+        limb_color (List[int]): Color palette for limbs.
+        kpt_color (List[int]): Color palette for keypoints.
+    """
 
     def __init__(self, im, line_width=None, font_size=None, font='Arial.ttf', pil=False, example='abc'):
         """Initialize the Annotator class with image and line width along with color palette for keypoints and limbs."""
         assert im.data.contiguous, 'Image not contiguous. Apply np.ascontiguousarray(im) to Annotator() input images.'
         non_ascii = not is_ascii(example)  # non-latin labels, i.e. asian, arabic, cyrillic
         self.pil = pil or non_ascii
         if self.pil:  # use PIL
@@ -108,20 +129,23 @@
                             0,
                             self.lw / 3,
                             txt_color,
                             thickness=tf,
                             lineType=cv2.LINE_AA)
 
     def masks(self, masks, colors, im_gpu, alpha=0.5, retina_masks=False):
-        """Plot masks at once.
+        """
+        Plot masks on image.
+
         Args:
-            masks (tensor): predicted masks on cuda, shape: [n, h, w]
-            colors (List[List[Int]]): colors for predicted masks, [[r, g, b] * n]
-            im_gpu (tensor): img is in cuda, shape: [3, h, w], range: [0, 1]
-            alpha (float): mask transparency: 0.0 fully transparent, 1.0 opaque
+            masks (tensor): Predicted masks on cuda, shape: [n, h, w]
+            colors (List[List[Int]]): Colors for predicted masks, [[r, g, b] * n]
+            im_gpu (tensor): Image is in cuda, shape: [3, h, w], range: [0, 1]
+            alpha (float): Mask transparency: 0.0 fully transparent, 1.0 opaque
+            retina_masks (bool): Whether to use high resolution masks or not. Defaults to False.
         """
         if self.pil:
             # Convert to numpy first
             self.im = np.asarray(self.im).copy()
         if len(masks) == 0:
             self.im[:] = im_gpu.permute(1, 2, 0).contiguous().cpu().numpy() * 255
         if im_gpu.device != masks.device:
@@ -141,15 +165,16 @@
         im_mask_np = im_mask.byte().cpu().numpy()
         self.im[:] = im_mask_np if retina_masks else scale_image(im_mask_np, self.im.shape)
         if self.pil:
             # Convert im back to PIL and update draw
             self.fromarray(self.im)
 
     def kpts(self, kpts, shape=(640, 640), radius=5, kpt_line=True):
-        """Plot keypoints on the image.
+        """
+        Plot keypoints on the image.
 
         Args:
             kpts (tensor): Predicted keypoints with shape [17, 3]. Each keypoint has (x, y, confidence).
             shape (tuple): Image shape as a tuple (h, w), where h is the height and w is the width.
             radius (int, optional): Radius of the drawn keypoints. Default is 5.
             kpt_line (bool, optional): If True, the function will draw lines connecting keypoints
                                        for human pose. Default is True.
@@ -235,26 +260,26 @@
         """Return annotated image as array."""
         return np.asarray(self.im)
 
 
 @TryExcept()  # known issue https://github.com/ultralytics/yolov5/issues/5395
 @plt_settings()
 def plot_labels(boxes, cls, names=(), save_dir=Path(''), on_plot=None):
-    """Save and plot image with no axis or spines."""
+    """Plot training labels including class histograms and box statistics."""
     import pandas as pd
     import seaborn as sn
 
     # Filter matplotlib>=3.7.2 warning
     warnings.filterwarnings('ignore', category=UserWarning, message='The figure layout has changed to tight')
 
     # Plot dataset labels
     LOGGER.info(f"Plotting labels to {save_dir / 'labels.jpg'}... ")
-    b = boxes.transpose()  # classes, boxes
     nc = int(cls.max() + 1)  # number of classes
-    x = pd.DataFrame(b.transpose(), columns=['x', 'y', 'width', 'height'])
+    boxes = boxes[:1000000]  # limit to 1M boxes
+    x = pd.DataFrame(boxes, columns=['x', 'y', 'width', 'height'])
 
     # Seaborn correlogram
     sn.pairplot(x, corner=True, diag_kind='auto', kind='hist', diag_kws=dict(bins=50), plot_kws=dict(pmax=0.9))
     plt.savefig(save_dir / 'labels_correlogram.jpg', dpi=200)
     plt.close()
 
     # Matplotlib labels
@@ -288,15 +313,45 @@
     plt.savefig(fname, dpi=200)
     plt.close()
     if on_plot:
         on_plot(fname)
 
 
 def save_one_box(xyxy, im, file=Path('im.jpg'), gain=1.02, pad=10, square=False, BGR=False, save=True):
-    """Save image crop as {file} with crop size multiple {gain} and {pad} pixels. Save and/or return crop."""
+    """Save image crop as {file} with crop size multiple {gain} and {pad} pixels. Save and/or return crop.
+
+    This function takes a bounding box and an image, and then saves a cropped portion of the image according
+    to the bounding box. Optionally, the crop can be squared, and the function allows for gain and padding
+    adjustments to the bounding box.
+
+    Args:
+        xyxy (torch.Tensor or list): A tensor or list representing the bounding box in xyxy format.
+        im (numpy.ndarray): The input image.
+        file (Path, optional): The path where the cropped image will be saved. Defaults to 'im.jpg'.
+        gain (float, optional): A multiplicative factor to increase the size of the bounding box. Defaults to 1.02.
+        pad (int, optional): The number of pixels to add to the width and height of the bounding box. Defaults to 10.
+        square (bool, optional): If True, the bounding box will be transformed into a square. Defaults to False.
+        BGR (bool, optional): If True, the image will be saved in BGR format, otherwise in RGB. Defaults to False.
+        save (bool, optional): If True, the cropped image will be saved to disk. Defaults to True.
+
+    Returns:
+        (numpy.ndarray): The cropped image.
+
+    Example:
+        ```python
+        from ultralytics.utils.plotting import save_one_box
+
+        xyxy = [50, 50, 150, 150]
+        im = cv2.imread('image.jpg')
+        cropped_im = save_one_box(xyxy, im, file='cropped.jpg', square=True)
+        ```
+    """
+
+    if not isinstance(xyxy, torch.Tensor):  # may be list
+        xyxy = torch.stack(xyxy)
     b = xyxy2xywh(xyxy.view(-1, 4))  # boxes
     if square:
         b[:, 2:] = b[:, 2:].max(1)[0].unsqueeze(1)  # attempt rectangle to square
     b[:, 2:] = b[:, 2:] * gain + pad  # box wh * gain + pad
     xyxy = xywh2xyxy(b).long()
     clip_boxes(xyxy, im.shape)
     crop = im[int(xyxy[0, 1]):int(xyxy[0, 3]), int(xyxy[0, 0]):int(xyxy[0, 2]), ::(1 if BGR else -1)]
@@ -438,16 +493,26 @@
     annotator.im.save(fname)  # save
     if on_plot:
         on_plot(fname)
 
 
 @plt_settings()
 def plot_results(file='path/to/results.csv', dir='', segment=False, pose=False, classify=False, on_plot=None):
-    """Plot training results.csv. Usage: from utils.plots import *; plot_results('path/to/results.csv')."""
+    """
+    Plot training results from results CSV file.
+
+    Example:
+        ```python
+        from ultralytics.utils.plotting import plot_results
+
+        plot_results('path/to/results.csv')
+        ```
+    """
     import pandas as pd
+    from scipy.ndimage import gaussian_filter1d
     save_dir = Path(file).parent if file else Path(dir)
     if classify:
         fig, ax = plt.subplots(2, 2, figsize=(6, 6), tight_layout=True)
         index = [1, 4, 2, 3]
     elif segment:
         fig, ax = plt.subplots(2, 8, figsize=(18, 6), tight_layout=True)
         index = [1, 2, 3, 4, 5, 6, 9, 10, 13, 14, 15, 16, 7, 8, 11, 12]
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/tal.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/tal.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/torch_utils.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/utils/tuner.py` & `pyppbox-ultralytics-8.0.149/ultralytics/utils/tuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     try:
         from ray import tune
         from ray.air import RunConfig
         from ray.air.integrations.wandb import WandbLoggerCallback
         from ray.tune.schedulers import ASHAScheduler
     except ImportError:
-        raise ModuleNotFoundError("Tuning hyperparameters requires Ray Tune. Install with: pip install 'ray[tune]'")
+        raise ModuleNotFoundError('Tuning hyperparameters requires Ray Tune. Install with: pip install "ray[tune]"')
 
     try:
         import wandb
 
         assert hasattr(wandb, '__version__')
     except (ImportError, AssertionError):
         wandb = False
```

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/yolo/data/__init__.py` & `pyppbox-ultralytics-8.0.149/ultralytics/yolo/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.0.145/ultralytics/yolo/utils/__init__.py` & `pyppbox-ultralytics-8.0.149/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*

