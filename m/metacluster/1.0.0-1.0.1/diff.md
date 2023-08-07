# Comparing `tmp/metacluster-1.0.0.tar.gz` & `tmp/metacluster-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metacluster-1.0.0.tar", last modified: Fri Aug  4 10:44:53 2023, max compression
+gzip compressed data, was "metacluster-1.0.1.tar", last modified: Mon Aug  7 11:30:45 2023, max compression
```

## Comparing `metacluster-1.0.0.tar` & `metacluster-1.0.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:44:53.606516 metacluster-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-04 10:43:56.000000 metacluster-1.0.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-04 10:43:56.000000 metacluster-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-04 10:43:56.000000 metacluster-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-04 10:43:56.000000 metacluster-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-08-04 10:44:53.606516 metacluster-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-08-04 10:43:56.000000 metacluster-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:44:53.590515 metacluster-1.0.0/metacluster/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:44:53.606516 metacluster-1.0.0/metacluster/data/
--rw-r--r--   0 runner    (1001) docker     (123)   369879 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Arrhythmia.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Blood.csv
--rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/BreastCancer.csv
--rw-r--r--   0 runner    (1001) docker     (123)   119681 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/BreastEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/CongressEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)   498322 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Digits.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Glass.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/HeartEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)   438254 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Hill-valley.csv
--rw-r--r--   0 runner    (1001) docker     (123)    37338 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Horse.csv
--rw-r--r--   0 runner    (1001) docker     (123)    75329 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Ionosphere.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Iris.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Lymphography.csv
--rw-r--r--   0 runner    (1001) docker     (123)  5205194 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Madelon.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Monk1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Monk2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Monk3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    85876 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Sonar.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Soybean-small.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/SpectEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19160 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Tic-tac-toe.csv
--rw-r--r--   0 runner    (1001) docker     (123)    65346 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Vowel.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1053755 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/WaveformEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Wine.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/Zoo.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/aggregation.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40191 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/aniso.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/appendicitis.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/balance.csv
--rw-r--r--   0 runner    (1001) docker     (123)    45030 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/banknote.csv
--rw-r--r--   0 runner    (1001) docker     (123)    39793 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/blobs.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40156 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/circles.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/diagnosis_II.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/ecoli.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/flame.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/heart.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/jain.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/liver.csv
--rw-r--r--   0 runner    (1001) docker     (123)    39579 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/moons.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/mouse.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/pathbased.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/seeds.csv
--rw-r--r--   0 runner    (1001) docker     (123)    59518 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/segmentation.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/smiley.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40499 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/varied.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/vary-density.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/vertebral2.csv
--rw-r--r--   0 runner    (1001) docker     (123)   119889 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/data/wdbc.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/metacluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:44:53.606516 metacluster-1.0.0/metacluster/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/utils/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/utils/io_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/utils/mealpy_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/utils/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-04 10:43:56.000000 metacluster-1.0.0/metacluster/utils/visualize_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:44:53.594515 metacluster-1.0.0/metacluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-08-04 10:44:53.000000 metacluster-1.0.0/metacluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-04 10:44:53.000000 metacluster-1.0.0/metacluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 10:44:53.000000 metacluster-1.0.0/metacluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-04 10:44:53.000000 metacluster-1.0.0/metacluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 10:44:53.000000 metacluster-1.0.0/metacluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 10:44:53.606516 metacluster-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-04 10:43:56.000000 metacluster-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:44:53.606516 metacluster-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-04 10:43:56.000000 metacluster-1.0.0/tests/test_Data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-04 10:43:56.000000 metacluster-1.0.0/tests/test_MetaCluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:30:45.356442 metacluster-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-07 11:29:52.000000 metacluster-1.0.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-07 11:29:52.000000 metacluster-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 11:29:52.000000 metacluster-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-07 11:29:52.000000 metacluster-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-08-07 11:30:45.356442 metacluster-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-08-07 11:29:52.000000 metacluster-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:30:45.340442 metacluster-1.0.1/metacluster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:30:45.356442 metacluster-1.0.1/metacluster/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   369879 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Arrhythmia.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Blood.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/BreastCancer.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   119681 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/BreastEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/CongressEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   498322 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Digits.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Glass.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/HeartEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   438254 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Hill-valley.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    37338 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Horse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    75329 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Ionosphere.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Iris.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Lymphography.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  5205194 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Madelon.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Monk1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Monk2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Monk3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    85876 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Sonar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Soybean-small.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/SpectEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19160 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Tic-tac-toe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    65346 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Vowel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1053755 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/WaveformEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Wine.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/Zoo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/aggregation.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40191 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/aniso.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/appendicitis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/balance.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    45030 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/banknote.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    39793 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/blobs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40156 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/circles.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/diagnosis_II.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/ecoli.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/flame.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/heart.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/jain.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/liver.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    39579 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/moons.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/mouse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/pathbased.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/seeds.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    59518 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/segmentation.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/smiley.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40499 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/varied.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/vary-density.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/vertebral2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   119889 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/data/wdbc.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15058 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/metacluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:30:45.356442 metacluster-1.0.1/metacluster/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/utils/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/utils/io_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/utils/mealpy_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/utils/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-07 11:29:52.000000 metacluster-1.0.1/metacluster/utils/visualize_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:30:45.340442 metacluster-1.0.1/metacluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-08-07 11:30:45.000000 metacluster-1.0.1/metacluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-07 11:30:45.000000 metacluster-1.0.1/metacluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:30:45.000000 metacluster-1.0.1/metacluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-07 11:30:45.000000 metacluster-1.0.1/metacluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 11:30:45.000000 metacluster-1.0.1/metacluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 11:30:45.356442 metacluster-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-07 11:29:52.000000 metacluster-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:30:45.356442 metacluster-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-07 11:29:52.000000 metacluster-1.0.1/tests/test_Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-07 11:29:52.000000 metacluster-1.0.1/tests/test_MetaCluster.py
```

### Comparing `metacluster-1.0.0/CODE_OF_CONDUCT.md` & `metacluster-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/LICENSE` & `metacluster-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/PKG-INFO` & `metacluster-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metacluster
-Version: 1.0.0
+Version: 1.0.1
 Summary: MetaCluster: An Open-Source Python Library for Metaheuristic-based Clustering Problems
 Home-page: https://github.com/thieu1995/metacluster
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://metacluster.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/metacluster
@@ -38,20 +38,26 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-<p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MetaCluster" title="MetaCluster"/></p>
+<p align="center">
+<img style="max-width:100%;" 
+src="https://thieu1995.github.io/post/2023-08/MetaCluster-01.png" 
+alt="MetaCluster"/>
+</p>
+
+
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-1.0.0-yellow.svg)](https://github.com/thieu1995/metacluster/releases)
+[![GitHub release](https://img.shields.io/badge/release-1.0.1-yellow.svg)](https://github.com/thieu1995/metacluster/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/metacluster) 
 [![PyPI version](https://badge.fury.io/py/metacluster.svg)](https://badge.fury.io/py/metacluster)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/metacluster.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/metacluster.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/metacluster.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/metacluster.svg)
 [![Downloads](https://pepy.tech/badge/metacluster)](https://pepy.tech/project/metacluster)
@@ -79,15 +85,15 @@
 * **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics, plotly, kaleido
 
 
 # Installation
 
 * Install the [current PyPI release](https://pypi.python.org/pypi/metacluster):
 ```sh 
-$ pip install metacluster==1.0.0
+$ pip install metacluster==1.0.1
 ```
 
 * Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/metacluster.git
 $ cd metacluster
 $ python setup.py install
```

### Comparing `metacluster-1.0.0/README.md` & `metacluster-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 
-<p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MetaCluster" title="MetaCluster"/></p>
+<p align="center">
+<img style="max-width:100%;" 
+src="https://thieu1995.github.io/post/2023-08/MetaCluster-01.png" 
+alt="MetaCluster"/>
+</p>
+
+
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-1.0.0-yellow.svg)](https://github.com/thieu1995/metacluster/releases)
+[![GitHub release](https://img.shields.io/badge/release-1.0.1-yellow.svg)](https://github.com/thieu1995/metacluster/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/metacluster) 
 [![PyPI version](https://badge.fury.io/py/metacluster.svg)](https://badge.fury.io/py/metacluster)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/metacluster.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/metacluster.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/metacluster.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/metacluster.svg)
 [![Downloads](https://pepy.tech/badge/metacluster)](https://pepy.tech/project/metacluster)
@@ -36,15 +42,15 @@
 * **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics, plotly, kaleido
 
 
 # Installation
 
 * Install the [current PyPI release](https://pypi.python.org/pypi/metacluster):
 ```sh 
-$ pip install metacluster==1.0.0
+$ pip install metacluster==1.0.1
 ```
 
 * Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/metacluster.git
 $ cd metacluster
 $ python setup.py install
```

### Comparing `metacluster-1.0.0/metacluster/__init__.py` & `metacluster-1.0.1/metacluster/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,12 +27,12 @@
 # list_obj = ["BHI", "MIS", "XBI"]
 # list_metric = ["BRI", "DBI", "DRI", "DI", "KDI"]
 #
 # # Define MetaCluster model and execute it
 # model = MetaCluster(list_optimizer=list_optimizer, list_paras=list_paras, list_obj=list_obj, n_trials=3)
 # model.execute(data=data, cluster_finder="elbow", list_metric=list_metric, save_path="history", verbose=False)
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 from metacluster.utils.encoder import LabelEncoder
 from metacluster.utils.data_loader import Data, get_dataset
 from metacluster.metacluster import MetaCluster
```

### Comparing `metacluster-1.0.0/metacluster/data/Arrhythmia.csv` & `metacluster-1.0.1/metacluster/data/Arrhythmia.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Blood.csv` & `metacluster-1.0.1/metacluster/data/Blood.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/BreastCancer.csv` & `metacluster-1.0.1/metacluster/data/BreastCancer.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/BreastEW.csv` & `metacluster-1.0.1/metacluster/data/BreastEW.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Digits.csv` & `metacluster-1.0.1/metacluster/data/Digits.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Glass.csv` & `metacluster-1.0.1/metacluster/data/Glass.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/HeartEW.csv` & `metacluster-1.0.1/metacluster/data/HeartEW.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Hill-valley.csv` & `metacluster-1.0.1/metacluster/data/Hill-valley.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Horse.csv` & `metacluster-1.0.1/metacluster/data/Horse.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Ionosphere.csv` & `metacluster-1.0.1/metacluster/data/Ionosphere.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Iris.csv` & `metacluster-1.0.1/metacluster/data/Iris.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Lymphography.csv` & `metacluster-1.0.1/metacluster/data/Lymphography.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Madelon.csv` & `metacluster-1.0.1/metacluster/data/Madelon.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Monk1.csv` & `metacluster-1.0.1/metacluster/data/Monk1.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Monk2.csv` & `metacluster-1.0.1/metacluster/data/Monk2.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Monk3.csv` & `metacluster-1.0.1/metacluster/data/Monk3.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Sonar.csv` & `metacluster-1.0.1/metacluster/data/Sonar.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Soybean-small.csv` & `metacluster-1.0.1/metacluster/data/Soybean-small.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Vowel.csv` & `metacluster-1.0.1/metacluster/data/Vowel.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/WaveformEW.csv` & `metacluster-1.0.1/metacluster/data/WaveformEW.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Wine.csv` & `metacluster-1.0.1/metacluster/data/Wine.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/Zoo.csv` & `metacluster-1.0.1/metacluster/data/Zoo.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/aggregation.csv` & `metacluster-1.0.1/metacluster/data/aggregation.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/aniso.csv` & `metacluster-1.0.1/metacluster/data/aniso.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/appendicitis.csv` & `metacluster-1.0.1/metacluster/data/appendicitis.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/balance.csv` & `metacluster-1.0.1/metacluster/data/balance.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/banknote.csv` & `metacluster-1.0.1/metacluster/data/banknote.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/blobs.csv` & `metacluster-1.0.1/metacluster/data/blobs.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/circles.csv` & `metacluster-1.0.1/metacluster/data/circles.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/diagnosis_II.csv` & `metacluster-1.0.1/metacluster/data/diagnosis_II.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/ecoli.csv` & `metacluster-1.0.1/metacluster/data/ecoli.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/flame.csv` & `metacluster-1.0.1/metacluster/data/flame.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/heart.csv` & `metacluster-1.0.1/metacluster/data/heart.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/jain.csv` & `metacluster-1.0.1/metacluster/data/jain.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/liver.csv` & `metacluster-1.0.1/metacluster/data/liver.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/moons.csv` & `metacluster-1.0.1/metacluster/data/moons.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/mouse.csv` & `metacluster-1.0.1/metacluster/data/mouse.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/pathbased.csv` & `metacluster-1.0.1/metacluster/data/pathbased.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/seeds.csv` & `metacluster-1.0.1/metacluster/data/seeds.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/segmentation.csv` & `metacluster-1.0.1/metacluster/data/segmentation.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/smiley.csv` & `metacluster-1.0.1/metacluster/data/smiley.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/varied.csv` & `metacluster-1.0.1/metacluster/data/varied.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/vary-density.csv` & `metacluster-1.0.1/metacluster/data/vary-density.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/vertebral2.csv` & `metacluster-1.0.1/metacluster/data/vertebral2.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/data/wdbc.csv` & `metacluster-1.0.1/metacluster/data/wdbc.csv`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/metacluster.py` & `metacluster-1.0.1/metacluster/metacluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,19 +70,16 @@
 
     SUPPORT = {
         "cluster_finder": {"elbow": "get_clusters_by_elbow", "gap": "get_clusters_by_gap_statistic",
                            "silhouette": "get_clusters_by_silhouette_score", "davies_bouldin": "get_clusters_by_davies_bouldin",
                            "calinski_harabasz": "get_clusters_by_calinski_harabasz", "bic": "get_clusters_by_bic",
                            "all_min": "get_clusters_by_all_min", "all_max": "get_clusters_by_all_max",
                            "all_mean": "get_clusters_by_all_mean", "all_majority": "get_clusters_by_all_majority"},
-        "obj": {"BHI": "min", "CHI": "max", "XBI": "min", "BRI": "max", "DBI": "min", "DRI": "min",
-                "DI": "max", "KDI": "min", "LDRI": "min", "LSRI": "min", "SI": "max", "MIS": "max",
-                "NMIS": "max", "RaS": "max", "FMS": "max", "HS": "max", "CS": "max", "VMS": "max",
-                "PrS": "max", "ReS": "max", "FmS": "max", "CDS": "max", "HGS": "max", "JS": "max",
-                "KS": "max", "MNS": "min", "PhS": "max", "RTS": "max", "RRS": "max", "SS1S": "max", "SS2S": "max"},
+        "obj": cluster.get_all_clustering_metrics(),
+        "metrics": cluster.get_all_clustering_metrics(),
         "optimizer": list(get_all_optimizers().keys())
     }
 
     FILENAME_LABELS = "result_labels"
     FILENAME_METRICS = "result_metrics"
     FILENAME_METRICS_MEAN = "result_metrics_min"
     FILENAME_METRICS_STD = "result_metrics_mean"
```

### Comparing `metacluster-1.0.0/metacluster/utils/cluster.py` & `metacluster-1.0.1/metacluster/utils/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 17:39, 30/07/2023 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
+import numpy as np
+from sklearn import metrics
 from sklearn.cluster import KMeans
 from sklearn.mixture import GaussianMixture
-from sklearn import metrics
-import numpy as np
+from permetrics import ClusteringMetric
+
+
+def get_all_clustering_metrics():
+    dict_results = {}
+    for key, value in ClusteringMetric.SUPPORT.items():
+        if value["type"] in ("min", "max"):
+            dict_results[key] = value["type"]
+    return dict_results
 
 
 ### ELBOW
 def get_clusters_by_elbow(X, list_clusters=None, **kwargs):
     """
     1. First, apply K-means clustering to the dataset for a range of different values of K, where K is the number of clusters. For example, you might try K=1,2,3,...,10.
     2. For each value of K, compute the Sum of Squared Errors (SSE), which is the sum of the squared distances between each data point and its assigned centroid. The SSE can be obtained from the KMeans object's 'inertia_' attribute.
```

### Comparing `metacluster-1.0.0/metacluster/utils/data_loader.py` & `metacluster-1.0.1/metacluster/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/utils/encoder.py` & `metacluster-1.0.1/metacluster/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/utils/io_util.py` & `metacluster-1.0.1/metacluster/utils/io_util.py`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/utils/mealpy_util.py` & `metacluster-1.0.1/metacluster/utils/mealpy_util.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,41 +3,17 @@
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from mealpy.optimizer import Optimizer
 from mealpy import *
-import sys, inspect
 from permetrics import ClusteringMetric
 
 
-EXCLUDE_MODULES = ["__builtins__", "current_module", "inspect", "sys"]
-
-
-def get_all_optimizers():
-    cls = {}
-    for name, obj in inspect.getmembers(sys.modules[__name__]):
-        if inspect.ismodule(obj) and (name not in EXCLUDE_MODULES):
-            for cls_name, cls_obj in inspect.getmembers(obj):
-                if inspect.isclass(cls_obj) and issubclass(cls_obj, Optimizer):
-                    cls[cls_name] = cls_obj
-    del cls['Optimizer']
-    return cls
-
-
-def get_optimizer_by_name(name):
-    try:
-        cls = get_all_optimizers()[name]
-        return cls
-    except KeyError:
-        print(f"MetaCluster doesn't support optimizer named: {name}.\n"
-              f"Please see the supported Optimizer name from here: https://mealpy.readthedocs.io/en/latest/pages/support.html#classification-table")
-
-
 class KCenterClusteringProblem(Problem):
     def __init__(self, lb, ub, minmax, data=None, estimator=None, obj_name=None, obj_paras=None,
                  name="K Center Clustering Problem", **kwargs):
         ## data is assigned first because when initialize the Problem class, we need to check the output of fitness
         self.data = data
         self.estimator = estimator
         self.obj_name = obj_name
```

### Comparing `metacluster-1.0.0/metacluster/utils/validator.py` & `metacluster-1.0.1/metacluster/utils/validator.py`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster/utils/visualize_util.py` & `metacluster-1.0.1/metacluster/utils/visualize_util.py`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/metacluster.egg-info/PKG-INFO` & `metacluster-1.0.1/metacluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metacluster
-Version: 1.0.0
+Version: 1.0.1
 Summary: MetaCluster: An Open-Source Python Library for Metaheuristic-based Clustering Problems
 Home-page: https://github.com/thieu1995/metacluster
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://metacluster.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/metacluster
@@ -38,20 +38,26 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-<p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MetaCluster" title="MetaCluster"/></p>
+<p align="center">
+<img style="max-width:100%;" 
+src="https://thieu1995.github.io/post/2023-08/MetaCluster-01.png" 
+alt="MetaCluster"/>
+</p>
+
+
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-1.0.0-yellow.svg)](https://github.com/thieu1995/metacluster/releases)
+[![GitHub release](https://img.shields.io/badge/release-1.0.1-yellow.svg)](https://github.com/thieu1995/metacluster/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/metacluster) 
 [![PyPI version](https://badge.fury.io/py/metacluster.svg)](https://badge.fury.io/py/metacluster)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/metacluster.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/metacluster.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/metacluster.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/metacluster.svg)
 [![Downloads](https://pepy.tech/badge/metacluster)](https://pepy.tech/project/metacluster)
@@ -79,15 +85,15 @@
 * **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics, plotly, kaleido
 
 
 # Installation
 
 * Install the [current PyPI release](https://pypi.python.org/pypi/metacluster):
 ```sh 
-$ pip install metacluster==1.0.0
+$ pip install metacluster==1.0.1
 ```
 
 * Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/metacluster.git
 $ cd metacluster
 $ python setup.py install
```

### Comparing `metacluster-1.0.0/metacluster.egg-info/SOURCES.txt` & `metacluster-1.0.1/metacluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/setup.py` & `metacluster-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="metacluster",
-    version="1.0.0",
+    version="1.0.1",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="MetaCluster: An Open-Source Python Library for Metaheuristic-based Clustering Problems",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["clustering", "optimization", "k-center clustering", "data points", "centers", "euclidean distance", "maximum distance",
               "NP-hard", "greedy algorithm", "approximation algorithm", "covering problem", "computational complexity",
@@ -66,14 +66,14 @@
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Topic :: Software Development :: Build Tools",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
     ],
     install_requires=["numpy>=1.17.1", "scipy>=1.7.1", "scikit-learn>=1.0.2",
-                      "pandas>=1.3.5", "mealpy>=2.5.3", "permetrics>=1.4.1",
+                      "pandas>=1.3.5", "mealpy>=2.5.4", "permetrics>=1.4.2",
                       "plotly>=5.10.0", "kaleido>=0.2.1"],
     extras_require={
         "dev": ["pytest>=7.1.2", "pytest-cov==4.0.0", "flake8>=4.0.1"],
     },
     python_requires='>=3.7',
 )
```

### Comparing `metacluster-1.0.0/tests/test_Data.py` & `metacluster-1.0.1/tests/test_Data.py`

 * *Files identical despite different names*

### Comparing `metacluster-1.0.0/tests/test_MetaCluster.py` & `metacluster-1.0.1/tests/test_MetaCluster.py`

 * *Files identical despite different names*

