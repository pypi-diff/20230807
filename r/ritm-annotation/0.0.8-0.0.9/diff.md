# Comparing `tmp/ritm_annotation-0.0.8.tar.gz` & `tmp/ritm_annotation-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ritm_annotation-0.0.8.tar", last modified: Wed Aug  2 01:26:04 2023, max compression
+gzip compressed data, was "ritm_annotation-0.0.9.tar", last modified: Mon Aug  7 17:46:40 2023, max compression
```

## Comparing `ritm_annotation-0.0.8.tar` & `ritm_annotation-0.0.9.tar`

### file list

```diff
@@ -1,152 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.106387 ritm_annotation-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-02 01:26:04.106387 ritm_annotation-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/cli/annotate/
--rw-r--r--   0 runner    (1001) docker     (123)    24763 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/annotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/annotate/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/annotate/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/annotate/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/cli/dataset_lint/
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/dataset_lint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/cli/finetune/
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/finetune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/finetune/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/cli/model_info/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/model_info/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/cli/train/
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/cli/train/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.094386 ritm_annotation-0.0.8/ritm_annotation/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/berkeley.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/coco_lvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/davis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/grabcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/images_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/lvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/openimages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/pascalvoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/datasets/sbd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/data/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.094386 ritm_annotation-0.0.8/ritm_annotation/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/engine/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22091 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/engine/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.094386 ritm_annotation-0.0.8/ritm_annotation/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/clicker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.094386 ritm_annotation-0.0.8/ritm_annotation/inference/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/predictors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/predictors/brs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/predictors/brs_functors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/predictors/brs_losses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.098386 ritm_annotation-0.0.8/ritm_annotation/inference/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/transforms/crops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/transforms/flip.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/transforms/limit_longest_side.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/transforms/zoom_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/inference/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.098386 ritm_annotation-0.0.8/ritm_annotation/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/is_deeplab_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/is_hrnet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/is_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.098386 ritm_annotation-0.0.8/ritm_annotation/model/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modeling/basic_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modeling/deeplab_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modeling/hrnet_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modeling/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modeling/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modeling/resnetv1b.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/modifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/model/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.098386 ritm_annotation-0.0.8/ritm_annotation/models/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.102386 ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3534 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_bce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3463 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_fl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_nfl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3443 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_softiou.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.102386 ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet18_cocolvis_itermask_3p.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet18_sbd_itermask_3p.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet18s_cocolvis_itermask_3p.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet32_cocolvis_itermask_3p.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.102386 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3546 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_ade20k.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3541 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_coco.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3527 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_cocolvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3473 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_lvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3536 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_openimages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3517 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_sbd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3761 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_vocsbd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3385 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_ade20k.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3356 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_coco.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3345 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_cocolvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3313 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_lvis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3376 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_openimages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3356 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_sbd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3627 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_vocsbd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/models/test_exposed_model_stuff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.106387 ritm_annotation-0.0.8/ritm_annotation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.106387 ritm_annotation-0.0.8/ritm_annotation/utils/cython/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/cython/_get_dist_maps.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/cython/_get_dist_maps.pyxbld
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/cython/dist_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/exp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.106387 ritm_annotation-0.0.8/ritm_annotation/utils/exp_imports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/exp_imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/exp_imports/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/ritm_annotation/utils/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.090386 ritm_annotation-0.0.8/ritm_annotation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-02 01:26:04.000000 ritm_annotation-0.0.8/ritm_annotation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-08-02 01:26:04.000000 ritm_annotation-0.0.8/ritm_annotation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 01:26:04.000000 ritm_annotation-0.0.8/ritm_annotation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 01:26:04.000000 ritm_annotation-0.0.8/ritm_annotation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-02 01:26:04.000000 ritm_annotation-0.0.8/ritm_annotation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 01:26:04.000000 ritm_annotation-0.0.8/ritm_annotation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 01:26:04.106387 ritm_annotation-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:26:04.106387 ritm_annotation-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-02 01:25:51.000000 ritm_annotation-0.0.8/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.379608 ritm_annotation-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-07 17:46:40.379608 ritm_annotation-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.355607 ritm_annotation-0.0.9/ritm_annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.355607 ritm_annotation-0.0.9/ritm_annotation/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/cli/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.359607 ritm_annotation-0.0.9/ritm_annotation/cli/annotate/
+-rw-r--r--   0 runner    (1001) docker     (123)    24763 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/cli/annotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/cli/annotate/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/cli/annotate/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/cli/annotate/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.359607 ritm_annotation-0.0.9/ritm_annotation/cli/dataset_lint/
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/cli/dataset_lint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.359607 ritm_annotation-0.0.9/ritm_annotation/cli/finetune/
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/cli/finetune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/cli/finetune/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.359607 ritm_annotation-0.0.9/ritm_annotation/cli/model_info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/cli/model_info/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.359607 ritm_annotation-0.0.9/ritm_annotation/cli/train/
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/cli/train/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.359607 ritm_annotation-0.0.9/ritm_annotation/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.363607 ritm_annotation-0.0.9/ritm_annotation/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/datasets/berkeley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/datasets/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/datasets/coco_lvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/datasets/davis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/datasets/grabcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/datasets/images_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/datasets/lvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/datasets/openimages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/datasets/pascalvoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/datasets/sbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/data/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.363607 ritm_annotation-0.0.9/ritm_annotation/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/engine/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22091 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/engine/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.363607 ritm_annotation-0.0.9/ritm_annotation/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/clicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.367607 ritm_annotation-0.0.9/ritm_annotation/inference/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/predictors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/predictors/brs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/predictors/brs_functors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/predictors/brs_losses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.367607 ritm_annotation-0.0.9/ritm_annotation/inference/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/transforms/crops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/transforms/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/transforms/limit_longest_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/transforms/zoom_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/inference/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.367607 ritm_annotation-0.0.9/ritm_annotation/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/is_deeplab_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/is_hrnet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/is_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.367607 ritm_annotation-0.0.9/ritm_annotation/model/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/modeling/basic_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/modeling/deeplab_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/modeling/hrnet_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/modeling/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/modeling/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/modeling/resnetv1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/model/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.367607 ritm_annotation-0.0.9/ritm_annotation/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.367607 ritm_annotation-0.0.9/ritm_annotation/models/cocolvis_loss_ablation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/cocolvis_loss_ablation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3534 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_bce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3463 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_fl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_nfl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3443 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_softiou.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.367607 ritm_annotation-0.0.9/ritm_annotation/models/iter_mask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/iter_mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/iter_mask/hrnet18_cocolvis_itermask_3p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/iter_mask/hrnet18_sbd_itermask_3p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/iter_mask/hrnet18s_cocolvis_itermask_3p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/iter_mask/hrnet32_cocolvis_itermask_3p.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.375607 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3546 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_ade20k.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3541 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_coco.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3527 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_cocolvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3473 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_lvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3536 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_openimages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3517 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_sbd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3761 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_vocsbd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3385 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/r34_dh128_ade20k.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3356 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/r34_dh128_coco.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3345 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/r34_dh128_cocolvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3313 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/r34_dh128_lvis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3376 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/r34_dh128_openimages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3356 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/r34_dh128_sbd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3627 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/r34_dh128_vocsbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/models/test_exposed_model_stuff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.379608 ritm_annotation-0.0.9/ritm_annotation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.379608 ritm_annotation-0.0.9/ritm_annotation/utils/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/cython/_get_dist_maps.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/cython/_get_dist_maps.pyxbld
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/cython/dist_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/exp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.379608 ritm_annotation-0.0.9/ritm_annotation/utils/exp_imports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/exp_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/exp_imports/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/ritm_annotation/utils/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.355607 ritm_annotation-0.0.9/ritm_annotation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-07 17:46:40.000000 ritm_annotation-0.0.9/ritm_annotation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-08-07 17:46:40.000000 ritm_annotation-0.0.9/ritm_annotation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 17:46:40.000000 ritm_annotation-0.0.9/ritm_annotation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-07 17:46:40.000000 ritm_annotation-0.0.9/ritm_annotation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-07 17:46:40.000000 ritm_annotation-0.0.9/ritm_annotation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 17:46:40.000000 ritm_annotation-0.0.9/ritm_annotation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 17:46:40.379608 ritm_annotation-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:40.379608 ritm_annotation-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 17:46:29.000000 ritm_annotation-0.0.9/tests/test_base.py
```

### Comparing `ritm_annotation-0.0.8/LICENSE` & `ritm_annotation-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/PKG-INFO` & `ritm_annotation-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ritm_annotation
-Version: 0.0.8
+Version: 0.0.9
 Summary: Awesome ritm_annotation created by lucasew
 Home-page: https://github.com/lucasew/ritm_annotation/
 Author: lucasew
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `ritm_annotation-0.0.8/README.md` & `ritm_annotation-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/cli/__init__.py` & `ritm_annotation-0.0.9/ritm_annotation/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/cli/annotate/__init__.py` & `ritm_annotation-0.0.9/ritm_annotation/cli/annotate/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/cli/annotate/canvas.py` & `ritm_annotation-0.0.9/ritm_annotation/cli/annotate/canvas.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/cli/annotate/controller.py` & `ritm_annotation-0.0.9/ritm_annotation/cli/annotate/controller.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/cli/annotate/wrappers.py` & `ritm_annotation-0.0.9/ritm_annotation/cli/annotate/wrappers.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/cli/dataset_lint/__init__.py` & `ritm_annotation-0.0.9/ritm_annotation/cli/dataset_lint/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/cli/finetune/__init__.py` & `ritm_annotation-0.0.9/ritm_annotation/cli/finetune/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import os
 from pathlib import Path
 
 import torch
 
+from ritm_annotation.utils.env import load_cfg_from_env
 from ritm_annotation.utils.exp import init_experiment
 from ritm_annotation.utils.misc import load_module
 
 from .dataset import (
     AnnotationDataset,
     get_points_sampler,
     get_train_augmentator,
@@ -148,21 +149,15 @@
         model_script = load_module(model_path)
 
         model_base_name = model_script.__dict__.get("MODEL_NAME")
 
         args.distributed = "WORLD_SIZE" in os.environ
         cfg = init_experiment(args, model_base_name)
         cfg.weights = args.weights
-        for k, v in os.environ.items():
-            if k.startswith("RITM_"):
-                cfgkey = k.replace("RITM_", "")
-                logger.warning(
-                    f"Changing configuration entry from environment variable: {cfgkey}={v}"  # noqa:E501
-                )  # noqa: E501
-                cfg[cfgkey] = v
+        cfg = load_cfg_from_env(cfg, os.environ)
 
         torch.backends.cudnn.benchmark = True
         torch.multiprocessing.set_sharing_strategy("file_system")
         logger.debug("Basic validations passed")
         model, model_cfg = model_script.init_model(cfg)
 
         train_augmentator = get_train_augmentator(model_cfg)
```

### Comparing `ritm_annotation-0.0.8/ritm_annotation/cli/finetune/dataset.py` & `ritm_annotation-0.0.9/ritm_annotation/cli/finetune/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 class AnnotationDataset(ISDataset):
     def __init__(
         self,
         images_path: Path,
         masks_path: Path,
         split="train",
         dry_run=False,
-
         # the idea here is to resize the image to speed up data ingestion and training  # noqa:E501
         max_bigger_dimension=None,
         **kwargs,
     ):
         super(AnnotationDataset, self).__init__(**kwargs)
         self.images_path = images_path
         self.masks_path = masks_path
```

### Comparing `ritm_annotation-0.0.8/ritm_annotation/cli/model_info/__init__.py` & `ritm_annotation-0.0.9/ritm_annotation/cli/model_info/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/cli/train/__init__.py` & `ritm_annotation-0.0.9/ritm_annotation/cli/train/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,21 +132,15 @@
 
         model_script = load_module(model_path)
 
         model_base_name = model_script.__dict__.get("MODEL_NAME")
 
         args.distributed = "WORLD_SIZE" in os.environ
         cfg = init_experiment(args, model_base_name)
-        for k, v in os.environ.items():
-            if k.startswith("RITM_"):
-                cfgkey = k.replace("RITM_", "")
-                logger.warning(
-                    f"Changing configuration entry from environment variable: {cfgkey}={v}"  # noqa:E501
-                )  # noqa: E501
-                cfg[cfgkey] = v
+        cfg = load_cfg_from_env(cfg, os.environ)
 
         torch.backends.cudnn.benchmark = True
         torch.multiprocessing.set_sharing_strategy("file_system")
         logger.debug("Basic validations passed")
         model, model_cfg = model_script.init_model(cfg)
         trainer = model_script.get_trainer(model, cfg, model_cfg)
         if args.num_epochs is None:
```

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/base.py` & `ritm_annotation-0.0.9/ritm_annotation/data/base.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/compose.py` & `ritm_annotation-0.0.9/ritm_annotation/data/compose.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/datasets/__init__.py` & `ritm_annotation-0.0.9/ritm_annotation/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/datasets/ade20k.py` & `ritm_annotation-0.0.9/ritm_annotation/data/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/datasets/coco.py` & `ritm_annotation-0.0.9/ritm_annotation/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/datasets/coco_lvis.py` & `ritm_annotation-0.0.9/ritm_annotation/data/datasets/coco_lvis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/datasets/davis.py` & `ritm_annotation-0.0.9/ritm_annotation/data/datasets/davis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/datasets/grabcut.py` & `ritm_annotation-0.0.9/ritm_annotation/data/datasets/grabcut.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/datasets/images_dir.py` & `ritm_annotation-0.0.9/ritm_annotation/data/datasets/images_dir.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/datasets/lvis.py` & `ritm_annotation-0.0.9/ritm_annotation/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/datasets/openimages.py` & `ritm_annotation-0.0.9/ritm_annotation/data/datasets/openimages.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/datasets/pascalvoc.py` & `ritm_annotation-0.0.9/ritm_annotation/data/datasets/pascalvoc.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/datasets/sbd.py` & `ritm_annotation-0.0.9/ritm_annotation/data/datasets/sbd.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/points_sampler.py` & `ritm_annotation-0.0.9/ritm_annotation/data/points_sampler.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/sample.py` & `ritm_annotation-0.0.9/ritm_annotation/data/sample.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/data/transforms.py` & `ritm_annotation-0.0.9/ritm_annotation/data/transforms.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/engine/optimizer.py` & `ritm_annotation-0.0.9/ritm_annotation/engine/optimizer.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/engine/trainer.py` & `ritm_annotation-0.0.9/ritm_annotation/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/inference/clicker.py` & `ritm_annotation-0.0.9/ritm_annotation/inference/clicker.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/inference/evaluation.py` & `ritm_annotation-0.0.9/ritm_annotation/inference/evaluation.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/inference/predictors/__init__.py` & `ritm_annotation-0.0.9/ritm_annotation/inference/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/inference/predictors/base.py` & `ritm_annotation-0.0.9/ritm_annotation/inference/predictors/base.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/inference/predictors/brs.py` & `ritm_annotation-0.0.9/ritm_annotation/inference/predictors/brs.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/inference/predictors/brs_functors.py` & `ritm_annotation-0.0.9/ritm_annotation/inference/predictors/brs_functors.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/inference/predictors/brs_losses.py` & `ritm_annotation-0.0.9/ritm_annotation/inference/predictors/brs_losses.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/inference/transforms/base.py` & `ritm_annotation-0.0.9/ritm_annotation/inference/transforms/base.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/inference/transforms/crops.py` & `ritm_annotation-0.0.9/ritm_annotation/inference/transforms/crops.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/inference/transforms/flip.py` & `ritm_annotation-0.0.9/ritm_annotation/inference/transforms/flip.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/inference/transforms/limit_longest_side.py` & `ritm_annotation-0.0.9/ritm_annotation/inference/transforms/limit_longest_side.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/inference/transforms/zoom_in.py` & `ritm_annotation-0.0.9/ritm_annotation/inference/transforms/zoom_in.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/inference/utils.py` & `ritm_annotation-0.0.9/ritm_annotation/inference/utils.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/model/initializer.py` & `ritm_annotation-0.0.9/ritm_annotation/model/initializer.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/model/is_deeplab_model.py` & `ritm_annotation-0.0.9/ritm_annotation/model/is_deeplab_model.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/model/is_hrnet_model.py` & `ritm_annotation-0.0.9/ritm_annotation/model/is_hrnet_model.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/model/is_model.py` & `ritm_annotation-0.0.9/ritm_annotation/model/is_model.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/model/losses.py` & `ritm_annotation-0.0.9/ritm_annotation/model/losses.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/model/metrics.py` & `ritm_annotation-0.0.9/ritm_annotation/model/metrics.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/model/modeling/basic_blocks.py` & `ritm_annotation-0.0.9/ritm_annotation/model/modeling/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/model/modeling/deeplab_v3.py` & `ritm_annotation-0.0.9/ritm_annotation/model/modeling/deeplab_v3.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/model/modeling/hrnet_ocr.py` & `ritm_annotation-0.0.9/ritm_annotation/model/modeling/hrnet_ocr.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/model/modeling/ocr.py` & `ritm_annotation-0.0.9/ritm_annotation/model/modeling/ocr.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/model/modeling/resnet.py` & `ritm_annotation-0.0.9/ritm_annotation/model/modeling/resnet.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/model/modeling/resnetv1b.py` & `ritm_annotation-0.0.9/ritm_annotation/model/modeling/resnetv1b.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/model/ops.py` & `ritm_annotation-0.0.9/ritm_annotation/model/ops.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_bce.py` & `ritm_annotation-0.0.9/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_bce.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_fl.py` & `ritm_annotation-0.0.9/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_fl.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_nfl.py` & `ritm_annotation-0.0.9/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_nfl.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_softiou.py` & `ritm_annotation-0.0.9/ritm_annotation/models/cocolvis_loss_ablation/hrnet18_ocr64_softiou.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet18_cocolvis_itermask_3p.py` & `ritm_annotation-0.0.9/ritm_annotation/models/iter_mask/hrnet18_cocolvis_itermask_3p.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet18_sbd_itermask_3p.py` & `ritm_annotation-0.0.9/ritm_annotation/models/iter_mask/hrnet18_sbd_itermask_3p.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet18s_cocolvis_itermask_3p.py` & `ritm_annotation-0.0.9/ritm_annotation/models/iter_mask/hrnet18s_cocolvis_itermask_3p.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/iter_mask/hrnet32_cocolvis_itermask_3p.py` & `ritm_annotation-0.0.9/ritm_annotation/models/iter_mask/hrnet32_cocolvis_itermask_3p.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_ade20k.py` & `ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_ade20k.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_coco.py` & `ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_coco.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_cocolvis.py` & `ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_cocolvis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_lvis.py` & `ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_lvis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_openimages.py` & `ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_openimages.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_sbd.py` & `ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_sbd.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_vocsbd.py` & `ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/hrnet18_ocr64_vocsbd.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_ade20k.py` & `ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/r34_dh128_ade20k.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_coco.py` & `ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/r34_dh128_coco.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_cocolvis.py` & `ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/r34_dh128_cocolvis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_lvis.py` & `ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/r34_dh128_lvis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_openimages.py` & `ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/r34_dh128_openimages.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_sbd.py` & `ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/r34_dh128_sbd.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/noniterative_baselines/r34_dh128_vocsbd.py` & `ritm_annotation-0.0.9/ritm_annotation/models/noniterative_baselines/r34_dh128_vocsbd.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/models/test_exposed_model_stuff.py` & `ritm_annotation-0.0.9/ritm_annotation/models/test_exposed_model_stuff.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "model_file",
     all_models,
     ids=[f"{x.parent.name}/{x.name}" for x in all_models],
 )
 def test_model_exposes_the_right_stuff(model_file):
     model_script = load_module(model_file)
 
-    assert type(model_script.MODEL_NAME) == str
+    assert isinstance(model_script.MODEL_NAME, str)
     assert (
         model_script.__dict__.get("main") is None
     ), "Remove the main function"
 
     cfg = edict()
     cfg.device = "cpu"
     cfg.batch_size = -1  # use default
@@ -41,11 +41,11 @@
     cfg.start_epoch = 0
 
     model, model_cfg = model_script.init_model(cfg, dry_run=True)
     trainer = model_script.get_trainer(
         model, cfg, model_cfg, dry_run=True, no_dataset=True
     )
 
-    assert type(model_cfg.default_num_epochs) == int
-    assert type(trainer) == ISTrainer
+    assert isinstance(model_cfg.default_num_epochs, int)
+    assert isinstance(trainer, ISTrainer)
     assert trainer.trainset is None  # test handling of no_dataset
     assert trainer.valset is None
```

### Comparing `ritm_annotation-0.0.8/ritm_annotation/utils/cython/_get_dist_maps.pyx` & `ritm_annotation-0.0.9/ritm_annotation/utils/cython/_get_dist_maps.pyx`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/utils/distributed.py` & `ritm_annotation-0.0.9/ritm_annotation/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/utils/exp.py` & `ritm_annotation-0.0.9/ritm_annotation/utils/exp.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,17 @@
 
 def find_resume_exp(exp_parent_path, exp_pattern):
     candidates = sorted(exp_parent_path.glob(f"{exp_pattern}*"))
     if len(candidates) == 0:
         print(
             f'No experiments could be found that satisfies the pattern = "*{exp_pattern}"'  # noqa:E501
         )
+        print(
+            f"Candidates: {' '.join([e.name for e in exp_parent_path.iterdir()])}"  # noqa: E501
+        )
         sys.exit(1)
     elif len(candidates) > 1:
         print("More than one experiment found:")
         for x in candidates:
             print(x)
         sys.exit(1)
     else:
```

### Comparing `ritm_annotation-0.0.8/ritm_annotation/utils/exp_imports/default.py` & `ritm_annotation-0.0.9/ritm_annotation/utils/exp_imports/default.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/utils/log.py` & `ritm_annotation-0.0.9/ritm_annotation/utils/log.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/utils/misc.py` & `ritm_annotation-0.0.9/ritm_annotation/utils/misc.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/utils/serialization.py` & `ritm_annotation-0.0.9/ritm_annotation/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation/utils/vis.py` & `ritm_annotation-0.0.9/ritm_annotation/utils/vis.py`

 * *Files identical despite different names*

### Comparing `ritm_annotation-0.0.8/ritm_annotation.egg-info/PKG-INFO` & `ritm_annotation-0.0.9/ritm_annotation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ritm-annotation
-Version: 0.0.8
+Version: 0.0.9
 Summary: Awesome ritm_annotation created by lucasew
 Home-page: https://github.com/lucasew/ritm_annotation/
 Author: lucasew
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `ritm_annotation-0.0.8/ritm_annotation.egg-info/SOURCES.txt` & `ritm_annotation-0.0.9/ritm_annotation.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -105,18 +105,20 @@
 ritm_annotation/models/noniterative_baselines/r34_dh128_lvis.py
 ritm_annotation/models/noniterative_baselines/r34_dh128_openimages.py
 ritm_annotation/models/noniterative_baselines/r34_dh128_sbd.py
 ritm_annotation/models/noniterative_baselines/r34_dh128_vocsbd.py
 ritm_annotation/utils/README.md
 ritm_annotation/utils/__init__.py
 ritm_annotation/utils/distributed.py
+ritm_annotation/utils/env.py
 ritm_annotation/utils/exp.py
 ritm_annotation/utils/log.py
 ritm_annotation/utils/misc.py
 ritm_annotation/utils/serialization.py
+ritm_annotation/utils/test_env.py
 ritm_annotation/utils/vis.py
 ritm_annotation/utils/cython/__init__.py
 ritm_annotation/utils/cython/_get_dist_maps.pyx
 ritm_annotation/utils/cython/_get_dist_maps.pyxbld
 ritm_annotation/utils/cython/dist_maps.py
 ritm_annotation/utils/exp_imports/__init__.py
 ritm_annotation/utils/exp_imports/default.py
```

### Comparing `ritm_annotation-0.0.8/setup.py` & `ritm_annotation-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
             "*",
             ["ritm_annotation/**/*.pyx"],
             include_dirs=includes,
             libraries=libraries,
         ))
     return modules
 
+
 setup(
     name="ritm_annotation",
     version=read("ritm_annotation", "VERSION"),
     description="Awesome ritm_annotation created by lucasew",
     url="https://github.com/lucasew/ritm_annotation/",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
```

