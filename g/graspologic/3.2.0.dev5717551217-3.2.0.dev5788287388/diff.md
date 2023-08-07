# Comparing `tmp/graspologic-3.2.0.dev5717551217.tar.gz` & `tmp/graspologic-3.2.0.dev5788287388.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graspologic-3.2.0.dev5717551217.tar", last modified: Mon Jul 31 17:34:05 2023, max compression
+gzip compressed data, was "graspologic-3.2.0.dev5788287388.tar", last modified: Mon Aug  7 18:14:05 2023, max compression
```

## Comparing `graspologic-3.2.0.dev5717551217.tar` & `graspologic-3.2.0.dev5788287388.tar`

### file list

```diff
@@ -1,217 +1,217 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.533059 graspologic-3.2.0.dev5717551217/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-31 17:34:05.533059 graspologic-3.2.0.dev5717551217/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.481059 graspologic-3.2.0.dev5717551217/graspologic/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.481059 graspologic-3.2.0.dev5717551217/graspologic/align/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/align/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/align/orthogonal_procrustes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/align/seedless_procrustes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/align/sign_flips.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.485059 graspologic-3.2.0.dev5717551217/graspologic/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29918 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/cluster/autogmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/cluster/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/cluster/divisive_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/cluster/gclust.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/cluster/kclust.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.485059 graspologic-3.2.0.dev5717551217/graspologic/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.485059 graspologic-3.2.0.dev5717551217/graspologic/datasets/drosophila/
--rw-r--r--   0 runner    (1001) docker     (123)    87769 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/drosophila/left_adjacency.csv
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/drosophila/left_cell_labels.csv
--rw-r--r--   0 runner    (1001) docker     (123)    91164 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/drosophila/right_adjacency.csv
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/drosophila/right_cell_labels.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.485059 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/
--rw-r--r--   0 runner    (1001) docker     (123)    19847 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/atlas.csv
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/blocks.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.505059 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/
--rw-r--r--   0 runner    (1001) docker     (123)   465335 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   417268 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   481030 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   513067 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   486685 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   502512 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   501644 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   490182 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   423952 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   410522 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   418663 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   426113 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   459110 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   456778 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   500977 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   429240 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   412281 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   486497 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   466098 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   469626 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   431457 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   408031 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   450727 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   343162 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   451278 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   496115 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   493788 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   481678 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   479782 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   416610 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   363031 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   474339 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.513059 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/
--rwxr-xr-x   0 runner    (1001) docker     (123)    33536 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54776.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33530 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54777.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33537 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54779.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33535 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54781.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33544 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54790.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54793.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33549 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54794.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33555 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54797.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33519 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54811.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33525 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54813.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33530 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54815.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33528 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54817.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33501 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54821.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33510 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54823.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33536 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54829.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33538 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54831.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33530 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54833.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33535 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54835.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33505 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54842.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33508 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54847.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33520 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54849.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33520 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54851.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33525 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54853.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33527 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54855.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54864.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54866.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54868.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33552 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54870.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33508 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54883.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33514 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54885.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33509 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54887.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33496 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54890.csv
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/participants.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.517059 graspologic-3.2.0.dev5717551217/graspologic/embed/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/embed/ase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/embed/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/embed/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/embed/lse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/embed/mase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/embed/mds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/embed/mug2vec.py
--rw-r--r--   0 runner    (1001) docker     (123)    19443 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/embed/n2v.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/embed/omni.py
--rw-r--r--   0 runner    (1001) docker     (123)    11836 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/embed/svd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.517059 graspologic-3.2.0.dev5717551217/graspologic/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/inference/binomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/inference/density_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/inference/group_connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/inference/latent_distribution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/inference/latent_position_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/inference/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.517059 graspologic-3.2.0.dev5717551217/graspologic/layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/layouts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/layouts/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/layouts/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/layouts/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.521059 graspologic-3.2.0.dev5717551217/graspologic/layouts/include/
--rw-r--r--   0 runner    (1001) docker     (123)    28486 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/layouts/include/colors-100.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.521059 graspologic-3.2.0.dev5717551217/graspologic/layouts/nooverlap/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/layouts/nooverlap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/layouts/nooverlap/_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/layouts/nooverlap/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    42453 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/layouts/nooverlap/_quad_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/layouts/nooverlap/_quad_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/layouts/nooverlap/nooverlap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/layouts/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.521059 graspologic-3.2.0.dev5717551217/graspologic/match/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/match/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/match/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/match/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/match/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.521059 graspologic-3.2.0.dev5717551217/graspologic/models/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/models/edge_swaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/models/er.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/models/rdpg.py
--rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/models/sbm_estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.521059 graspologic-3.2.0.dev5717551217/graspologic/nominate/
--rw-r--r--   0 runner    (1001) docker     (123)    16972 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/nominate/VNviaSGM.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/nominate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/nominate/spectralVN.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.525059 graspologic-3.2.0.dev5717551217/graspologic/partition/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/partition/leiden.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/partition/modularity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.525059 graspologic-3.2.0.dev5717551217/graspologic/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.525059 graspologic-3.2.0.dev5717551217/graspologic/pipeline/embed/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/pipeline/embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/pipeline/embed/_elbow.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/pipeline/embed/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/pipeline/embed/adjacency_spectral_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/pipeline/embed/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/pipeline/embed/laplacian_spectral_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/pipeline/embed/omnibus_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/pipeline/graph_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.525059 graspologic-3.2.0.dev5717551217/graspologic/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63961 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    34796 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/plot/plot_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/preconditions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.525059 graspologic-3.2.0.dev5717551217/graspologic/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/preprocessing/graph_cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.529059 graspologic-3.2.0.dev5717551217/graspologic/simulations/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/simulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/simulations/rdpg_corr.py
--rw-r--r--   0 runner    (1001) docker     (123)    38533 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/simulations/simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/simulations/simulations_corr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.529059 graspologic-3.2.0.dev5717551217/graspologic/subgraph/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/subgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/subgraph/sg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.529059 graspologic-3.2.0.dev5717551217/graspologic/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/utils/ptr.py
--rw-r--r--   0 runner    (1001) docker     (123)    40460 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/graspologic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.481059 graspologic-3.2.0.dev5717551217/graspologic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-31 17:34:05.000000 graspologic-3.2.0.dev5717551217/graspologic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-07-31 17:34:05.000000 graspologic-3.2.0.dev5717551217/graspologic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:34:05.000000 graspologic-3.2.0.dev5717551217/graspologic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-31 17:34:05.000000 graspologic-3.2.0.dev5717551217/graspologic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 17:34:05.000000 graspologic-3.2.0.dev5717551217/graspologic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-31 17:34:05.533059 graspologic-3.2.0.dev5717551217/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.477059 graspologic-3.2.0.dev5717551217/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.529059 graspologic-3.2.0.dev5717551217/tests/embed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/tests/embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/tests/embed/test_n2v.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/tests/embed/test_omni.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.529059 graspologic-3.2.0.dev5717551217/tests/layouts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/tests/layouts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.529059 graspologic-3.2.0.dev5717551217/tests/layouts/nooverlap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/tests/layouts/nooverlap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/tests/layouts/nooverlap/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/tests/layouts/nooverlap/test_grid_cell_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/tests/layouts/nooverlap/test_nooverlap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/tests/layouts/nooverlap/test_overlap_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/tests/layouts/test_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.529059 graspologic-3.2.0.dev5717551217/tests/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/tests/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/tests/pipeline/test_graph_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:05.533059 graspologic-3.2.0.dev5717551217/tests/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/tests/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-07-31 17:32:39.000000 graspologic-3.2.0.dev5717551217/tests/preprocessing/graph_cuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.558326 graspologic-3.2.0.dev5788287388/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-08-07 18:14:05.558326 graspologic-3.2.0.dev5788287388/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.514323 graspologic-3.2.0.dev5788287388/graspologic/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.514323 graspologic-3.2.0.dev5788287388/graspologic/align/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/align/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/align/orthogonal_procrustes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/align/seedless_procrustes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/align/sign_flips.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.518323 graspologic-3.2.0.dev5788287388/graspologic/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29918 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/cluster/autogmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/cluster/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/cluster/divisive_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/cluster/gclust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/cluster/kclust.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.518323 graspologic-3.2.0.dev5788287388/graspologic/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.518323 graspologic-3.2.0.dev5788287388/graspologic/datasets/drosophila/
+-rw-r--r--   0 runner    (1001) docker     (123)    87769 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/drosophila/left_adjacency.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/drosophila/left_cell_labels.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    91164 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/drosophila/right_adjacency.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/drosophila/right_cell_labels.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.518323 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/
+-rw-r--r--   0 runner    (1001) docker     (123)    19847 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/atlas.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/blocks.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.538324 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/
+-rw-r--r--   0 runner    (1001) docker     (123)   465335 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   417268 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   481030 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   513067 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   486685 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   502512 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   501644 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   490182 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   423952 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   410522 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   418663 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   426113 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   459110 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   456778 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   500977 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   429240 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   412281 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   486497 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   466098 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   469626 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   431457 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   408031 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   450727 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   343162 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   451278 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   496115 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   493788 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   481678 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   479782 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   416610 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   363031 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   474339 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.546325 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33536 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54776.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33530 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54777.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33537 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54779.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33535 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54781.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33544 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54790.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54793.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33549 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54794.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33555 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54797.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33519 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54811.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33525 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54813.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33530 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54815.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33528 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54817.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33501 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54821.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33510 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54823.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33536 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54829.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33538 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54831.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33530 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54833.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33535 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54835.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33505 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54842.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33508 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54847.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33520 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54849.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33520 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54851.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33525 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54853.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33527 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54855.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54864.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54866.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54868.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33552 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54870.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33508 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54883.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33514 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54885.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33509 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54887.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33496 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54890.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/participants.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.550325 graspologic-3.2.0.dev5788287388/graspologic/embed/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/embed/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/embed/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/embed/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/embed/lse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/embed/mase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/embed/mds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/embed/mug2vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19443 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/embed/n2v.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/embed/omni.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11836 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/embed/svd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.550325 graspologic-3.2.0.dev5788287388/graspologic/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/inference/binomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/inference/density_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/inference/group_connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/inference/latent_distribution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/inference/latent_position_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/inference/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.550325 graspologic-3.2.0.dev5788287388/graspologic/layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/layouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/layouts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/layouts/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/layouts/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/layouts/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.550325 graspologic-3.2.0.dev5788287388/graspologic/layouts/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    28486 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/layouts/include/colors-100.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.550325 graspologic-3.2.0.dev5788287388/graspologic/layouts/nooverlap/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/layouts/nooverlap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/layouts/nooverlap/_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/layouts/nooverlap/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42453 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/layouts/nooverlap/_quad_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/layouts/nooverlap/_quad_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/layouts/nooverlap/nooverlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/layouts/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.550325 graspologic-3.2.0.dev5788287388/graspologic/match/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/match/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26978 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/match/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/match/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/match/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.554325 graspologic-3.2.0.dev5788287388/graspologic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/models/edge_swaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/models/er.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/models/rdpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/models/sbm_estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.554325 graspologic-3.2.0.dev5788287388/graspologic/nominate/
+-rw-r--r--   0 runner    (1001) docker     (123)    16972 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/nominate/VNviaSGM.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/nominate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/nominate/spectralVN.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.554325 graspologic-3.2.0.dev5788287388/graspologic/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/partition/leiden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/partition/modularity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.554325 graspologic-3.2.0.dev5788287388/graspologic/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.554325 graspologic-3.2.0.dev5788287388/graspologic/pipeline/embed/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/pipeline/embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/pipeline/embed/_elbow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/pipeline/embed/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/pipeline/embed/adjacency_spectral_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/pipeline/embed/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/pipeline/embed/laplacian_spectral_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/pipeline/embed/omnibus_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/pipeline/graph_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.554325 graspologic-3.2.0.dev5788287388/graspologic/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63961 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34796 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/plot/plot_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/preconditions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.554325 graspologic-3.2.0.dev5788287388/graspologic/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/preprocessing/graph_cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.558326 graspologic-3.2.0.dev5788287388/graspologic/simulations/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/simulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/simulations/rdpg_corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38533 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/simulations/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/simulations/simulations_corr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.558326 graspologic-3.2.0.dev5788287388/graspologic/subgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/subgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/subgraph/sg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.558326 graspologic-3.2.0.dev5788287388/graspologic/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/utils/ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40460 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/graspologic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.514323 graspologic-3.2.0.dev5788287388/graspologic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-08-07 18:14:05.000000 graspologic-3.2.0.dev5788287388/graspologic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-08-07 18:14:05.000000 graspologic-3.2.0.dev5788287388/graspologic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:14:05.000000 graspologic-3.2.0.dev5788287388/graspologic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-07 18:14:05.000000 graspologic-3.2.0.dev5788287388/graspologic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 18:14:05.000000 graspologic-3.2.0.dev5788287388/graspologic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-07 18:14:05.562326 graspologic-3.2.0.dev5788287388/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.514323 graspologic-3.2.0.dev5788287388/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.558326 graspologic-3.2.0.dev5788287388/tests/embed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/tests/embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/tests/embed/test_n2v.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/tests/embed/test_omni.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.558326 graspologic-3.2.0.dev5788287388/tests/layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/tests/layouts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.558326 graspologic-3.2.0.dev5788287388/tests/layouts/nooverlap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/tests/layouts/nooverlap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/tests/layouts/nooverlap/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/tests/layouts/nooverlap/test_grid_cell_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/tests/layouts/nooverlap/test_nooverlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/tests/layouts/nooverlap/test_overlap_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/tests/layouts/test_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.558326 graspologic-3.2.0.dev5788287388/tests/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/tests/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/tests/pipeline/test_graph_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:14:05.558326 graspologic-3.2.0.dev5788287388/tests/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/tests/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-08-07 18:12:39.000000 graspologic-3.2.0.dev5788287388/tests/preprocessing/graph_cuts.py
```

### Comparing `graspologic-3.2.0.dev5717551217/LICENSE.txt` & `graspologic-3.2.0.dev5788287388/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/PKG-INFO` & `graspologic-3.2.0.dev5788287388/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graspologic
-Version: 3.2.0.dev5717551217
+Version: 3.2.0.dev5788287388
 Summary: A set of python modules for graph statistics
 Home-page: https://github.com/microsoft/graspologic
 Author: Eric Bridgeford, Jaewon Chung, Benjamin Pedigo, Bijan Varjavand
 Author-email: j1c@jhu.edu
 Maintainer: Dax Pryce
 Maintainer-email: daxpryce@microsoft.com
 License: MIT
```

### Comparing `graspologic-3.2.0.dev5717551217/README.md` & `graspologic-3.2.0.dev5788287388/README.md`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/__init__.py` & `graspologic-3.2.0.dev5788287388/graspologic/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/align/base.py` & `graspologic-3.2.0.dev5788287388/graspologic/align/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/align/orthogonal_procrustes.py` & `graspologic-3.2.0.dev5788287388/graspologic/align/orthogonal_procrustes.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/align/seedless_procrustes.py` & `graspologic-3.2.0.dev5788287388/graspologic/align/seedless_procrustes.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/align/sign_flips.py` & `graspologic-3.2.0.dev5788287388/graspologic/align/sign_flips.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/cluster/autogmm.py` & `graspologic-3.2.0.dev5788287388/graspologic/cluster/autogmm.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/cluster/base.py` & `graspologic-3.2.0.dev5788287388/graspologic/cluster/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/cluster/divisive_cluster.py` & `graspologic-3.2.0.dev5788287388/graspologic/cluster/divisive_cluster.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/cluster/gclust.py` & `graspologic-3.2.0.dev5788287388/graspologic/cluster/gclust.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/cluster/kclust.py` & `graspologic-3.2.0.dev5788287388/graspologic/cluster/kclust.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/base.py` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/drosophila/left_adjacency.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/drosophila/left_adjacency.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/drosophila/right_adjacency.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/drosophila/right_adjacency.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/atlas.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/atlas.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54776.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54776.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54777.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54777.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54779.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54779.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54781.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54781.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54790.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54790.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54793.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54793.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54794.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54794.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54797.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54797.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54811.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54811.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54813.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54813.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54815.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54815.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54817.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54817.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54821.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54821.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54823.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54823.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54829.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54829.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54831.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54831.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54833.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54833.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54835.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54835.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54842.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54842.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54847.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54847.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54849.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54849.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54851.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54851.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54853.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54853.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54855.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54855.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54864.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54864.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54866.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54866.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54868.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54868.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54870.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54870.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54883.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54883.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54885.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54885.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54887.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54887.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/features/54890.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/features/54890.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/datasets/mice/participants.csv` & `graspologic-3.2.0.dev5788287388/graspologic/datasets/mice/participants.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/embed/__init__.py` & `graspologic-3.2.0.dev5788287388/graspologic/embed/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/embed/ase.py` & `graspologic-3.2.0.dev5788287388/graspologic/embed/ase.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/embed/base.py` & `graspologic-3.2.0.dev5788287388/graspologic/embed/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/embed/case.py` & `graspologic-3.2.0.dev5788287388/graspologic/embed/case.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/embed/lse.py` & `graspologic-3.2.0.dev5788287388/graspologic/embed/lse.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/embed/mase.py` & `graspologic-3.2.0.dev5788287388/graspologic/embed/mase.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/embed/mds.py` & `graspologic-3.2.0.dev5788287388/graspologic/embed/mds.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/embed/mug2vec.py` & `graspologic-3.2.0.dev5788287388/graspologic/embed/mug2vec.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/embed/n2v.py` & `graspologic-3.2.0.dev5788287388/graspologic/embed/n2v.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/embed/omni.py` & `graspologic-3.2.0.dev5788287388/graspologic/embed/omni.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/embed/svd.py` & `graspologic-3.2.0.dev5788287388/graspologic/embed/svd.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/inference/binomial.py` & `graspologic-3.2.0.dev5788287388/graspologic/inference/binomial.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/inference/density_test.py` & `graspologic-3.2.0.dev5788287388/graspologic/inference/density_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/inference/group_connection_test.py` & `graspologic-3.2.0.dev5788287388/graspologic/inference/group_connection_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/inference/latent_distribution_test.py` & `graspologic-3.2.0.dev5788287388/graspologic/inference/latent_distribution_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/inference/latent_position_test.py` & `graspologic-3.2.0.dev5788287388/graspologic/inference/latent_position_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/inference/utils.py` & `graspologic-3.2.0.dev5788287388/graspologic/inference/utils.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/layouts/__main__.py` & `graspologic-3.2.0.dev5788287388/graspologic/layouts/__main__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/layouts/auto.py` & `graspologic-3.2.0.dev5788287388/graspologic/layouts/auto.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/layouts/colors.py` & `graspologic-3.2.0.dev5788287388/graspologic/layouts/colors.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/layouts/include/colors-100.json` & `graspologic-3.2.0.dev5788287388/graspologic/layouts/include/colors-100.json`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/layouts/nooverlap/_grid.py` & `graspologic-3.2.0.dev5788287388/graspologic/layouts/nooverlap/_grid.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/layouts/nooverlap/_node.py` & `graspologic-3.2.0.dev5788287388/graspologic/layouts/nooverlap/_node.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/layouts/nooverlap/_quad_node.py` & `graspologic-3.2.0.dev5788287388/graspologic/layouts/nooverlap/_quad_node.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/layouts/nooverlap/_quad_tree.py` & `graspologic-3.2.0.dev5788287388/graspologic/layouts/nooverlap/_quad_tree.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/layouts/nooverlap/nooverlap.py` & `graspologic-3.2.0.dev5788287388/graspologic/layouts/nooverlap/nooverlap.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/layouts/render.py` & `graspologic-3.2.0.dev5788287388/graspologic/layouts/render.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/match/solver.py` & `graspologic-3.2.0.dev5788287388/graspologic/match/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from functools import wraps
 from typing import Callable, Optional, Union
 
 import numpy as np
 from beartype import beartype
 from ot import sinkhorn
 from scipy.optimize import linear_sum_assignment
-from scipy.sparse import csr_array
 from sklearn.utils import check_scalar
 
 from graspologic.types import List, RngType, Tuple
 
 from .types import (
     AdjacencyMatrix,
     Int,
@@ -78,14 +77,15 @@
         maximize: bool = True,
         max_iter: Int = 30,
         tol: Scalar = 0.03,
         transport: bool = False,
         transport_regularizer: Scalar = 100,
         transport_tol: Scalar = 5e-2,
         transport_max_iter: Int = 1000,
+        fast: bool = True,
     ):
         # TODO check if init is doubly stochastic
         self.init = init
         check_scalar(
             init_perturbation,
             name="init_perturbation",
             target_type=(float, int),
@@ -109,14 +109,16 @@
         )
         self.transport_tol = transport_tol
         check_scalar(
             transport_max_iter, name="transport_max_iter", target_type=int, min_val=1
         )
         self.transport_max_iter = transport_max_iter
 
+        self.fast = fast
+
         if maximize:
             self.obj_func_scalar = -1
         else:
             self.obj_func_scalar = 1
 
         # convert everything to make sure they are 3D arrays (first dim is layer)
         A = _check_input_matrix(A, n_layers=None)
@@ -402,14 +404,15 @@
             self.B_ns,
             self.B_sn,
             self.AB_ns,
             self.AB_sn,
             self.BA_ns,
             self.BA_sn,
             self.S_nn,
+            fast=self.fast,
         )
         if a * self.obj_func_scalar > 0 and 0 <= -b / (2 * a) <= 1:
             alpha = -b / (2 * a)
         else:
             alpha = float(np.argmin([0, (b + a) * self.obj_func_scalar]))
         return alpha
 
@@ -534,14 +537,22 @@
             + A[i].T @ P @ B[i]
             + AB[i] @ P.T @ BA[i].T
             + BA[i].T @ P.T @ AB[i]
         )
     return grad
 
 
+def _fast_trace(X: np.ndarray, Y: np.ndarray) -> float:
+    return (X * Y.T).sum()
+
+
+def _fast_traceT(X: np.ndarray, Y: np.ndarray) -> float:
+    return (X * Y).sum()
+
+
 def _compute_coefficients(
     P: np.ndarray,
     Q: np.ndarray,
     A: MultilayerAdjacency,
     B: MultilayerAdjacency,
     AB: MultilayerAdjacency,
     BA: MultilayerAdjacency,
@@ -550,33 +561,58 @@
     B_ns: MultilayerAdjacency,
     B_sn: MultilayerAdjacency,
     AB_ns: MultilayerAdjacency,
     AB_sn: MultilayerAdjacency,
     BA_ns: MultilayerAdjacency,
     BA_sn: MultilayerAdjacency,
     S: AdjacencyMatrix,
+    fast: bool,
 ) -> Tuple[float, float]:
     R = P - Q
-    # TODO make these "smart" traces like in the scipy code, couldn't hurt
-    # TODO can also refactor to not repeat multiplications like the old code but I was
-    # finding it harder to follow that way.
+
     n_layers = len(A)
-    a_cross = 0
-    b_cross = 0
-    a_intra = 0
-    b_intra = 0
+    a_cross = 0.0
+    b_cross = 0.0
+    a_intra = 0.0
+    b_intra = 0.0
+
     for i in range(n_layers):
-        a_cross += np.trace(AB[i].T @ R @ BA[i] @ R)
-        b_cross += np.trace(AB[i].T @ R @ BA[i] @ Q) + np.trace(AB[i].T @ Q @ BA[i] @ R)
-        b_cross += np.trace(AB_ns[i].T @ R @ BA_ns[i]) + np.trace(
-            AB_sn[i].T @ BA_sn[i] @ R
-        )
-        a_intra += np.trace(A[i] @ R @ B[i].T @ R.T)
-        b_intra += np.trace(A[i] @ Q @ B[i].T @ R.T) + np.trace(A[i] @ R @ B[i].T @ Q.T)
-        b_intra += np.trace(A_ns[i].T @ R @ B_ns[i]) + np.trace(A_sn[i] @ R @ B_sn[i].T)
+        if fast:
+            # could maybe be even faster if we do `opt_einsum` or something
+            ABiTR = AB[i].T @ R
+            BAiR = BA[i] @ R
+            AiR = A[i] @ R
+            RBi = R @ B[i]
+
+            a_cross += _fast_trace(ABiTR, BAiR)
+            b_cross += _fast_trace(ABiTR, BA[i] @ Q)
+            b_cross += _fast_trace(AB[i].T @ Q, BAiR)
+            b_cross += _fast_trace(AB_ns[i].T @ R, BA_ns[i])
+            b_cross += _fast_trace(AB_sn[i].T @ BA_sn[i], R)
+
+            a_intra += _fast_traceT(AiR, RBi)
+            b_intra += _fast_traceT(A[i] @ Q, RBi)
+            b_intra += _fast_traceT(AiR, Q @ B[i])
+            b_intra += _fast_trace(A_ns[i].T @ R, B_ns[i])
+            b_intra += _fast_traceT(A_sn[i] @ R, B_sn[i])
+        else:
+            a_cross += np.trace(AB[i].T @ R @ BA[i] @ R)
+            b_cross += np.trace(AB[i].T @ R @ BA[i] @ Q) + np.trace(
+                AB[i].T @ Q @ BA[i] @ R
+            )
+            b_cross += np.trace(AB_ns[i].T @ R @ BA_ns[i]) + np.trace(
+                AB_sn[i].T @ BA_sn[i] @ R
+            )
+            a_intra += np.trace(A[i] @ R @ B[i].T @ R.T)
+            b_intra += np.trace(A[i] @ Q @ B[i].T @ R.T) + np.trace(
+                A[i] @ R @ B[i].T @ Q.T
+            )
+            b_intra += np.trace(A_ns[i].T @ R @ B_ns[i]) + np.trace(
+                A_sn[i] @ R @ B_sn[i].T
+            )
 
     a = a_cross + a_intra
     b = b_cross + b_intra
     b += np.sum(S * R)  # equivalent to S.T @ R
 
     return a, b
```

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/match/types.py` & `graspologic-3.2.0.dev5788287388/graspologic/match/types.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/match/wrappers.py` & `graspologic-3.2.0.dev5788287388/graspologic/match/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     tol: Scalar = 0.01,
     verbose: Int = 0,
     rng: Optional[RngType] = None,
     transport: bool = False,
     transport_regularizer: Scalar = 100,
     transport_tol: Scalar = 5e-2,
     transport_max_iter: Int = 1000,
+    fast: bool = True,
 ) -> MatchResult:
     """
     Attempts to solve the Graph Matching Problem or the Quadratic Assignment Problem
     (QAP) through an implementation of the Fast Approximate QAP (FAQ) Algorithm [1].
 
     This algorithm can be thought of as finding an alignment of the vertices of two
     graphs which minimizes the number of induced edge disagreements, or, in the case
@@ -188,14 +189,20 @@
         computation time.
 
     transport_max_iter : int, default=1000
         Must be positive. Maximum number of iterations for the optimal transport solver.
         Setting this value higher may provide more precise solutions at the cost of
         longer computation time.
 
+    fast: bool, default=True
+        Whether to use numerical shortcuts to speed up the computation. Typically will
+        be faster for most applications, although requires storing intermediate
+        computations in memory which may be undesirable for very large inputs or when
+        memory is a bottleneck.
+
     Returns
     -------
     res: MatchResult
         ``MatchResult`` containing the following fields.
 
         indices_A : ndarray
             Sorted indices in ``A`` which were matched.
@@ -277,24 +284,24 @@
         B=B,
         AB=AB,
         BA=BA,
         S=S,
         partial_match=partial_match,
         init=init,
         init_perturbation=init_perturbation,
-        verbose=solver_verbose,
         shuffle_input=shuffle_input,
         padding=padding,
         maximize=maximize,
         max_iter=max_iter,
         tol=tol,
         transport=transport,
         transport_regularizer=transport_regularizer,
         transport_tol=transport_tol,
         transport_max_iter=transport_max_iter,
+        fast=fast,
     )
 
     def run_single_graph_matching(seed: RngType) -> MatchResult:
         solver.solve(seed)
         matching = solver.matching_
         indices_A = matching[:, 0]
         indices_B = matching[:, 1]
```

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/models/base.py` & `graspologic-3.2.0.dev5788287388/graspologic/models/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/models/edge_swaps.py` & `graspologic-3.2.0.dev5788287388/graspologic/models/edge_swaps.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/models/er.py` & `graspologic-3.2.0.dev5788287388/graspologic/models/er.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/models/rdpg.py` & `graspologic-3.2.0.dev5788287388/graspologic/models/rdpg.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/models/sbm_estimators.py` & `graspologic-3.2.0.dev5788287388/graspologic/models/sbm_estimators.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/nominate/VNviaSGM.py` & `graspologic-3.2.0.dev5788287388/graspologic/nominate/VNviaSGM.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/nominate/spectralVN.py` & `graspologic-3.2.0.dev5788287388/graspologic/nominate/spectralVN.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/partition/leiden.py` & `graspologic-3.2.0.dev5788287388/graspologic/partition/leiden.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/partition/modularity.py` & `graspologic-3.2.0.dev5788287388/graspologic/partition/modularity.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/pipeline/__init__.py` & `graspologic-3.2.0.dev5788287388/graspologic/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/pipeline/embed/__init__.py` & `graspologic-3.2.0.dev5788287388/graspologic/pipeline/embed/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/pipeline/embed/_elbow.py` & `graspologic-3.2.0.dev5788287388/graspologic/pipeline/embed/_elbow.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/pipeline/embed/adjacency_spectral_embedding.py` & `graspologic-3.2.0.dev5788287388/graspologic/pipeline/embed/adjacency_spectral_embedding.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/pipeline/embed/embeddings.py` & `graspologic-3.2.0.dev5788287388/graspologic/pipeline/embed/embeddings.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/pipeline/embed/laplacian_spectral_embedding.py` & `graspologic-3.2.0.dev5788287388/graspologic/pipeline/embed/laplacian_spectral_embedding.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/pipeline/embed/omnibus_embedding.py` & `graspologic-3.2.0.dev5788287388/graspologic/pipeline/embed/omnibus_embedding.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/pipeline/graph_builder.py` & `graspologic-3.2.0.dev5788287388/graspologic/pipeline/graph_builder.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/plot/__init__.py` & `graspologic-3.2.0.dev5788287388/graspologic/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/plot/plot.py` & `graspologic-3.2.0.dev5788287388/graspologic/plot/plot.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/plot/plot_matrix.py` & `graspologic-3.2.0.dev5788287388/graspologic/plot/plot_matrix.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/preconditions.py` & `graspologic-3.2.0.dev5788287388/graspologic/preconditions.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/preprocessing/__init__.py` & `graspologic-3.2.0.dev5788287388/graspologic/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/preprocessing/graph_cuts.py` & `graspologic-3.2.0.dev5788287388/graspologic/preprocessing/graph_cuts.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/simulations/rdpg_corr.py` & `graspologic-3.2.0.dev5788287388/graspologic/simulations/rdpg_corr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/simulations/simulations.py` & `graspologic-3.2.0.dev5788287388/graspologic/simulations/simulations.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/simulations/simulations_corr.py` & `graspologic-3.2.0.dev5788287388/graspologic/simulations/simulations_corr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/subgraph/sg.py` & `graspologic-3.2.0.dev5788287388/graspologic/subgraph/sg.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/types.py` & `graspologic-3.2.0.dev5788287388/graspologic/types.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/utils/__init__.py` & `graspologic-3.2.0.dev5788287388/graspologic/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/utils/ptr.py` & `graspologic-3.2.0.dev5788287388/graspologic/utils/ptr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/utils/utils.py` & `graspologic-3.2.0.dev5788287388/graspologic/utils/utils.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic/version.py` & `graspologic-3.2.0.dev5788287388/graspologic/version.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic.egg-info/PKG-INFO` & `graspologic-3.2.0.dev5788287388/graspologic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graspologic
-Version: 3.2.0.dev5717551217
+Version: 3.2.0.dev5788287388
 Summary: A set of python modules for graph statistics
 Home-page: https://github.com/microsoft/graspologic
 Author: Eric Bridgeford, Jaewon Chung, Benjamin Pedigo, Bijan Varjavand
 Author-email: j1c@jhu.edu
 Maintainer: Dax Pryce
 Maintainer-email: daxpryce@microsoft.com
 License: MIT
```

### Comparing `graspologic-3.2.0.dev5717551217/graspologic.egg-info/SOURCES.txt` & `graspologic-3.2.0.dev5788287388/graspologic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/graspologic.egg-info/requires.txt` & `graspologic-3.2.0.dev5788287388/graspologic.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/setup.cfg` & `graspologic-3.2.0.dev5788287388/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -61,10 +61,10 @@
 	pytest-cov>=3.0.0
 	sphinx>=4.2.0
 	sphinxcontrib-rawfiles>=0.1.1
 	sphinx-rtd-theme>=1.0.0
 	testfixtures>=6.18.3
 
 [egg_info]
-tag_build = dev5717551217
+tag_build = dev5788287388
 tag_date = 0
```

### Comparing `graspologic-3.2.0.dev5717551217/tests/embed/test_n2v.py` & `graspologic-3.2.0.dev5788287388/tests/embed/test_n2v.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/tests/embed/test_omni.py` & `graspologic-3.2.0.dev5788287388/tests/embed/test_omni.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/tests/layouts/nooverlap/test_grid.py` & `graspologic-3.2.0.dev5788287388/tests/layouts/nooverlap/test_grid.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/tests/layouts/nooverlap/test_grid_cell_creation.py` & `graspologic-3.2.0.dev5788287388/tests/layouts/nooverlap/test_grid_cell_creation.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/tests/layouts/nooverlap/test_nooverlap.py` & `graspologic-3.2.0.dev5788287388/tests/layouts/nooverlap/test_nooverlap.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/tests/layouts/nooverlap/test_overlap_check.py` & `graspologic-3.2.0.dev5788287388/tests/layouts/nooverlap/test_overlap_check.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/tests/layouts/test_auto.py` & `graspologic-3.2.0.dev5788287388/tests/layouts/test_auto.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/tests/pipeline/test_graph_builder.py` & `graspologic-3.2.0.dev5788287388/tests/pipeline/test_graph_builder.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.2.0.dev5717551217/tests/preprocessing/graph_cuts.py` & `graspologic-3.2.0.dev5788287388/tests/preprocessing/graph_cuts.py`

 * *Files identical despite different names*

