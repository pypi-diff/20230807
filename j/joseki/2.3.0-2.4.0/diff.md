# Comparing `tmp/joseki-2.3.0.tar.gz` & `tmp/joseki-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joseki-2.3.0.tar", last modified: Thu Jul 20 12:59:04 2023, max compression
+gzip compressed data, was "joseki-2.4.0.tar", last modified: Mon Aug  7 12:37:39 2023, max compression
```

## Comparing `joseki-2.3.0.tar` & `joseki-2.4.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1075 2023-07-20 12:58:45.952765 joseki-2.3.0/LICENSE
--rw-r--r--   0        0        0     2048 2023-07-20 12:58:45.952765 joseki-2.3.0/README.md
--rw-r--r--   0        0        0     1813 2023-07-20 12:58:45.960763 joseki-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      421 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/__init__.py
--rw-r--r--   0        0        0     3769 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/__main__.py
--rw-r--r--   0        0        0       22 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/__version__.py
--rw-r--r--   0        0        0    15568 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/accessor.py
--rw-r--r--   0        0        0     1741 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/constants.py
--rw-r--r--   0        0        0     5034 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/core.py
--rw-r--r--   0        0        0       92 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/README.md
--rw-r--r--   0        0        0       22 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/__init__.py
--rw-r--r--   0        0        0      396 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/README.md
--rw-r--r--   0        0        0       84 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/__init__.py
--rw-r--r--   0        0        0     3871 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_1a.csv
--rw-r--r--   0        0        0     3871 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_1b.csv
--rw-r--r--   0        0        0     3871 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_1c.csv
--rw-r--r--   0        0        0     3871 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_1d.csv
--rw-r--r--   0        0        0     3871 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_1e.csv
--rw-r--r--   0        0        0     3871 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_1f.csv
--rw-r--r--   0        0        0     3422 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_2a.csv
--rw-r--r--   0        0        0     3423 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_2b.csv
--rw-r--r--   0        0        0     3426 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_2c.csv
--rw-r--r--   0        0        0     3429 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_2d.csv
--rw-r--r--   0        0        0      151 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/ecmwf/README.md
--rw-r--r--   0        0        0     4542 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/ecmwf/model_levels_60.csv
--rw-r--r--   0        0        0     1788 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/README.md
--rw-r--r--   0        0        0       93 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/__init__.py
--rw-r--r--   0        0        0     5683 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/extra.atm
--rw-r--r--   0        0        0    42274 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/midlatitude_day.atm
--rw-r--r--   0        0        0    42276 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/midlatitude_night.atm
--rw-r--r--   0        0        0    42270 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/polar_summer.atm
--rw-r--r--   0        0        0    42270 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/polar_winter.atm
--rw-r--r--   0        0        0    42270 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/tropical.atm
--rw-r--r--   0        0        0      789 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/__init__.py
--rw-r--r--   0        0        0    13295 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/afgl_1986.py
--rw-r--r--   0        0        0    27728 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/cams.py
--rw-r--r--   0        0        0    13343 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/core.py
--rw-r--r--   0        0        0     1921 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/factory.py
--rw-r--r--   0        0        0    11728 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/mipas_2007.py
--rw-r--r--   0        0        0    10466 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/schema.py
--rw-r--r--   0        0        0     2887 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/ussa_1976.py
--rw-r--r--   0        0        0     4404 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/util.py
--rw-r--r--   0        0        0      393 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/tests_util.py
--rw-r--r--   0        0        0     3325 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/units.py
--rw-r--r--   0        0        0       41 2023-07-20 12:58:45.960763 joseki-2.3.0/tests/__init__.py
--rw-r--r--   0        0        0     2168 2023-07-20 12:58:45.960763 joseki-2.3.0/tests/data/232f85b4-b3e9-47a7-a52d-9f955c38b9f6.nc
--rw-r--r--   0        0        0    11316 2023-07-20 12:58:45.960763 joseki-2.3.0/tests/data/25b63a29-3eab-4599-92f4-7bba42ec6add.zip
--rw-r--r--   0        0        0    56340 2023-07-20 12:58:45.960763 joseki-2.3.0/tests/data/774f1fd2-63c5-4b59-b23d-eadcad7d6b83.zip
--rw-r--r--   0        0        0    29668 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/data/86dbfcd6-9e0b-40df-8ea7-aa2e328339dc.zip
--rw-r--r--   0        0        0    54028 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_ml.nc
--rw-r--r--   0        0        0     1496 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_sfc.nc
--rw-r--r--   0        0        0    55752 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb.zip
--rw-r--r--   0        0        0     3617 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/data/README.md
--rw-r--r--   0        0        0        0 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/data/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/__init__.py
--rw-r--r--   0        0        0     1556 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/test_afgl_1986.py
--rw-r--r--   0        0        0     7227 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/test_cams.py
--rw-r--r--   0        0        0     7023 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/test_core.py
--rw-r--r--   0        0        0      160 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/test_factory.py
--rw-r--r--   0        0        0     6159 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/test_mipas_2007.py
--rw-r--r--   0        0        0      233 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/test_ussa_1976.py
--rw-r--r--   0        0        0      767 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/test_util.py
--rw-r--r--   0        0        0     7066 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/test_accessor.py
--rw-r--r--   0        0        0     4832 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/test_core.py
--rw-r--r--   0        0        0     2918 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/test_main.py
--rw-r--r--   0        0        0     1972 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/test_units.py
--rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 joseki-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-08-07 12:37:13.796116 joseki-2.4.0/LICENSE
+-rw-r--r--   0        0        0     2219 2023-08-07 12:37:13.796116 joseki-2.4.0/README.md
+-rw-r--r--   0        0        0     1813 2023-08-07 12:37:13.804116 joseki-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      421 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/__init__.py
+-rw-r--r--   0        0        0     3248 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/__main__.py
+-rw-r--r--   0        0        0       22 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/__version__.py
+-rw-r--r--   0        0        0    14649 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/accessor.py
+-rw-r--r--   0        0        0     1741 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/constants.py
+-rw-r--r--   0        0        0     6195 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/core.py
+-rw-r--r--   0        0        0       92 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/README.md
+-rw-r--r--   0        0        0       22 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/__init__.py
+-rw-r--r--   0        0        0      396 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/afgl_1986/README.md
+-rw-r--r--   0        0        0       84 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/afgl_1986/__init__.py
+-rw-r--r--   0        0        0     3871 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/afgl_1986/table_1a.csv
+-rw-r--r--   0        0        0     3871 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/afgl_1986/table_1b.csv
+-rw-r--r--   0        0        0     3871 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/afgl_1986/table_1c.csv
+-rw-r--r--   0        0        0     3871 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/afgl_1986/table_1d.csv
+-rw-r--r--   0        0        0     3871 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/afgl_1986/table_1e.csv
+-rw-r--r--   0        0        0     3871 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/afgl_1986/table_1f.csv
+-rw-r--r--   0        0        0     3422 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/afgl_1986/table_2a.csv
+-rw-r--r--   0        0        0     3423 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/afgl_1986/table_2b.csv
+-rw-r--r--   0        0        0     3426 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/afgl_1986/table_2c.csv
+-rw-r--r--   0        0        0     3429 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/afgl_1986/table_2d.csv
+-rw-r--r--   0        0        0      151 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/ecmwf/README.md
+-rw-r--r--   0        0        0     4542 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/ecmwf/model_levels_60.csv
+-rw-r--r--   0        0        0     1788 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/mipas_2007/README.md
+-rw-r--r--   0        0        0       93 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/mipas_2007/__init__.py
+-rw-r--r--   0        0        0     5683 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/mipas_2007/extra.atm
+-rw-r--r--   0        0        0    42274 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/mipas_2007/midlatitude_day.atm
+-rw-r--r--   0        0        0    42276 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/mipas_2007/midlatitude_night.atm
+-rw-r--r--   0        0        0    42270 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/mipas_2007/polar_summer.atm
+-rw-r--r--   0        0        0    42270 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/mipas_2007/polar_winter.atm
+-rw-r--r--   0        0        0    42270 2023-08-07 12:37:13.804116 joseki-2.4.0/src/joseki/data/mipas_2007/tropical.atm
+-rw-r--r--   0        0        0      789 2023-08-07 12:37:13.808116 joseki-2.4.0/src/joseki/profiles/__init__.py
+-rw-r--r--   0        0        0    13295 2023-08-07 12:37:13.808116 joseki-2.4.0/src/joseki/profiles/afgl_1986.py
+-rw-r--r--   0        0        0    30840 2023-08-07 12:37:13.808116 joseki-2.4.0/src/joseki/profiles/cams.py
+-rw-r--r--   0        0        0    10759 2023-08-07 12:37:13.808116 joseki-2.4.0/src/joseki/profiles/core.py
+-rw-r--r--   0        0        0     1921 2023-08-07 12:37:13.808116 joseki-2.4.0/src/joseki/profiles/factory.py
+-rw-r--r--   0        0        0    11728 2023-08-07 12:37:13.808116 joseki-2.4.0/src/joseki/profiles/mipas_2007.py
+-rw-r--r--   0        0        0    10466 2023-08-07 12:37:13.808116 joseki-2.4.0/src/joseki/profiles/schema.py
+-rw-r--r--   0        0        0     2887 2023-08-07 12:37:13.808116 joseki-2.4.0/src/joseki/profiles/ussa_1976.py
+-rw-r--r--   0        0        0     4545 2023-08-07 12:37:13.808116 joseki-2.4.0/src/joseki/profiles/util.py
+-rw-r--r--   0        0        0      393 2023-08-07 12:37:13.808116 joseki-2.4.0/src/joseki/tests_util.py
+-rw-r--r--   0        0        0     3325 2023-08-07 12:37:13.808116 joseki-2.4.0/src/joseki/units.py
+-rw-r--r--   0        0        0       41 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     2168 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/data/232f85b4-b3e9-47a7-a52d-9f955c38b9f6.nc
+-rw-r--r--   0        0        0    11316 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/data/25b63a29-3eab-4599-92f4-7bba42ec6add.zip
+-rw-r--r--   0        0        0    56340 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/data/774f1fd2-63c5-4b59-b23d-eadcad7d6b83.zip
+-rw-r--r--   0        0        0    29668 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/data/86dbfcd6-9e0b-40df-8ea7-aa2e328339dc.zip
+-rw-r--r--   0        0        0    54028 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_ml.nc
+-rw-r--r--   0        0        0     1496 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_sfc.nc
+-rw-r--r--   0        0        0    55752 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb.zip
+-rw-r--r--   0        0        0     3617 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/data/README.md
+-rw-r--r--   0        0        0        0 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/profiles/__init__.py
+-rw-r--r--   0        0        0     1556 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/profiles/test_afgl_1986.py
+-rw-r--r--   0        0        0     7227 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/profiles/test_cams.py
+-rw-r--r--   0        0        0     6510 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/profiles/test_core.py
+-rw-r--r--   0        0        0      160 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/profiles/test_factory.py
+-rw-r--r--   0        0        0     6159 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/profiles/test_mipas_2007.py
+-rw-r--r--   0        0        0      233 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/profiles/test_ussa_1976.py
+-rw-r--r--   0        0        0      767 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/profiles/test_util.py
+-rw-r--r--   0        0        0     6165 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/test_accessor.py
+-rw-r--r--   0        0        0     4934 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/test_core.py
+-rw-r--r--   0        0        0     2494 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/test_main.py
+-rw-r--r--   0        0        0     1972 2023-08-07 12:37:13.808116 joseki-2.4.0/tests/test_units.py
+-rw-r--r--   0        0        0     2931 1970-01-01 00:00:00.000000 joseki-2.4.0/PKG-INFO
```

### Comparing `joseki-2.3.0/LICENSE` & `joseki-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/README.md` & `joseki-2.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 ## Features
 
 * Available profiles:
   * *AFGL Atmospheric Constituent Profiles (0-120 km)*
   * *MIPAS (2007) reference atmospheres*
   * *U.S. Standard Atmosphere, 1976*
 * Specify the altitude mesh to interpolate the atmospheric profile at.
-* Move from the nodes-representation to the cells-representation of the 
-  altitude mesh.
 * Command-line interface.
 * Python API.
 
 
 ## Requirements
 
 * Python 3.8+
@@ -46,16 +44,24 @@
 
 ```shell
 conda install -c conda-forge joseki
 ```
 
 ## Documentation
 
-Visit https://nollety.github.io/joseki/latest.
+Visit https://rayference.github.io/joseki/latest.
 
 ## Ikigai
 
 *Joseki* was born in the context of the development of the 
 [Eradiate](https://github.com/eradiate/eradiate) radiative transfer model, from
 the need to collect, document and trace, integrate and modify *popular* 
 thermophysical profiles.
 As such, its features evolve in close relationship to those of *Eradiate*.
+
+## About
+
+Joseki is written and maintained by [Yvan Nollet](https://github.com/nollety).
+
+Development is supported by [Rayference](https://www.rayference.eu).
+
+Joseki is a component of the [Eradiate radiative transfer model](https://www.eradiate.eu/site/).
```

### Comparing `joseki-2.3.0/pyproject.toml` & `joseki-2.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "xarray>=2022.12.0",
     "ussa1976>=0.3.4",
     "attrs>=22.2.0",
     "importlib-resources>=5.10.2",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "2.3.0"
+version = "2.4.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Changelog = "https://github.com/nollety/joseki/blob/main/docs/changelog.md"
 homepage = "https://github.com/nollety/joseki"
```

### Comparing `joseki-2.3.0/src/joseki/__main__.py` & `joseki-2.4.0/src/joseki/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -57,30 +57,18 @@
     "--altitude-units",
     "-u",
     help="Altitude units",
     default="km",
     show_default=True,
 )
 @click.option(
-    "--represent-in-cells",
-    "-r",
-    help=(
-        "Compute the cells representation of the atmospheric profile. The "
-        "initial altitude values are used to define the altitude bounds of "
-        "each cell. The pressure, temperature, number density and mixing "
-        "ratio fields are interpolated at the cells' center altitudes."
-    ),
-    is_flag=True,
-)
-@click.option(
     "--conserve-column",
     "-c",
     help=(
-        "Ensure that column densities are conserved during interpolation or "
-        "when representing the profile in cells."
+        "Ensure that column densities are conserved during interpolation."
     ),
     is_flag=True,
 )
 @click.option(
     "--p-interp-method",
     "-p",
     help="Pressure interpolation method.",
@@ -126,15 +114,14 @@
 )
 @click.version_option()
 def main(
     file_name: str,
     identifier: str,
     altitudes: t.Optional[str],
     altitude_units: str,
-    represent_in_cells: bool,
     conserve_column: bool,
     p_interp_method: str,
     t_interp_method: str,
     n_interp_method: str,
     x_interp_method: str,
 ) -> None:
     """Joseki command-line interface."""
@@ -154,15 +141,14 @@
     }
 
     # make dataset
     ds = make(
         identifier=identifier,
         z=z,
         interp_method=interp_method,
-        represent_in_cells=represent_in_cells,
         conserve_column=conserve_column,
     )
 
     # write dataset
     ds.to_netcdf(file_name)
```

### Comparing `joseki-2.3.0/src/joseki/accessor.py` & `joseki-2.4.0/src/joseki/accessor.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,61 +97,35 @@
             * $z$ is the altitude,
             * $x_{\mathrm{M}}(z)$ is the mole fraction of molecule M
             at altitude $z$,
             * $n(z)$ is the air number density at altitude $z$,
             * $n_{\mathrm{M}}(z)$ is the number density of molecule M at
             altitude $z$.
 
-            If the dataset has a `z_bounds` coordinate, the integral is computed
-            using the centered rectangle method, where the `z` coordinate
-            corresponds to the rectangle centers.
-
-            If the dataset does not have a `z_bounds` coordinate, the 
-            integration is performed using the trapezoidal rule.
+            The  integration is performed using the trapezoidal rule.
         """
         ds = self._obj
-        try:
-            with xr.set_options(keep_attrs=True):
-                dz = to_quantity(ds.z_bounds.diff(dim="zbv", n=1).squeeze())
-            
-            logger.debug(
-                "Computing column number density using the centered rectangle "
-                "rule."
-            )
-
-            n = to_quantity(ds.n)
-
-            _column_number_density = {}
-            for m in self.molecules:
-                xm = to_quantity(ds[f"x_{m}"])
-                _column_number_density[m] = (
-                    (xm * n * dz).sum().to_base_units()
-                )  # integrate using the centered rectangle rule
-
-            return _column_number_density
-
-        except AttributeError:  # z_bounds attribute does not exist
+        
+        logger.debug(
+            "Computing column number density using the trapezoidal rule."
+        )
 
-            logger.debug(
-                "Computing column number density using the trapezoidal rule."
+        _column_number_density = {}
+        for m in self.molecules:
+            integral = (ds[f"x_{m}"] * ds.n).integrate(
+                coord="z"
+            )  # integrate using the trapezoidal rule
+            units = " ".join(
+                [ds[var].attrs["units"] for var in [f"x_{m}", "n", "z"]]
             )
+            _column_number_density[m] = (
+                integral.values * ureg.Unit(units)
+            ).to_base_units()
 
-            _column_number_density = {}
-            for m in self.molecules:
-                integral = (ds[f"x_{m}"] * ds.n).integrate(
-                    coord="z"
-                )  # integrate using the trapezoidal rule
-                units = " ".join(
-                    [ds[var].attrs["units"] for var in [f"x_{m}", "n", "z"]]
-                )
-                _column_number_density[m] = (
-                    integral.values * ureg.Unit(units)
-                ).to_base_units()
-
-            return _column_number_density
+        return _column_number_density
 
     @property
     def column_mass_density(
         self,
     ) -> t.Dict[str, pint.Quantity]:
         r"""Compute column mass density.
 
@@ -183,15 +157,18 @@
         """Compute number density at sea level.
 
         Returns:
             A mapping of molecule and number density at sea level.
         """
         ds = self._obj
         n = to_quantity(ds.n.isel(z=0))
-        return {m: (to_quantity(ds[f"x_{m}"].isel(z=0)) * n) for m in self.molecules}
+        return {
+            m: (to_quantity(ds[f"x_{m}"].isel(z=0)) * n)
+            for m in self.molecules
+        }
 
     @property
     def mass_density_at_sea_level(
         self,
     ) -> t.Dict[str, pint.Quantity]:
         """Compute mass density at sea level.
 
@@ -441,14 +418,16 @@
         Args:
             target: Mapping of molecule and target total column density. 
                 Total column must be either a column number density 
                 [`length^-2`], a column mass density [`mass * length^-2`], a 
                 number densitx at sea level [`length^-3`], a mass density at 
                 sea level [`mass * length^-3`], a mole fraction at 
                 sea level [`dimensionless`].
+            check_x_sum: if True, check that mole fraction sums are never
+                larger than one.
         
         Returns:
             Rescaled dataset (new object).    
         """
         return self.rescale(
             factors=self.scaling_factors(target=target),
             check_x_sum=check_x_sum,
```

### Comparing `joseki-2.3.0/src/joseki/constants.py` & `joseki-2.4.0/src/joseki/constants.py`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/afgl_1986/table_1a.csv` & `joseki-2.4.0/src/joseki/data/afgl_1986/table_1a.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/afgl_1986/table_1b.csv` & `joseki-2.4.0/src/joseki/data/afgl_1986/table_1b.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/afgl_1986/table_1c.csv` & `joseki-2.4.0/src/joseki/data/afgl_1986/table_1c.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/afgl_1986/table_1d.csv` & `joseki-2.4.0/src/joseki/data/afgl_1986/table_1d.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/afgl_1986/table_1e.csv` & `joseki-2.4.0/src/joseki/data/afgl_1986/table_1e.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/afgl_1986/table_1f.csv` & `joseki-2.4.0/src/joseki/data/afgl_1986/table_1f.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/afgl_1986/table_2a.csv` & `joseki-2.4.0/src/joseki/data/afgl_1986/table_2a.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/afgl_1986/table_2b.csv` & `joseki-2.4.0/src/joseki/data/afgl_1986/table_2b.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/afgl_1986/table_2c.csv` & `joseki-2.4.0/src/joseki/data/afgl_1986/table_2c.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/afgl_1986/table_2d.csv` & `joseki-2.4.0/src/joseki/data/afgl_1986/table_2d.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/ecmwf/model_levels_60.csv` & `joseki-2.4.0/src/joseki/data/ecmwf/model_levels_60.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/mipas_2007/README.md` & `joseki-2.4.0/src/joseki/data/mipas_2007/README.md`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/mipas_2007/extra.atm` & `joseki-2.4.0/src/joseki/data/mipas_2007/extra.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/mipas_2007/midlatitude_day.atm` & `joseki-2.4.0/src/joseki/data/mipas_2007/midlatitude_day.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/mipas_2007/midlatitude_night.atm` & `joseki-2.4.0/src/joseki/data/mipas_2007/midlatitude_night.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/mipas_2007/polar_summer.atm` & `joseki-2.4.0/src/joseki/data/mipas_2007/polar_summer.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/mipas_2007/polar_winter.atm` & `joseki-2.4.0/src/joseki/data/mipas_2007/polar_winter.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/data/mipas_2007/tropical.atm` & `joseki-2.4.0/src/joseki/data/mipas_2007/tropical.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/profiles/__init__.py` & `joseki-2.4.0/src/joseki/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/profiles/afgl_1986.py` & `joseki-2.4.0/src/joseki/profiles/afgl_1986.py`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/profiles/cams.py` & `joseki-2.4.0/src/joseki/profiles/cams.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,112 @@
           The pressure data injected in the profile build here is also based
           on the *L60 model level table*, i.e. the U.S. Standard Atmosphere, 
           1976 model. This means that the pressure profile is always the same.
     """
     longitude = to_quantity(lon, units="degree")
     latitude = to_quantity(lat, units="degree")
 
+    # format data into timeseries
+    timeseries = from_cams_reanalysis_helper(
+        data=data,
+        identifier=identifier,
+        lat=lat,
+        lon=lon,
+        molecules=molecules,
+        missing_molecules_from=missing_molecules_from,
+        extract_dir=extract_dir,
+        pressure_data=pressure_data,
+    )
+
+    # interpolate data in time
+    # TODO: handle case where time coordinate has 1 value only
+    data = timeseries.interp(
+        time=time,
+        method="linear",
+        kwargs={"bounds_error": True},
+    )
+
+    ds = schema.convert(
+        data_vars={
+            "p": to_quantity(data.p),
+            "t": to_quantity(data.t),
+            **{
+                xm: to_quantity(data[xm])
+                for xm in data if xm.startswith("x_")
+            },
+        },
+        coords={
+            "z": to_quantity(data.z),
+        },
+        attrs=generate_cams_attrs(
+            latitude=latitude,
+            longitude=longitude,
+            time=time,
+            identifier=identifier,
+        )
+    )
+
+    if extrapolate:
+        extrapolate_up = extrapolate.get("up", None)
+        extrapolate_down = extrapolate.get("down", None)
+
+        if extrapolate_up is None and extrapolate_down is None:
+            raise ValueError("Either 'up' or 'down' must be specified.")
+
+        if extrapolate_up:
+            z_up = extrapolate_up.get("z", None)
+            method_up = extrapolate_up.get("method", {"default": "nearest"})
+            ds = _extrapolate(
+                ds=ds,
+                direction="up",
+                z_extra=z_up,
+                method=method_up,
+            )
+        if extrapolate_down:
+            z_down = extrapolate_down.get("z", None)
+            method_down = extrapolate_down.get("method", {"default": "linear"})
+            ds = _extrapolate(
+                ds=ds,
+                direction="down",
+                z_extra=z_down,
+                method=method_down,
+            )
+    else:
+        ds = ds
+
+    if regularize:
+        z = to_quantity(ds.z)
+        default_num = int((z.max() - z.min()) // np.diff(z).min())
+        if isinstance(regularize, bool):
+            regularize = {}
+        ds = _regularize(
+            ds=ds,
+            method=regularize.get("method", DEFAULT_METHOD),
+            conserve_column=regularize.get("conserve_column", False),
+            options=regularize.get('options', {"num": default_num}),
+        )
+    else:
+        ds = ds
+    
+    return ds
+
+def from_cams_reanalysis_helper(
+    data: PathLike | list[PathLike],
+    identifier: str,
+    lat: float | pint.Quantity,
+    lon: float | pint.Quantity,
+    molecules: list[str] | None = None,
+    missing_molecules_from: xr.Dataset | None = None,
+    extract_dir : Path | None = None,
+    pressure_data : str | None = "surface_pressure",
+) -> xr.Dataset:
+    
+    longitude = to_quantity(lon, units="degree")
+    latitude = to_quantity(lat, units="degree")
+
     # Open datasets (we sort by time because CAMS data is not always sorted by 
     # time and this is required to select at a timestamp)
     datasets = [
         xr.open_dataset(p).sortby("time") for p in to_paths(
             cams_data=data,
             extract_dir=extract_dir,
         )
@@ -155,29 +253,27 @@
     logger.debug("Opened %d datasets.", len(datasets))
 
     level_dataset, surface_dataset = identify(datasets)
 
     if level_dataset is None:  # pragma: no cover
         raise ValueError("Could not find a multi-level dataset.") 
 
-    # Select in time and space
-    interpolated = interp_time_space(
+    # Interpolate in space
+    interpolated = interp_space(
         level_dataset,
-        time,
         longitude.m,
         latitude.m,
     )
 
     pressure_data = "surface_pressure" if pressure_data is None else pressure_data
 
     # Read surface pressure if available
     if surface_dataset is not None:
-        surface_selected = interp_time_space(
+        surface_selected = interp_space(
             surface_dataset,
-            time,
             longitude.m,
             latitude.m,
         )
         if "sp" in surface_selected:
             surface_pressure = to_quantity(surface_selected["sp"])
         else:
             if pressure_data == "surface_pressure":  # pragma: no cover
@@ -235,60 +331,99 @@
             raise ValueError(
                 "Missing molecules were requested but no reference dataset "
                 "was provided."
             )
     
     # add missing molecules
     if missing_molecules_from is not None:
+
+        # drop all variables in dataset 'missing_molecules_from' that do not 
+        # start with 'x_'
         _data = missing_molecules_from.drop_vars([
             v for v in missing_molecules_from.data_vars
             if not v.startswith("x_")
         ])
 
+        # list all molecules in dataset 'missing_molecules_from'
         _all_molecules = [x[2:] for x in _data.data_vars]
+
+        # compute molecules to drop in dataset 'missing_molecules_from'
         _drop_molecules = [
             m for m in _all_molecules
             if m not in missing_molecules
         ]
+
+        # select the molecules data to add
         _missing_data = _data.drop_vars([
             f"x_{m}" for m in _drop_molecules
         ])
     
         logger.debug("data z units: %s", data.z.units)
         # missing molecule data must be on the same altitude grid
         _missing_data = _missing_data.interp(
             z=data.z.values,
         )
 
+        # TODO: time coordinate must match or not exist
+        # TODO: if it does not exist, '_missing_data' dims must expanded
+
         # missing molecule data can be added
         data = data.assign(
             **{
                 f"x_{m}": _missing_data[f"x_{m}"]
                 for m in missing_molecules
             }
         )
 
     # add pressure and temperature data
     data = data.assign(
         {
             "p": (
-                    "z",
+                    ["time", "z"],
                     altitude_dataset["p"].values,
-                    {"units": altitude_dataset["p"].units},
+                    {
+                        "standard_name": "air_pressure",
+                        "long_name": "air pressure",
+                        "units": altitude_dataset["p"].units
+                    },
                 ),
             "t": (
-                    "z",
+                    ["time", "z"],
                     altitude_dataset["t"].values,
-                    {"units": altitude_dataset["t"].units},
+                    {
+                        "standard_name": "air_temperature",
+                        "long_name": "air temperature",
+                        "units": altitude_dataset["t"].units
+                    },
                 ),
         }
     )
 
+    lower_time = data.time.values.min()
+    upper_time = data.time.values.max()
+    time = f"{lower_time} to {upper_time}"
+
+    attrs = generate_cams_attrs(
+        latitude=latitude,
+        longitude=longitude,
+        time=time,
+        identifier=identifier,
+    )
+
+    data.attrs.update(attrs)
+
+    return data
 
-    # Dataset attributes
+def generate_cams_attrs(
+    latitude: pint.Quantity,
+    longitude: pint.Quantity,
+    time: str,
+    identifier: str,
+) -> dict:
+    
     INSTITUTION = "European Centre for Medium-Range Weather Forecasts (ECMWF)"
     SOURCE = (
         "4DVar data assimilation in CY42R1 of ECMWF’s Integrated Forecast "
         "System (IFS)"
     )
 
     utcnow = datetime.datetime.utcnow().replace(microsecond=0).isoformat()
@@ -323,86 +458,29 @@
     }
 
     URL_DATE = {
         "EAC4": "2023-06-16",
         "EGG4": "2023-06-16",
     }
 
-    ds = schema.convert(
-        data_vars={
-            "p": to_quantity(data.p),
-            "t": to_quantity(data.t),
-            **{
-                xm: to_quantity(data[xm])
-                for xm in data if xm.startswith("x_")
-            },
-        },
-        coords={
-            "z": to_quantity(data.z),
-        },
-        attrs={
-            "title": "CAMS global reanalysis (EAC4) atmospheric profile",
-            "institution": INSTITUTION,
-            "source": SOURCE,
-            "history": f"{utcnow} - CAMS data converted to Joseki format",
-            "references": REFERENCE[identifier],
-            "comment": COMMENT,
-            "acknowledgment": acknowledgment,
-            "url": URL[identifier],
-            "urldate": URL_DATE[identifier],
-            "latitude": f"{latitude:~}",
-            "longitude": f"{longitude:~}",
-            "Conventions": "CF-1.10",
-        }
-    )
-
-    if extrapolate:
-        #z = to_quantity(ds.z)
-        extrapolate_up = extrapolate.get("up", None)
-        extrapolate_down = extrapolate.get("down", None)
-
-        if extrapolate_up is None and extrapolate_down is None:
-            raise ValueError("Either 'up' or 'down' must be specified.")
-
-        if extrapolate_up:
-            z_up = extrapolate_up.get("z", None)
-            method_up = extrapolate_up.get("method", {"default": "nearest"})
-            ds = _extrapolate(
-                ds=ds,
-                direction="up",
-                z_extra=z_up,
-                method=method_up,
-            )
-        if extrapolate_down:
-            z_down = extrapolate_down.get("z", None)
-            method_down = extrapolate_down.get("method", {"default": "linear"})
-            ds = _extrapolate(
-                ds=ds,
-                direction="down",
-                z_extra=z_down,
-                method=method_down,
-            )
-    else:
-        ds = ds
-
-    if regularize:
-        z = to_quantity(ds.z)
-        default_num = int((z.max() - z.min()) // np.diff(z).min())
-        if isinstance(regularize, bool):
-            regularize = {}
-        ds = _regularize(
-            ds=ds,
-            method=regularize.get("method", DEFAULT_METHOD),
-            conserve_column=regularize.get("conserve_column", False),
-            options=regularize.get('options', {"num": default_num}),
-        )
-    else:
-        ds = ds
-    
-    return ds
+    return {
+        "title": "CAMS global reanalysis (EAC4) atmospheric profile",
+        "institution": INSTITUTION,
+        "source": SOURCE,
+        "history": f"{utcnow} - CAMS data converted to Joseki format",
+        "references": REFERENCE[identifier],
+        "comment": COMMENT,
+        "acknowledgment": acknowledgment,
+        "url": URL[identifier],
+        "urldate": URL_DATE[identifier],
+        "latitude": f"{latitude:~}",
+        "longitude": f"{longitude:~}",
+        "time": time,
+        "Conventions": "CF-1.10",
+    }
 
 
 # TODO: add support for .tar.gz archives
 def from_archive(path: Path, extract_dir : Path | None = None) -> Path:
     """Extract archive file and return directory with extracted files.
 
     Args:
@@ -526,14 +604,37 @@
             level_dataset = dataset
         else:
             surface_dataset = dataset
     
     return level_dataset, surface_dataset
 
 
+def interp_space(
+    ds: xr.Dataset,
+    lon: float,
+    lat: float,
+):
+    """Interpolate a CAMS dataset at specific longitude and latitude.
+    
+    Args:
+        ds: CAMS Dataset.
+        lon: Longitude [degrees].
+        lat: Latitude [degrees].
+
+    Notes:
+        The dataset is interpolated using the linear method.
+    """
+    return ds.interp(
+        latitude=lat,
+        longitude=lon,
+        method="linear",
+        kwargs={"bounds_error": True},
+    )
+
+
 def interp_time_space(
     ds: xr.Dataset,
     datetime: str | datetime.datetime | np.datetime64,
     lon: float,
     lat: float,
 ):
     """Interpolate a CAMS dataset at specific datetime, longitude and latitude.
@@ -590,22 +691,22 @@
         the surface pressure matches the provided surface pressure.
     """
     logger.debug("Rescaling pressure data with surface pressure")
     ds_surface_pressure = to_quantity(ds.p.sel(z=0, method="nearest"))
     logger.debug("Surface pressure: %s", ds_surface_pressure)
     scaling_factor = (
         surface_pressure / ds_surface_pressure
-    ).m_as("dimensionless")
+    ).m_as("dimensionless")[:, np.newaxis]
     logger.debug("Scaling factor: %s", scaling_factor)
     with xr.set_options(keep_attrs=True):
         ds["p"] = ds["p"] * scaling_factor
     return ds
 
 
-# TODO: the model level to altitude conversion is approximated
+# TODO: the model level to altitude conversion is approximate
 def model_level_to_altitude(
     ds: xr.Dataset,
     pressure_data: str = "model_level_60",
     surface_pressure: pint.Quantity | None = None,
 ) -> xr.Dataset:
     """
     Convert model level data to altitude data and add pressure data.
@@ -658,28 +759,39 @@
         },
     )
 
     # first, drop any variable called 'z' as that 
     ds = ds.drop_vars("z") if "z" in ds else ds
 
     interpolated = ds.interp(level=level).drop_vars("level")
+    p = np.array(df["pf [hPa]"].values[1:], dtype=float)
+    p_tiled = np.tile(p, interpolated.time.values.size)
+    p_tiled_reshaped = p_tiled.reshape(interpolated.time.values.size, p.size)
     ds = interpolated.assign(
         {
             "p": (
-                "z",
-                np.array(df["pf [hPa]"].values[1:], dtype=float),
+                ["time", "z"],
+                p_tiled_reshaped,
                 {"units": "hPa"},
             ),
         }
     ).sortby("z")
 
     # Ensure altitude are in kilometer
     z = to_quantity(ds.z)
     ds = ds.assign({
-        "z": ("z", z.m_as("km"), {"units": "km", "long_name": "altitude"})
+        "z": (
+            "z",
+            z.m_as("km"),
+            {
+                "units": "km",
+                "long_name": "altitude",
+                "standard_name": "altitude",
+            }
+        )
     })
 
     if pressure_data == "surface_pressure":  # pragma: no cover
         rescale_pressure_profile(ds, surface_pressure)
 
     # Report on surface pressure discrepancy
     if surface_pressure is not None:  # pragma: no cover
@@ -691,15 +803,15 @@
         )
         logger.info(
             "Surface pressure from CAMS surface dataset, %s",
             f"{surface_pressure:~P}",
         )
         logger.info(
             "Surface pressure discrepancy: %s",
-            f"{rel_diff.m_as('1'):.1%}",
+            f"{rel_diff.to('1'):.1%}",
         )
 
     return ds
 
 
 def mole_fractions(ds: xr.Dataset) -> xr.DataArray:
     """Get the mole fractions data from a dataset.
@@ -728,14 +840,15 @@
                     ds[x].values
                     for x in molecules_cams
                 ]
             )
         ),
         coords={
             "m": ("m", molecules_joseki),
+            "time": ds["time"],
             "z": ds["z"],
         }
     )
 
     # Convert mass mixing ratio to mole mixing ratio
     x = mass_fraction_to_mole_fraction3(y=y)
 
@@ -785,24 +898,29 @@
         )
     ]
     logger.debug("Opened %d datasets.", len(datasets))
 
     _, surface_dataset = identify(datasets)
 
     # Select in time and space
-    selected = interp_time_space(surface_dataset, time, longitude.m, latitude.m)
+    interpolated = interp_time_space(
+        surface_dataset,
+        time,
+        longitude.m,
+        latitude.m,
+    )
 
     amount = {}
-    for dv in selected.data_vars:
+    for dv in interpolated.data_vars:
         try:
             m = MOLECULE_TOTALS[dv]
         except KeyError:  # pragma: no cover
             pass
         else:
-            amount[m] = to_quantity(selected[dv])
+            amount[m] = to_quantity(interpolated[dv])
     
     # check that all molecules are present
     if molecules is not None:
         for m in molecules:
             if m not in amount:
                 raise ValueError(f"Molecule {m} not found in dataset.")
```

### Comparing `joseki-2.3.0/src/joseki/profiles/core.py` & `joseki-2.4.0/src/joseki/profiles/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Core module for atmosphere thermophysical profiles.
 
 The `Profile` abstract class defines the interface for atmosphere thermophysical
 profiles.
 The `interp` function is used to interpolate an atmosphere thermophysical
 profile on new altitude values.
-The `represent_profile_in_cells` function is used to compute the cells
-representation of the atmosphere thermophysical profile.
 """
 import logging
 import typing as t
 from abc import ABC, abstractmethod
 
 import numpy as np
 import pint
@@ -149,82 +147,14 @@
     # Compute scaling factors to conserve column densities
     if conserve_column:
         return rescale_to_column(reference=ds, ds=interpolated)
 
     return interpolated
 
 
-def represent_profile_in_cells(
-    ds: xr.Dataset,
-    method: t.Dict[str, str] = DEFAULT_METHOD,
-    conserve_column: bool = False,
-) -> xr.Dataset:
-    """Compute the cells representation of the atmosphere thermophysical profile.
-
-    Args:
-        ds: Initial atmospheric profile.
-        method: Mapping of variable and interpolation method.
-            If a variable is not in the mapping, the linear interpolation is used.
-            By default, linear interpolation is used for all variables.
-        conserve_column: If True, ensure that column densities are conserved.
-
-    Returns:
-        Cells representation of the atmosphere thermophysical profile.
-
-    Notes:
-        Atmosphere cells (or layers) are defined by two consecutive altitude 
-        values. The layer's center altitude is defined as the arithmetic 
-        average of these two values. The pressure, temperature, number density 
-        and mole fraction fields are interpolated at these layer' center 
-        altitude values. In the new atmospheric profile, the `z` coordinate 
-        is updated with layer' center altitude values and a data variable 
-        `z_bounds` indicating the altitude bounds of each layer, is added.
-        A copy of the dataset is returned, the original dataset is not 
-        modified.
-    """
-    # if the profile is already represented in cells, do nothing
-    if ds.z.standard_name == "layer_center_altitude":
-        return ds
-
-    z_nodes = to_quantity(ds.z)
-    z_centers = (z_nodes[:-1] + z_nodes[1:]) / 2.0
-
-    interpolated = interp(
-        ds=ds,
-        z_new=z_centers,
-        method=method,
-        conserve_column=False,  # we rescale later
-    )
-    interpolated.z.attrs = dict(
-        standard_name="layer_center_altitude",
-        long_name="layer center altitude",
-        units="km",
-    )
-    z_bounds = np.stack([z_nodes[:-1], z_nodes[1:]])
-    interpolated = interpolated.assign(
-        z_bounds=(
-            ("zbv", "z"),
-            z_bounds.m_as("km"),
-            dict(
-                standard_name="cell_bound_altitude",
-                long_name="cell bound altitude",
-                units="km",
-            ),
-        )
-    )
-    interpolated.attrs.update(
-        history=interpolated.history + f"\n{utcnow()} "
-        f"- represent profile on cells - joseki, version {__version__}"
-    )
-
-    if conserve_column:
-        return rescale_to_column(reference=ds, ds=interpolated)
-    return interpolated
-
-
 def extrapolate(
     ds: xr.Dataset,
     z_extra: pint.Quantity,
     direction: str,
     method: t.Dict[str, str] = DEFAULT_METHOD,
     conserve_column: bool = False,
 ) -> xr.Dataset:
```

### Comparing `joseki-2.3.0/src/joseki/profiles/factory.py` & `joseki-2.4.0/src/joseki/profiles/factory.py`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/profiles/mipas_2007.py` & `joseki-2.4.0/src/joseki/profiles/mipas_2007.py`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/profiles/schema.py` & `joseki-2.4.0/src/joseki/profiles/schema.py`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/profiles/ussa_1976.py` & `joseki-2.4.0/src/joseki/profiles/ussa_1976.py`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/src/joseki/profiles/util.py` & `joseki-2.4.0/src/joseki/profiles/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,19 @@
     """
     data_var_name = da.name
     data_var_attrs = da.attrs
     molecules = da.m.values
     ds = xr.Dataset()
     for m in molecules:
         ds[f"{data_var_name}_{m}"] = da.sel(m=m, drop=True)
-        ds[f"{data_var_name}_{m}"].attrs = data_var_attrs
+        ds[f"{data_var_name}_{m}"].attrs = {
+            "standard_name": f"{m}_mole_fraction",
+            "long_name": f"{m} mole fraction",
+            "units": data_var_attrs["units"],
+        }
     return ds
 
 
 def air_molar_mass_from_mass_fraction(
     y: xr.DataArray
 ) -> xr.DataArray:
     r"""
```

### Comparing `joseki-2.3.0/src/joseki/units.py` & `joseki-2.4.0/src/joseki/units.py`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/tests/data/232f85b4-b3e9-47a7-a52d-9f955c38b9f6.nc` & `joseki-2.4.0/tests/data/232f85b4-b3e9-47a7-a52d-9f955c38b9f6.nc`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/tests/data/25b63a29-3eab-4599-92f4-7bba42ec6add.zip` & `joseki-2.4.0/tests/data/25b63a29-3eab-4599-92f4-7bba42ec6add.zip`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/tests/data/774f1fd2-63c5-4b59-b23d-eadcad7d6b83.zip` & `joseki-2.4.0/tests/data/774f1fd2-63c5-4b59-b23d-eadcad7d6b83.zip`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/tests/data/86dbfcd6-9e0b-40df-8ea7-aa2e328339dc.zip` & `joseki-2.4.0/tests/data/86dbfcd6-9e0b-40df-8ea7-aa2e328339dc.zip`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_ml.nc` & `joseki-2.4.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_ml.nc`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_sfc.nc` & `joseki-2.4.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_sfc.nc`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb.zip` & `joseki-2.4.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb.zip`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/tests/data/README.md` & `joseki-2.4.0/tests/data/README.md`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/tests/profiles/test_afgl_1986.py` & `joseki-2.4.0/tests/profiles/test_afgl_1986.py`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/tests/profiles/test_cams.py` & `joseki-2.4.0/tests/profiles/test_cams.py`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/tests/profiles/test_core.py` & `joseki-2.4.0/tests/profiles/test_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from joseki.profiles.core import (
     rescale_to_column,
     interp,
     extrapolate,
     regularize,
     select_molecules,
 )
-from joseki.core import represent_profile_in_cells
 from joseki.units import to_quantity
 
 @pytest.fixture
 def test_data_set() -> xr.Dataset:
     """Test dataset fixture."""
     return make(identifier="afgl_1986-tropical")
 
@@ -78,26 +77,14 @@
         ds=test_data_set,
         z_new=np.linspace(0, 100) * ureg.km,
         bounds_error=True,
     )
     assert interpolated.joseki.is_valid
 
 
-def test_represent_profile_in_cells(test_data_set: xr.Dataset):
-    """Returns a xarray.Dataset object."""
-    interpolated = represent_profile_in_cells(ds=test_data_set)
-    assert isinstance(interpolated, xr.Dataset)
-
-
-def test_represent_profile_in_cells_twice(test_data_set: xr.Dataset):
-    """Running function twice has no effect."""
-    ds1 = represent_profile_in_cells(ds=test_data_set)
-    ds2 = represent_profile_in_cells(ds=ds1)
-    assert ds1 == ds2
-
 @pytest.mark.parametrize(
     "z_down",
     [
         -0.1 * ureg.km,
         np.linspace(-0.5, -0.1, 5) * ureg.km,
     ]
 )
```

### Comparing `joseki-2.3.0/tests/profiles/test_mipas_2007.py` & `joseki-2.4.0/tests/profiles/test_mipas_2007.py`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/tests/profiles/test_util.py` & `joseki-2.4.0/tests/profiles/test_util.py`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/tests/test_accessor.py` & `joseki-2.4.0/tests/test_accessor.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,70 +6,54 @@
 
 import joseki
 from joseki.accessor import _scaling_factor
 from joseki.units import to_quantity
 from joseki.units import ureg
 
 
-def test_column_number_density_integration():
-    """Same result is returned when profile is represented in cells or not."""
-    ds1 = joseki.make("mipas_2007-midlatitude_day")
-    ds2 = joseki.make("mipas_2007-midlatitude_day", represent_in_cells=True)
-    assert_approx_equal(
-        ds1.joseki.column_number_density["CO2"].m,
-        ds2.joseki.column_number_density["CO2"].m,
-        significant=5,
-    )
-
 @pytest.mark.parametrize(
     "identifier",
     ["ussa_1976", "afgl_1986-us_standard", "mipas_2007-midlatitude_day"]
 )
 def test_column_mass_density(identifier: str):
     """Returns a dictionary."""
     ds = joseki.make(identifier)
     assert isinstance(ds.joseki.column_mass_density, dict)
 
 
 @pytest.mark.parametrize(
-    "identifier, represent_in_cells, expected",
+    "identifier, expected",
     [
-        ("afgl_1986-us_standard", True, 14.27 * ureg.kg / ureg.m**2),
-        ("afgl_1986-us_standard", False, 14.38 * ureg.kg / ureg.m**2),
-        ("mipas_2007-midlatitude_day", True, 19.33 * ureg.kg / ureg.m**2),
-        ("mipas_2007-midlatitude_day", False, 19.51 * ureg.kg / ureg.m**2),
+        ("afgl_1986-us_standard", 14.38 * ureg.kg / ureg.m**2),
+        ("mipas_2007-midlatitude_day", 19.51 * ureg.kg / ureg.m**2),
     ]
 )
 def test_water_vapour_column_mass_density_in_cells(
     identifier: str,
-    represent_in_cells: bool,
     expected: pint.Quantity
 ):
     """Column mass density of water vapor is close to expected values."""
-    ds = joseki.make(identifier, represent_in_cells=represent_in_cells)
+    ds = joseki.make(identifier)
     water_vapor_amount = ds.joseki.column_mass_density["H2O"].to("kg/m^2")
     assert_approx_equal(water_vapor_amount.m, expected.m, significant=3)
 
 
 @pytest.mark.parametrize(
-    "identifier, represent_in_cells, expected",
+    "identifier, expected",
     [
-        ("afgl_1986-us_standard", True, 348.3 * ureg.dobson_unit),
-        ("afgl_1986-us_standard", False, 345.7 * ureg.dobson_unit),
-        ("mipas_2007-midlatitude_day", True, 303.4 * ureg.dobson_unit),
-        ("mipas_2007-midlatitude_day", False, 301.7 * ureg.dobson_unit)
+        ("afgl_1986-us_standard", 345.7 * ureg.dobson_unit),
+        ("mipas_2007-midlatitude_day", 301.7 * ureg.dobson_unit)
     ]
 )
 def test_column_number_density(
     identifier: str,
-    represent_in_cells: bool,
     expected: pint.Quantity
 ):
     """Column number density of ozone matches expected value."""
-    ds = joseki.make(identifier, represent_in_cells=represent_in_cells)
+    ds = joseki.make(identifier)
     ozone_amount = ds.joseki.column_number_density["O3"].to("dobson_unit")
     assert_approx_equal(ozone_amount.m, expected.m, significant=3)
 
 
 @pytest.mark.parametrize(
     "identifier", ["afgl_1986-midlatitude_summer", "mipas_2007-midlatitude_day"]
 )
```

### Comparing `joseki-2.3.0/tests/test_core.py` & `joseki-2.4.0/tests/test_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,25 +9,14 @@
 
 
 def test_make():
     """Returns xr.Dataset."""
     assert isinstance(make(identifier="afgl_1986-tropical"), xr.Dataset)
 
 
-def test_make_represent_in_cells():
-    """Returned dataset has dimensions zbv and z and data variable z_bounds."""
-    ds = make(
-        identifier="afgl_1986-tropical",
-        represent_in_cells=True,
-    )
-    for dim in ["zbv", "z"]:
-        assert dim in ds.dims
-    assert "z_bounds" in ds.data_vars
-
-
 def test_make_altitudes():
     """Assigns dataset' altitude values from file."""
     z = np.linspace(0, 120, 121) * ureg.km
     ds = make(identifier="afgl_1986-tropical", z=z)
     assert np.allclose(ds.z.values, z.m_as(ds.z.attrs["units"]))
 
 
@@ -74,15 +63,15 @@
 def test_make_ussa_1976_z():
     """Returns dataset."""
     z = np.linspace(0.0, 100) * ureg.km
     ds = make(identifier="ussa_1976", z=z)
     assert ds.joseki.is_valid
 
 
-def test_make_conserve_column_1():
+def test_make_conserve_column():
     """Column densities are conserved when conserve_column is True."""
     ds0 = make(identifier="afgl_1986-us_standard")
     ds1 = make(
         identifier="afgl_1986-us_standard",
         z=np.linspace(0, 100, 21) * ureg.km,  # different than default
         conserve_column=True,
     )
@@ -90,70 +79,100 @@
     for m in ds0.joseki.molecules:
         assert_approx_equal(
             ds0.joseki.column_number_density[m].m,
             ds1.joseki.column_number_density[m].m,
             significant=6
         )
 
-def test_make_conserve_column_2():
-    """Column densities are conserved when conserve_column is True."""
-    ds0 = make(identifier="afgl_1986-us_standard")
-    ds1 = make(
-        identifier="afgl_1986-us_standard",
-        represent_in_cells=True,
-        conserve_column=True,
+def test_make_molecules():
+    """Returns dataset with molecules corresponding to selection."""
+    ds = make(identifier="afgl_1986-tropical", molecules=["H2O", "CO2"])
+    assert ds.joseki.molecules == ["H2O", "CO2"]
+
+
+def test_make_regularize_bool():
+    """Returns valid dataset with constant altitude step."""
+    ds = make(identifier="afgl_1986-tropical", regularize=True)
+
+    assert np.allclose(
+        np.diff(ds.z.values),
+        np.diff(ds.z.values)[0],
+        rtol=1e-9,
+        atol=1e-6,
     )
+    assert ds.joseki.is_valid
 
-    for m in ds0.joseki.molecules:
-        assert_approx_equal(
-            ds0.joseki.column_number_density[m].m,
-            ds1.joseki.column_number_density[m].m,
-            significant=6
-        )
 
-def test_make_conserve_column_3():
-    """Column densities are conserved when conserve_column is True."""
-    ds0 = make(identifier="afgl_1986-us_standard")
-    ds1 = make(
-        identifier="afgl_1986-us_standard",
-        z=np.linspace(0, 100, 21) * ureg.km,  # different than default
-        represent_in_cells=True,
-        conserve_column=True,
+def test_make_regularize_dict():
+    """Returns valid dataset with constant altitude step."""
+    num = 1201
+    ds = make(
+        identifier="afgl_1986-tropical",
+        regularize={"options": {"num": num}},
     )
 
-    for m in ds0.joseki.molecules:
+    assert ds.z.size == num
+
+
+@pytest.mark.parametrize(
+    "target",
+    [
+        {
+            "H2O": 25 * ureg.kg / ureg.m**2
+        },
+        {
+            "H2O": 25 * ureg.kg / ureg.m**2,
+            "CO2": 420 * ureg.ppm
+        },
+        {
+            "H2O": 25 * ureg.kg / ureg.m**2,
+            "CO2": 420 * ureg.ppm,
+            "O3": 350 * ureg.dobson_unit
+        }
+    ],
+)
+def test_make_rescale_to(target):
+    ds = make(
+        identifier="afgl_1986-tropical",
+        rescale_to=target,
+    )
+    value = {
+        "H2O": ds.joseki.column_mass_density["H2O"],
+        "CO2": ds.joseki.mole_fraction_at_sea_level["CO2"],
+        "O3": ds.joseki.column_number_density["O3"],
+    }
+
+    for molecule in target:
         assert_approx_equal(
-            ds0.joseki.column_number_density[m].m,
-            ds1.joseki.column_number_density[m].m,
-            significant=6
+            value[molecule].m_as(target[molecule].units),
+            target[molecule].m,
+            significant=6,
         )
 
-def test_select_molecules():
-    """Returns xr.Dataset."""
-    ds = make(identifier="afgl_1986-tropical", molecules=["H2O", "CO2"])
-    assert ds.joseki.molecules == ["H2O", "CO2"]
-
 def test_open_dataset(tmpdir):
     """Returns xr.Dataset."""
     ds = make(identifier="afgl_1986-tropical")
     path = tmpdir.join("test.nc")
     ds.to_netcdf(path)
     ds2 = open_dataset(path)
     assert ds2.joseki.is_valid
 
+
 def test_load_dataset(tmpdir):
     """Returns xr.Dataset."""
     ds = make(identifier="afgl_1986-tropical")
     path = tmpdir.join("test.nc")
     ds.to_netcdf(path)
     ds2 = load_dataset(path)
     assert ds2.joseki.is_valid
 
-def test_merge_1():
+
+def test_merge():
     ds1 = make(identifier="afgl_1986-tropical", molecules=["H2O", "CO2"])
     ds2 = make(identifier="afgl_1986-tropical", molecules=["O3"])
     ds = merge([ds1, ds2])
     assert ds.joseki.molecules == ["H2O", "CO2", "O3"]
 
+
 def test_identifiers():
     """Returns list of identifiers."""
     assert isinstance(identifiers(), list)
```

### Comparing `joseki-2.3.0/tests/test_main.py` & `joseki-2.4.0/tests/test_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,27 +59,14 @@
             f"--file-name={tmpdir / 'ds.nc'}",
             f"--altitudes={altitudes_path}",
         ],
     )
     assert result.exit_code == 0
 
 
-def test_main_represent_in_cells(runner: CliRunner, tmpdir: t.Any):
-    """Exits with a status code of zero with option --represent-in-cells."""
-    result = runner.invoke(
-        __main__.main,
-        [
-            "--identifier=afgl_1986-tropical",
-            f"--file-name={tmpdir / 'ds.nc'}",
-            "--represent-in-cells",
-        ],
-    )
-    assert result.exit_code == 0
-
-
 def test_main_interp_method(runner: CliRunner, tmpdir: t.Any):
     """Exits with a status code of zero with option --p-interp-method."""
     result = runner.invoke(
         __main__.main,
         [
             "--identifier=afgl_1986-tropical",
             f"--file-name={tmpdir / 'ds.nc'}",
@@ -92,12 +79,11 @@
 def test_main_conserve_column(runner: CliRunner, tmpdir: t.Any):
     """Exits with a status code of zero with option --conserve-column"""
     result = runner.invoke(
         __main__.main,
         [
             "--identifier=afgl_1986-tropical",
             f"--file-name={tmpdir / 'ds.nc'}",
-            "--represent-in-cells",
             "--conserve-column",
         ],
     )
     assert result.exit_code == 0
```

### Comparing `joseki-2.3.0/tests/test_units.py` & `joseki-2.4.0/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `joseki-2.3.0/PKG-INFO` & `joseki-2.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joseki
-Version: 2.3.0
+Version: 2.4.0
 Summary: Reference atmosphere's thermophysical profiles for radiative transfer applications in Earth's atmosphere.
 License: MIT
 Author-email: Yvan Nollet <yvan.nollet@rayference.eu>
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -35,16 +35,14 @@
 ## Features
 
 * Available profiles:
   * *AFGL Atmospheric Constituent Profiles (0-120 km)*
   * *MIPAS (2007) reference atmospheres*
   * *U.S. Standard Atmosphere, 1976*
 * Specify the altitude mesh to interpolate the atmospheric profile at.
-* Move from the nodes-representation to the cells-representation of the 
-  altitude mesh.
 * Command-line interface.
 * Python API.
 
 
 ## Requirements
 
 * Python 3.8+
@@ -62,17 +60,25 @@
 
 ```shell
 conda install -c conda-forge joseki
 ```
 
 ## Documentation
 
-Visit https://nollety.github.io/joseki/latest.
+Visit https://rayference.github.io/joseki/latest.
 
 ## Ikigai
 
 *Joseki* was born in the context of the development of the 
 [Eradiate](https://github.com/eradiate/eradiate) radiative transfer model, from
 the need to collect, document and trace, integrate and modify *popular* 
 thermophysical profiles.
 As such, its features evolve in close relationship to those of *Eradiate*.
 
+## About
+
+Joseki is written and maintained by [Yvan Nollet](https://github.com/nollety).
+
+Development is supported by [Rayference](https://www.rayference.eu).
+
+Joseki is a component of the [Eradiate radiative transfer model](https://www.eradiate.eu/site/).
+
```

