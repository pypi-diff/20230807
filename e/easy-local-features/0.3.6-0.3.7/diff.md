# Comparing `tmp/easy_local_features-0.3.6.tar.gz` & `tmp/easy_local_features-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_local_features-0.3.6.tar", last modified: Sun Jul 23 02:33:34 2023, max compression
+gzip compressed data, was "easy_local_features-0.3.7.tar", last modified: Tue Aug  1 15:20:45 2023, max compression
```

## Comparing `easy_local_features-0.3.6.tar` & `easy_local_features-0.3.7.tar`

### file list

```diff
@@ -1,105 +1,112 @@
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.061481 easy_local_features-0.3.6/
--rw-r--r--   0 cadar      (501) staff       (20)     1520 2023-07-22 09:17:15.000000 easy_local_features-0.3.6/LICENSE_ALIKED.txt
--rw-r--r--   0 cadar      (501) staff       (20)    32722 2023-07-01 15:16:15.000000 easy_local_features-0.3.6/LICENSE_DISK.txt
--rw-r--r--   0 cadar      (501) staff       (20)    21121 2023-07-01 17:04:24.000000 easy_local_features-0.3.6/LICENSE_R2D2.txt
--rw-r--r--   0 cadar      (501) staff       (20)     7009 2023-07-01 16:24:52.000000 easy_local_features-0.3.6/LICENSE_SUPERGLUE.txt
--rw-r--r--   0 cadar      (501) staff       (20)     2545 2023-07-23 02:33:34.061238 easy_local_features-0.3.6/PKG-INFO
--rw-r--r--   0 cadar      (501) staff       (20)     2260 2023-07-23 02:24:00.000000 easy_local_features-0.3.6/README.md
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.032258 easy_local_features-0.3.6/easy_local_features/
--rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-01 15:35:14.000000 easy_local_features-0.3.6/easy_local_features/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.034945 easy_local_features-0.3.6/easy_local_features/datasets/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-06-12 19:58:13.000000 easy_local_features-0.3.6/easy_local_features/datasets/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)    10688 2023-07-11 20:37:33.000000 easy_local_features-0.3.6/easy_local_features/datasets/augmentor.py
--rw-r--r--   0 cadar      (501) staff       (20)     3034 2023-06-12 19:58:13.000000 easy_local_features-0.3.6/easy_local_features/datasets/download.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.037694 easy_local_features-0.3.6/easy_local_features/feature/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/feature/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     3774 2023-07-23 02:12:15.000000 easy_local_features-0.3.6/easy_local_features/feature/baseline_aliked.py
--rw-r--r--   0 cadar      (501) staff       (20)    34684 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/feature/baseline_dalf.py
--rw-r--r--   0 cadar      (501) staff       (20)     2624 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/feature/baseline_deal.py
--rw-r--r--   0 cadar      (501) staff       (20)     6746 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/feature/baseline_disk.py
--rw-r--r--   0 cadar      (501) staff       (20)     6012 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/feature/baseline_r2d2.py
--rw-r--r--   0 cadar      (501) staff       (20)     2857 2023-07-23 01:46:09.000000 easy_local_features-0.3.6/easy_local_features/feature/baseline_superpoint.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.038824 easy_local_features-0.3.6/easy_local_features/matching/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 21:59:23.000000 easy_local_features-0.3.6/easy_local_features/matching/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2075 2023-07-23 02:33:04.000000 easy_local_features-0.3.6/easy_local_features/matching/baseline_loftr.py
--rw-r--r--   0 cadar      (501) staff       (20)     5144 2023-07-23 02:32:46.000000 easy_local_features-0.3.6/easy_local_features/matching/baseline_superglue.py
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 22:06:22.000000 easy_local_features-0.3.6/easy_local_features/matching/core.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.038994 easy_local_features-0.3.6/easy_local_features/submodules/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:42:35.000000 easy_local_features-0.3.6/easy_local_features/submodules/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.039160 easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-22 08:58:42.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.039755 easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/custom_ops/
--rw-r--r--   0 cadar      (501) staff       (20)     5503 2023-07-23 02:07:54.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/custom_ops/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)      599 2023-07-22 11:59:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/custom_ops/setup.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.042454 easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/nets/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-22 08:58:50.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/nets/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     7454 2023-07-23 02:06:58.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/nets/aliked.py
--rw-r--r--   0 cadar      (501) staff       (20)     9383 2023-07-22 12:01:18.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/nets/blocks.py
--rw-r--r--   0 cadar      (501) staff       (20)      863 2023-07-22 08:46:52.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/nets/padder.py
--rw-r--r--   0 cadar      (501) staff       (20)     8080 2023-07-22 08:46:52.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/nets/soft_detect.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.043023 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:23:41.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.043288 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/
--rw-r--r--   0 cadar      (501) staff       (20)       24 2023-07-01 15:39:51.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.043946 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/common/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:40:58.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/common/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2652 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/common/structs.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.045186 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/geom/
--rw-r--r--   0 cadar      (501) staff       (20)       79 2023-07-01 08:54:41.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/geom/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)      291 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/geom/distance_matrix.py
--rw-r--r--   0 cadar      (501) staff       (20)     2096 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/geom/epi.py
--rw-r--r--   0 cadar      (501) staff       (20)     3406 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/geom/pose.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.046981 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/model/
--rw-r--r--   0 cadar      (501) staff       (20)      113 2023-07-01 08:54:41.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/model/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2732 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py
--rw-r--r--   0 cadar      (501) staff       (20)     2566 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py
--rw-r--r--   0 cadar      (501) staff       (20)     5454 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/model/detector.py
--rw-r--r--   0 cadar      (501) staff       (20)     2177 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/model/disk.py
--rw-r--r--   0 cadar      (501) staff       (20)      865 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/model/nms.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.049264 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/unets/
--rw-r--r--   0 cadar      (501) staff       (20)      249 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/unets/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     4159 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/unets/blocks.py
--rw-r--r--   0 cadar      (501) staff       (20)     2070 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/unets/ops.py
--rw-r--r--   0 cadar      (501) staff       (20)     3289 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/unets/unet.py
--rw-r--r--   0 cadar      (501) staff       (20)     1291 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/unets/utils.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.051344 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:53:50.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     6223 2023-07-01 17:01:09.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/extract.py
--rw-r--r--   0 cadar      (501) staff       (20)     9927 2023-07-01 16:26:30.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/extract_kapture.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.053940 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/nets/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:54.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/nets/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2360 2023-07-01 16:26:31.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/nets/ap_loss.py
--rw-r--r--   0 cadar      (501) staff       (20)     1720 2023-07-01 16:26:31.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/nets/losses.py
--rw-r--r--   0 cadar      (501) staff       (20)     7158 2023-07-01 16:26:31.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/nets/patchnet.py
--rw-r--r--   0 cadar      (501) staff       (20)     1760 2023-07-01 16:26:31.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py
--rw-r--r--   0 cadar      (501) staff       (20)     2006 2023-07-01 16:26:31.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py
--rw-r--r--   0 cadar      (501) staff       (20)    15031 2023-07-01 16:26:31.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/nets/sampler.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.056249 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/tools/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:23.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/tools/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     1080 2023-07-01 16:26:31.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/tools/common.py
--rw-r--r--   0 cadar      (501) staff       (20)    14318 2023-07-01 17:00:44.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/tools/dataloader.py
--rw-r--r--   0 cadar      (501) staff       (20)     2208 2023-07-01 16:26:31.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/tools/trainer.py
--rw-r--r--   0 cadar      (501) staff       (20)    18298 2023-07-01 16:26:31.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/tools/transforms.py
--rw-r--r--   0 cadar      (501) staff       (20)     7160 2023-07-01 16:26:31.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py
--rw-r--r--   0 cadar      (501) staff       (20)     5647 2023-07-01 16:26:31.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/tools/viz.py
--rw-r--r--   0 cadar      (501) staff       (20)     5018 2023-07-01 16:26:31.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/train.py
--rw-r--r--   0 cadar      (501) staff       (20)     4203 2023-07-01 16:26:31.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/viz_heatmaps.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.056511 easy_local_features-0.3.6/easy_local_features/submodules/git_superglue/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:22:28.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_superglue/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.059843 easy_local_features-0.3.6/easy_local_features/submodules/git_superglue/models/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:16:09.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_superglue/models/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     3417 2023-07-01 16:16:09.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_superglue/models/matching.py
--rw-r--r--   0 cadar      (501) staff       (20)    11537 2023-07-01 16:40:16.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_superglue/models/superglue.py
--rw-r--r--   0 cadar      (501) staff       (20)     8092 2023-07-01 16:40:03.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_superglue/models/superpoint.py
--rw-r--r--   0 cadar      (501) staff       (20)    20039 2023-07-01 16:16:09.000000 easy_local_features-0.3.6/easy_local_features/submodules/git_superglue/models/utils.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.060768 easy_local_features-0.3.6/easy_local_features/utils/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/utils/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)      293 2023-07-11 16:38:37.000000 easy_local_features-0.3.6/easy_local_features/utils/generic_match.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-23 02:33:34.033716 easy_local_features-0.3.6/easy_local_features.egg-info/
--rw-r--r--   0 cadar      (501) staff       (20)     2545 2023-07-23 02:33:33.000000 easy_local_features-0.3.6/easy_local_features.egg-info/PKG-INFO
--rw-r--r--   0 cadar      (501) staff       (20)     4188 2023-07-23 02:33:33.000000 easy_local_features-0.3.6/easy_local_features.egg-info/SOURCES.txt
--rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-23 02:33:33.000000 easy_local_features-0.3.6/easy_local_features.egg-info/dependency_links.txt
--rw-r--r--   0 cadar      (501) staff       (20)       73 2023-07-23 02:33:33.000000 easy_local_features-0.3.6/easy_local_features.egg-info/requires.txt
--rw-r--r--   0 cadar      (501) staff       (20)       20 2023-07-23 02:33:33.000000 easy_local_features-0.3.6/easy_local_features.egg-info/top_level.txt
--rw-r--r--   0 cadar      (501) staff       (20)       38 2023-07-23 02:33:34.061551 easy_local_features-0.3.6/setup.cfg
--rw-r--r--   0 cadar      (501) staff       (20)     1703 2023-07-23 02:33:15.000000 easy_local_features-0.3.6/setup.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.333652 easy_local_features-0.3.7/
+-rw-r--r--   0 cadar      (501) staff       (20)     1520 2023-08-01 15:17:45.000000 easy_local_features-0.3.7/LICENSE_ALIKE.txt
+-rw-r--r--   0 cadar      (501) staff       (20)     1520 2023-07-22 09:17:15.000000 easy_local_features-0.3.7/LICENSE_ALIKED.txt
+-rw-r--r--   0 cadar      (501) staff       (20)    32722 2023-07-01 15:16:15.000000 easy_local_features-0.3.7/LICENSE_DISK.txt
+-rw-r--r--   0 cadar      (501) staff       (20)    21121 2023-07-01 17:04:24.000000 easy_local_features-0.3.7/LICENSE_R2D2.txt
+-rw-r--r--   0 cadar      (501) staff       (20)     7009 2023-07-01 16:24:52.000000 easy_local_features-0.3.7/LICENSE_SUPERGLUE.txt
+-rw-r--r--   0 cadar      (501) staff       (20)     2663 2023-08-01 15:20:45.333481 easy_local_features-0.3.7/PKG-INFO
+-rw-r--r--   0 cadar      (501) staff       (20)     2346 2023-08-01 15:18:38.000000 easy_local_features-0.3.7/README.md
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.311744 easy_local_features-0.3.7/easy_local_features/
+-rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-01 15:35:14.000000 easy_local_features-0.3.7/easy_local_features/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.313552 easy_local_features-0.3.7/easy_local_features/datasets/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-06-12 19:58:13.000000 easy_local_features-0.3.7/easy_local_features/datasets/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)    10688 2023-07-11 20:37:33.000000 easy_local_features-0.3.7/easy_local_features/datasets/augmentor.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3034 2023-06-12 19:58:13.000000 easy_local_features-0.3.7/easy_local_features/datasets/download.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.316163 easy_local_features-0.3.7/easy_local_features/feature/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/feature/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     4145 2023-08-01 15:16:47.000000 easy_local_features-0.3.7/easy_local_features/feature/baseline_alike.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3774 2023-07-23 02:12:15.000000 easy_local_features-0.3.7/easy_local_features/feature/baseline_aliked.py
+-rw-r--r--   0 cadar      (501) staff       (20)    34684 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/feature/baseline_dalf.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2624 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/feature/baseline_deal.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6746 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/feature/baseline_disk.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6012 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/feature/baseline_r2d2.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2857 2023-07-23 01:46:09.000000 easy_local_features-0.3.7/easy_local_features/feature/baseline_superpoint.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.317252 easy_local_features-0.3.7/easy_local_features/matching/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 21:59:23.000000 easy_local_features-0.3.7/easy_local_features/matching/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2075 2023-07-23 02:33:04.000000 easy_local_features-0.3.7/easy_local_features/matching/baseline_loftr.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5144 2023-07-23 02:32:46.000000 easy_local_features-0.3.7/easy_local_features/matching/baseline_superglue.py
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 22:06:22.000000 easy_local_features-0.3.7/easy_local_features/matching/core.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.317383 easy_local_features-0.3.7/easy_local_features/submodules/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:42:35.000000 easy_local_features-0.3.7/easy_local_features/submodules/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.318358 easy_local_features-0.3.7/easy_local_features/submodules/git_alike/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-08-01 14:23:20.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_alike/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6006 2023-08-01 15:13:54.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_alike/alike.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6384 2023-08-01 15:13:48.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_alike/alnet.py
+-rw-r--r--   0 cadar      (501) staff       (20)     8734 2023-08-01 14:24:15.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_alike/soft_detect.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.318780 easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-22 08:58:42.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.319212 easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/custom_ops/
+-rw-r--r--   0 cadar      (501) staff       (20)     5503 2023-07-23 02:07:54.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/custom_ops/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)      599 2023-07-22 11:59:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/custom_ops/setup.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.320500 easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/nets/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-22 08:58:50.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/nets/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     7454 2023-07-23 02:06:58.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/nets/aliked.py
+-rw-r--r--   0 cadar      (501) staff       (20)     9383 2023-07-22 12:01:18.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/nets/blocks.py
+-rw-r--r--   0 cadar      (501) staff       (20)      863 2023-07-22 08:46:52.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/nets/padder.py
+-rw-r--r--   0 cadar      (501) staff       (20)     8080 2023-07-22 08:46:52.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/nets/soft_detect.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.320774 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:23:41.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.320885 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/
+-rw-r--r--   0 cadar      (501) staff       (20)       24 2023-07-01 15:39:51.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.321282 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/common/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:40:58.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/common/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2652 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/common/structs.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.322155 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/geom/
+-rw-r--r--   0 cadar      (501) staff       (20)       79 2023-07-01 08:54:41.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/geom/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)      291 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/geom/distance_matrix.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2096 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/geom/epi.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3406 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/geom/pose.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.323371 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/model/
+-rw-r--r--   0 cadar      (501) staff       (20)      113 2023-07-01 08:54:41.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/model/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2732 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2566 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5454 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/model/detector.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2177 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/model/disk.py
+-rw-r--r--   0 cadar      (501) staff       (20)      865 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/model/nms.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.324254 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/unets/
+-rw-r--r--   0 cadar      (501) staff       (20)      249 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/unets/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     4159 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/unets/blocks.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2070 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/unets/ops.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3289 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/unets/unet.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1291 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/unets/utils.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.325465 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:53:50.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6223 2023-07-01 17:01:09.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/extract.py
+-rw-r--r--   0 cadar      (501) staff       (20)     9927 2023-07-01 16:26:30.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/extract_kapture.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.327422 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/nets/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:54.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/nets/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2360 2023-07-01 16:26:31.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/nets/ap_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1720 2023-07-01 16:26:31.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/nets/losses.py
+-rw-r--r--   0 cadar      (501) staff       (20)     7158 2023-07-01 16:26:31.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/nets/patchnet.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1760 2023-07-01 16:26:31.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2006 2023-07-01 16:26:31.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)    15031 2023-07-01 16:26:31.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/nets/sampler.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.329065 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/tools/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:23.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/tools/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1080 2023-07-01 16:26:31.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/tools/common.py
+-rw-r--r--   0 cadar      (501) staff       (20)    14318 2023-07-01 17:00:44.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/tools/dataloader.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2208 2023-07-01 16:26:31.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/tools/trainer.py
+-rw-r--r--   0 cadar      (501) staff       (20)    18298 2023-07-01 16:26:31.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/tools/transforms.py
+-rw-r--r--   0 cadar      (501) staff       (20)     7160 2023-07-01 16:26:31.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5647 2023-07-01 16:26:31.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/tools/viz.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5018 2023-07-01 16:26:31.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/train.py
+-rw-r--r--   0 cadar      (501) staff       (20)     4203 2023-07-01 16:26:31.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/viz_heatmaps.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.329527 easy_local_features-0.3.7/easy_local_features/submodules/git_superglue/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:22:28.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_superglue/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.332409 easy_local_features-0.3.7/easy_local_features/submodules/git_superglue/models/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:16:09.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_superglue/models/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3417 2023-07-01 16:16:09.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_superglue/models/matching.py
+-rw-r--r--   0 cadar      (501) staff       (20)    11537 2023-07-01 16:40:16.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_superglue/models/superglue.py
+-rw-r--r--   0 cadar      (501) staff       (20)     8092 2023-07-01 16:40:03.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_superglue/models/superpoint.py
+-rw-r--r--   0 cadar      (501) staff       (20)    20039 2023-07-01 16:16:09.000000 easy_local_features-0.3.7/easy_local_features/submodules/git_superglue/models/utils.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.333052 easy_local_features-0.3.7/easy_local_features/utils/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/utils/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)      293 2023-07-11 16:38:37.000000 easy_local_features-0.3.7/easy_local_features/utils/generic_match.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-08-01 15:20:45.312840 easy_local_features-0.3.7/easy_local_features.egg-info/
+-rw-r--r--   0 cadar      (501) staff       (20)     2663 2023-08-01 15:20:45.000000 easy_local_features-0.3.7/easy_local_features.egg-info/PKG-INFO
+-rw-r--r--   0 cadar      (501) staff       (20)     4461 2023-08-01 15:20:45.000000 easy_local_features-0.3.7/easy_local_features.egg-info/SOURCES.txt
+-rw-r--r--   0 cadar      (501) staff       (20)        1 2023-08-01 15:20:45.000000 easy_local_features-0.3.7/easy_local_features.egg-info/dependency_links.txt
+-rw-r--r--   0 cadar      (501) staff       (20)       73 2023-08-01 15:20:45.000000 easy_local_features-0.3.7/easy_local_features.egg-info/requires.txt
+-rw-r--r--   0 cadar      (501) staff       (20)       20 2023-08-01 15:20:45.000000 easy_local_features-0.3.7/easy_local_features.egg-info/top_level.txt
+-rw-r--r--   0 cadar      (501) staff       (20)       38 2023-08-01 15:20:45.333712 easy_local_features-0.3.7/setup.cfg
+-rw-r--r--   0 cadar      (501) staff       (20)     1703 2023-08-01 15:20:02.000000 easy_local_features-0.3.7/setup.py
```

### Comparing `easy_local_features-0.3.6/LICENSE_ALIKED.txt` & `easy_local_features-0.3.7/LICENSE_ALIKE.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/LICENSE_DISK.txt` & `easy_local_features-0.3.7/LICENSE_DISK.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/LICENSE_R2D2.txt` & `easy_local_features-0.3.7/LICENSE_R2D2.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/LICENSE_SUPERGLUE.txt` & `easy_local_features-0.3.7/LICENSE_SUPERGLUE.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/PKG-INFO` & `easy_local_features-0.3.7/easy_local_features.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
-Name: easy_local_features
-Version: 0.3.6
+Name: easy-local-features
+Version: 0.3.7
 Author: eucadar
 Author-email: python@eucadar.com
 Description-Content-Type: text/markdown
+License-File: LICENSE_ALIKE.txt
 License-File: LICENSE_ALIKED.txt
 License-File: LICENSE_DISK.txt
 License-File: LICENSE_R2D2.txt
 License-File: LICENSE_SUPERGLUE.txt
 
 # easy-local-features-baselines
 
@@ -41,14 +42,15 @@
 
 # How to use
 
 ```python
 from easy_local_features.feature.baseline_deal import DEAL_baseline
 # from easy_local_features.feature.baseline_dalf import DALF_baseline
 # from easy_local_features.feature.baseline_aliked import ALIKED_baseline
+# from easy_local_features.feature.baseline_alike import ALIKE_baseline
 # from easy_local_features.feature.baseline_disk import DISK_baseline
 # from easy_local_features.feature.baseline_r2d2 import R2D2_baseline
 # from easy_local_features.feature.baseline_superpoint import SuperPoint_baseline
 # from easy_local_features.matching.baseline_superglue import SuperGlue_baseline
 
 # Load an image
 img = cv2.imread("assets/notredame.png")
@@ -76,12 +78,13 @@
   - [ ] DKM
   - [ ] ASLFeat
   - [x] R2D2
   - [x] DISK
   - [x] SuperPoin
   - [x] SuperGlue
   - [x] LoFTR
+  - [x] ALIKE
   - [ ] ALIKED
     - [x] Add LICENSE file
     - [x] Test on MAC M1 with CPU
     - [ ] Test on Linux with CPU
     - [ ] Test with CUDA
```

### Comparing `easy_local_features-0.3.6/README.md` & `easy_local_features-0.3.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 # How to use
 
 ```python
 from easy_local_features.feature.baseline_deal import DEAL_baseline
 # from easy_local_features.feature.baseline_dalf import DALF_baseline
 # from easy_local_features.feature.baseline_aliked import ALIKED_baseline
+# from easy_local_features.feature.baseline_alike import ALIKE_baseline
 # from easy_local_features.feature.baseline_disk import DISK_baseline
 # from easy_local_features.feature.baseline_r2d2 import R2D2_baseline
 # from easy_local_features.feature.baseline_superpoint import SuperPoint_baseline
 # from easy_local_features.matching.baseline_superglue import SuperGlue_baseline
 
 # Load an image
 img = cv2.imread("assets/notredame.png")
@@ -65,12 +66,13 @@
   - [ ] DKM
   - [ ] ASLFeat
   - [x] R2D2
   - [x] DISK
   - [x] SuperPoin
   - [x] SuperGlue
   - [x] LoFTR
+  - [x] ALIKE
   - [ ] ALIKED
     - [x] Add LICENSE file
     - [x] Test on MAC M1 with CPU
     - [ ] Test on Linux with CPU
     - [ ] Test with CUDA
```

### Comparing `easy_local_features-0.3.6/easy_local_features/datasets/augmentor.py` & `easy_local_features-0.3.7/easy_local_features/datasets/augmentor.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/datasets/download.py` & `easy_local_features-0.3.7/easy_local_features/datasets/download.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/feature/baseline_aliked.py` & `easy_local_features-0.3.7/easy_local_features/feature/baseline_aliked.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/feature/baseline_dalf.py` & `easy_local_features-0.3.7/easy_local_features/feature/baseline_dalf.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/feature/baseline_deal.py` & `easy_local_features-0.3.7/easy_local_features/feature/baseline_deal.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/feature/baseline_disk.py` & `easy_local_features-0.3.7/easy_local_features/feature/baseline_disk.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/feature/baseline_r2d2.py` & `easy_local_features-0.3.7/easy_local_features/feature/baseline_r2d2.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/feature/baseline_superpoint.py` & `easy_local_features-0.3.7/easy_local_features/feature/baseline_superpoint.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/matching/baseline_loftr.py` & `easy_local_features-0.3.7/easy_local_features/matching/baseline_loftr.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/matching/baseline_superglue.py` & `easy_local_features-0.3.7/easy_local_features/matching/baseline_superglue.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/custom_ops/__init__.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/custom_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/custom_ops/setup.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/custom_ops/setup.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/nets/aliked.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/nets/aliked.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/nets/blocks.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/nets/blocks.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/nets/padder.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/nets/padder.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_aliked/nets/soft_detect.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_aliked/nets/soft_detect.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/common/structs.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/common/structs.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/geom/epi.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/geom/epi.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/geom/pose.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/geom/pose.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/model/detector.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/model/detector.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/model/disk.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/model/disk.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/model/nms.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/model/nms.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/unets/blocks.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/unets/blocks.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/unets/ops.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/unets/ops.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/unets/unet.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/unets/unet.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_disk/disk/unets/utils.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_disk/disk/unets/utils.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/extract.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/extract.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/extract_kapture.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/extract_kapture.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/nets/ap_loss.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/nets/ap_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/nets/losses.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/nets/losses.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/nets/patchnet.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/nets/patchnet.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/nets/sampler.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/nets/sampler.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/tools/common.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/tools/common.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/tools/dataloader.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/tools/dataloader.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/tools/trainer.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/tools/transforms.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/tools/transforms.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/tools/viz.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/tools/viz.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/train.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/train.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_r2d2/viz_heatmaps.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_r2d2/viz_heatmaps.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_superglue/models/matching.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_superglue/models/matching.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_superglue/models/superglue.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_superglue/models/superglue.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_superglue/models/superpoint.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_superglue/models/superpoint.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features/submodules/git_superglue/models/utils.py` & `easy_local_features-0.3.7/easy_local_features/submodules/git_superglue/models/utils.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.6/easy_local_features.egg-info/PKG-INFO` & `easy_local_features-0.3.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
-Name: easy-local-features
-Version: 0.3.6
+Name: easy_local_features
+Version: 0.3.7
 Author: eucadar
 Author-email: python@eucadar.com
 Description-Content-Type: text/markdown
+License-File: LICENSE_ALIKE.txt
 License-File: LICENSE_ALIKED.txt
 License-File: LICENSE_DISK.txt
 License-File: LICENSE_R2D2.txt
 License-File: LICENSE_SUPERGLUE.txt
 
 # easy-local-features-baselines
 
@@ -41,14 +42,15 @@
 
 # How to use
 
 ```python
 from easy_local_features.feature.baseline_deal import DEAL_baseline
 # from easy_local_features.feature.baseline_dalf import DALF_baseline
 # from easy_local_features.feature.baseline_aliked import ALIKED_baseline
+# from easy_local_features.feature.baseline_alike import ALIKE_baseline
 # from easy_local_features.feature.baseline_disk import DISK_baseline
 # from easy_local_features.feature.baseline_r2d2 import R2D2_baseline
 # from easy_local_features.feature.baseline_superpoint import SuperPoint_baseline
 # from easy_local_features.matching.baseline_superglue import SuperGlue_baseline
 
 # Load an image
 img = cv2.imread("assets/notredame.png")
@@ -76,12 +78,13 @@
   - [ ] DKM
   - [ ] ASLFeat
   - [x] R2D2
   - [x] DISK
   - [x] SuperPoin
   - [x] SuperGlue
   - [x] LoFTR
+  - [x] ALIKE
   - [ ] ALIKED
     - [x] Add LICENSE file
     - [x] Test on MAC M1 with CPU
     - [ ] Test on Linux with CPU
     - [ ] Test with CUDA
```

### Comparing `easy_local_features-0.3.6/easy_local_features.egg-info/SOURCES.txt` & `easy_local_features-0.3.7/easy_local_features.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE_ALIKE.txt
 LICENSE_ALIKED.txt
 LICENSE_DISK.txt
 LICENSE_R2D2.txt
 LICENSE_SUPERGLUE.txt
 README.md
 setup.py
 easy_local_features/__init__.py
@@ -10,25 +11,30 @@
 easy_local_features.egg-info/dependency_links.txt
 easy_local_features.egg-info/requires.txt
 easy_local_features.egg-info/top_level.txt
 easy_local_features/datasets/__init__.py
 easy_local_features/datasets/augmentor.py
 easy_local_features/datasets/download.py
 easy_local_features/feature/__init__.py
+easy_local_features/feature/baseline_alike.py
 easy_local_features/feature/baseline_aliked.py
 easy_local_features/feature/baseline_dalf.py
 easy_local_features/feature/baseline_deal.py
 easy_local_features/feature/baseline_disk.py
 easy_local_features/feature/baseline_r2d2.py
 easy_local_features/feature/baseline_superpoint.py
 easy_local_features/matching/__init__.py
 easy_local_features/matching/baseline_loftr.py
 easy_local_features/matching/baseline_superglue.py
 easy_local_features/matching/core.py
 easy_local_features/submodules/__init__.py
+easy_local_features/submodules/git_alike/__init__.py
+easy_local_features/submodules/git_alike/alike.py
+easy_local_features/submodules/git_alike/alnet.py
+easy_local_features/submodules/git_alike/soft_detect.py
 easy_local_features/submodules/git_aliked/__init__.py
 easy_local_features/submodules/git_aliked/custom_ops/__init__.py
 easy_local_features/submodules/git_aliked/custom_ops/setup.py
 easy_local_features/submodules/git_aliked/nets/__init__.py
 easy_local_features/submodules/git_aliked/nets/aliked.py
 easy_local_features/submodules/git_aliked/nets/blocks.py
 easy_local_features/submodules/git_aliked/nets/padder.py
```

### Comparing `easy_local_features-0.3.6/setup.py` & `easy_local_features-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                 name='easy_local_features.submodules.git_aliked.custom_ops.get_patches', 
                 sources=[CUSTOM_OPS+'get_patches_cpu.cpp']
             )
         ]
 
 setup(
     name='easy_local_features',
-    version='0.3.6',
+    version='0.3.7',
     author='eucadar',
     author_email='python@eucadar.com',
     packages=find_packages(exclude=('tests', 'docs', 'assets', 'custom_ops')),
     include_package_data=True,
     install_requires=[
         'numpy',
         'scipy',
```

