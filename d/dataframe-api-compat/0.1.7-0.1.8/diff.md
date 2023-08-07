# Comparing `tmp/dataframe_api_compat-0.1.7.tar.gz` & `tmp/dataframe_api_compat-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataframe_api_compat-0.1.7.tar", last modified: Thu Aug  3 18:55:27 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `dataframe_api_compat-0.1.7.tar` & `dataframe_api_compat-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,92 @@
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-03 18:55:27.834583 dataframe_api_compat-0.1.7/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1071 2023-05-05 10:36:05.000000 dataframe_api_compat-0.1.7/LICENSE
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2527 2023-08-03 18:55:27.834583 dataframe_api_compat-0.1.7/PKG-INFO
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     1893 2023-08-03 18:36:13.000000 dataframe_api_compat-0.1.7/README.md
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-03 18:55:27.834583 dataframe_api_compat-0.1.7/dataframe_api_compat/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      207 2023-08-03 18:54:40.000000 dataframe_api_compat-0.1.7/dataframe_api_compat/__init__.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-03 18:55:27.834583 dataframe_api_compat-0.1.7/dataframe_api_compat/pandas_standard/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     4298 2023-08-03 15:01:07.000000 dataframe_api_compat-0.1.7/dataframe_api_compat/pandas_standard/__init__.py
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    28860 2023-08-02 15:50:34.000000 dataframe_api_compat-0.1.7/dataframe_api_compat/pandas_standard/pandas_standard.py
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-03 18:55:27.834583 dataframe_api_compat-0.1.7/dataframe_api_compat/polars_standard/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     3872 2023-08-03 18:37:11.000000 dataframe_api_compat-0.1.7/dataframe_api_compat/polars_standard/__init__.py
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)    26651 2023-08-03 18:37:11.000000 dataframe_api_compat-0.1.7/dataframe_api_compat/polars_standard/polars_standard.py
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-02 19:14:05.000000 dataframe_api_compat-0.1.7/dataframe_api_compat/py.typed
-drwxr-xr-x   0 marcogorelli  (1000) marcogorelli  (1000)        0 2023-08-03 18:55:27.834583 dataframe_api_compat-0.1.7/dataframe_api_compat.egg-info/
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)     2527 2023-08-03 18:55:27.000000 dataframe_api_compat-0.1.7/dataframe_api_compat.egg-info/PKG-INFO
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      500 2023-08-03 18:55:27.000000 dataframe_api_compat-0.1.7/dataframe_api_compat.egg-info/SOURCES.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)        1 2023-08-03 18:55:27.000000 dataframe_api_compat-0.1.7/dataframe_api_compat.egg-info/dependency_links.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       21 2023-08-03 18:55:27.000000 dataframe_api_compat-0.1.7/dataframe_api_compat.egg-info/top_level.txt
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      570 2023-08-03 18:38:08.000000 dataframe_api_compat-0.1.7/pyproject.toml
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)      947 2023-08-03 18:55:27.834583 dataframe_api_compat-0.1.7/setup.cfg
--rw-r--r--   0 marcogorelli  (1000) marcogorelli  (1000)       74 2023-08-02 10:13:15.000000 dataframe_api_compat-0.1.7/setup.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/blog_post.md
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/check_completeness.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/contributing.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/make.sh
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/mypy.ini
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/requirements-dev.txt
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/t.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/type-check.sh
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/update-pandas.sh
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/.github/workflows/tox.yml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/dataframe_api_compat/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/dataframe_api_compat/py.typed
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/dataframe_api_compat/pandas_standard/__init__.py
+-rw-r--r--   0        0        0    28860 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/dataframe_api_compat/pandas_standard/pandas_standard.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/dataframe_api_compat/polars_standard/__init__.py
+-rw-r--r--   0        0        0    28447 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/dataframe_api_compat/polars_standard/polars_standard.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/conftest.py
+-rw-r--r--   0        0        0    23648 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/utils.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/and_or_test.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/any_all_test.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/col_to_array_object_test.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/column_test.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/comparisons_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/conftest.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/cumulative_test.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/divmod_test.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/fill_nan_test.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/fill_null_test.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/get_rows_by_mask_test.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/get_rows_test.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/get_value_test.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/invalid_pandas_test.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/invert_test.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/is_in_test.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/is_nan_test.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/is_null_test.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/len_test.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/pow_test.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/reductions_test.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/rename_test.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/slice_rows_test.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/sorted_indices_test.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/statistics_test.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/column/unique_indices_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/all_rowwise_test.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/and_test.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/any_all_test.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/any_rowwise_test.py
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/comparisons_test.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/divmod_test.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/drop_column_test.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/fill_nan_test.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/fill_null_test.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/get_column_by_name_test.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/get_column_names_test.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/get_columns_by_name_test.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/get_rows_by_mask_test.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/get_rows_test.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/insert_test.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/invert_test.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/is_nan_test.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/is_null_test.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/or_test.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/pow_test.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/reductions_test.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/rename_columns_test.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/shape_test.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/slice_rows_test.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/sorted_indices_test.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/to_array_object_test.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/dataframe/unique_indices_test.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/groupby/groupby_any_all_test.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/groupby/invalid_test.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/groupby/numeric_test.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/groupby/size_test.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/namespace/column_from_1d_array_test.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/namespace/column_from_sequence_test.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/namespace/column_names_test.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/namespace/concat_test.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/namespace/dataframe_from_2d_array_test.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/namespace/namespace_is_null_test.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/tests/namespace/to_array_object_test.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/README.md
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 dataframe_api_compat-0.1.8/PKG-INFO
```

### Comparing `dataframe_api_compat-0.1.7/LICENSE` & `dataframe_api_compat-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.7/PKG-INFO` & `dataframe_api_compat-0.1.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: dataframe_api_compat
-Version: 0.1.7
-Summary: Implementation of the DataFrame Standard for pandas and polars
-Home-page: https://github.com/data-apis/dataframe-api-compat
-Author: Marco Gorelli
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Build Status](https://github.com/data-apis/dataframe-api-compat/workflows/tox/badge.svg)](https://github.com/data-apis/dataframe-api-compat/actions?workflow=tox)
 [![Coverage](https://codecov.io/gh/MarcoGorelli/cython-lint/branch/main/graph/badge.svg)](https://codecov.io/gh/data-apis/dataframe-api-compat)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/MarcoGorelli/dataframe-api-compat/main.svg)](https://results.pre-commit.ci/latest/github/MarcoGorelli/dataframe-api-compat/main)
 
 # DataFrame API Compat
 
 <h1 align="center">
@@ -61,9 +44,7 @@
 The object `df_std` is a Standard-compliant DataFrame.
 
 Installation
 ------------
 ```
 pip install dataframe-api-compat
 ```
-
-
```

### Comparing `dataframe_api_compat-0.1.7/dataframe_api_compat/pandas_standard/__init__.py` & `dataframe_api_compat-0.1.8/dataframe_api_compat/pandas_standard/__init__.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.7/dataframe_api_compat/pandas_standard/pandas_standard.py` & `dataframe_api_compat-0.1.8/dataframe_api_compat/pandas_standard/pandas_standard.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.7/dataframe_api_compat/polars_standard/__init__.py` & `dataframe_api_compat-0.1.8/dataframe_api_compat/polars_standard/__init__.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.1.7/dataframe_api_compat/polars_standard/polars_standard.py` & `dataframe_api_compat-0.1.8/dataframe_api_compat/polars_standard/polars_standard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from __future__ import annotations
 
 import collections
+import secrets
 from typing import Any
 from typing import Generic
 from typing import Literal
 from typing import NoReturn
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import polars as pl
 
 import dataframe_api_compat.polars_standard
 
+# do we need a separate class for polars lazy?
+# might be best - after all, we can't mix lazy
+# and eager
+# BUT most things will probably work the same way?
+
 _ARRAY_API_DTYPES = frozenset(
     (
         "bool",
         "int8",
         "int16",
         "int32",
         "int64",
@@ -68,16 +74,19 @@
             pl.UInt16,
             pl.UInt8,
         )
     )
 
 
 class PolarsColumn(Column[DType]):
-    def __init__(self, column: pl.Series) -> None:
+    def __init__(self, column: pl.Series, *, hash: str | None = None) -> None:
+        # _df only necessary in the lazy case
+        # keep track of which dataframe the column came from
         self._series = column
+        self._hash = hash
 
     # In the standard
     def __column_namespace__(self, *, api_version: str | None = None) -> Any:
         return dataframe_api_compat.polars_standard
 
     @property
     def name(self) -> str:
@@ -167,58 +176,59 @@
     def var(self, *, correction: int | float = 1.0, skip_nulls: bool = True) -> Any:
         return self.column.var()
 
     def __eq__(  # type: ignore[override]
         self, other: Column[DType] | Any
     ) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
-            return PolarsColumn(self.column == other.column)
-        return PolarsColumn(self.column == other)
+            return PolarsColumn(self.column == other.column, hash=self._hash)
+        return PolarsColumn(self.column == other, hash=self._hash)
 
     def __ne__(  # type: ignore[override]
         self, other: Column[DType] | Any
     ) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
-            return PolarsColumn(self.column != other.column)
-        return PolarsColumn(self.column != other)
+            return PolarsColumn(self.column != other.column, hash=self._hash)
+        return PolarsColumn(self.column != other, hash=self._hash)
 
     def __ge__(self, other: Column[DType] | Any) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
-            return PolarsColumn(self.column >= other.column)
-        return PolarsColumn(self.column >= other)
+            return PolarsColumn(self.column >= other.column, hash=self._hash)
+        return PolarsColumn(self.column >= other, hash=self._hash)
 
     def __gt__(self, other: Column[DType] | Any) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
-            return PolarsColumn(self.column > other.column)
-        return PolarsColumn(self.column > other)
+            # todo: validate other column's ._df
+            return PolarsColumn(self.column > other.column, hash=self._hash)
+        return PolarsColumn(self.column > other, hash=self._hash)
 
     def __le__(self, other: Column[DType] | Any) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
-            return PolarsColumn(self.column <= other.column)
-        return PolarsColumn(self.column <= other)
+            return PolarsColumn(self.column <= other.column, hash=self._hash)
+        return PolarsColumn(self.column <= other, hash=self._hash)
 
     def __lt__(self, other: Column[DType] | Any) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
-            return PolarsColumn(self.column < other.column)
-        return PolarsColumn(self.column < other)
+            return PolarsColumn(self.column < other.column, hash=self._hash)
+        return PolarsColumn(self.column < other, hash=self._hash)
 
     def __mul__(self, other: Column[DType] | Any) -> PolarsColumn[Any]:
         if isinstance(other, PolarsColumn):
-            return PolarsColumn(self.column * other.column)
-        return PolarsColumn(self.column * other)
+            return PolarsColumn(self.column * other.column, hash=self._hash)
+        return PolarsColumn(self.column * other, hash=self._hash)
 
     def __floordiv__(self, other: Column[DType] | Any) -> PolarsColumn[Any]:
         if isinstance(other, PolarsColumn):
-            return PolarsColumn(self.column // other.column)
-        return PolarsColumn(self.column // other)
+            return PolarsColumn(self.column // other.column, hash=self._hash)
+        return PolarsColumn(self.column // other, hash=self._hash)
 
     def __truediv__(self, other: Column[DType] | Any) -> PolarsColumn[Any]:
         if isinstance(other, PolarsColumn):
-            return PolarsColumn(self.column / other.column)
-        return PolarsColumn(self.column / other)
+            return PolarsColumn(self.column / other.column, hash=self._hash)
+        return PolarsColumn(self.column / other, hash=self._hash)
 
     def __pow__(self, other: Column[DType] | Any) -> PolarsColumn[Any]:
         original_type = self.column.dtype
         if isinstance(other, PolarsColumn):
             ret = self.column.pow(other.column)
             if _is_integer_dtype(original_type) and _is_integer_dtype(other.column.dtype):
                 if (other.column < 0).any():
@@ -243,34 +253,34 @@
     ) -> tuple[PolarsColumn[Any], PolarsColumn[Any]]:
         quotient = self // other
         remainder = self - quotient * other
         return quotient, remainder
 
     def __and__(self, other: Column[Bool] | bool) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
-            return PolarsColumn(self.column & other.column)
-        return PolarsColumn(self.column & other)  # type: ignore[operator]
+            return PolarsColumn(self.column & other.column, hash=self._hash)
+        return PolarsColumn(self.column & other, hash=self._hash)  # type: ignore[operator]
 
     def __or__(self, other: Column[Bool] | bool) -> PolarsColumn[Bool]:
         if isinstance(other, PolarsColumn):
-            return PolarsColumn(self.column | other.column)
-        return PolarsColumn(self.column | other)  # type: ignore[operator]
+            return PolarsColumn(self.column | other.column, hash=self._hash)
+        return PolarsColumn(self.column | other, hash=self._hash)  # type: ignore[operator]
 
     def __invert__(self) -> PolarsColumn[Bool]:
-        return PolarsColumn(~self.column)
+        return PolarsColumn(~self.column, hash=self._hash)
 
     def __add__(self, other: Column[Any] | Any) -> PolarsColumn[Any]:
         if isinstance(other, PolarsColumn):
-            return PolarsColumn(self.column + other.column)
-        return PolarsColumn(self.column + other)
+            return PolarsColumn(self.column + other.column, hash=self._hash)
+        return PolarsColumn(self.column + other, hash=self._hash)
 
     def __sub__(self, other: Column[Any] | Any) -> PolarsColumn[Any]:
         if isinstance(other, PolarsColumn):
-            return PolarsColumn(self.column - other.column)
-        return PolarsColumn(self.column - other)
+            return PolarsColumn(self.column - other.column, hash=self._hash)
+        return PolarsColumn(self.column - other, hash=self._hash)
 
     def sorted_indices(
         self, *, ascending: bool = True, nulls_position: Literal["first", "last"] = "last"
     ) -> PolarsColumn[Any]:
         df = self.column.to_frame()
         keys = df.columns
         if ascending:
@@ -303,15 +313,17 @@
         if dtype not in _ARRAY_API_DTYPES:
             raise ValueError(
                 f"Invalid dtype {dtype}. Expected one of {_ARRAY_API_DTYPES}"
             )
         return self.column.to_numpy().astype(dtype)
 
     def rename(self, name: str | None) -> PolarsColumn[DType]:
-        return PolarsColumn(self.column.rename(name or ""))
+        if isinstance(self.column, pl.Series):
+            return PolarsColumn(self.column.rename(name or ""))
+        return PolarsColumn(self.column.alias(name or ""), hash=self._hash)
 
 
 class PolarsGroupBy(GroupBy):
     def __init__(self, df: pl.DataFrame | pl.LazyFrame, keys: Sequence[str]) -> None:
         for key in keys:
             if key not in df.columns:
                 raise KeyError(f"key {key} not present in DataFrame's columns")
@@ -368,14 +380,23 @@
 
 
 class PolarsDataFrame(DataFrame):
     def __init__(self, df: pl.DataFrame | pl.LazyFrame) -> None:
         # columns already have to be strings, and duplicates aren't
         # allowed, so no validation required
         self.df = df
+        self._hash = secrets.token_hex(3)
+
+    def _validate_column(self, column) -> None:
+        if isinstance(column.column, pl.Expr) and column._hash != self._hash:
+            raise ValueError(
+                "Column was created from a different dataframe!",
+                column._hash,
+                self._hash,
+            )
 
     def __dataframe_namespace__(self, *, api_version: str | None = None) -> Any:
         return dataframe_api_compat.polars_standard
 
     @property
     def dataframe(self) -> pl.DataFrame | pl.LazyFrame:
         return self.df
@@ -384,14 +405,16 @@
         return self.df.shape  # type: ignore[union-attr]
 
     def groupby(self, keys: Sequence[str]) -> PolarsGroupBy:
         return PolarsGroupBy(self.df, keys)
 
     def get_column_by_name(self, name: str) -> PolarsColumn[DType]:
         # todo: make single-column df so it can work with lazyframe?
+        if isinstance(self.dataframe, pl.LazyFrame):
+            return PolarsColumn(pl.col(name), hash=self._hash)
         return PolarsColumn(self.df.get_column(name))  # type: ignore[union-attr]
 
     def get_columns_by_name(self, names: Sequence[str]) -> PolarsDataFrame:
         if isinstance(names, str):
             raise TypeError(f"Expected sequence of str, got {type(names)}")
         return PolarsDataFrame(self.df.select(names))
 
@@ -400,20 +423,21 @@
 
     def slice_rows(
         self, start: int | None, stop: int | None, step: int | None
     ) -> PolarsDataFrame:
         return PolarsDataFrame(self.df[start:stop:step])
 
     def get_rows_by_mask(self, mask: Column[Bool]) -> PolarsDataFrame:
+        self._validate_column(mask)
         return PolarsDataFrame(self.df.filter(mask.column))
 
     def insert(self, loc: int, label: str, value: Column[Any]) -> PolarsDataFrame:
-        df = self.df.clone()
-        # how to do this for lazy frame?
-        df.insert_at_idx(loc, pl.Series(label, value.column))  # type: ignore[union-attr]
+        columns = self.dataframe.columns
+        new_columns = columns[:loc] + [label] + columns[loc:]
+        df = self.dataframe.with_columns(value.column.alias(label)).select(new_columns)
         return PolarsDataFrame(df)
 
     def drop_column(self, label: str) -> PolarsDataFrame:
         if not isinstance(label, str):
             raise TypeError(f"Expected str, got: {type(label)}")
         return PolarsDataFrame(self.dataframe.drop(label))
 
@@ -584,18 +608,24 @@
     def any(self, *, skip_nulls: bool = True) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe.select(pl.col("*").any()))
 
     def all(self, *, skip_nulls: bool = True) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe.select(pl.col("*").all()))
 
     def any_rowwise(self, *, skip_nulls: bool = True) -> PolarsColumn[Bool]:
-        return PolarsColumn(self.dataframe.select(pl.any_horizontal(pl.col("*"))).get_column("any"))  # type: ignore[union-attr]
+        expr = pl.any_horizontal(pl.col("*"))
+        if isinstance(self.dataframe, pl.LazyFrame):
+            return PolarsColumn(expr, hash=self._hash)
+        return PolarsColumn(self.dataframe.select(expr).get_column("any"))  # type: ignore[union-attr]
 
     def all_rowwise(self, *, skip_nulls: bool = True) -> PolarsColumn[Bool]:
-        return PolarsColumn(self.dataframe.select(pl.all_horizontal(pl.col("*"))).get_column("all"))  # type: ignore[union-attr]
+        expr = pl.all_horizontal(pl.col("*"))
+        if isinstance(self.dataframe, pl.LazyFrame):
+            return PolarsColumn(expr, hash=self._hash)
+        return PolarsColumn(self.dataframe.select(expr).get_column("all"))  # type: ignore[union-attr]
 
     def min(self, *, skip_nulls: bool = True) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe.select(pl.col("*").min()))
 
     def max(self, *, skip_nulls: bool = True) -> PolarsDataFrame:
         return PolarsDataFrame(self.dataframe.select(pl.col("*").max()))
 
@@ -669,9 +699,10 @@
 
     def to_array_object(self, dtype: str) -> Any:
         if dtype not in _ARRAY_API_DTYPES:
             raise ValueError(
                 f"Invalid dtype {dtype}. Expected one of {_ARRAY_API_DTYPES}"
             )
         if isinstance(self.dataframe, pl.LazyFrame):
+            # todo - remove this? should it raise?
             return self.dataframe.collect().to_numpy().astype(dtype)
         return self.dataframe.to_numpy().astype(dtype)
```

### Comparing `dataframe_api_compat-0.1.7/dataframe_api_compat.egg-info/PKG-INFO` & `dataframe_api_compat-0.1.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
-Name: dataframe-api-compat
-Version: 0.1.7
-Summary: Implementation of the DataFrame Standard for pandas and polars
-Home-page: https://github.com/data-apis/dataframe-api-compat
-Author: Marco Gorelli
-License: MIT
-Platform: UNKNOWN
+Name: dataframe_api_compat
+Version: 0.1.8
+Summary: Implementation of the DataFrame Standard for pandas and Polars
+Project-URL: Homepage, https://github.com/data-apis/dataframe-api-compat
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 [![Build Status](https://github.com/data-apis/dataframe-api-compat/workflows/tox/badge.svg)](https://github.com/data-apis/dataframe-api-compat/actions?workflow=tox)
 [![Coverage](https://codecov.io/gh/MarcoGorelli/cython-lint/branch/main/graph/badge.svg)](https://codecov.io/gh/data-apis/dataframe-api-compat)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/MarcoGorelli/dataframe-api-compat/main.svg)](https://results.pre-commit.ci/latest/github/MarcoGorelli/dataframe-api-compat/main)
 
 # DataFrame API Compat
 
@@ -61,9 +58,7 @@
 The object `df_std` is a Standard-compliant DataFrame.
 
 Installation
 ------------
 ```
 pip install dataframe-api-compat
 ```
-
-
```

