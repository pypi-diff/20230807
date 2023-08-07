# Comparing `tmp/siman-1.4.0.tar.gz` & `tmp/siman-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/siman-1.4.0.tar", last modified: Thu Aug  3 08:59:39 2023, max compression
+gzip compressed data, was "dist/siman-1.4.1.tar", last modified: Mon Aug  7 11:55:55 2023, max compression
```

## Comparing `siman-1.4.0.tar` & `siman-1.4.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.780261 siman-1.4.0/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.4.0/LICENSE
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.4.0/MANIFEST.in
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-08-03 08:59:39.780261 siman-1.4.0/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.4.0/README.md
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-08-03 08:59:39.780261 siman-1.4.0/setup.cfg
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-08-03 08:59:36.000000 siman-1.4.0/setup.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.777261 siman-1.4.0/siman/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2023-07-14 10:44:19.000000 siman-1.4.0/siman/3d_plot.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2023-07-14 10:44:19.000000 siman-1.4.0/siman/SSHTools.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       32 2023-07-14 10:44:19.000000 siman-1.4.0/siman/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50708 2023-07-16 18:04:57.000000 siman-1.4.0/siman/analysis.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2023-07-14 10:44:19.000000 siman-1.4.0/siman/analysis_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.777261 siman-1.4.0/siman/analyze/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.4.0/siman/analyze/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.4.0/siman/analyze/segregation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2023-07-14 10:44:19.000000 siman-1.4.0/siman/approximation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2023-07-14 10:44:19.000000 siman-1.4.0/siman/bands.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   120904 2023-07-26 17:08:05.000000 siman-1.4.0/siman/calc_manage.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2023-07-14 10:44:19.000000 siman-1.4.0/siman/calcul.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.778261 siman-1.4.0/siman/calculators/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.4.0/siman/calculators/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.4.0/siman/calculators/aims.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.4.0/siman/calculators/gaussian.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.4.0/siman/calculators/qe.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56599 2023-07-16 18:04:57.000000 siman-1.4.0/siman/calculators/vasp.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.4.0/siman/calculators/vasp_old.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.778261 siman-1.4.0/siman/chg/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.4.0/siman/chg/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.4.0/siman/chg/chg_func.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.4.0/siman/chg/vasputil_chgarith_module.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    11041 2023-07-16 18:04:57.000000 siman-1.4.0/siman/classes.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.779261 siman-1.4.0/siman/core/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.4.0/siman/core/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53318 2023-07-16 18:04:57.000000 siman-1.4.0/siman/core/calculation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.4.0/siman/core/calculation_old.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33350 2023-07-14 09:47:42.000000 siman-1.4.0/siman/core/cluster_batch_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3783 2023-07-26 16:52:32.000000 siman-1.4.0/siman/core/cluster_run_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2122 2023-07-16 18:04:57.000000 siman-1.4.0/siman/core/molecule.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   119405 2023-07-16 18:04:57.000000 siman-1.4.0/siman/core/structure.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    20407 2023-07-18 15:59:51.000000 siman-1.4.0/siman/database.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2023-07-14 10:44:19.000000 siman-1.4.0/siman/default_project_conf.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2023-07-14 10:44:19.000000 siman-1.4.0/siman/dev_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33287 2023-07-14 10:44:19.000000 siman-1.4.0/siman/dos_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2023-07-14 10:44:19.000000 siman-1.4.0/siman/fit_hex.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-07-14 10:44:19.000000 siman-1.4.0/siman/functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   113839 2023-07-14 10:44:19.000000 siman-1.4.0/siman/geo.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16531 2023-07-26 16:52:32.000000 siman-1.4.0/siman/header.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      286 2023-07-14 10:44:19.000000 siman-1.4.0/siman/helper_for_writing_beatiful_code.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    40269 2023-07-14 10:44:19.000000 siman-1.4.0/siman/impurity.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    88257 2023-08-03 08:41:20.000000 siman-1.4.0/siman/inout.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2023-07-14 10:44:19.000000 siman-1.4.0/siman/kpoints_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.779261 siman-1.4.0/siman/mat_prop/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.4.0/siman/mat_prop/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.4.0/siman/mat_prop/mat_prop.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    46189 2023-07-14 10:44:19.000000 siman-1.4.0/siman/matproj_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2023-07-14 10:44:19.000000 siman-1.4.0/siman/monte.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      980 2023-07-14 10:44:19.000000 siman-1.4.0/siman/monte_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31637 2023-07-14 10:44:19.000000 siman-1.4.0/siman/neb.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2023-07-14 10:44:19.000000 siman-1.4.0/siman/pairs.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50595 2023-07-29 18:04:07.000000 siman-1.4.0/siman/picture_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2023-07-14 10:44:19.000000 siman-1.4.0/siman/plot_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-14 10:44:19.000000 siman-1.4.0/siman/polaron.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2023-07-14 10:44:19.000000 siman-1.4.0/siman/polaron_hop.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2023-07-14 10:44:19.000000 siman-1.4.0/siman/polaron_mod.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   194660 2023-07-26 17:00:29.000000 siman-1.4.0/siman/project_funcs.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2023-07-14 10:44:19.000000 siman-1.4.0/siman/properties_2d.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2023-07-14 10:44:19.000000 siman-1.4.0/siman/properties_energy.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2023-07-14 10:44:19.000000 siman-1.4.0/siman/properties_lattice.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    30687 2023-07-14 10:44:19.000000 siman-1.4.0/siman/set_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2023-07-14 10:44:19.000000 siman-1.4.0/siman/simanrc.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      174 2023-07-14 10:44:19.000000 siman-1.4.0/siman/small_classes.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6663 2023-07-14 10:44:19.000000 siman-1.4.0/siman/small_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2023-07-14 10:44:19.000000 siman-1.4.0/siman/structure_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2023-07-14 10:44:19.000000 siman-1.4.0/siman/table_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2023-07-14 10:44:19.000000 siman-1.4.0/siman/thermo.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2023-07-14 10:44:19.000000 siman-1.4.0/siman/workflow_utilities.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.777261 siman-1.4.0/siman.egg-info/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-08-03 08:59:39.000000 siman-1.4.0/siman.egg-info/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-08-03 08:59:39.000000 siman-1.4.0/siman.egg-info/SOURCES.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-08-03 08:59:39.000000 siman-1.4.0/siman.egg-info/dependency_links.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-08-03 08:59:39.000000 siman-1.4.0/siman.egg-info/requires.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-08-03 08:59:39.000000 siman-1.4.0/siman.egg-info/top_level.txt
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-07 11:55:55.353443 siman-1.4.1/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.4.1/LICENSE
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.4.1/MANIFEST.in
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-08-07 11:55:55.353443 siman-1.4.1/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.4.1/README.md
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-08-07 11:55:55.353443 siman-1.4.1/setup.cfg
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-08-07 11:55:52.000000 siman-1.4.1/setup.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-07 11:55:55.350443 siman-1.4.1/siman/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2023-07-14 10:44:19.000000 siman-1.4.1/siman/3d_plot.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2023-07-14 10:44:19.000000 siman-1.4.1/siman/SSHTools.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       32 2023-07-14 10:44:19.000000 siman-1.4.1/siman/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50708 2023-07-16 18:04:57.000000 siman-1.4.1/siman/analysis.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2023-07-14 10:44:19.000000 siman-1.4.1/siman/analysis_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-07 11:55:55.350443 siman-1.4.1/siman/analyze/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.4.1/siman/analyze/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.4.1/siman/analyze/segregation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2023-07-14 10:44:19.000000 siman-1.4.1/siman/approximation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2023-07-14 10:44:19.000000 siman-1.4.1/siman/bands.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   120904 2023-07-26 17:08:05.000000 siman-1.4.1/siman/calc_manage.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2023-07-14 10:44:19.000000 siman-1.4.1/siman/calcul.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-07 11:55:55.351443 siman-1.4.1/siman/calculators/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.4.1/siman/calculators/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.4.1/siman/calculators/aims.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.4.1/siman/calculators/gaussian.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.4.1/siman/calculators/qe.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56599 2023-07-16 18:04:57.000000 siman-1.4.1/siman/calculators/vasp.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.4.1/siman/calculators/vasp_old.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-07 11:55:55.351443 siman-1.4.1/siman/chg/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.4.1/siman/chg/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.4.1/siman/chg/chg_func.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.4.1/siman/chg/vasputil_chgarith_module.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    11041 2023-07-16 18:04:57.000000 siman-1.4.1/siman/classes.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-07 11:55:55.352443 siman-1.4.1/siman/core/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.4.1/siman/core/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53359 2023-08-07 11:53:59.000000 siman-1.4.1/siman/core/calculation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.4.1/siman/core/calculation_old.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33350 2023-07-14 09:47:42.000000 siman-1.4.1/siman/core/cluster_batch_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3783 2023-07-26 16:52:32.000000 siman-1.4.1/siman/core/cluster_run_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2122 2023-07-16 18:04:57.000000 siman-1.4.1/siman/core/molecule.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   119405 2023-07-16 18:04:57.000000 siman-1.4.1/siman/core/structure.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    20407 2023-07-18 15:59:51.000000 siman-1.4.1/siman/database.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2023-07-14 10:44:19.000000 siman-1.4.1/siman/default_project_conf.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2023-07-14 10:44:19.000000 siman-1.4.1/siman/dev_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33308 2023-08-04 17:05:30.000000 siman-1.4.1/siman/dos_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2023-07-14 10:44:19.000000 siman-1.4.1/siman/fit_hex.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    28293 2023-08-07 11:38:09.000000 siman-1.4.1/siman/functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   113839 2023-07-14 10:44:19.000000 siman-1.4.1/siman/geo.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16531 2023-07-26 16:52:32.000000 siman-1.4.1/siman/header.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      286 2023-07-14 10:44:19.000000 siman-1.4.1/siman/helper_for_writing_beatiful_code.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    40269 2023-07-14 10:44:19.000000 siman-1.4.1/siman/impurity.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    88257 2023-08-03 08:41:20.000000 siman-1.4.1/siman/inout.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2023-07-14 10:44:19.000000 siman-1.4.1/siman/kpoints_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-07 11:55:55.352443 siman-1.4.1/siman/mat_prop/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.4.1/siman/mat_prop/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.4.1/siman/mat_prop/mat_prop.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    46189 2023-07-14 10:44:19.000000 siman-1.4.1/siman/matproj_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2023-07-14 10:44:19.000000 siman-1.4.1/siman/monte.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      980 2023-07-14 10:44:19.000000 siman-1.4.1/siman/monte_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31637 2023-07-14 10:44:19.000000 siman-1.4.1/siman/neb.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2023-07-14 10:44:19.000000 siman-1.4.1/siman/pairs.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50595 2023-07-29 18:04:07.000000 siman-1.4.1/siman/picture_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2023-07-14 10:44:19.000000 siman-1.4.1/siman/plot_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-14 10:44:19.000000 siman-1.4.1/siman/polaron.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2023-07-14 10:44:19.000000 siman-1.4.1/siman/polaron_hop.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2023-07-14 10:44:19.000000 siman-1.4.1/siman/polaron_mod.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   194660 2023-07-26 17:00:29.000000 siman-1.4.1/siman/project_funcs.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2023-07-14 10:44:19.000000 siman-1.4.1/siman/properties_2d.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2023-07-14 10:44:19.000000 siman-1.4.1/siman/properties_energy.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2023-07-14 10:44:19.000000 siman-1.4.1/siman/properties_lattice.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    30687 2023-07-14 10:44:19.000000 siman-1.4.1/siman/set_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2023-07-14 10:44:19.000000 siman-1.4.1/siman/simanrc.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      174 2023-07-14 10:44:19.000000 siman-1.4.1/siman/small_classes.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6663 2023-07-14 10:44:19.000000 siman-1.4.1/siman/small_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2023-07-14 10:44:19.000000 siman-1.4.1/siman/structure_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2023-07-14 10:44:19.000000 siman-1.4.1/siman/table_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2023-07-14 10:44:19.000000 siman-1.4.1/siman/thermo.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2023-07-14 10:44:19.000000 siman-1.4.1/siman/workflow_utilities.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-07 11:55:55.350443 siman-1.4.1/siman.egg-info/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-08-07 11:55:55.000000 siman-1.4.1/siman.egg-info/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-08-07 11:55:55.000000 siman-1.4.1/siman.egg-info/SOURCES.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-08-07 11:55:55.000000 siman-1.4.1/siman.egg-info/dependency_links.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-08-07 11:55:55.000000 siman-1.4.1/siman.egg-info/requires.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-08-07 11:55:55.000000 siman-1.4.1/siman.egg-info/top_level.txt
```

### Comparing `siman-1.4.0/LICENSE` & `siman-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/PKG-INFO` & `siman-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.4.0
+Version: 1.4.1
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.4.0/setup.py` & `siman-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="siman",
-    version="1.4.0",
+    version="1.4.1",
     author="Dmitry Aksenov",
     author_email="dimonaks@gmail.com",
     description="Manager for DFT calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dimonaks/siman",
     license = 'GPL',
```

### Comparing `siman-1.4.0/siman/3d_plot.py` & `siman-1.4.1/siman/3d_plot.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/SSHTools.py` & `siman-1.4.1/siman/SSHTools.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/analysis.py` & `siman-1.4.1/siman/analysis.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/analysis_functions.py` & `siman-1.4.1/siman/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/analyze/segregation.py` & `siman-1.4.1/siman/analyze/segregation.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/approximation.py` & `siman-1.4.1/siman/approximation.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/bands.py` & `siman-1.4.1/siman/bands.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/calc_manage.py` & `siman-1.4.1/siman/calc_manage.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/calcul.py` & `siman-1.4.1/siman/calcul.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/calculators/aims.py` & `siman-1.4.1/siman/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/calculators/gaussian.py` & `siman-1.4.1/siman/calculators/gaussian.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/calculators/qe.py` & `siman-1.4.1/siman/calculators/qe.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/calculators/vasp.py` & `siman-1.4.1/siman/calculators/vasp.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/calculators/vasp_old.py` & `siman-1.4.1/siman/calculators/vasp_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/chg/chg_func.py` & `siman-1.4.1/siman/chg/chg_func.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/chg/vasputil_chgarith_module.py` & `siman-1.4.1/siman/chg/vasputil_chgarith_module.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/classes.py` & `siman-1.4.1/siman/classes.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/core/calculation.py` & `siman-1.4.1/siman/core/calculation.py`

 * *Files 1% similar despite different names*

```diff
@@ -806,22 +806,24 @@
 
         if fontsize:
             # header.mpl.rcParams.update({'font.size': fontsize+4})
             # fontsize = 2
             SMALL_SIZE = fontsize
             MEDIUM_SIZE = fontsize
             BIGGER_SIZE = fontsize
-
-            header.mpl.rc('font', size=SMALL_SIZE)          # controls default text sizes
-            header.mpl.rc('axes', titlesize=SMALL_SIZE)     # fontsize of the axes title
-            header.mpl.rc('axes', labelsize=MEDIUM_SIZE)    # fontsize of the x and y labels
-            header.mpl.rc('xtick', labelsize=SMALL_SIZE)    # fontsize of the tick labels
-            header.mpl.rc('ytick', labelsize=SMALL_SIZE)    # fontsize of the tick labels
-            header.mpl.rc('legend', fontsize=SMALL_SIZE)    # legend fontsize
-            header.mpl.rc('figure', titlesize=BIGGER_SIZE)  # fontsize of the figure title
+            
+            from siman.picture_functions import mpl
+            
+            mpl.rc('font', size=SMALL_SIZE)          # controls default text sizes
+            mpl.rc('axes', titlesize=SMALL_SIZE)     # fontsize of the axes title
+            mpl.rc('axes', labelsize=MEDIUM_SIZE)    # fontsize of the x and y labels
+            mpl.rc('xtick', labelsize=SMALL_SIZE)    # fontsize of the tick labels
+            mpl.rc('ytick', labelsize=SMALL_SIZE)    # fontsize of the tick labels
+            mpl.rc('legend', fontsize=SMALL_SIZE)    # legend fontsize
+            mpl.rc('figure', titlesize=BIGGER_SIZE)  # fontsize of the figure title
 
 
 
 
         if not iatoms:
             #just one plot
             plot_dos(cl,  iatom = iTM+1,  
@@ -1276,15 +1278,15 @@
 
         if os.path.exists(path_to_file) and '2' not in up: 
             out = None
         else:
             # printlog('File', path_to_file, 'was not found. Trying to update from server')
             out = get_from_server(path2file_cluster, os.path.dirname(path_to_file), addr = address)
             if out:
-                printlog('File', path2file_cluster, 'was not found, trying archive:',header.PATH2ARCHIVE, imp = 'Y')
+                printlog('File', path2file_cluster, 'was not found! checking remote and local archives ...', imp = 'Y')
                 # printlog(out, imp  = 'Y')
 
         if out:
             if header.PATH2ARCHIVE:
                 # printlog('Charge file', path_to_file, 'was not found')
                 try:
                     pp = self.project_path_cluster.replace(self.cluster_home, '') #project path without home
@@ -1292,39 +1294,39 @@
                     pp = ''
                 # print(pp)
                 path_to_file_scratch = header.PATH2ARCHIVE+'/'+pp+'/'+path_to_file
 
                 out = get_from_server(path_to_file_scratch, os.path.dirname(path_to_file), addr = self.cluster['address'])
                 
                 if out:
-                    printlog('File', path_to_file, ' was downloaded from archive', imp = 'e')
+                    printlog('File', path_to_file_scratch, 'was not found, trying local archive path', imp = 'n')
 
                 else:
-                    printlog('File', path_to_file_scratch, 'was not found, trying local archive path', imp = 'Y')
+                    printlog('File', path_to_file, ' was downloaded from archive', imp = 'Y')
 
 
             else:
-                printlog('project_conf.PATH2ARCHIVE is empty, trying local archive path', imp = 'Y')
+                printlog('project_conf.PATH2ARCHIVE is empty, trying local archive path', imp = 'n')
 
 
         if out: 
             if header.PATH2ARCHIVE_LOCAL:
 
                 path_to_file_AL= header.PATH2ARCHIVE_LOCAL+'/'+path_to_file
                 # print(path_to_file_AL)
                 if os.path.exists(path_to_file_AL):
                     shutil.copyfile(path_to_file_AL, path_to_file)
 
                     printlog('Succefully found in local archive and copied to the current project folder', imp = 'Y')
                 else:
-                    printlog('File', path_to_file_AL,'not found in local archive', imp = 'Y')
+                    printlog('File', path_to_file_AL,'not found in local archive', imp = 'n')
 
             else:
                 path_to_file = None
-                printlog('project_path.PATH2ARCHIVE_LOCAL is empty', imp = 'Y')
+                printlog('project_path.PATH2ARCHIVE_LOCAL is empty, skipping', imp = 'n')
 
 
 
         return path_to_file
 
     def run_on_server(self, command, addr = None):
         setting_sshpass(self)
```

### Comparing `siman-1.4.0/siman/core/calculation_old.py` & `siman-1.4.1/siman/core/calculation_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/core/cluster_batch_script.py` & `siman-1.4.1/siman/core/cluster_batch_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/core/cluster_run_script.py` & `siman-1.4.1/siman/core/cluster_run_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/core/molecule.py` & `siman-1.4.1/siman/core/molecule.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/core/structure.py` & `siman-1.4.1/siman/core/structure.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/database.py` & `siman-1.4.1/siman/database.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/default_project_conf.py` & `siman-1.4.1/siman/default_project_conf.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/dev_functions.py` & `siman-1.4.1/siman/dev_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/dos_functions.py` & `siman-1.4.1/siman/dos_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -641,14 +641,15 @@
         # print(orbitals)
         for orb in orbitals:
             printlog('Orbital is ', orb, imp = 'y')
             # sys.exit()
             i = 0
             for n, l, iat, el, d in zip(names, lts, atoms,els, ds):
                 if el in ['Ti','Fe', 'Co', 'V', 'Mn', 'Ni'] and orb in ['p', 's', 'p_all']:
+                    
                     continue
                 if el == 'O' and orb in ('d', 't2g', 'eg', 'dxy', 'dyz', 'dxz', 'dz2', 'dx2', 'd_all'):
                     continue
                 nam = orb
                 nam_down = nam+'_down'
                 # print('name', n)
                 # print('lts', l)
```

### Comparing `siman-1.4.0/siman/fit_hex.py` & `siman-1.4.1/siman/fit_hex.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/functions.py` & `siman-1.4.1/siman/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -347,21 +347,27 @@
         else:
             to_file_l = to_file
 
         makedir(to_file_l)
 
         out = download(file, to_file_l)
 
-        if out and trygz:
+        if out and trygz and not header.SIMAN_WEB:
 
             printlog('File', file, 'does not exist, trying gz', imp = 'n')
             # run_on_server
             files = run_on_server(' ls '+file+'*', addr)
+            if 'No such file' in files:
+                printlog('    No gz either!', imp = 'n')
+
+                break
             file = files.split()[-1]
             # print(file)
+            printlog('From the list files', files, 'the last file is taken:', file, '', imp = 'n')
+
             nz = file.count('gz')
             ext = '.gz'*nz
 
             # file+='.gz'
             to_file_l+=ext
 
             if file:
```

### Comparing `siman-1.4.0/siman/geo.py` & `siman-1.4.1/siman/geo.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/header.py` & `siman-1.4.1/siman/header.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/impurity.py` & `siman-1.4.1/siman/impurity.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/inout.py` & `siman-1.4.1/siman/inout.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/kpoints_functions.py` & `siman-1.4.1/siman/kpoints_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/mat_prop/mat_prop.py` & `siman-1.4.1/siman/mat_prop/mat_prop.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/matproj_functions.py` & `siman-1.4.1/siman/matproj_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/monte.py` & `siman-1.4.1/siman/monte.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/monte_functions.py` & `siman-1.4.1/siman/monte_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/neb.py` & `siman-1.4.1/siman/neb.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/pairs.py` & `siman-1.4.1/siman/pairs.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/picture_functions.py` & `siman-1.4.1/siman/picture_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/plot_functions.py` & `siman-1.4.1/siman/plot_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/polaron.py` & `siman-1.4.1/siman/polaron.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/polaron_hop.py` & `siman-1.4.1/siman/polaron_hop.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/polaron_mod.py` & `siman-1.4.1/siman/polaron_mod.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/project_funcs.py` & `siman-1.4.1/siman/project_funcs.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/properties_2d.py` & `siman-1.4.1/siman/properties_2d.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/properties_energy.py` & `siman-1.4.1/siman/properties_energy.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/properties_lattice.py` & `siman-1.4.1/siman/properties_lattice.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/set_functions.py` & `siman-1.4.1/siman/set_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/simanrc.py` & `siman-1.4.1/siman/simanrc.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/small_functions.py` & `siman-1.4.1/siman/small_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/structure_functions.py` & `siman-1.4.1/siman/structure_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/table_functions.py` & `siman-1.4.1/siman/table_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/thermo.py` & `siman-1.4.1/siman/thermo.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman/workflow_utilities.py` & `siman-1.4.1/siman/workflow_utilities.py`

 * *Files identical despite different names*

### Comparing `siman-1.4.0/siman.egg-info/PKG-INFO` & `siman-1.4.1/siman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.4.0
+Version: 1.4.1
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.4.0/siman.egg-info/SOURCES.txt` & `siman-1.4.1/siman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

