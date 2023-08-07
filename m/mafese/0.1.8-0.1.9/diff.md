# Comparing `tmp/mafese-0.1.8.tar.gz` & `tmp/mafese-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafese-0.1.8.tar", last modified: Fri Jul 14 03:49:53 2023, max compression
+gzip compressed data, was "mafese-0.1.9.tar", last modified: Mon Aug  7 11:12:57 2023, max compression
```

## Comparing `mafese-0.1.8.tar` & `mafese-0.1.9.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.029676 mafese-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-14 03:48:45.000000 mafese-0.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-14 03:48:45.000000 mafese-0.1.8/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 03:48:45.000000 mafese-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 03:48:45.000000 mafese-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-07-14 03:49:53.029676 mafese-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-07-14 03:48:45.000000 mafese-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.009676 mafese-0.1.8/mafese/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.005676 mafese-0.1.8/mafese/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.021676 mafese-0.1.8/mafese/data/cls/
--rw-r--r--   0 runner    (1001) docker     (123)   369879 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Arrhythmia.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Blood.csv
--rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/BreastCancer.csv
--rw-r--r--   0 runner    (1001) docker     (123)   119681 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/BreastEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/CongressEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)   498322 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Digits.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Glass.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/HeartEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)   438254 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Hill-valley.csv
--rw-r--r--   0 runner    (1001) docker     (123)    37338 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Horse.csv
--rw-r--r--   0 runner    (1001) docker     (123)    75329 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Ionosphere.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Iris.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Lymphography.csv
--rw-r--r--   0 runner    (1001) docker     (123)  5205194 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Madelon.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Monk1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Monk2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Monk3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    85876 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Sonar.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Soybean-small.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/SpectEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19160 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Tic-tac-toe.csv
--rw-r--r--   0 runner    (1001) docker     (123)    65346 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Vowel.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1053755 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/WaveformEW.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Wine.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Zoo.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/aggregation.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40191 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/aniso.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/appendicitis.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/balance.csv
--rw-r--r--   0 runner    (1001) docker     (123)    45030 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/banknote.csv
--rw-r--r--   0 runner    (1001) docker     (123)    39793 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/blobs.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40156 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/circles.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/diagnosis_II.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/ecoli.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/flame.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/heart.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/jain.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/liver.csv
--rw-r--r--   0 runner    (1001) docker     (123)    39579 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/moons.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/mouse.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/pathbased.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/seeds.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/smiley.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40499 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/varied.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/vary-density.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/vertebral2.csv
--rw-r--r--   0 runner    (1001) docker     (123)   119889 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/wdbc.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.025676 mafese-0.1.8/mafese/data/reg/
--rw-r--r--   0 runner    (1001) docker     (123)    35644 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/reg/boston-housing.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/reg/computer-hardware.csv
--rw-r--r--   0 runner    (1001) docker     (123)    25774 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/reg/diabetes.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1981727 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/reg/gauss-100-20.csv
--rw-r--r--   0 runner    (1001) docker     (123)   400064 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/reg/gauss-50-12.csv
--rw-r--r--   0 runner    (1001) docker     (123)   894463 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/reg/gauss-75-17.csv
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/reg/linnerud.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.025676 mafese-0.1.8/mafese/embedded/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/embedded/lasso.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/embedded/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/unsupervised.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.029676 mafese-0.1.8/mafese/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/mealpy_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.029676 mafese-0.1.8/mafese/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32353 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/wrapper/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/wrapper/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/wrapper/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.009676 mafese-0.1.8/mafese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-07-14 03:49:52.000000 mafese-0.1.8/mafese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-14 03:49:52.000000 mafese-0.1.8/mafese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 03:49:52.000000 mafese-0.1.8/mafese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-14 03:49:52.000000 mafese-0.1.8/mafese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 03:49:52.000000 mafese-0.1.8/mafese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 03:49:53.029676 mafese-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-14 03:48:45.000000 mafese-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.029676 mafese-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-14 03:48:45.000000 mafese-0.1.8/tests/test_embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-14 03:48:45.000000 mafese-0.1.8/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-14 03:48:45.000000 mafese-0.1.8/tests/test_unsupervised.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-14 03:48:45.000000 mafese-0.1.8/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:12:57.595532 mafese-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-07 11:11:45.000000 mafese-0.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-08-07 11:11:45.000000 mafese-0.1.9/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 11:11:45.000000 mafese-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-07 11:11:45.000000 mafese-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-08-07 11:12:57.595532 mafese-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-08-07 11:11:45.000000 mafese-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:12:57.567532 mafese-0.1.9/mafese/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:12:57.563532 mafese-0.1.9/mafese/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:12:57.587532 mafese-0.1.9/mafese/data/cls/
+-rw-r--r--   0 runner    (1001) docker     (123)   369879 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Arrhythmia.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Blood.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/BreastCancer.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   119681 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/BreastEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/CongressEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   498322 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Digits.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Glass.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/HeartEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   438254 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Hill-valley.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    37338 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Horse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    75329 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Ionosphere.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Iris.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Lymphography.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  5205194 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Madelon.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Monk1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Monk2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Monk3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    85876 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Sonar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Soybean-small.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/SpectEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19160 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Tic-tac-toe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    65346 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Vowel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1053755 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/WaveformEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Wine.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/Zoo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/aggregation.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40191 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/aniso.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/appendicitis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/balance.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    45030 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/banknote.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    39793 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/blobs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40156 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/circles.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/diagnosis_II.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/ecoli.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/flame.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/heart.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/jain.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/liver.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    39579 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/moons.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/mouse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/pathbased.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/seeds.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/smiley.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40499 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/varied.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/vary-density.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/vertebral2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   119889 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/cls/wdbc.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:12:57.591532 mafese-0.1.9/mafese/data/reg/
+-rw-r--r--   0 runner    (1001) docker     (123)    35644 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/reg/boston-housing.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/reg/computer-hardware.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25774 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/reg/diabetes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1981727 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/reg/gauss-100-20.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   400064 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/reg/gauss-50-12.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   894463 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/reg/gauss-75-17.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/data/reg/linnerud.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:12:57.591532 mafese-0.1.9/mafese/embedded/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/embedded/lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/embedded/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/unsupervised.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:12:57.591532 mafese-0.1.9/mafese/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/utils/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/utils/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/utils/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/utils/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/utils/mealpy_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/utils/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:12:57.595532 mafese-0.1.9/mafese/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31517 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/wrapper/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/wrapper/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-07 11:11:45.000000 mafese-0.1.9/mafese/wrapper/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:12:57.567532 mafese-0.1.9/mafese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-08-07 11:12:57.000000 mafese-0.1.9/mafese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-08-07 11:12:57.000000 mafese-0.1.9/mafese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:12:57.000000 mafese-0.1.9/mafese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-07 11:12:57.000000 mafese-0.1.9/mafese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 11:12:57.000000 mafese-0.1.9/mafese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 11:12:57.595532 mafese-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-08-07 11:11:45.000000 mafese-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:12:57.595532 mafese-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-07 11:11:45.000000 mafese-0.1.9/tests/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-07 11:11:45.000000 mafese-0.1.9/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-07 11:11:45.000000 mafese-0.1.9/tests/test_unsupervised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-07 11:11:45.000000 mafese-0.1.9/tests/test_wrapper.py
```

### Comparing `mafese-0.1.8/CODE_OF_CONDUCT.md` & `mafese-0.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/ChangeLog.md` & `mafese-0.1.9/ChangeLog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,22 @@
+# Version 0.1.9
+
++ Add more Optimizers in MhaSelector and MultiMhaSelector 
++ Add more Regression and Classification objectives for fitness function
++ Add more Regression and Classification metrics for evaluate() function 
++ Update logo and documents
++ Add more examples
+
+---------------------------------------------------------------------
+
 # Version 0.1.8
 
 + Fix bug load data from library.
 
+
 ---------------------------------------------------------------------
 
 # Version 0.1.7
 
 + Remove some unknown datasets
 + Fix bug name in Kendall and Spearman functions of FilterSelector 
 + Add Relief-based family to FilterSelector
```

### Comparing `mafese-0.1.8/LICENSE` & `mafese-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/PKG-INFO` & `mafese-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafese
-Version: 0.1.8
+Version: 0.1.9
 Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
 Home-page: https://github.com/thieu1995/mafese
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mafese
@@ -38,20 +38,24 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-<p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
+<p align="center">
+<img style="max-width:100%;" 
+src="https://thieu1995.github.io/post/2023-08/mafese-02.png" 
+alt="MAFESE"/>
+</p>
 
----
 
+---
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.8-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.9-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -60,46 +64,57 @@
 [![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
 ![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/mafese.svg)
 [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![DOI](https://zenodo.org/badge/545209353.svg)](https://doi.org/10.5281/zenodo.7969042)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
-MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library for feature selection problem 
-using meta-heuristic algorithms. 
+MAFESE (Metaheuristic Algorithms for FEature SElection) is the biggest python library for feature selection (FS) 
+problem using meta-heuristic algorithms.
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
+* **Total Wrapper-based (Metaheuristic Algorithms)**: > 200 methods
 * **Total Filter-based (Statistical-based)**: > 15 methods
 * **Total Embedded-based (Tree and Lasso)**: > 10 methods
 * **Total Unsupervised-based**: >= 4 methods
-* **Total classification dataset**: >= 30 datasets
-* **Total regression dataset**: >= 7 datasets
-* **Total performance metrics (as fitness)**: > 30 metrics
+* **Total datasets**: >= 30 (47 classifications and 7 regressions)
+* **Total performance metrics**: >= 61 (45 regressions and 16 classifications)
+* **Total objective functions (as fitness functions)**: >= 61 (45 regressions and 16 classifications)
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
-* **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
-* **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics
+* **Python versions:** >= 3.7.x
+* **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics, plotly, kaleido
 
 
 # Installation
 
-### Install with pip
-
-Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
+* Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.8
+$ pip install mafese==0.1.9
 ```
 
-### Install directly from source code
+* Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
 ```
 
+* In case, you want to install the development version from Github:
+```sh 
+$ pip install git+https://github.com/thieu1995/mafese 
+```
+
+After installation, you can import MAFESE as any other Python module:
+
+```sh
+$ python
+>>> import mafese
+>>> mafese.__version__
+```
+
 
 ### Lib's structure
 
 ```code 
 docs
 examples
 mafese
@@ -131,31 +146,18 @@
         validator.py
     __init__.py
     selector.py
 README.md
 setup.py
 ```
 
-
-# Usage
-
-After installation, you can import MAFESE as any other Python module:
-
-```sh
-$ python
->>> import mafese
->>> mafese.__version__
-```
+### Examples
 
 Let's go through some examples.
 
-
-
-### Examples
-
 #### 1. First, load dataset. You can use the available datasets from Mafese:
 
 ```python 
 # Load available dataset from MAFESE
 from mafese import get_dataset
 
 # Try unknown data
@@ -272,17 +274,23 @@
 ii) You can use the same estimator in feature selection process 
 ```python 
 X_test, y_test = data.X_test, data.y_test
 feat_selector.evaluate(estimator=None, data=data, metrics=["AS", "PS", "RS"])
 ```
 
 1) Where do I find the supported metrics like above ["AS", "PS", "RS"]. What is that?
-You can find it here: https://github.com/thieu1995/permetrics
+You can find it here: https://github.com/thieu1995/permetrics or use this 
+```python 
+from mafese import MhaSelector 
 
-2) How do I know my Selector support which estimator? which methods?
+print(MhaSelector.SUPPORTED_REGRESSION_METRICS)
+print(MhaSelector.SUPPORTED_CLASSIFICATION_METRICS)
+```
+
+3) How do I know my Selector support which estimator? which methods?
 ```python 
 print(feat_selector.SUPPORT) 
 ```
 Or you better read the document from: https://mafese.readthedocs.io/en/latest/
 
 3) I got this type of error
 ```python 
@@ -323,58 +331,68 @@
 data.split_train_test(test_size=0.2, random_state=10)   # Try different random_state value 
 ```
 
 
 For more usage examples please look at [examples](/examples) folder.
 
 
-# Get helps (questions, problems)
+# Support (questions, problems)
+
+### Official Links 
 
 * Official source code repo: https://github.com/thieu1995/mafese
 * Official document: https://mafese.readthedocs.io/
 * Download releases: https://pypi.org/project/mafese/
 * Issue tracker: https://github.com/thieu1995/mafese/issues
 * Notable changes log: https://github.com/thieu1995/mafese/blob/master/ChangeLog.md
 * Examples with different mealpy version: https://github.com/thieu1995/mafese/blob/master/examples.md
 * Official chat group: https://t.me/+fRVCJGuGJg1mNDg1
 
-* This project also related to our another projects which are "meta-heuristics", "neural-network", and "optimization" 
-  check it here
+* This project also related to our another projects which are "optimization" and "machine learning", check it here:
     * https://github.com/thieu1995/mealpy
     * https://github.com/thieu1995/metaheuristics
     * https://github.com/thieu1995/opfunu
     * https://github.com/thieu1995/enoppy
     * https://github.com/thieu1995/permetrics
+    * https://github.com/thieu1995/MetaCluster
+    * https://github.com/thieu1995/pfevaluator
     * https://github.com/aiir-team
 
+### Citation Request 
 
-# References 
-
-If you are using mafese in your project, we would appreciate citations:
+Please include these citations if you plan to use this library:
 
 ```code 
 @software{nguyen_van_thieu_2023_7969043,
-  author       = {Nguyen Van Thieu},
-  title        = {MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library},
+  author       = {Nguyen Van Thieu, Ngoc Hung Nguyen, Ali Asghar Heidari},
+  title        = {Feature Selection using Metaheuristics Made Easy: Open Source MAFESE Library in Python},
   month        = may,
   year         = 2023,
   publisher    = {Zenodo},
   doi          = {10.5281/zenodo.7969042},
   url          = {https://github.com/thieu1995/mafese}
 }
+
+@article{van2023mealpy,
+  title={MEALPY: An open-source library for latest meta-heuristic algorithms in Python},
+  author={Van Thieu, Nguyen and Mirjalili, Seyedali},
+  journal={Journal of Systems Architecture},
+  year={2023},
+  publisher={Elsevier},
+  doi={10.1016/j.sysarc.2023.102871}
+}
 ```
 
 
 
-```code 
+### Related Documents
+
 1. https://neptune.ai/blog/feature-selection-methods
 2. https://www.blog.trainindata.com/feature-selection-machine-learning-with-python/
 3. https://github.com/LBBSoft/FeatureSelect
 4. https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2754-0
 5. https://github.com/scikit-learn-contrib/boruta_py
-6.  https://elki-project.github.io/
+6. https://elki-project.github.io/
 7. https://sci2s.ugr.es/keel/index.php
 8. https://archive.ics.uci.edu/datasets
 9. https://python-charts.com/distribution/box-plot-plotly/
 10. https://plotly.com/python/box-plots/?_ga=2.50659434.2126348639.1688086416-114197406.1688086416#box-plot-styling-mean--standard-deviation
-
-```
```

### Comparing `mafese-0.1.8/README.md` & `mafese-0.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 
-<p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
+<p align="center">
+<img style="max-width:100%;" 
+src="https://thieu1995.github.io/post/2023-08/mafese-02.png" 
+alt="MAFESE"/>
+</p>
 
----
 
+---
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.8-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.9-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -17,46 +21,57 @@
 [![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
 ![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/mafese.svg)
 [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![DOI](https://zenodo.org/badge/545209353.svg)](https://doi.org/10.5281/zenodo.7969042)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
-MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library for feature selection problem 
-using meta-heuristic algorithms. 
+MAFESE (Metaheuristic Algorithms for FEature SElection) is the biggest python library for feature selection (FS) 
+problem using meta-heuristic algorithms.
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
+* **Total Wrapper-based (Metaheuristic Algorithms)**: > 200 methods
 * **Total Filter-based (Statistical-based)**: > 15 methods
 * **Total Embedded-based (Tree and Lasso)**: > 10 methods
 * **Total Unsupervised-based**: >= 4 methods
-* **Total classification dataset**: >= 30 datasets
-* **Total regression dataset**: >= 7 datasets
-* **Total performance metrics (as fitness)**: > 30 metrics
+* **Total datasets**: >= 30 (47 classifications and 7 regressions)
+* **Total performance metrics**: >= 61 (45 regressions and 16 classifications)
+* **Total objective functions (as fitness functions)**: >= 61 (45 regressions and 16 classifications)
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
-* **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
-* **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics
+* **Python versions:** >= 3.7.x
+* **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics, plotly, kaleido
 
 
 # Installation
 
-### Install with pip
-
-Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
+* Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.8
+$ pip install mafese==0.1.9
 ```
 
-### Install directly from source code
+* Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
 ```
 
+* In case, you want to install the development version from Github:
+```sh 
+$ pip install git+https://github.com/thieu1995/mafese 
+```
+
+After installation, you can import MAFESE as any other Python module:
+
+```sh
+$ python
+>>> import mafese
+>>> mafese.__version__
+```
+
 
 ### Lib's structure
 
 ```code 
 docs
 examples
 mafese
@@ -88,31 +103,18 @@
         validator.py
     __init__.py
     selector.py
 README.md
 setup.py
 ```
 
-
-# Usage
-
-After installation, you can import MAFESE as any other Python module:
-
-```sh
-$ python
->>> import mafese
->>> mafese.__version__
-```
+### Examples
 
 Let's go through some examples.
 
-
-
-### Examples
-
 #### 1. First, load dataset. You can use the available datasets from Mafese:
 
 ```python 
 # Load available dataset from MAFESE
 from mafese import get_dataset
 
 # Try unknown data
@@ -229,17 +231,23 @@
 ii) You can use the same estimator in feature selection process 
 ```python 
 X_test, y_test = data.X_test, data.y_test
 feat_selector.evaluate(estimator=None, data=data, metrics=["AS", "PS", "RS"])
 ```
 
 1) Where do I find the supported metrics like above ["AS", "PS", "RS"]. What is that?
-You can find it here: https://github.com/thieu1995/permetrics
+You can find it here: https://github.com/thieu1995/permetrics or use this 
+```python 
+from mafese import MhaSelector 
 
-2) How do I know my Selector support which estimator? which methods?
+print(MhaSelector.SUPPORTED_REGRESSION_METRICS)
+print(MhaSelector.SUPPORTED_CLASSIFICATION_METRICS)
+```
+
+3) How do I know my Selector support which estimator? which methods?
 ```python 
 print(feat_selector.SUPPORT) 
 ```
 Or you better read the document from: https://mafese.readthedocs.io/en/latest/
 
 3) I got this type of error
 ```python 
@@ -280,58 +288,68 @@
 data.split_train_test(test_size=0.2, random_state=10)   # Try different random_state value 
 ```
 
 
 For more usage examples please look at [examples](/examples) folder.
 
 
-# Get helps (questions, problems)
+# Support (questions, problems)
+
+### Official Links 
 
 * Official source code repo: https://github.com/thieu1995/mafese
 * Official document: https://mafese.readthedocs.io/
 * Download releases: https://pypi.org/project/mafese/
 * Issue tracker: https://github.com/thieu1995/mafese/issues
 * Notable changes log: https://github.com/thieu1995/mafese/blob/master/ChangeLog.md
 * Examples with different mealpy version: https://github.com/thieu1995/mafese/blob/master/examples.md
 * Official chat group: https://t.me/+fRVCJGuGJg1mNDg1
 
-* This project also related to our another projects which are "meta-heuristics", "neural-network", and "optimization" 
-  check it here
+* This project also related to our another projects which are "optimization" and "machine learning", check it here:
     * https://github.com/thieu1995/mealpy
     * https://github.com/thieu1995/metaheuristics
     * https://github.com/thieu1995/opfunu
     * https://github.com/thieu1995/enoppy
     * https://github.com/thieu1995/permetrics
+    * https://github.com/thieu1995/MetaCluster
+    * https://github.com/thieu1995/pfevaluator
     * https://github.com/aiir-team
 
+### Citation Request 
 
-# References 
-
-If you are using mafese in your project, we would appreciate citations:
+Please include these citations if you plan to use this library:
 
 ```code 
 @software{nguyen_van_thieu_2023_7969043,
-  author       = {Nguyen Van Thieu},
-  title        = {MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library},
+  author       = {Nguyen Van Thieu, Ngoc Hung Nguyen, Ali Asghar Heidari},
+  title        = {Feature Selection using Metaheuristics Made Easy: Open Source MAFESE Library in Python},
   month        = may,
   year         = 2023,
   publisher    = {Zenodo},
   doi          = {10.5281/zenodo.7969042},
   url          = {https://github.com/thieu1995/mafese}
 }
+
+@article{van2023mealpy,
+  title={MEALPY: An open-source library for latest meta-heuristic algorithms in Python},
+  author={Van Thieu, Nguyen and Mirjalili, Seyedali},
+  journal={Journal of Systems Architecture},
+  year={2023},
+  publisher={Elsevier},
+  doi={10.1016/j.sysarc.2023.102871}
+}
 ```
 
 
 
-```code 
+### Related Documents
+
 1. https://neptune.ai/blog/feature-selection-methods
 2. https://www.blog.trainindata.com/feature-selection-machine-learning-with-python/
 3. https://github.com/LBBSoft/FeatureSelect
 4. https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2754-0
 5. https://github.com/scikit-learn-contrib/boruta_py
-6.  https://elki-project.github.io/
+6. https://elki-project.github.io/
 7. https://sci2s.ugr.es/keel/index.php
 8. https://archive.ics.uci.edu/datasets
 9. https://python-charts.com/distribution/box-plot-plotly/
 10. https://plotly.com/python/box-plots/?_ga=2.50659434.2126348639.1688086416-114197406.1688086416#box-plot-styling-mean--standard-deviation
-
-```
```

### Comparing `mafese-0.1.8/mafese/__init__.py` & `mafese-0.1.9/mafese/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 15:23, 06/03/2022 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 from mafese.utils.data_loader import Data, get_dataset
 from mafese.filter import FilterSelector
 from mafese.wrapper.recursive import RecursiveSelector
 from mafese.wrapper.sequential import SequentialSelector
 from mafese.wrapper.mha import MhaSelector, MultiMhaSelector
 from mafese.embedded.lasso import LassoSelector
```

### Comparing `mafese-0.1.8/mafese/data/cls/Arrhythmia.csv` & `mafese-0.1.9/mafese/data/cls/Arrhythmia.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Blood.csv` & `mafese-0.1.9/mafese/data/cls/Blood.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/BreastCancer.csv` & `mafese-0.1.9/mafese/data/cls/BreastCancer.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/BreastEW.csv` & `mafese-0.1.9/mafese/data/cls/BreastEW.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Digits.csv` & `mafese-0.1.9/mafese/data/cls/Digits.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Glass.csv` & `mafese-0.1.9/mafese/data/cls/Glass.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/HeartEW.csv` & `mafese-0.1.9/mafese/data/cls/HeartEW.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Hill-valley.csv` & `mafese-0.1.9/mafese/data/cls/Hill-valley.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Horse.csv` & `mafese-0.1.9/mafese/data/cls/Horse.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Ionosphere.csv` & `mafese-0.1.9/mafese/data/cls/Ionosphere.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Iris.csv` & `mafese-0.1.9/mafese/data/cls/Iris.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Lymphography.csv` & `mafese-0.1.9/mafese/data/cls/Lymphography.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Madelon.csv` & `mafese-0.1.9/mafese/data/cls/Madelon.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Monk1.csv` & `mafese-0.1.9/mafese/data/cls/Monk1.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Monk2.csv` & `mafese-0.1.9/mafese/data/cls/Monk2.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Monk3.csv` & `mafese-0.1.9/mafese/data/cls/Monk3.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Sonar.csv` & `mafese-0.1.9/mafese/data/cls/Sonar.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Soybean-small.csv` & `mafese-0.1.9/mafese/data/cls/Soybean-small.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Vowel.csv` & `mafese-0.1.9/mafese/data/cls/Vowel.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/WaveformEW.csv` & `mafese-0.1.9/mafese/data/cls/WaveformEW.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Wine.csv` & `mafese-0.1.9/mafese/data/cls/Wine.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/Zoo.csv` & `mafese-0.1.9/mafese/data/cls/Zoo.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/aggregation.csv` & `mafese-0.1.9/mafese/data/cls/aggregation.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/aniso.csv` & `mafese-0.1.9/mafese/data/cls/aniso.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/appendicitis.csv` & `mafese-0.1.9/mafese/data/cls/appendicitis.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/balance.csv` & `mafese-0.1.9/mafese/data/cls/balance.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/banknote.csv` & `mafese-0.1.9/mafese/data/cls/banknote.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/blobs.csv` & `mafese-0.1.9/mafese/data/cls/blobs.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/circles.csv` & `mafese-0.1.9/mafese/data/cls/circles.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/diagnosis_II.csv` & `mafese-0.1.9/mafese/data/cls/diagnosis_II.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/ecoli.csv` & `mafese-0.1.9/mafese/data/cls/ecoli.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/flame.csv` & `mafese-0.1.9/mafese/data/cls/flame.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/heart.csv` & `mafese-0.1.9/mafese/data/cls/heart.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/jain.csv` & `mafese-0.1.9/mafese/data/cls/jain.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/liver.csv` & `mafese-0.1.9/mafese/data/cls/liver.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/moons.csv` & `mafese-0.1.9/mafese/data/cls/moons.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/mouse.csv` & `mafese-0.1.9/mafese/data/cls/mouse.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/pathbased.csv` & `mafese-0.1.9/mafese/data/cls/pathbased.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/seeds.csv` & `mafese-0.1.9/mafese/data/cls/seeds.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/smiley.csv` & `mafese-0.1.9/mafese/data/cls/smiley.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/varied.csv` & `mafese-0.1.9/mafese/data/cls/varied.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/vary-density.csv` & `mafese-0.1.9/mafese/data/cls/vary-density.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/vertebral2.csv` & `mafese-0.1.9/mafese/data/cls/vertebral2.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/cls/wdbc.csv` & `mafese-0.1.9/mafese/data/cls/wdbc.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/reg/boston-housing.csv` & `mafese-0.1.9/mafese/data/reg/boston-housing.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/reg/computer-hardware.csv` & `mafese-0.1.9/mafese/data/reg/computer-hardware.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/reg/diabetes.csv` & `mafese-0.1.9/mafese/data/reg/diabetes.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/reg/gauss-100-20.csv` & `mafese-0.1.9/mafese/data/reg/gauss-100-20.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/reg/gauss-50-12.csv` & `mafese-0.1.9/mafese/data/reg/gauss-50-12.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/reg/gauss-75-17.csv` & `mafese-0.1.9/mafese/data/reg/gauss-75-17.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/data/reg/linnerud.csv` & `mafese-0.1.9/mafese/data/reg/linnerud.csv`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/embedded/lasso.py` & `mafese-0.1.9/mafese/embedded/lasso.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/embedded/tree.py` & `mafese-0.1.9/mafese/embedded/tree.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/filter.py` & `mafese-0.1.9/mafese/filter.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/selector.py` & `mafese-0.1.9/mafese/selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 from abc import ABC
 from mafese.utils import validator
 from mafese.utils.estimator import get_general_estimator
-from mafese.utils.evaluator import get_metrics
+from mafese.utils.evaluator import get_metrics, get_all_classification_metrics, get_all_regression_metrics
 from mafese.utils.data_loader import Data
 
 
 class Selector(ABC):
     """
     Defines an abstract class for Feature Selector.
     """
     name = "Feature Selector"
     SUPPORTED_PROBLEMS = ["classification", "regression"]
     SUPPORTED_ESTIMATORS = ["knn", "svm", "rf", "adaboost", "xgb", "tree", "ann"]
+    SUPPORTED_REGRESSION_METRICS = list(get_all_regression_metrics().keys())
+    SUPPORTED_CLASSIFICATION_METRICS = list(get_all_classification_metrics().keys())
 
     def __init__(self, problem="classification"):
         self.problem = self._set_problem(problem)
         self.selector = None
         self.estimator = None
         self.paras = {}
         self.selected_feature_indexes = []
```

### Comparing `mafese-0.1.8/mafese/unsupervised.py` & `mafese-0.1.9/mafese/unsupervised.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/utils/correlation.py` & `mafese-0.1.9/mafese/utils/correlation.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/utils/data_loader.py` & `mafese-0.1.9/mafese/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/utils/encoder.py` & `mafese-0.1.9/mafese/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/utils/estimator.py` & `mafese-0.1.9/mafese/utils/estimator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/utils/evaluator.py` & `mafese-0.1.9/mafese/utils/evaluator.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,7 +30,24 @@
     final_result = {}
     for key, value in result.items():
         if testcase is None or testcase == "":
             final_result[f"{key}"] = value
         else:
             final_result[f"{key}_{testcase}"] = value
     return final_result
+
+
+def get_all_regression_metrics():
+    UNUSED_METRICS = ("RE", "RB", "AE", "SE", "SLE")
+    dict_results = {}
+    for key, value in RegressionMetric.SUPPORT.items():
+        if (key not in UNUSED_METRICS) and (value["type"] in ("min", "max")):
+            dict_results[key] = value["type"]
+    return dict_results
+
+
+def get_all_classification_metrics():
+    dict_results = {}
+    for key, value in ClassificationMetric.SUPPORT.items():
+        if value["type"] in ("min", "max"):
+            dict_results[key] = value["type"]
+    return dict_results
```

### Comparing `mafese-0.1.8/mafese/utils/mealpy_util.py` & `mafese-0.1.9/mafese/utils/mealpy_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,38 +3,14 @@
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from mealpy.optimizer import Optimizer
 from mealpy import *
-import sys, inspect
-
-
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
-        print(f"Mafese doesn't support optimizer named: {name}.\n"
-              f"Please see the supported Optimizer name from here: https://mealpy.readthedocs.io/en/latest/pages/support.html#classification-table")
 
 
 class FeatureSelectionProblem(Problem):
     def __init__(self, lb, ub, minmax, data=None, estimator=None,
                  transfer_func=None, obj_name=None,
                  metric_class=None, fit_weights=(0.9, 0.1), fit_sign=1, obj_paras=None,
                  name="Feature Selection Problem", **kwargs):
```

### Comparing `mafese-0.1.8/mafese/utils/transfer.py` & `mafese-0.1.9/mafese/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/utils/validator.py` & `mafese-0.1.9/mafese/utils/validator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/wrapper/mha.py` & `mafese-0.1.9/mafese/wrapper/mha.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import os
 from mafese.selector import Selector
 from mafese.utils import validator
 from mafese.utils.estimator import get_general_estimator
 from mafese.utils.mealpy_util import get_optimizer_by_name, get_all_optimizers, FeatureSelectionProblem, Optimizer
 from mafese.utils import transfer
 from mafese.utils.data_loader import Data
-from mafese.utils.evaluator import get_metrics
+from mafese.utils.evaluator import get_metrics, get_all_regression_metrics, get_all_classification_metrics
 from permetrics.regression import RegressionMetric
 from permetrics.classification import ClassificationMetric
 import plotly.express as px
 import plotly.io as pio
 
 pio.kaleido.scope.mathjax = None
 
@@ -98,19 +98,16 @@
     >>> # call transform() on X to filter it down to selected features
     >>> X_filtered = feat_selector.transform(X)
     """
 
     SUPPORT = {
         "estimator": ["knn", "svm", "rf", "adaboost", "xgb", "tree", "ann"],
         "transfer_func": ["vstf_01", "vstf_02", "vstf_03", "vstf_04", "sstf_01", "sstf_02", "sstf_03", "sstf_04"],
-        "regression_objective": {"MAE": "min", "MSE": "min", "RMSE": "min", "MRE": "min", "MAPE": "min", "MASE": "min",
-                             "NSE": "max", "NNSE": "max", "WI": "max", "PCC": "max", "R2s": "max", "R2": "max", "AR2": "max",
-                             "CI": "max", "KGE": "max", "VAF": "max", "A10": "max", "A20": "max"},
-        "classification_objective": {"AS": "max", "PS": "max", "NPV": "max", "RS": "max", "F1S": "max", "F2S": "max",
-                             "FBS": "max", "SS": "max", "MCC": "max", "JSI": "max", "CKS": "max", "ROC-AUC": "max"},
+        "regression_objective": get_all_regression_metrics(),
+        "classification_objective": get_all_classification_metrics(),
         "optimizer": list(get_all_optimizers().keys())
     }
 
     def __init__(self, problem="classification", estimator="knn", estimator_paras=None,
                  optimizer="BaseGA", optimizer_paras=None, transfer_func="vstf_01", obj_name=None):
         super().__init__(problem)
         self.estimator = self._set_estimator(estimator, estimator_paras)
@@ -239,19 +236,16 @@
 
 
 class MultiMhaSelector(Selector):
 
     SUPPORT = {
         "estimator": ["knn", "svm", "rf", "adaboost", "xgb", "tree", "ann"],
         "transfer_func": ["vstf_01", "vstf_02", "vstf_03", "vstf_04", "sstf_01", "sstf_02", "sstf_03", "sstf_04"],
-        "regression_objective": {"MAE": "min", "MSE": "min", "RMSE": "min", "MRE": "min", "MAPE": "min", "MASE": "min",
-                             "NSE": "max", "NNSE": "max", "WI": "max", "PCC": "max", "R2s": "max", "R2": "max", "AR2": "max",
-                             "CI": "max", "KGE": "max", "VAF": "max", "A10": "max", "A20": "max"},
-        "classification_objective": {"AS": "max", "PS": "max", "NPV": "max", "RS": "max", "F1S": "max", "F2S": "max",
-                             "FBS": "max", "SS": "max", "MCC": "max", "JSI": "max", "CKS": "max", "ROC-AUC": "max"},
+        "regression_objective": get_all_regression_metrics(),
+        "classification_objective": get_all_classification_metrics(),
         "optimizer": list(get_all_optimizers().keys())
     }
 
     def __init__(self, problem="classification", estimator="knn", estimator_paras=None,
                  list_optimizers=("BaseGA",), list_optimizer_paras=None, transfer_func="vstf_01", obj_name=None):
         super().__init__(problem)
         self.estimator, self.estimator_paras = self._set_estimator(estimator, estimator_paras)
```

### Comparing `mafese-0.1.8/mafese/wrapper/recursive.py` & `mafese-0.1.9/mafese/wrapper/recursive.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese/wrapper/sequential.py` & `mafese-0.1.9/mafese/wrapper/sequential.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/mafese.egg-info/PKG-INFO` & `mafese-0.1.9/mafese.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafese
-Version: 0.1.8
+Version: 0.1.9
 Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
 Home-page: https://github.com/thieu1995/mafese
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mafese
@@ -38,20 +38,24 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-<p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
+<p align="center">
+<img style="max-width:100%;" 
+src="https://thieu1995.github.io/post/2023-08/mafese-02.png" 
+alt="MAFESE"/>
+</p>
 
----
 
+---
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.8-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.9-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -60,46 +64,57 @@
 [![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
 ![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/mafese.svg)
 [![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![DOI](https://zenodo.org/badge/545209353.svg)](https://doi.org/10.5281/zenodo.7969042)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
-MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library for feature selection problem 
-using meta-heuristic algorithms. 
+MAFESE (Metaheuristic Algorithms for FEature SElection) is the biggest python library for feature selection (FS) 
+problem using meta-heuristic algorithms.
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
+* **Total Wrapper-based (Metaheuristic Algorithms)**: > 200 methods
 * **Total Filter-based (Statistical-based)**: > 15 methods
 * **Total Embedded-based (Tree and Lasso)**: > 10 methods
 * **Total Unsupervised-based**: >= 4 methods
-* **Total classification dataset**: >= 30 datasets
-* **Total regression dataset**: >= 7 datasets
-* **Total performance metrics (as fitness)**: > 30 metrics
+* **Total datasets**: >= 30 (47 classifications and 7 regressions)
+* **Total performance metrics**: >= 61 (45 regressions and 16 classifications)
+* **Total objective functions (as fitness functions)**: >= 61 (45 regressions and 16 classifications)
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
-* **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
-* **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics
+* **Python versions:** >= 3.7.x
+* **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics, plotly, kaleido
 
 
 # Installation
 
-### Install with pip
-
-Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
+* Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.8
+$ pip install mafese==0.1.9
 ```
 
-### Install directly from source code
+* Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
 ```
 
+* In case, you want to install the development version from Github:
+```sh 
+$ pip install git+https://github.com/thieu1995/mafese 
+```
+
+After installation, you can import MAFESE as any other Python module:
+
+```sh
+$ python
+>>> import mafese
+>>> mafese.__version__
+```
+
 
 ### Lib's structure
 
 ```code 
 docs
 examples
 mafese
@@ -131,31 +146,18 @@
         validator.py
     __init__.py
     selector.py
 README.md
 setup.py
 ```
 
-
-# Usage
-
-After installation, you can import MAFESE as any other Python module:
-
-```sh
-$ python
->>> import mafese
->>> mafese.__version__
-```
+### Examples
 
 Let's go through some examples.
 
-
-
-### Examples
-
 #### 1. First, load dataset. You can use the available datasets from Mafese:
 
 ```python 
 # Load available dataset from MAFESE
 from mafese import get_dataset
 
 # Try unknown data
@@ -272,17 +274,23 @@
 ii) You can use the same estimator in feature selection process 
 ```python 
 X_test, y_test = data.X_test, data.y_test
 feat_selector.evaluate(estimator=None, data=data, metrics=["AS", "PS", "RS"])
 ```
 
 1) Where do I find the supported metrics like above ["AS", "PS", "RS"]. What is that?
-You can find it here: https://github.com/thieu1995/permetrics
+You can find it here: https://github.com/thieu1995/permetrics or use this 
+```python 
+from mafese import MhaSelector 
 
-2) How do I know my Selector support which estimator? which methods?
+print(MhaSelector.SUPPORTED_REGRESSION_METRICS)
+print(MhaSelector.SUPPORTED_CLASSIFICATION_METRICS)
+```
+
+3) How do I know my Selector support which estimator? which methods?
 ```python 
 print(feat_selector.SUPPORT) 
 ```
 Or you better read the document from: https://mafese.readthedocs.io/en/latest/
 
 3) I got this type of error
 ```python 
@@ -323,58 +331,68 @@
 data.split_train_test(test_size=0.2, random_state=10)   # Try different random_state value 
 ```
 
 
 For more usage examples please look at [examples](/examples) folder.
 
 
-# Get helps (questions, problems)
+# Support (questions, problems)
+
+### Official Links 
 
 * Official source code repo: https://github.com/thieu1995/mafese
 * Official document: https://mafese.readthedocs.io/
 * Download releases: https://pypi.org/project/mafese/
 * Issue tracker: https://github.com/thieu1995/mafese/issues
 * Notable changes log: https://github.com/thieu1995/mafese/blob/master/ChangeLog.md
 * Examples with different mealpy version: https://github.com/thieu1995/mafese/blob/master/examples.md
 * Official chat group: https://t.me/+fRVCJGuGJg1mNDg1
 
-* This project also related to our another projects which are "meta-heuristics", "neural-network", and "optimization" 
-  check it here
+* This project also related to our another projects which are "optimization" and "machine learning", check it here:
     * https://github.com/thieu1995/mealpy
     * https://github.com/thieu1995/metaheuristics
     * https://github.com/thieu1995/opfunu
     * https://github.com/thieu1995/enoppy
     * https://github.com/thieu1995/permetrics
+    * https://github.com/thieu1995/MetaCluster
+    * https://github.com/thieu1995/pfevaluator
     * https://github.com/aiir-team
 
+### Citation Request 
 
-# References 
-
-If you are using mafese in your project, we would appreciate citations:
+Please include these citations if you plan to use this library:
 
 ```code 
 @software{nguyen_van_thieu_2023_7969043,
-  author       = {Nguyen Van Thieu},
-  title        = {MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library},
+  author       = {Nguyen Van Thieu, Ngoc Hung Nguyen, Ali Asghar Heidari},
+  title        = {Feature Selection using Metaheuristics Made Easy: Open Source MAFESE Library in Python},
   month        = may,
   year         = 2023,
   publisher    = {Zenodo},
   doi          = {10.5281/zenodo.7969042},
   url          = {https://github.com/thieu1995/mafese}
 }
+
+@article{van2023mealpy,
+  title={MEALPY: An open-source library for latest meta-heuristic algorithms in Python},
+  author={Van Thieu, Nguyen and Mirjalili, Seyedali},
+  journal={Journal of Systems Architecture},
+  year={2023},
+  publisher={Elsevier},
+  doi={10.1016/j.sysarc.2023.102871}
+}
 ```
 
 
 
-```code 
+### Related Documents
+
 1. https://neptune.ai/blog/feature-selection-methods
 2. https://www.blog.trainindata.com/feature-selection-machine-learning-with-python/
 3. https://github.com/LBBSoft/FeatureSelect
 4. https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2754-0
 5. https://github.com/scikit-learn-contrib/boruta_py
-6.  https://elki-project.github.io/
+6. https://elki-project.github.io/
 7. https://sci2s.ugr.es/keel/index.php
 8. https://archive.ics.uci.edu/datasets
 9. https://python-charts.com/distribution/box-plot-plotly/
 10. https://plotly.com/python/box-plots/?_ga=2.50659434.2126348639.1688086416-114197406.1688086416#box-plot-styling-mean--standard-deviation
-
-```
```

### Comparing `mafese-0.1.8/mafese.egg-info/SOURCES.txt` & `mafese-0.1.9/mafese.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/setup.py` & `mafese-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="mafese",
-    version="0.1.8",
+    version="0.1.9",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["engineering optimization problems", "mathematical optimization",
               "feature selection", "classification problem",
@@ -67,14 +67,14 @@
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Topic :: Software Development :: Build Tools",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
     ],
     install_requires=["numpy>=1.17.1", "scipy>=1.7.1", "scikit-learn>=1.0.2",
-                      "pandas>=1.3.5", "mealpy>=2.5.3", "permetrics>=1.3.3",
+                      "pandas>=1.3.5", "mealpy>=2.5.4", "permetrics>=1.4.2",
                       "plotly>=5.10.0", "kaleido>=0.2.1"],
     extras_require={
         "dev": ["pytest>=7.0", "pytest-cov==4.0.0", "flake8>=4.0.1"],
     },
     python_requires='>=3.7',
 )
```

### Comparing `mafese-0.1.8/tests/test_embedded.py` & `mafese-0.1.9/tests/test_embedded.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/tests/test_filter.py` & `mafese-0.1.9/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/tests/test_unsupervised.py` & `mafese-0.1.9/tests/test_unsupervised.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.8/tests/test_wrapper.py` & `mafese-0.1.9/tests/test_wrapper.py`

 * *Files identical despite different names*

