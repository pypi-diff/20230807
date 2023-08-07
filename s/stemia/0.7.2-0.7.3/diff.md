# Comparing `tmp/stemia-0.7.2.tar.gz` & `tmp/stemia-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stemia-0.7.2.tar", last modified: Fri Aug  4 17:12:14 2023, max compression
+gzip compressed data, was "stemia-0.7.3.tar", last modified: Mon Aug  7 15:17:38 2023, max compression
```

## Comparing `stemia-0.7.2.tar` & `stemia-0.7.3.tar`

### file list

```diff
@@ -1,80 +1,79 @@
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.708431 stemia-0.7.2/
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.698431 stemia-0.7.2/.github/
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.701764 stemia-0.7.2/.github/workflows/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      978 2022-04-11 14:23:40.000000 stemia-0.7.2/.github/workflows/deploy.yml
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       12 2022-04-11 14:23:40.000000 stemia-0.7.2/.gitignore
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    35149 2022-04-11 14:23:40.000000 stemia-0.7.2/LICENSE
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    14455 2023-08-04 17:12:14.708431 stemia-0.7.2/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    13350 2023-08-02 14:56:58.000000 stemia-0.7.2/README.md
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.701764 stemia-0.7.2/docs/
--rwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)      568 2022-04-11 14:23:40.000000 stemia-0.7.2/docs/generate_readme.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      192 2022-04-11 14:23:40.000000 stemia-0.7.2/pyproject.toml
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1911 2023-08-04 17:12:14.708431 stemia-0.7.2/setup.cfg
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.701764 stemia-0.7.2/stemia/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      798 2023-08-04 16:48:15.000000 stemia-0.7.2/stemia/__init__.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      160 2023-08-04 17:12:14.000000 stemia-0.7.2/stemia/_version.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.701764 stemia-0.7.2/stemia/aretomo/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       59 2022-04-11 14:23:40.000000 stemia-0.7.2/stemia/aretomo/__init__.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1119 2022-04-11 14:23:40.000000 stemia-0.7.2/stemia/aretomo/aln2xf.py
--rwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)      343 2022-04-11 14:23:40.000000 stemia-0.7.2/stemia/aretomo/batch.sh
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.705098 stemia-0.7.2/stemia/aretomo/batch_warp/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       22 2022-04-20 16:08:24.000000 stemia-0.7.2/stemia/aretomo/batch_warp/__init__.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4743 2023-06-29 08:24:36.000000 stemia-0.7.2/stemia/aretomo/batch_warp/aretomo.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      982 2022-04-25 08:11:45.000000 stemia-0.7.2/stemia/aretomo/batch_warp/fix.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1577 2023-04-14 11:56:12.000000 stemia-0.7.2/stemia/aretomo/batch_warp/fix_mdoc.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     8816 2023-05-09 13:01:47.000000 stemia-0.7.2/stemia/aretomo/batch_warp/main.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4225 2023-06-29 08:24:08.000000 stemia-0.7.2/stemia/aretomo/batch_warp/parse.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      995 2022-05-04 11:58:56.000000 stemia-0.7.2/stemia/aretomo/batch_warp/stack.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1495 2022-09-21 09:50:11.000000 stemia-0.7.2/stemia/aretomo/batch_warp/threaded.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1493 2023-04-14 10:13:44.000000 stemia-0.7.2/stemia/aretomo/batch_warp/topaz.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.705098 stemia-0.7.2/stemia/cryosparc/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       61 2022-04-11 14:23:40.000000 stemia-0.7.2/stemia/cryosparc/__init__.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.705098 stemia-0.7.2/stemia/cryosparc/csplot/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       22 2022-05-05 15:58:18.000000 stemia-0.7.2/stemia/cryosparc/csplot/__init__.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1675 2022-11-29 17:02:24.000000 stemia-0.7.2/stemia/cryosparc/csplot/main.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     6768 2023-03-29 12:16:09.000000 stemia-0.7.2/stemia/cryosparc/csplot/parse.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1060 2022-05-05 15:55:26.000000 stemia-0.7.2/stemia/cryosparc/csplot/plot.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1226 2023-01-24 16:11:10.000000 stemia-0.7.2/stemia/cryosparc/fix_filament_ids.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2137 2023-03-15 10:17:51.000000 stemia-0.7.2/stemia/cryosparc/generate_tilt_angles.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1627 2023-05-23 13:09:08.000000 stemia-0.7.2/stemia/cryosparc/merge_defects_gainref.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.705098 stemia-0.7.2/stemia/image/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       50 2022-04-11 14:23:40.000000 stemia-0.7.2/stemia/image/__init__.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.705098 stemia-0.7.2/stemia/image/center_filament/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       33 2022-04-11 14:23:40.000000 stemia-0.7.2/stemia/image/center_filament/__init__.py
--rwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)     2696 2022-04-11 14:23:40.000000 stemia-0.7.2/stemia/image/center_filament/center_filament.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3648 2022-04-11 14:23:40.000000 stemia-0.7.2/stemia/image/center_filament/funcs.py
--rwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)     3164 2023-08-04 15:25:34.000000 stemia-0.7.2/stemia/image/classify_densities.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1822 2023-08-04 07:54:29.000000 stemia-0.7.2/stemia/image/create_mask.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2813 2023-03-13 15:27:29.000000 stemia-0.7.2/stemia/image/extract_z_snapshots.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2446 2022-04-11 14:23:40.000000 stemia-0.7.2/stemia/image/flip_z.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1440 2023-05-31 09:55:55.000000 stemia-0.7.2/stemia/image/fourier_crop.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1281 2022-04-11 14:23:40.000000 stemia-0.7.2/stemia/image/rescale.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.708431 stemia-0.7.2/stemia/imod/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       54 2023-08-04 07:56:23.000000 stemia-0.7.2/stemia/imod/__init__.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1775 2023-08-03 09:37:11.000000 stemia-0.7.2/stemia/imod/find_NAD_params.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.708431 stemia-0.7.2/stemia/relion/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       58 2023-04-19 14:38:33.000000 stemia-0.7.2/stemia/relion/__init__.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3767 2023-04-19 14:38:33.000000 stemia-0.7.2/stemia/relion/align_filament_particles.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.708431 stemia-0.7.2/stemia/utils/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        0 2022-04-11 14:06:35.000000 stemia-0.7.2/stemia/utils/__init__.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3629 2023-08-04 17:06:57.000000 stemia-0.7.2/stemia/utils/click.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3497 2023-08-04 07:54:29.000000 stemia-0.7.2/stemia/utils/image_processing.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2725 2023-04-14 07:53:59.000000 stemia-0.7.2/stemia/utils/io_.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.708431 stemia-0.7.2/stemia/warp/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       56 2022-04-11 14:23:40.000000 stemia-0.7.2/stemia/warp/__init__.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1706 2023-02-09 14:24:11.000000 stemia-0.7.2/stemia/warp/fix_mdoc.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1431 2023-07-24 14:21:09.000000 stemia-0.7.2/stemia/warp/merge_star.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1874 2023-04-19 14:38:33.000000 stemia-0.7.2/stemia/warp/offset_angle.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      315 2022-04-11 14:23:40.000000 stemia-0.7.2/stemia/warp/parse_xml.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1065 2022-04-11 14:23:40.000000 stemia-0.7.2/stemia/warp/prepare_isonet.py
--rwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)     1252 2022-06-08 12:59:40.000000 stemia-0.7.2/stemia/warp/preprocess_serialem.sh
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1912 2023-03-08 10:19:20.000000 stemia-0.7.2/stemia/warp/spoof_mdoc.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2011 2022-09-20 11:31:25.000000 stemia-0.7.2/stemia/warp/summarize.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-08-04 17:12:14.701764 stemia-0.7.2/stemia.egg-info/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    14455 2023-08-04 17:12:14.000000 stemia-0.7.2/stemia.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1829 2023-08-04 17:12:14.000000 stemia-0.7.2/stemia.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-08-04 17:12:14.000000 stemia-0.7.2/stemia.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-08-04 17:12:14.000000 stemia-0.7.2/stemia.egg-info/entry_points.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-08-04 17:12:14.000000 stemia-0.7.2/stemia.egg-info/not-zip-safe
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      919 2023-08-04 17:12:14.000000 stemia-0.7.2/stemia.egg-info/requires.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        7 2023-08-04 17:12:14.000000 stemia-0.7.2/stemia.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.053570 stemia-0.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.029570 stemia-0.7.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.033570 stemia-0.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-07 15:17:18.000000 stemia-0.7.3/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 15:17:18.000000 stemia-0.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 15:17:18.000000 stemia-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-08-07 15:17:38.053570 stemia-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-08-07 15:17:18.000000 stemia-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.033570 stemia-0.7.3/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-08-07 15:17:18.000000 stemia-0.7.3/docs/generate_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-07 15:17:18.000000 stemia-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-07 15:17:38.053570 stemia-0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.033570 stemia-0.7.3/stemia/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-07 15:17:37.000000 stemia-0.7.3/stemia/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.037570 stemia-0.7.3/stemia/aretomo/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/aretomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/aretomo/aln2xf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/aretomo/batch.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.041570 stemia-0.7.3/stemia/aretomo/batch_warp/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/aretomo/batch_warp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/aretomo/batch_warp/aretomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/aretomo/batch_warp/fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/aretomo/batch_warp/fix_mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/aretomo/batch_warp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/aretomo/batch_warp/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/aretomo/batch_warp/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/aretomo/batch_warp/threaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/aretomo/batch_warp/topaz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.041570 stemia-0.7.3/stemia/cryosparc/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/cryosparc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.045570 stemia-0.7.3/stemia/cryosparc/csplot/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/cryosparc/csplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/cryosparc/csplot/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/cryosparc/csplot/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/cryosparc/csplot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/cryosparc/fix_filament_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/cryosparc/generate_tilt_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/cryosparc/merge_defects_gainref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.045570 stemia-0.7.3/stemia/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.045570 stemia-0.7.3/stemia/image/center_filament/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/image/center_filament/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2696 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/image/center_filament/center_filament.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/image/center_filament/funcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3185 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/image/classify_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/image/create_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/image/extract_z_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/image/flip_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/image/fourier_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/image/rescale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.045570 stemia-0.7.3/stemia/imod/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/imod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/imod/find_NAD_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.049570 stemia-0.7.3/stemia/relion/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/relion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/relion/align_filament_particles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.049570 stemia-0.7.3/stemia/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/utils/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/utils/io_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.053570 stemia-0.7.3/stemia/warp/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/warp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/warp/fix_mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/warp/offset_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/warp/parse_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/warp/prepare_isonet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/warp/preprocess_serialem.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/warp/spoof_mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-07 15:17:18.000000 stemia-0.7.3/stemia/warp/summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:17:38.037570 stemia-0.7.3/stemia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-08-07 15:17:38.000000 stemia-0.7.3/stemia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-07 15:17:38.000000 stemia-0.7.3/stemia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:17:38.000000 stemia-0.7.3/stemia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 15:17:38.000000 stemia-0.7.3/stemia.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:17:38.000000 stemia-0.7.3/stemia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-07 15:17:38.000000 stemia-0.7.3/stemia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 15:17:38.000000 stemia-0.7.3/stemia.egg-info/top_level.txt
```

### Comparing `stemia-0.7.2/.github/workflows/deploy.yml` & `stemia-0.7.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/LICENSE` & `stemia-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/PKG-INFO` & `stemia-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemia
-Version: 0.7.2
+Version: 0.7.3
 Summary: Scripts and Tools for Electron Microscopy Analysis.
 Home-page: https://github.com/brisvag/stemia/
 Author: Lorenzo Gaifas
 Author-email: brisvag@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `stemia-0.7.2/README.md` & `stemia-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/docs/generate_readme.py` & `stemia-0.7.3/docs/generate_readme.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/setup.cfg` & `stemia-0.7.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/__init__.py` & `stemia-0.7.3/stemia/__init__.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/aretomo/aln2xf.py` & `stemia-0.7.3/stemia/aretomo/aln2xf.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/aretomo/batch_warp/aretomo.py` & `stemia-0.7.3/stemia/aretomo/batch_warp/aretomo.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/aretomo/batch_warp/fix.py` & `stemia-0.7.3/stemia/aretomo/batch_warp/fix.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/aretomo/batch_warp/fix_mdoc.py` & `stemia-0.7.3/stemia/aretomo/batch_warp/fix_mdoc.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/aretomo/batch_warp/main.py` & `stemia-0.7.3/stemia/aretomo/batch_warp/main.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/aretomo/batch_warp/parse.py` & `stemia-0.7.3/stemia/aretomo/batch_warp/parse.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/aretomo/batch_warp/stack.py` & `stemia-0.7.3/stemia/aretomo/batch_warp/stack.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/aretomo/batch_warp/threaded.py` & `stemia-0.7.3/stemia/aretomo/batch_warp/threaded.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/aretomo/batch_warp/topaz.py` & `stemia-0.7.3/stemia/aretomo/batch_warp/topaz.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/cryosparc/csplot/main.py` & `stemia-0.7.3/stemia/cryosparc/csplot/main.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/cryosparc/csplot/parse.py` & `stemia-0.7.3/stemia/cryosparc/csplot/parse.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/cryosparc/csplot/plot.py` & `stemia-0.7.3/stemia/cryosparc/csplot/plot.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/cryosparc/fix_filament_ids.py` & `stemia-0.7.3/stemia/cryosparc/fix_filament_ids.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/cryosparc/generate_tilt_angles.py` & `stemia-0.7.3/stemia/cryosparc/generate_tilt_angles.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/cryosparc/merge_defects_gainref.py` & `stemia-0.7.3/stemia/cryosparc/merge_defects_gainref.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/image/center_filament/center_filament.py` & `stemia-0.7.3/stemia/image/center_filament/center_filament.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/image/center_filament/funcs.py` & `stemia-0.7.3/stemia/image/center_filament/funcs.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/image/classify_densities.py` & `stemia-0.7.3/stemia/image/classify_densities.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,11 +80,11 @@
 
         for cl, df_cl in progress.track(df.groupby('class'), description='Splitting classes...'):
             stacked = {}
             for img in df_cl.index:
                 *img_name, idx = img.split('_')
                 img_name = '_'.join(img_name)
                 idx = int(idx)
-                stacked[img_name] = images[img_name][idx]
+                stacked.setdefault(img_name, []).append(images[img_name][idx])
             for img_name, data in stacked.items():
                 mrc = mrcfile.new(f'{img_name}_class_{cl:04}.mrc', np.stack(data), overwrite=True)
                 mrc.close()
```

### Comparing `stemia-0.7.2/stemia/image/create_mask.py` & `stemia-0.7.3/stemia/image/create_mask.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/image/extract_z_snapshots.py` & `stemia-0.7.3/stemia/image/extract_z_snapshots.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/image/flip_z.py` & `stemia-0.7.3/stemia/image/flip_z.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/image/fourier_crop.py` & `stemia-0.7.3/stemia/image/fourier_crop.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/image/rescale.py` & `stemia-0.7.3/stemia/image/rescale.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/imod/find_NAD_params.py` & `stemia-0.7.3/stemia/imod/find_NAD_params.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/relion/align_filament_particles.py` & `stemia-0.7.3/stemia/relion/align_filament_particles.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/utils/click.py` & `stemia-0.7.3/stemia/utils/click.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/utils/image_processing.py` & `stemia-0.7.3/stemia/utils/image_processing.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/utils/io_.py` & `stemia-0.7.3/stemia/utils/io_.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/warp/fix_mdoc.py` & `stemia-0.7.3/stemia/warp/fix_mdoc.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/warp/offset_angle.py` & `stemia-0.7.3/stemia/warp/offset_angle.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/warp/prepare_isonet.py` & `stemia-0.7.3/stemia/warp/prepare_isonet.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/warp/preprocess_serialem.sh` & `stemia-0.7.3/stemia/warp/preprocess_serialem.sh`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/warp/spoof_mdoc.py` & `stemia-0.7.3/stemia/warp/spoof_mdoc.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia/warp/summarize.py` & `stemia-0.7.3/stemia/warp/summarize.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.2/stemia.egg-info/PKG-INFO` & `stemia-0.7.3/stemia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemia
-Version: 0.7.2
+Version: 0.7.3
 Summary: Scripts and Tools for Electron Microscopy Analysis.
 Home-page: https://github.com/brisvag/stemia/
 Author: Lorenzo Gaifas
 Author-email: brisvag@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `stemia-0.7.2/stemia.egg-info/SOURCES.txt` & `stemia-0.7.3/stemia.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,13 @@
 stemia/relion/align_filament_particles.py
 stemia/utils/__init__.py
 stemia/utils/click.py
 stemia/utils/image_processing.py
 stemia/utils/io_.py
 stemia/warp/__init__.py
 stemia/warp/fix_mdoc.py
-stemia/warp/merge_star.py
 stemia/warp/offset_angle.py
 stemia/warp/parse_xml.py
 stemia/warp/prepare_isonet.py
 stemia/warp/preprocess_serialem.sh
 stemia/warp/spoof_mdoc.py
 stemia/warp/summarize.py
```

### Comparing `stemia-0.7.2/stemia.egg-info/requires.txt` & `stemia-0.7.3/stemia.egg-info/requires.txt`

 * *Files identical despite different names*

