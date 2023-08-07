# Comparing `tmp/whyqd-1.0.2.tar.gz` & `tmp/whyqd-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyqd-1.0.2.tar", max compression
+gzip compressed data, was "whyqd-1.0.3.tar", max compression
```

## Comparing `whyqd-1.0.2.tar` & `whyqd-1.0.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rwxr-xr-x   0        0        0     1543 2020-02-03 11:45:00.076853 whyqd-1.0.2/LICENSE
--rwxr-xr-x   0        0        0     7853 2023-05-12 07:06:44.670906 whyqd-1.0.2/README.md
--rwxr-xr-x   0        0        0     1736 2023-07-05 16:10:15.076550 whyqd-1.0.2/pyproject.toml
--rwxr-xr-x   0        0        0    23800 2023-05-10 14:13:08.619398 whyqd-1.0.2/tests/data/2023-05-09-human-development-report-interim.PARQUET
--rwxr-xr-x   0        0        0    40526 2021-08-23 16:43:27.488340 whyqd-1.0.2/tests/data/HDR-2007-2008-Table-03.xlsx
--rwxr-xr-x   0        0        0   242453 2020-02-12 10:37:10.119769 whyqd-1.0.2/tests/data/raw_E06000044_014_0.XLSX
--rwxr-xr-x   0        0        0     1422 2023-05-10 14:13:08.621402 whyqd-1.0.2/tests/data/raw_E06000044_014_0.data
--rwxr-xr-x   0        0        0    38885 2020-02-12 10:37:08.070860 whyqd-1.0.2/tests/data/raw_E06000044_014_1.XLSX
--rwxr-xr-x   0        0        0   306675 2020-02-12 10:37:12.460459 whyqd-1.0.2/tests/data/raw_E06000044_014_2.XLSX
--rwxr-xr-x   0        0        0   330970 2023-05-10 14:13:08.625396 whyqd-1.0.2/tests/data/raw_duplicated_E06000044_014.xlsx
--rwxr-xr-x   0        0        0   508171 2023-05-10 14:13:08.631399 whyqd-1.0.2/tests/data/raw_multi_E06000044_014.xlsx
--rwxr-xr-x   0        0        0   246405 2023-02-14 09:10:52.024386 whyqd-1.0.2/tests/data/restructured_test_data.xlsx
--rwxr-xr-x   0        0        0     4229 2023-05-10 14:13:08.631399 whyqd-1.0.2/tests/data/test_crosswalk.crosswalk
--rwxr-xr-x   0        0        0     1435 2023-05-19 09:38:36.782172 whyqd-1.0.2/tests/data/test_cthulu_destination.schema
--rwxr-xr-x   0        0        0     3144 2023-05-19 09:38:38.269033 whyqd-1.0.2/tests/data/test_cthulu_interim.data
--rwxr-xr-x   0        0        0     3022 2023-05-19 09:38:39.967455 whyqd-1.0.2/tests/data/test_cthulu_interim.schema
--rwxr-xr-x   0        0        0     2538 2023-05-19 09:38:41.929747 whyqd-1.0.2/tests/data/test_cthulu_source.data
--rwxr-xr-x   0        0        0     2606 2023-05-19 09:38:44.186689 whyqd-1.0.2/tests/data/test_cthulu_source.schema
--rwxr-xr-x   0        0        0   582612 2023-05-10 14:13:08.640397 whyqd-1.0.2/tests/data/test_data.csv
--rwxr-xr-x   0        0        0     1159 2023-05-10 14:13:08.641397 whyqd-1.0.2/tests/data/test_derived_schema.schema
--rwxr-xr-x   0        0        0     2529 2023-05-10 14:13:08.642398 whyqd-1.0.2/tests/data/test_portsmouth_destination.schema
--rwxr-xr-x   0        0        0     1234 2023-05-10 14:13:08.643397 whyqd-1.0.2/tests/data/test_portsmouth_source.data
--rwxr-xr-x   0        0        0     1978 2023-05-10 14:13:08.643397 whyqd-1.0.2/tests/data/test_portsmouth_source.schema
--rwxr-xr-x   0        0        0     1943 2021-08-23 16:43:27.501347 whyqd-1.0.2/tests/data/test_schema.json
--rwxr-xr-x   0        0        0     2529 2023-05-10 14:13:08.644397 whyqd-1.0.2/tests/data/test_schema.schema
--rwxr-xr-x   0        0        0     1986 2023-05-10 14:13:08.645397 whyqd-1.0.2/tests/data/test_source_schema.schema
--rwxr-xr-x   0        0        0     1728 2021-08-23 16:43:27.501347 whyqd-1.0.2/tests/data/urban_population.json
--rwxr-xr-x   0        0        0   505134 2023-02-14 09:10:52.029354 whyqd-1.0.2/tests/data/working_test_data.xlsx
--rwxr-xr-x   0        0        0   153076 2020-05-03 21:13:05.504203 whyqd-1.0.2/tests/data/working_test_world_bank_data.xlsx
--rwxr-xr-x   0        0        0      165 2023-06-06 14:19:33.611783 whyqd-1.0.2/tests/data/~$HDR-2007-2008-Table-03.xlsx
--rwxr-xr-x   0        0        0        5 2023-07-05 16:07:13.556261 whyqd-1.0.2/whyqd/VERSION
--rwxr-xr-x   0        0        0      315 2023-05-10 14:13:08.655398 whyqd-1.0.2/whyqd/__init__.py
--rwxr-xr-x   0        0        0      214 2021-08-23 16:43:27.509335 whyqd-1.0.2/whyqd/__main__.py
--rwxr-xr-x   0        0        0        0 2023-02-14 09:10:52.048356 whyqd-1.0.2/whyqd/config/__init__.py
--rwxr-xr-x   0        0        0     2607 2023-05-10 14:13:08.656397 whyqd-1.0.2/whyqd/config/ray_init.py
--rwxr-xr-x   0        0        0      520 2023-05-10 14:13:08.657397 whyqd-1.0.2/whyqd/config/settings.py
--rwxr-xr-x   0        0        0      172 2023-05-10 14:13:08.657397 whyqd-1.0.2/whyqd/core/__init__.py
--rwxr-xr-x   0        0        0     8358 2023-05-10 14:13:08.658398 whyqd-1.0.2/whyqd/core/base.py
--rwxr-xr-x   0        0        0     6068 2023-05-12 06:36:03.714646 whyqd-1.0.2/whyqd/core/crosswalk.py
--rwxr-xr-x   0        0        0    10547 2023-05-12 06:36:33.964292 whyqd-1.0.2/whyqd/core/datasource.py
--rwxr-xr-x   0        0        0     3862 2023-05-12 06:37:05.626333 whyqd-1.0.2/whyqd/core/schema.py
--rwxr-xr-x   0        0        0    11580 2023-05-11 08:09:37.227431 whyqd-1.0.2/whyqd/core/transform.py
--rwxr-xr-x   0        0        0        0 2023-05-10 14:13:08.662396 whyqd-1.0.2/whyqd/crosswalk/__init__.py
--rwxr-xr-x   0        0        0     1537 2023-05-10 14:13:08.662396 whyqd-1.0.2/whyqd/crosswalk/actions/__init__.py
--rwxr-xr-x   0        0        0     2934 2023-05-10 14:13:08.663396 whyqd-1.0.2/whyqd/crosswalk/actions/calculate.py
--rwxr-xr-x   0        0        0     1507 2023-05-10 14:13:08.664396 whyqd-1.0.2/whyqd/crosswalk/actions/categorise.py
--rwxr-xr-x   0        0        0     1090 2023-05-10 14:13:08.664396 whyqd-1.0.2/whyqd/crosswalk/actions/deblank.py
--rwxr-xr-x   0        0        0      975 2023-05-10 14:13:08.665396 whyqd-1.0.2/whyqd/crosswalk/actions/dedupe.py
--rwxr-xr-x   0        0        0     1249 2023-05-10 14:13:08.665396 whyqd-1.0.2/whyqd/crosswalk/actions/delete_rows.py
--rwxr-xr-x   0        0        0     1538 2023-05-10 14:13:08.666397 whyqd-1.0.2/whyqd/crosswalk/actions/new.py
--rwxr-xr-x   0        0        0     4021 2023-05-10 14:13:08.667401 whyqd-1.0.2/whyqd/crosswalk/actions/pivot_categories.py
--rwxr-xr-x   0        0        0     1893 2023-05-10 14:13:08.667401 whyqd-1.0.2/whyqd/crosswalk/actions/pivot_longer.py
--rwxr-xr-x   0        0        0     1535 2023-05-10 14:13:08.668401 whyqd-1.0.2/whyqd/crosswalk/actions/rename.py
--rwxr-xr-x   0        0        0     2200 2023-05-10 14:13:08.669397 whyqd-1.0.2/whyqd/crosswalk/actions/select.py
--rwxr-xr-x   0        0        0     3832 2023-05-10 14:13:08.669397 whyqd-1.0.2/whyqd/crosswalk/actions/select_newest.py
--rwxr-xr-x   0        0        0     3826 2023-05-10 14:13:08.670396 whyqd-1.0.2/whyqd/crosswalk/actions/select_oldest.py
--rwxr-xr-x   0        0        0     3418 2023-05-10 14:13:08.671399 whyqd-1.0.2/whyqd/crosswalk/actions/separate.py
--rwxr-xr-x   0        0        0     2105 2023-05-10 14:13:08.672397 whyqd-1.0.2/whyqd/crosswalk/actions/unite.py
--rwxr-xr-x   0        0        0      131 2023-05-10 14:13:08.673398 whyqd-1.0.2/whyqd/crosswalk/base/__init__.py
--rwxr-xr-x   0        0        0     6247 2023-05-10 14:13:08.674398 whyqd-1.0.2/whyqd/crosswalk/base/action_base.py
--rwxr-xr-x   0        0        0     8242 2023-05-10 14:13:08.675397 whyqd-1.0.2/whyqd/crosswalk/base/category_base.py
--rwxr-xr-x   0        0        0     3940 2023-05-10 14:13:08.675397 whyqd-1.0.2/whyqd/crosswalk/base/morph_base.py
--rwxr-xr-x   0        0        0      258 2023-05-10 14:13:08.676397 whyqd-1.0.2/whyqd/crud/__init__.py
--rwxr-xr-x   0        0        0    12381 2023-05-12 06:38:16.658348 whyqd-1.0.2/whyqd/crud/action.py
--rwxr-xr-x   0        0        0     4873 2023-05-10 14:13:08.677395 whyqd-1.0.2/whyqd/crud/base.py
--rwxr-xr-x   0        0        0     7873 2023-05-12 06:38:36.849050 whyqd-1.0.2/whyqd/crud/field.py
--rwxr-xr-x   0        0        0       88 2023-05-10 14:13:08.679396 whyqd-1.0.2/whyqd/dtypes/__init__.py
--rwxr-xr-x   0        0        0     1928 2023-05-10 14:13:08.679396 whyqd-1.0.2/whyqd/dtypes/field.py
--rwxr-xr-x   0        0        0      900 2023-05-10 14:13:08.680396 whyqd-1.0.2/whyqd/dtypes/mime.py
--rwxr-xr-x   0        0        0     1294 2023-05-10 14:13:08.680396 whyqd-1.0.2/whyqd/dtypes/status.py
--rwxr-xr-x   0        0        0      617 2023-05-10 14:13:08.681397 whyqd-1.0.2/whyqd/models/__init__.py
--rwxr-xr-x   0        0        0     1077 2023-05-10 14:13:08.681397 whyqd-1.0.2/whyqd/models/action_category.py
--rwxr-xr-x   0        0        0     1086 2023-05-10 14:13:08.682397 whyqd-1.0.2/whyqd/models/action_morph.py
--rwxr-xr-x   0        0        0     1665 2023-05-10 14:13:08.682397 whyqd-1.0.2/whyqd/models/action_schema.py
--rwxr-xr-x   0        0        0      530 2023-05-10 14:13:08.683396 whyqd-1.0.2/whyqd/models/actionscript.py
--rwxr-xr-x   0        0        0      584 2023-05-10 14:13:08.683396 whyqd-1.0.2/whyqd/models/category.py
--rwxr-xr-x   0        0        0     2569 2023-05-10 14:13:08.684399 whyqd-1.0.2/whyqd/models/citation.py
--rwxr-xr-x   0        0        0     1366 2023-05-10 14:13:08.684399 whyqd-1.0.2/whyqd/models/column.py
--rwxr-xr-x   0        0        0     2162 2023-05-10 14:13:08.685395 whyqd-1.0.2/whyqd/models/constraints.py
--rwxr-xr-x   0        0        0     1977 2023-05-10 14:13:08.685395 whyqd-1.0.2/whyqd/models/crosswalk.py
--rwxr-xr-x   0        0        0     4358 2023-05-10 14:13:08.686398 whyqd-1.0.2/whyqd/models/datasource.py
--rwxr-xr-x   0        0        0     1367 2023-05-10 14:13:08.687398 whyqd-1.0.2/whyqd/models/fields.py
--rwxr-xr-x   0        0        0      608 2023-05-10 14:13:08.688398 whyqd-1.0.2/whyqd/models/modifier.py
--rwxr-xr-x   0        0        0     2650 2023-05-10 14:13:08.688398 whyqd-1.0.2/whyqd/models/schema.py
--rwxr-xr-x   0        0        0     2046 2023-05-10 14:13:08.690396 whyqd-1.0.2/whyqd/models/transform.py
--rwxr-xr-x   0        0        0      527 2023-05-10 14:13:08.690396 whyqd-1.0.2/whyqd/models/version.py
--rwxr-xr-x   0        0        0      210 2023-05-10 14:13:08.691396 whyqd-1.0.2/whyqd/parsers/__init__.py
--rwxr-xr-x   0        0        0    14750 2023-05-10 14:13:08.692394 whyqd-1.0.2/whyqd/parsers/action.py
--rwxr-xr-x   0        0        0    10614 2023-05-10 14:13:08.692394 whyqd-1.0.2/whyqd/parsers/category.py
--rwxr-xr-x   0        0        0     9550 2023-06-06 14:17:55.467244 whyqd-1.0.2/whyqd/parsers/core.py
--rwxr-xr-x   0        0        0    31304 2023-06-06 14:29:01.427298 whyqd-1.0.2/whyqd/parsers/datasource.py
--rwxr-xr-x   0        0        0     9021 2023-05-10 14:13:08.694397 whyqd-1.0.2/whyqd/parsers/morph.py
--rwxr-xr-x   0        0        0     6789 2023-05-10 14:13:08.695395 whyqd-1.0.2/whyqd/parsers/script.py
--rw-r--r--   0        0        0     9028 1970-01-01 00:00:00.000000 whyqd-1.0.2/setup.py
--rw-r--r--   0        0        0     9331 1970-01-01 00:00:00.000000 whyqd-1.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1543 2020-02-03 11:45:00.076853 whyqd-1.0.3/LICENSE
+-rwxr-xr-x   0        0        0     7853 2023-05-13 19:34:07.560475 whyqd-1.0.3/README.md
+-rwxr-xr-x   0        0        0     1736 2023-08-07 14:16:58.903347 whyqd-1.0.3/pyproject.toml
+-rwxr-xr-x   0        0        0    23800 2023-05-10 19:39:38.964982 whyqd-1.0.3/tests/data/2023-05-09-human-development-report-interim.PARQUET
+-rwxr-xr-x   0        0        0    40526 2021-08-23 16:43:27.488340 whyqd-1.0.3/tests/data/HDR-2007-2008-Table-03.xlsx
+-rwxr-xr-x   0        0        0   242453 2020-02-12 10:37:10.119769 whyqd-1.0.3/tests/data/raw_E06000044_014_0.XLSX
+-rwxr-xr-x   0        0        0     1422 2023-05-10 19:39:38.966995 whyqd-1.0.3/tests/data/raw_E06000044_014_0.data
+-rwxr-xr-x   0        0        0    38885 2020-02-12 10:37:08.070860 whyqd-1.0.3/tests/data/raw_E06000044_014_1.XLSX
+-rwxr-xr-x   0        0        0   306675 2020-02-12 10:37:12.460459 whyqd-1.0.3/tests/data/raw_E06000044_014_2.XLSX
+-rwxr-xr-x   0        0        0   330970 2023-05-10 19:39:38.972980 whyqd-1.0.3/tests/data/raw_duplicated_E06000044_014.xlsx
+-rwxr-xr-x   0        0        0   508171 2023-05-10 19:39:38.981997 whyqd-1.0.3/tests/data/raw_multi_E06000044_014.xlsx
+-rwxr-xr-x   0        0        0   246405 2023-05-10 19:39:39.004113 whyqd-1.0.3/tests/data/restructured_test_data.xlsx
+-rwxr-xr-x   0        0        0     4229 2023-05-10 19:39:39.005119 whyqd-1.0.3/tests/data/test_crosswalk.crosswalk
+-rwxr-xr-x   0        0        0     1435 2023-05-10 19:39:39.006118 whyqd-1.0.3/tests/data/test_cthulu_destination.schema
+-rwxr-xr-x   0        0        0     3144 2023-05-10 19:39:39.007117 whyqd-1.0.3/tests/data/test_cthulu_interim.data
+-rwxr-xr-x   0        0        0     3022 2023-05-10 19:39:39.008118 whyqd-1.0.3/tests/data/test_cthulu_interim.schema
+-rwxr-xr-x   0        0        0     2538 2023-05-10 19:39:39.009117 whyqd-1.0.3/tests/data/test_cthulu_source.data
+-rwxr-xr-x   0        0        0     2606 2023-05-10 19:39:39.010117 whyqd-1.0.3/tests/data/test_cthulu_source.schema
+-rwxr-xr-x   0        0        0   582612 2023-05-10 19:39:39.019118 whyqd-1.0.3/tests/data/test_data.csv
+-rwxr-xr-x   0        0        0     1159 2023-05-10 19:39:39.020119 whyqd-1.0.3/tests/data/test_derived_schema.schema
+-rwxr-xr-x   0        0        0     2529 2023-05-10 19:39:39.021120 whyqd-1.0.3/tests/data/test_portsmouth_destination.schema
+-rwxr-xr-x   0        0        0     1234 2023-05-10 19:39:39.022124 whyqd-1.0.3/tests/data/test_portsmouth_source.data
+-rwxr-xr-x   0        0        0     1978 2023-05-10 19:39:39.023120 whyqd-1.0.3/tests/data/test_portsmouth_source.schema
+-rwxr-xr-x   0        0        0     1943 2021-08-23 16:43:27.501347 whyqd-1.0.3/tests/data/test_schema.json
+-rwxr-xr-x   0        0        0     2529 2023-05-10 19:39:39.025119 whyqd-1.0.3/tests/data/test_schema.schema
+-rwxr-xr-x   0        0        0     1986 2023-05-10 19:39:39.026125 whyqd-1.0.3/tests/data/test_source_schema.schema
+-rwxr-xr-x   0        0        0     1728 2021-08-23 16:43:27.501347 whyqd-1.0.3/tests/data/urban_population.json
+-rwxr-xr-x   0        0        0   505134 2023-05-10 19:39:39.053123 whyqd-1.0.3/tests/data/working_test_data.xlsx
+-rwxr-xr-x   0        0        0   153076 2020-05-03 21:13:05.504203 whyqd-1.0.3/tests/data/working_test_world_bank_data.xlsx
+-rwxr-xr-x   0        0        0      165 2023-05-10 19:39:39.054119 whyqd-1.0.3/tests/data/~$HDR-2007-2008-Table-03.xlsx
+-rwxr-xr-x   0        0        0        5 2023-08-07 14:16:58.909740 whyqd-1.0.3/whyqd/VERSION
+-rwxr-xr-x   0        0        0      315 2023-05-10 19:39:39.071114 whyqd-1.0.3/whyqd/__init__.py
+-rwxr-xr-x   0        0        0      214 2021-08-23 16:43:27.509335 whyqd-1.0.3/whyqd/__main__.py
+-rwxr-xr-x   0        0        0        0 2023-05-10 19:39:39.072114 whyqd-1.0.3/whyqd/config/__init__.py
+-rwxr-xr-x   0        0        0     2607 2023-05-10 19:39:39.073115 whyqd-1.0.3/whyqd/config/ray_init.py
+-rwxr-xr-x   0        0        0      520 2023-05-10 19:39:39.074121 whyqd-1.0.3/whyqd/config/settings.py
+-rwxr-xr-x   0        0        0      172 2023-05-10 19:39:39.075121 whyqd-1.0.3/whyqd/core/__init__.py
+-rwxr-xr-x   0        0        0     8358 2023-05-10 19:39:39.076119 whyqd-1.0.3/whyqd/core/base.py
+-rwxr-xr-x   0        0        0     6068 2023-05-13 19:34:07.740588 whyqd-1.0.3/whyqd/core/crosswalk.py
+-rwxr-xr-x   0        0        0    10547 2023-05-13 19:34:07.747587 whyqd-1.0.3/whyqd/core/datasource.py
+-rwxr-xr-x   0        0        0     3862 2023-05-13 19:34:07.756364 whyqd-1.0.3/whyqd/core/schema.py
+-rwxr-xr-x   0        0        0    11580 2023-05-13 19:34:07.763419 whyqd-1.0.3/whyqd/core/transform.py
+-rwxr-xr-x   0        0        0        0 2023-05-10 19:39:39.083136 whyqd-1.0.3/whyqd/crosswalk/__init__.py
+-rwxr-xr-x   0        0        0     1537 2023-05-10 19:39:39.085133 whyqd-1.0.3/whyqd/crosswalk/actions/__init__.py
+-rwxr-xr-x   0        0        0     2934 2023-05-10 19:39:39.086135 whyqd-1.0.3/whyqd/crosswalk/actions/calculate.py
+-rwxr-xr-x   0        0        0     1507 2023-05-10 19:39:39.087131 whyqd-1.0.3/whyqd/crosswalk/actions/categorise.py
+-rwxr-xr-x   0        0        0     1090 2023-05-10 19:39:39.088132 whyqd-1.0.3/whyqd/crosswalk/actions/deblank.py
+-rwxr-xr-x   0        0        0      975 2023-05-10 19:39:39.089133 whyqd-1.0.3/whyqd/crosswalk/actions/dedupe.py
+-rwxr-xr-x   0        0        0     1249 2023-05-10 19:39:39.090134 whyqd-1.0.3/whyqd/crosswalk/actions/delete_rows.py
+-rwxr-xr-x   0        0        0     1538 2023-05-10 19:39:39.091134 whyqd-1.0.3/whyqd/crosswalk/actions/new.py
+-rwxr-xr-x   0        0        0     4021 2023-05-10 19:39:39.092133 whyqd-1.0.3/whyqd/crosswalk/actions/pivot_categories.py
+-rwxr-xr-x   0        0        0     1893 2023-05-10 19:39:39.092647 whyqd-1.0.3/whyqd/crosswalk/actions/pivot_longer.py
+-rwxr-xr-x   0        0        0     1535 2023-05-10 19:39:39.093662 whyqd-1.0.3/whyqd/crosswalk/actions/rename.py
+-rwxr-xr-x   0        0        0     2200 2023-05-10 19:39:39.094664 whyqd-1.0.3/whyqd/crosswalk/actions/select.py
+-rwxr-xr-x   0        0        0     3832 2023-05-10 19:39:39.096673 whyqd-1.0.3/whyqd/crosswalk/actions/select_newest.py
+-rwxr-xr-x   0        0        0     3826 2023-05-10 19:39:39.097667 whyqd-1.0.3/whyqd/crosswalk/actions/select_oldest.py
+-rwxr-xr-x   0        0        0     3418 2023-05-10 19:39:39.098663 whyqd-1.0.3/whyqd/crosswalk/actions/separate.py
+-rwxr-xr-x   0        0        0     2105 2023-05-10 19:39:39.100671 whyqd-1.0.3/whyqd/crosswalk/actions/unite.py
+-rwxr-xr-x   0        0        0      131 2023-05-10 19:39:39.101665 whyqd-1.0.3/whyqd/crosswalk/base/__init__.py
+-rwxr-xr-x   0        0        0     6247 2023-05-10 19:39:39.103672 whyqd-1.0.3/whyqd/crosswalk/base/action_base.py
+-rwxr-xr-x   0        0        0     8242 2023-05-10 19:39:39.104663 whyqd-1.0.3/whyqd/crosswalk/base/category_base.py
+-rwxr-xr-x   0        0        0     3940 2023-05-10 19:39:39.106661 whyqd-1.0.3/whyqd/crosswalk/base/morph_base.py
+-rwxr-xr-x   0        0        0      258 2023-05-10 19:39:39.107673 whyqd-1.0.3/whyqd/crud/__init__.py
+-rwxr-xr-x   0        0        0    12381 2023-05-13 19:34:07.771430 whyqd-1.0.3/whyqd/crud/action.py
+-rwxr-xr-x   0        0        0     4873 2023-05-10 19:39:39.110671 whyqd-1.0.3/whyqd/crud/base.py
+-rwxr-xr-x   0        0        0     7873 2023-05-13 19:34:07.778427 whyqd-1.0.3/whyqd/crud/field.py
+-rwxr-xr-x   0        0        0       88 2023-05-10 19:39:39.114666 whyqd-1.0.3/whyqd/dtypes/__init__.py
+-rwxr-xr-x   0        0        0     1928 2023-05-10 19:39:39.115666 whyqd-1.0.3/whyqd/dtypes/field.py
+-rwxr-xr-x   0        0        0      900 2023-05-10 19:39:39.117666 whyqd-1.0.3/whyqd/dtypes/mime.py
+-rwxr-xr-x   0        0        0     1294 2023-05-10 19:39:39.118665 whyqd-1.0.3/whyqd/dtypes/status.py
+-rwxr-xr-x   0        0        0      617 2023-05-10 19:39:39.120672 whyqd-1.0.3/whyqd/models/__init__.py
+-rwxr-xr-x   0        0        0     1077 2023-05-10 19:39:39.121673 whyqd-1.0.3/whyqd/models/action_category.py
+-rwxr-xr-x   0        0        0     1086 2023-05-10 19:39:39.122672 whyqd-1.0.3/whyqd/models/action_morph.py
+-rwxr-xr-x   0        0        0     1665 2023-05-10 19:39:39.123666 whyqd-1.0.3/whyqd/models/action_schema.py
+-rwxr-xr-x   0        0        0      530 2023-05-10 19:39:39.124666 whyqd-1.0.3/whyqd/models/actionscript.py
+-rwxr-xr-x   0        0        0      584 2023-05-10 19:39:39.125682 whyqd-1.0.3/whyqd/models/category.py
+-rwxr-xr-x   0        0        0     2569 2023-05-10 19:39:39.126666 whyqd-1.0.3/whyqd/models/citation.py
+-rwxr-xr-x   0        0        0     1366 2023-05-10 19:39:39.127665 whyqd-1.0.3/whyqd/models/column.py
+-rwxr-xr-x   0        0        0     2162 2023-05-10 19:39:39.129665 whyqd-1.0.3/whyqd/models/constraints.py
+-rwxr-xr-x   0        0        0     1977 2023-05-10 19:39:39.130663 whyqd-1.0.3/whyqd/models/crosswalk.py
+-rwxr-xr-x   0        0        0     4358 2023-05-10 19:39:39.132667 whyqd-1.0.3/whyqd/models/datasource.py
+-rwxr-xr-x   0        0        0     1367 2023-05-10 19:39:39.133666 whyqd-1.0.3/whyqd/models/fields.py
+-rwxr-xr-x   0        0        0      608 2023-05-10 19:39:39.134662 whyqd-1.0.3/whyqd/models/modifier.py
+-rwxr-xr-x   0        0        0     2650 2023-05-10 19:39:39.135665 whyqd-1.0.3/whyqd/models/schema.py
+-rwxr-xr-x   0        0        0     2046 2023-05-10 19:39:39.137665 whyqd-1.0.3/whyqd/models/transform.py
+-rwxr-xr-x   0        0        0      527 2023-05-10 19:39:39.138661 whyqd-1.0.3/whyqd/models/version.py
+-rwxr-xr-x   0        0        0      210 2023-05-10 19:39:39.140663 whyqd-1.0.3/whyqd/parsers/__init__.py
+-rwxr-xr-x   0        0        0    14750 2023-05-10 19:39:39.141664 whyqd-1.0.3/whyqd/parsers/action.py
+-rwxr-xr-x   0        0        0    10921 2023-08-07 14:16:58.917604 whyqd-1.0.3/whyqd/parsers/category.py
+-rwxr-xr-x   0        0        0     9550 2023-07-15 10:41:40.381613 whyqd-1.0.3/whyqd/parsers/core.py
+-rwxr-xr-x   0        0        0    31304 2023-07-15 10:41:40.389611 whyqd-1.0.3/whyqd/parsers/datasource.py
+-rwxr-xr-x   0        0        0     9021 2023-05-10 19:39:39.146673 whyqd-1.0.3/whyqd/parsers/morph.py
+-rwxr-xr-x   0        0        0     6789 2023-05-10 19:39:39.148672 whyqd-1.0.3/whyqd/parsers/script.py
+-rw-r--r--   0        0        0     9028 1970-01-01 00:00:00.000000 whyqd-1.0.3/setup.py
+-rw-r--r--   0        0        0     9331 1970-01-01 00:00:00.000000 whyqd-1.0.3/PKG-INFO
```

### Comparing `whyqd-1.0.2/LICENSE` & `whyqd-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/README.md` & `whyqd-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/pyproject.toml` & `whyqd-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whyqd"
-version = "1.0.2"
+version = "1.0.3"
 description = "data wrangling simplicity, complete audit transparency, and at speed"
 authors = ["Gavin Chait <gchait@whythawk.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://whyqd.com"
 repository = "https://github.com/whythawk/whyqd/"
 documentation = "https://whyqd.readthedocs.io/"
```

### Comparing `whyqd-1.0.2/tests/data/2023-05-09-human-development-report-interim.PARQUET` & `whyqd-1.0.3/tests/data/2023-05-09-human-development-report-interim.PARQUET`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/HDR-2007-2008-Table-03.xlsx` & `whyqd-1.0.3/tests/data/HDR-2007-2008-Table-03.xlsx`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/raw_E06000044_014_0.XLSX` & `whyqd-1.0.3/tests/data/raw_E06000044_014_0.XLSX`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/raw_E06000044_014_0.data` & `whyqd-1.0.3/tests/data/raw_E06000044_014_0.data`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/raw_E06000044_014_1.XLSX` & `whyqd-1.0.3/tests/data/raw_E06000044_014_1.XLSX`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/raw_E06000044_014_2.XLSX` & `whyqd-1.0.3/tests/data/raw_E06000044_014_2.XLSX`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/raw_duplicated_E06000044_014.xlsx` & `whyqd-1.0.3/tests/data/raw_duplicated_E06000044_014.xlsx`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/raw_multi_E06000044_014.xlsx` & `whyqd-1.0.3/tests/data/raw_multi_E06000044_014.xlsx`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/restructured_test_data.xlsx` & `whyqd-1.0.3/tests/data/restructured_test_data.xlsx`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/test_crosswalk.crosswalk` & `whyqd-1.0.3/tests/data/test_crosswalk.crosswalk`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/test_cthulu_destination.schema` & `whyqd-1.0.3/tests/data/test_cthulu_destination.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/test_cthulu_interim.data` & `whyqd-1.0.3/tests/data/test_cthulu_interim.data`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/test_cthulu_interim.schema` & `whyqd-1.0.3/tests/data/test_cthulu_interim.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/test_cthulu_source.data` & `whyqd-1.0.3/tests/data/test_cthulu_source.data`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/test_cthulu_source.schema` & `whyqd-1.0.3/tests/data/test_cthulu_source.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/test_data.csv` & `whyqd-1.0.3/tests/data/test_data.csv`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/test_derived_schema.schema` & `whyqd-1.0.3/tests/data/test_derived_schema.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/test_portsmouth_destination.schema` & `whyqd-1.0.3/tests/data/test_portsmouth_destination.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/test_portsmouth_source.data` & `whyqd-1.0.3/tests/data/test_portsmouth_source.data`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/test_portsmouth_source.schema` & `whyqd-1.0.3/tests/data/test_portsmouth_source.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/test_schema.json` & `whyqd-1.0.3/tests/data/test_schema.json`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/test_schema.schema` & `whyqd-1.0.3/tests/data/test_schema.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/test_source_schema.schema` & `whyqd-1.0.3/tests/data/test_source_schema.schema`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/urban_population.json` & `whyqd-1.0.3/tests/data/urban_population.json`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/working_test_data.xlsx` & `whyqd-1.0.3/tests/data/working_test_data.xlsx`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/tests/data/working_test_world_bank_data.xlsx` & `whyqd-1.0.3/tests/data/working_test_world_bank_data.xlsx`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/config/ray_init.py` & `whyqd-1.0.3/whyqd/config/ray_init.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/config/settings.py` & `whyqd-1.0.3/whyqd/config/settings.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/core/base.py` & `whyqd-1.0.3/whyqd/core/base.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/core/crosswalk.py` & `whyqd-1.0.3/whyqd/core/crosswalk.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/core/datasource.py` & `whyqd-1.0.3/whyqd/core/datasource.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/core/schema.py` & `whyqd-1.0.3/whyqd/core/schema.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/core/transform.py` & `whyqd-1.0.3/whyqd/core/transform.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/__init__.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/calculate.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/calculate.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/categorise.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/categorise.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/deblank.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/deblank.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/dedupe.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/dedupe.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/delete_rows.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/delete_rows.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/new.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/new.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/pivot_categories.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/pivot_categories.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/pivot_longer.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/pivot_longer.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/rename.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/rename.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/select.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/select.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/select_newest.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/select_newest.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/select_oldest.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/select_oldest.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/separate.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/separate.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/actions/unite.py` & `whyqd-1.0.3/whyqd/crosswalk/actions/unite.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/base/action_base.py` & `whyqd-1.0.3/whyqd/crosswalk/base/action_base.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/base/category_base.py` & `whyqd-1.0.3/whyqd/crosswalk/base/category_base.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crosswalk/base/morph_base.py` & `whyqd-1.0.3/whyqd/crosswalk/base/morph_base.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crud/action.py` & `whyqd-1.0.3/whyqd/crud/action.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crud/base.py` & `whyqd-1.0.3/whyqd/crud/base.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/crud/field.py` & `whyqd-1.0.3/whyqd/crud/field.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/dtypes/field.py` & `whyqd-1.0.3/whyqd/dtypes/field.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/dtypes/mime.py` & `whyqd-1.0.3/whyqd/dtypes/mime.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/dtypes/status.py` & `whyqd-1.0.3/whyqd/dtypes/status.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/__init__.py` & `whyqd-1.0.3/whyqd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/action_category.py` & `whyqd-1.0.3/whyqd/models/action_category.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/action_morph.py` & `whyqd-1.0.3/whyqd/models/action_morph.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/action_schema.py` & `whyqd-1.0.3/whyqd/models/action_schema.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/actionscript.py` & `whyqd-1.0.3/whyqd/models/actionscript.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/category.py` & `whyqd-1.0.3/whyqd/models/category.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/citation.py` & `whyqd-1.0.3/whyqd/models/citation.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/column.py` & `whyqd-1.0.3/whyqd/models/column.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/constraints.py` & `whyqd-1.0.3/whyqd/models/constraints.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/crosswalk.py` & `whyqd-1.0.3/whyqd/models/crosswalk.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/datasource.py` & `whyqd-1.0.3/whyqd/models/datasource.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/fields.py` & `whyqd-1.0.3/whyqd/models/fields.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/modifier.py` & `whyqd-1.0.3/whyqd/models/modifier.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/schema.py` & `whyqd-1.0.3/whyqd/models/schema.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/transform.py` & `whyqd-1.0.3/whyqd/models/transform.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/models/version.py` & `whyqd-1.0.3/whyqd/models/version.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/parsers/action.py` & `whyqd-1.0.3/whyqd/parsers/action.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/parsers/category.py` & `whyqd-1.0.3/whyqd/parsers/category.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,18 @@
                 assigned = parsed["source_category"]
         # Get destination column and assigned category term
         destination = self.parser.get_literal(text=parsed["destination"])
         destination = self.schema_destination.fields.get(name=destination)
         if parsed.get("category"):
             category = self.parser.get_literal(text=parsed["category"])
             category = self.schema_destination.fields.get_category(name=destination.uuid.hex, category=category)
+            # Disambiguation step ... source and destination can have identical category names
+            if not category:
+              category = self.parser.get_literal(text=parsed["category"])
+              category = self.schema_source.fields.get_category(name=source.uuid.hex, category=category)
         if not destination and category:
             raise ValueError(
                 f"Destination field and category are not valid for this category action script ({parsed['destination']}, {parsed['category']})."
             )
         # Return validated terms
         return {
             "action": action,
```

### Comparing `whyqd-1.0.2/whyqd/parsers/core.py` & `whyqd-1.0.3/whyqd/parsers/core.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/parsers/datasource.py` & `whyqd-1.0.3/whyqd/parsers/datasource.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/parsers/morph.py` & `whyqd-1.0.3/whyqd/parsers/morph.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/whyqd/parsers/script.py` & `whyqd-1.0.3/whyqd/parsers/script.py`

 * *Files identical despite different names*

### Comparing `whyqd-1.0.2/setup.py` & `whyqd-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'ray>=2.2.0,<3.0.0',
  'setuptools>=67.7.2',
  'tabulate>=0.8.9,<0.9.0',
  'xlrd>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'whyqd',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': 'data wrangling simplicity, complete audit transparency, and at speed',
     'long_description': '# whyqd: simplicity, transparency, speed\n\n[![Documentation Status](https://readthedocs.org/projects/whyqd/badge/?version=latest)](docs/en/latest/?badge=latest)\n[![Build Status](https://travis-ci.com/whythawk/whyqd.svg?branch=master)](https://travis-ci.com/whythawk/whyqd.svg?branch=master)\n[![DOI](https://zenodo.org/badge/239159569.svg)](https://zenodo.org/badge/latestdoi/239159569)\n\n## What is it?\n\n> More research, less wrangling\n\n[**whyqd**](https://whyqd.com) (/wɪkɪd/) is a curatorial toolkit intended to produce well-structured and predictable \ndata for research analysis.\n\nIt provides an intuitive method for creating schema-to-schema crosswalks for restructuring messy data to conform to a \nstandardised metadata schema. It supports rapid and continuous transformation of messy data using a simple series of \nsteps. Once complete, you can import wrangled data into more complex analytical or database systems.\n\n**whyqd** plays well with your existing Python-based data-analytical tools. It uses [Ray](https://www.ray.io/) and \n[Modin](https://modin.readthedocs.io/) as a drop-in replacement for [Pandas](https://pandas.pydata.org/) to support \nprocessing of large datasets, and [Pydantic](https://pydantic-docs.helpmanual.io/) for data models. \n\nEach definition is saved as [JSON Schema-compliant](https://json-schema.org/) file. This permits others to read and \nscrutinise your approach, validate your methodology, or even use your crosswalks to import and transform data in \nproduction.\n\nOnce complete, a transform file can be shared, along with your input data, and anyone can import and validate your \ncrosswalk to verify that your output data is the product of these inputs.\n\n## Why use it?\n\n**whyqd** allows you to get to work without requiring you to achieve buy-in from anyone or change your existing code.\n\nIf you don\'t want to spend days or weeks slogging through data when all you want to do is test whether your source \ndata are even useful. If you already have a workflow and established software which includes Python and pandas, and \ndon\'t want to change your code every time your source data changes.\n\nIf you want to go from a [Cthulhu dataset](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial3) like this:\n\n![UNDP Human Development Index 2007-2008: a beautiful example of messy data.](docs/images/undp-hdi-2007-8.jpg)\n*UNDP Human Development Index 2007-2008: a beautiful example of messy data.*\n\nTo this:\n\n|    | country_name           | indicator_name   | reference   |   year |   values |\n|:---|:-----------------------|:-----------------|:------------|:-------|:---------|\n|  0 | Hong Kong, China (SAR) | HDI rank         | e           |   2008 |       21 |\n|  1 | Singapore              | HDI rank         | nan         |   2008 |       25 |\n|  2 | Korea (Republic of)    | HDI rank         | nan         |   2008 |       26 |\n|  3 | Cyprus                 | HDI rank         | nan         |   2008 |       28 |\n|  4 | Brunei Darussalam      | HDI rank         | nan         |   2008 |       30 |\n|  5 | Barbados               | HDI rank         | e,g,f       |   2008 |       31 |\n\nWith a readable set of scripts to ensure that your process can be audited and repeated:\n\n```python\nschema_scripts = [\n    f"UNITE > \'reference\' < {REFERENCE_COLUMNS}",\n    "RENAME > \'country_name\' < [\'Country\']",\n    "PIVOT_LONGER > [\'indicator_name\', \'values\'] < [\'HDI rank\', \'HDI Category\', \'Human poverty index (HPI-1) - Rank;;2008\', \'Human poverty index (HPI-1) - Value (%);;2008\', \'Probability at birth of not surviving to age 40 (% of cohort);;2000-05\', \'Adult illiteracy rate (% aged 15 and older);;1995-2005\', \'Population not using an improved water source (%);;2004\', \'Children under weight for age (% under age 5);;1996-2005\', \'Population below income poverty line (%) - $1 a day;;1990-2005\', \'Population below income poverty line (%) - $2 a day;;1990-2005\', \'Population below income poverty line (%) - National poverty line;;1990-2004\', \'HPI-1 rank minus income poverty rank;;2008\']",\n    "SEPARATE > [\'indicator_name\', \'year\'] < \';;\'::[\'indicator_name\']",\n    "DEBLANK",\n    "DEDUPE",\n]\n```\n\nThen **whyqd** may be for you.\n\n## How does it work?\n\n> Crosswalks are mappings of the relationships between fields defined in different metadata \n> [schemas](https://whyqd.readthedocs.io/en/latest/strategies/schema). Ideally, these are one-to-one, where a field in \n> one has an exact match in the other. In practice, it\'s more complicated than that.\n\nYour workflow is:\n\n1. Define a single destination schema,\n2. Derive a source schema from a data source,\n3. Review your source data structure,\n4. Develop a crosswalk to define the relationship between source and destination,\n5. Transform and validate your outputs,\n6. Share your output data, transform definitions, and a citation.\n\nIt starts like this:\n\n```python\nimport whyqd as qd\n```\n\n[Install](https://whyqd.readthedocs.io/en/latest/installation) and then read the [quickstart](https://whyqd.readthedocs.io/en/latest/quickstart).\n\nThere are three worked tutorials to guide you through three typical scenarios:\n\n- [Aligning multiple disparate data sources to a single schema](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial1)\n- [Pivoting wide-format data into archival long-format](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial2)\n- [Wrangling Cthulhu data without losing your mind](https://whyqd.readthedocs.io/en/latest/tutorials/tutorial3)\n\n## Installation\n\nYou\'ll need at least Python 3.8, then install with your favourite package manager:\n\n```bash\npip install whyqd\n```\n\nTo derive a source schema from tabular data, import from `DATASOURCE_PATH`, define its `MIMETYPE`, and derive a schema:\n\n```python\nimport whyqd as qd\n\ndatasource = qd.DataSourceDefinition()\ndatasource.derive_model(source=DATASOURCE_PATH, mimetype=MIMETYPE)\nschema_source = qd.SchemaDefinition()\nschema_source.derive_model(data=datasource.get)\nschema_source.fields.set_categories(name=CATEGORY_FIELD, \n                                    terms=datasource.get_data())\nschema_source.save()\n```\n\n[Get started...](https://whyqd.readthedocs.io/en/latest/quickstart)\n\n## Changelog\n\nThe version history can be found in the [changelog](https://whyqd.readthedocs.io/en/latest/changelog).\n\n## Background and funding\n\n**whyqd** was created to serve a continuous data wrangling process, including collaboration on more complex messy \nsources, ensuring the integrity of the source data, and producing a complete audit trail from data imported to our \ndatabase, back to source. You can see the product of that at [openLocal.uk](https://openlocal.uk).\n\n**whyqd** [received initial funding](https://eoscfuture-grants.eu/meet-the-grantees/implementation-no-code-method-schema-schema-data-transformations-interoperability)\nfrom the European Union\'s Horizon 2020 research and innovation programme under grant agreement No 101017536. Technical \ndevelopment support is from [EOSC Future](https://eoscfuture.eu/) through the \n[RDA Open Call mechanism](https://eoscfuture-grants.eu/provider/research-data-alliance), based on evaluations of \nexternal, independent experts.\n\nThe \'backronym\' for **whyqd** /wɪkɪd/ is *Whythawk Quantitative Data*, [Whythawk](https://whythawk.com)\nis an open data science and open research technical consultancy.\n\n## Licence\n\nThe [**whyqd** Python distribution](https://github.com/whythawk/whyqd) is licensed under the terms of the \n[BSD 3-Clause license](https://github.com/whythawk/whyqd/blob/master/LICENSE). All documentation is released under \n[Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). **whyqd** tradenames and \nmarks are copyright [Whythawk](https://whythawk.com).\n',
     'author': 'Gavin Chait',
     'author_email': 'gchait@whythawk.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://whyqd.com',
```

### Comparing `whyqd-1.0.2/PKG-INFO` & `whyqd-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whyqd
-Version: 1.0.2
+Version: 1.0.3
 Summary: data wrangling simplicity, complete audit transparency, and at speed
 Home-page: https://whyqd.com
 License: BSD-3-Clause
 Keywords: python,data-science,pandas,open-data,open-science,data-analysis,data-wrangling,data-management,munging,crosswalks
 Author: Gavin Chait
 Author-email: gchait@whythawk.com
 Requires-Python: >=3.8.1,<4.0
```

