# Comparing `tmp/AutoCarver-5.1.9.tar.gz` & `tmp/AutoCarver-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.1.9.tar", last modified: Sun Jul 30 11:57:57 2023, max compression
+gzip compressed data, was "AutoCarver-5.2.0.tar", last modified: Mon Aug  7 19:14:47 2023, max compression
```

## Comparing `AutoCarver-5.1.9.tar` & `AutoCarver-5.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.201018 AutoCarver-5.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.197018 AutoCarver-5.1.9/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35502 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/auto_carver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.197018 AutoCarver-5.1.9/AutoCarver/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/converters/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.197018 AutoCarver-5.1.9/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25459 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.197018 AutoCarver-5.1.9/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35455 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/utils/grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    32441 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/discretizers/utils/type_discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.197018 AutoCarver-5.1.9/AutoCarver/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.197018 AutoCarver-5.1.9/AutoCarver/feature_selection/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/filters/base_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/filters/qualitative_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/filters/quantitative_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.201018 AutoCarver-5.1.9/AutoCarver/feature_selection/measures/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/measures/base_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/measures/qualitative_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/AutoCarver/feature_selection/measures/quantitative_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.197018 AutoCarver-5.1.9/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-30 11:57:57.000000 AutoCarver-5.1.9/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-30 11:57:57.000000 AutoCarver-5.1.9/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 11:57:57.000000 AutoCarver-5.1.9/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-30 11:57:57.000000 AutoCarver-5.1.9/AutoCarver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-30 11:57:57.000000 AutoCarver-5.1.9/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-30 11:57:57.201018 AutoCarver-5.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-30 11:57:57.201018 AutoCarver-5.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:57:57.201018 AutoCarver-5.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-07-30 11:57:47.000000 AutoCarver-5.1.9/tests/test_auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:14:47.484786 AutoCarver-5.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:14:47.480786 AutoCarver-5.2.0/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41715 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:14:47.484786 AutoCarver-5.2.0/AutoCarver/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/converters/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:14:47.484786 AutoCarver-5.2.0/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25459 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:14:47.484786 AutoCarver-5.2.0/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35051 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32441 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/discretizers/utils/type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:14:47.484786 AutoCarver-5.2.0/AutoCarver/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/feature_selection/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:14:47.484786 AutoCarver-5.2.0/AutoCarver/feature_selection/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/feature_selection/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/feature_selection/filters/base_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/feature_selection/filters/qualitative_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/feature_selection/filters/quantitative_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:14:47.484786 AutoCarver-5.2.0/AutoCarver/feature_selection/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/feature_selection/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/feature_selection/measures/base_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/feature_selection/measures/qualitative_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/AutoCarver/feature_selection/measures/quantitative_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:14:47.484786 AutoCarver-5.2.0/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-08-07 19:14:47.000000 AutoCarver-5.2.0/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-07 19:14:47.000000 AutoCarver-5.2.0/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:14:47.000000 AutoCarver-5.2.0/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-07 19:14:47.000000 AutoCarver-5.2.0/AutoCarver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 19:14:47.000000 AutoCarver-5.2.0/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-08-07 19:14:47.484786 AutoCarver-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-07 19:14:47.488786 AutoCarver-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:14:47.484786 AutoCarver-5.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-08-07 19:14:37.000000 AutoCarver-5.2.0/tests/test_auto_carver.py
```

### Comparing `AutoCarver-5.1.9/AutoCarver/auto_carver.py` & `AutoCarver-5.2.0/AutoCarver/auto_carver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Tool to build optimized buckets out of Quantitative and Qualitative features
 for a binary classification model.
 """
 
-from typing import Any
+from typing import Any, Callable, Union
 
-from numpy import add, array, searchsorted, sqrt, unique, zeros
+from numpy import add, array, mean, searchsorted, sqrt, unique, zeros
 from pandas import DataFrame, Series, crosstab
-from scipy.stats import chi2_contingency
+from scipy.stats import chi2_contingency, kruskal
 from tqdm import tqdm
 
 from .discretizers import GroupedList
 from .discretizers.discretizers import Discretizer
 from .discretizers.utils.base_discretizers import (
     BaseDiscretizer,
     convert_to_labels,
@@ -25,30 +25,30 @@
     _has_idisplay = False
 else:
     _has_idisplay = True
 
 
 class AutoCarver(BaseDiscretizer):
     """Automatic carving of continuous, discrete, categorical and ordinal
-    features that maximizes association with a binary target.
+    features that maximizes association with a binary or continuous target.
 
     First fits a :ref:`Discretizer`. Raw data should be provided as input (not a result of ``Discretizer.transform()``).
     """
 
     def __init__(
         self,
         min_freq: float,
+        sort_by: str,
         *,
         quantitative_features: list[str] = None,
         qualitative_features: list[str] = None,
         ordinal_features: list[str] = None,
         values_orders: dict[str, GroupedList] = None,
         max_n_mod: int = 5,
         # min_carved_freq: float = 0,  # TODO: update this parameter so that it is set according to frequency rather than number of groups
-        sort_by: str = "tschuprowt",
         output_dtype: str = "float",
         dropna: bool = True,
         unknown_handling: str = "raises",
         copy: bool = False,
         verbose: bool = False,
         pretty_print: bool = False,
         str_nan: str = "__NAN__",
@@ -63,14 +63,25 @@
 
             * Features whose most frequent modality is less frequent than ``min_freq`` will not be carved.
             * Sets the number of quantiles in which to discretize the continuous features.
             * Sets the minimum frequency of a quantitative feature's modality.
 
             **Tip**: should be set between 0.02 (slower, preciser, less robust) and 0.05 (faster, more robust)
 
+        sort_by : str
+            To be choosen amongst ``["tschuprowt", "cramerv", "kruskal"]``
+            Metric to be used to perform association measure between features and target.
+
+            * Binary target: use ``"tschuprowt"``, for Tschuprow's T.
+            * Binary target: use ``"cramerv"``, for Cramér's V.
+            * Continuous target: use ``"kruskal"``, for Kruskal-Wallis' H test statistic.
+
+            **Tip**: use ``"tschuprowt"`` for more robust, or less output modalities,
+            use ``"cramerv"`` for more output modalities.
+
         quantitative_features : list[str], optional
             List of column names of quantitative features (continuous and discrete) to be carved, by default ``None``
 
         qualitative_features : list[str], optional
             List of column names of qualitative features (non-ordinal) to be carved, by default ``None``
 
         ordinal_features : list[str], optional
@@ -85,24 +96,14 @@
             Maximum number of modality per feature, by default ``5``
 
             All combinations of modalities for groups of modalities of sizes from 1 to ``max_n_mod`` will be tested.
             The combination with the greatest association (as defined by ``sort_by``) will be the selected one.
 
             **Tip**: should be set between 4 (faster, more robust) and 7 (slower, preciser, less robust)
 
-        sort_by : str, optional
-            To be choosen amongst ``["tschuprowt", "cramerv"]``, by default ``"tschuprowt"``
-            Metric to be used to perform association measure between features and target.
-
-            * ``"tschuprowt"``, Tschuprow's T will be used as the association measure (more robust).
-            * ``"cramerv"``, Cramér's V will be used as the association measure (less robust).
-
-            **Tip**: use ``"tschuprowt"`` for more robust, or less output modalities,
-            use ``"cramerv"`` for more output modalities.
-
         output_dtype : str, optional
             To be choosen amongst ``["float", "str"]``, by default ``"float"``
 
             * ``"float"``, grouped modalities will be converted to there corresponding floating rank.
             * ``"str"``, a per-group modality will be set for all the modalities of a group.
 
         dropna : bool, optional
@@ -183,15 +184,19 @@
                 self.pretty_print = pretty_print
             else:
                 self.verbose = True
                 print(
                     "Package not found: ipython. Defaulting to verbose=True. Install extra dependencies with pip install autocarver[jupyter]"
                 )
 
-        measures = ["tschuprowt", "cramerv"]  # association measure used to find the best groups
+        measures = [
+            "tschuprowt",
+            "cramerv",
+            "kruskal",
+        ]  # association measure used to find the best groups
         assert (
             sort_by in measures
         ), f""" - [AutoCarver] Measure '{sort_by}' not yet implemented. Choose from: {str(measures)}."""
         self.sort_by = sort_by
 
         assert unknown_handling in [
             "drop",
@@ -203,15 +208,15 @@
 
     def _prepare_data(
         self,
         X: DataFrame,
         y: Series,
         X_dev: DataFrame = None,
         y_dev: Series = None,
-    ) -> tuple[DataFrame, DataFrame]:
+    ) -> tuple[DataFrame, DataFrame, dict[str, Callable]]:
         """Validates format and content of X and y.
 
         Parameters
         ----------
         X : DataFrame
             Dataset used to discretize. Needs to have columns has specified in ``AutoCarver.features``.
 
@@ -223,22 +228,80 @@
             It should have the same distribution as X.
 
         y_dev : Series, optional
             Binary target feature with wich the robustness of discretization is evaluated, by default ``None``
 
         Returns
         -------
-        tuple[DataFrame, DataFrame]
-            Copies of (X, X_dev)
+        tuple[DataFrame, DataFrame, dict[str, Callable]]
+            Copies of (X, X_dev) and helpers to be used according to target type
         """
         # Checking for binary target and copying X
         x_copy = super()._prepare_data(X, y)
         x_dev_copy = super()._prepare_data(X_dev, y_dev)
 
-        return x_copy, x_dev_copy
+        # checking for nans in the target
+        assert not any(y.isna()), " - [AutoCarver] y should not contain numpy.nan"
+
+        # checking for binary target
+        y_values = unique(y)
+        is_binary = len(y_values) == 2
+        # case 0: binary target, checking values
+        if is_binary:
+            assert (0 in y_values) & (
+                1 in y_values
+            ), " - [AutoCarver] y must be a binary Series (int or float, not object)"
+            assert (
+                len(y_values) == 2
+            ), " - [AutoCarver] y must be a binary Series (int or float, not object)"
+
+            # setting up helper functions to be used in autocarver
+            helpers = {
+                "aggregator": get_xtabs,
+                "grouper": xtab_grouper,
+                "association_measure": association_xtab,
+                "target_rate": xtab_target_rate,
+                "combination_formatter": xtab_combination_formatter,
+                "printer": pretty_xtab,
+            }
+
+            # checking for a corresponding sorting measure
+            measures = ["tschuprowt", "cramerv"]
+            assert (
+                self.sort_by in measures
+            ), f""" - [AutoCarver] Measure '{self.sort_by}' not implemented for a binary target. Choose from: {str(measures)}."""
+
+        # case 1: continuous target, checking values
+        else:
+            not_numeric = str in y.apply(type).unique()
+            assert (
+                not not_numeric
+            ), " - [AutoCarver] y must be a continuous Series (int or float, not object)"
+            pct_y = len(y_values) / len(y)
+            assert (
+                pct_y > 0.01
+            ), f" - [AutoCarver] y must be a continuous or binary Series (not implemented for multiclass, only {pct_y:2.2%} distinct values)"
+
+            # setting up helper functions to be used in autocarver
+            helpers = {
+                "aggregator": get_yvals,
+                "grouper": yval_grouper,
+                "association_measure": association_yval,
+                "target_rate": yval_target_rate,
+                "combination_formatter": yval_combination_formatter,
+                "printer": pretty_yval,
+            }
+
+            # checking for a corresponding sorting measure
+            measures = ["kruskal"]
+            assert (
+                self.sort_by in measures
+            ), f""" - [AutoCarver] Measure '{self.sort_by}' not implemented for a binary target. Choose from: {str(measures)}."""
+
+        return x_copy, x_dev_copy, helpers
 
     def _remove_feature(self, feature: str) -> None:
         """Removes a feature from all ``AutoCarver.features`` attributes
 
         Parameters
         ----------
         feature : str
@@ -249,14 +312,15 @@
             if feature in self.ordinal_features:
                 self.ordinal_features.remove(feature)
 
     def fit(
         self,
         X: DataFrame,
         y: Series,
+        *,
         X_dev: DataFrame = None,
         y_dev: Series = None,
     ) -> None:
         """Finds the combination of modalities of X that provides the best association with y.
 
         Parameters
         ----------
@@ -270,15 +334,15 @@
             Dataset to evalute the robustness of discretization, by default None
             It should have the same distribution as X.
 
         y_dev : Series, optional
             Binary target feature with wich the robustness of discretization is evaluated, by default None
         """
         # preparing datasets and checking for wrong values
-        x_copy, x_dev_copy = self._prepare_data(X, y, X_dev, y_dev)
+        x_copy, x_dev_copy, helpers = self._prepare_data(X, y, X_dev, y_dev)
 
         # discretizing all features
         discretizer = Discretizer(
             quantitative_features=self.quantitative_features,
             qualitative_features=self.qualitative_features,
             min_freq=self.min_freq,
             ordinal_features=self.ordinal_features,
@@ -300,54 +364,54 @@
         # removing dropped features
         removed_features = [
             feature for feature in self.features if feature not in discretizer.features
         ]
         for feature in removed_features:
             self._remove_feature(feature)
 
-        # converting potential quantiles into there respective labels
+        # converting quantiles into there respective labels
         labels_orders = convert_to_labels(
             features=self.features,
             quantitative_features=self.quantitative_features,
             values_orders=self.values_orders,
             str_nan=self.str_nan,
             dropna=False,
         )
 
         # computing crosstabs for each feature on train/test
-        xtabs = get_xtabs(self.features, x_copy, y, labels_orders)
-        xtabs_dev = get_xtabs(self.features, x_dev_copy, y_dev, labels_orders)
+        xaggs = helpers["aggregator"](self.features, x_copy, y, labels_orders)
+        xaggs_dev = helpers["aggregator"](self.features, x_dev_copy, y_dev, labels_orders)
 
         # optimal butcketization/carving of each feature
         all_features = self.features[:]  # (features are being removed from self.features)
         for n, feature in enumerate(all_features):
             if self.verbose:  # verbose if requested
                 print(f"\n------\n[AutoCarver] Fit {feature} ({n+1}/{len(all_features)})\n---")
 
             # getting xtabs on train/test
-            xtab = xtabs[feature]
-            xtab_dev = xtabs_dev[feature]
+            xagg = xaggs[feature]
+            xagg_dev = xaggs_dev[feature]
             if self.verbose:  # verbose if requested
                 print("\n - [AutoCarver] Raw feature distribution")
-                print_xtabs(xtab, xtab_dev, pretty_print=self.pretty_print)
+                # TODO: get the good labels
+                print_xagg(xagg, xagg_dev=xagg_dev, pretty_print=self.pretty_print, **helpers)
 
             # ordering
             order = labels_orders[feature]
 
             # getting best combination
-            best_combination = self._get_best_combination(order, xtab, xtab_dev=xtab_dev)
+            best_combination = self._get_best_combination(order, xagg, helpers, xagg_dev=xagg_dev)
 
             # checking that a suitable combination has been found
             if best_combination is not None:
-                order, xtab, xtab_dev = best_combination
+                order, xagg, xagg_dev = best_combination
                 if self.verbose:  # verbose if requested
                     print("\n - [AutoCarver] Carved feature distribution")
-                    print_xtabs(
-                        xtab, xtab_dev, pretty_print=self.pretty_print
-                    )  # TODO get the good labels
+                    # TODO: get the good labels
+                    print_xagg(xagg, xagg_dev=xagg_dev, pretty_print=self.pretty_print, **helpers)
 
                 # updating label_orders
                 labels_orders.update({feature: order})
 
             # no suitable combination has been found -> removing feature
             else:
                 print(
@@ -375,65 +439,67 @@
         super().fit(X, y)
 
         return self
 
     def _get_best_combination(
         self,
         order: GroupedList,
-        xtab: DataFrame,
+        xagg: DataFrame,
+        helpers: dict[str, Callable],
         *,
-        xtab_dev: DataFrame = None,
+        xagg_dev: DataFrame = None,
     ) -> tuple[GroupedList, DataFrame, DataFrame]:
         """_summary_
 
         Parameters
         ----------
         order : GroupedList
             _description_
-        xtab : DataFrame
+        xagg : DataFrame
             _description_
-        xtab_dev : DataFrame, optional
+        xagg_dev : DataFrame, optional
             _description_, by default None
 
         Returns
         -------
         tuple[GroupedList, DataFrame, DataFrame]
             _description_
         """
         # raw ordering
         raw_order = GroupedList(order)
         if self.str_nan in raw_order:
             raw_order.remove(self.str_nan)
 
         # filtering out nans if requested from train/test crosstabs
-        raw_xtab = filter_nan_xtab(xtab, self.str_nan)
-        raw_xtab_dev = filter_nan_xtab(xtab_dev, self.str_nan)
+        raw_xagg = filter_nan(xagg, self.str_nan)
+        raw_xagg_dev = filter_nan(xagg_dev, self.str_nan)
 
         # checking for non-nan values
         best_association = None
-        if raw_xtab.shape[0] > 1:
+        if raw_xagg.shape[0] > 1:
             # all possible consecutive combinations
             combinations = consecutive_combinations(
                 raw_order, self.max_n_mod, min_group_size=self.min_group_size
             )
 
             # getting most associated combination
             best_association = get_best_association(
-                raw_xtab,
+                raw_xagg,
                 combinations,
                 sort_by=self.sort_by,
-                xtab_dev=raw_xtab_dev,
+                xagg_dev=raw_xagg_dev,
                 verbose=self.verbose,
+                **helpers,
             )
 
             # applying best_combination to order and xtabs
             if best_association is not None:
                 order = order_apply_combination(order, best_association["combination"])
-                xtab = xtab_apply_order(xtab, order)
-                xtab_dev = xtab_apply_order(xtab_dev, order)
+                xagg = xagg_apply_order(xagg, order)
+                xagg_dev = xagg_apply_order(xagg_dev, order)
 
             # grouping NaNs if requested to drop them (dropna=True)
             if self.dropna and self.str_nan in order and best_association is not None:
                 # raw ordering without nans
                 raw_order = GroupedList(order)
                 raw_order.remove(self.str_nan)
 
@@ -445,30 +511,31 @@
                 # adding combinations with NaNs
                 nan_combinations = add_nan_in_combinations(
                     combinations, self.str_nan, self.max_n_mod
                 )
 
                 # getting most associated combination
                 best_association = get_best_association(
-                    xtab,
+                    xagg,
                     nan_combinations,
                     sort_by=self.sort_by,
-                    xtab_dev=xtab_dev,
+                    xagg_dev=xagg_dev,
                     verbose=self.verbose,
+                    **helpers,
                 )
 
                 # applying best_combination to order and xtab
                 if best_association is not None:
                     order = order_apply_combination(order, best_association["combination"])
-                    xtab = xtab_apply_order(xtab, order)
-                    xtab_dev = xtab_apply_order(xtab_dev, order)
+                    xagg = xagg_apply_order(xagg, order)
+                    xagg_dev = xagg_apply_order(xagg_dev, order)
 
         # checking that a suitable combination has been found
         if best_association is not None:
-            return order, xtab, xtab_dev
+            return order, xagg, xagg_dev
 
 
 def xtab_target_rate(xtab: DataFrame) -> DataFrame:
     """Computes target rate per row for a binary target (column) in a crosstab
 
     Parameters
     ----------
@@ -476,41 +543,57 @@
         _description_
 
     Returns
     -------
     DataFrame
         _description_
     """
-    return xtab[1].divide(xtab[0]).sort_values()
+    return xtab[1].divide(xtab.sum(axis=0)).sort_values()
 
 
-def filter_nan_xtab(xtab: DataFrame, str_nan: str) -> DataFrame:
-    """Filters out nans from the crosstab
+def yval_target_rate(yval: Series) -> Series:
+    """Computes target rate per row for a binary target (column) in a crosstab
 
     Parameters
     ----------
-    xtab : DataFrame
+    yval : Series
+        _description_
+
+    Returns
+    -------
+    Series
+        _description_
+    """
+    return yval.apply(mean).sort_values()
+
+
+def filter_nan(xagg: Union[Series, DataFrame], str_nan: str) -> DataFrame:
+    """Filters out nans from crosstab or y values
+
+    Parameters
+    ----------
+    xagg : Union[Series, DataFrame]
         _description_
     str_nan : str
         _description_
 
     Returns
     -------
-    DataFrame
+    Union[Series, DataFrame]
         _description_
     """
     # cehcking for values in crosstab
-    filtered_xtab = None
-    if xtab is not None:
+    filtered_xagg = None
+    if xagg is not None:
         # filtering out nans if requested from train crosstab
-        filtered_xtab = xtab.copy()
-        if str_nan in xtab.index:
-            filtered_xtab = xtab.drop(str_nan, axis=0)
+        filtered_xagg = xagg.copy()
+        if str_nan in xagg.index:
+            filtered_xagg = xagg.drop(str_nan, axis=0)
 
-    return filtered_xtab
+    return filtered_xagg
 
 
 def get_xtabs(
     features: list[str], X: DataFrame, y: Series, labels_orders: dict[str, GroupedList]
 ) -> dict[str, DataFrame]:
     """Computes crosstabs for specified features and ensures that the crosstab is ordered according to the known labels
 
@@ -543,14 +626,52 @@
 
             # storing results
             xtabs.update({feature: xtab})
 
     return xtabs
 
 
+def get_yvals(
+    features: list[str], X: DataFrame, y: Series, labels_orders: dict[str, GroupedList]
+) -> dict[str, DataFrame]:
+    """Computes y values for modalities of specified features and ensures the ordering according to the known labels
+
+    Parameters
+    ----------
+    features : list[str]
+        _description_
+    X : DataFrame
+        _description_
+    y : Series
+        _description_
+    labels_orders : dict[str, GroupedList]
+        _description_
+
+    Returns
+    -------
+    dict[str, DataFrame]
+        _description_
+    """
+    # checking for empty datasets
+    yvals = {feature: None for feature in features}
+    if X is not None:
+        # crosstab for each feature
+        for feature in features:
+            # computing crosstab with str_nan
+            yval = y.groupby(X[feature]).apply(lambda u: list(u))
+
+            # reordering according to known_order
+            yval = yval.reindex(labels_orders[feature])
+
+            # storing results
+            yvals.update({feature: yval})
+
+    return yvals
+
+
 def association_xtab(xtab: DataFrame, n_obs: int) -> dict[str, float]:
     """Computes measures of association between feature and target by crosstab.
 
     Parameters
     ----------
     xtab : DataFrame
         Crosstab between feature and target.
@@ -574,16 +695,39 @@
 
     # Tschuprow's T
     tschuprowt = cramerv / sqrt(sqrt(n_mod_x - 1))
 
     return {"cramerv": cramerv, "tschuprowt": tschuprowt}
 
 
-def vectorized_groupby_sum(xtab: DataFrame, groupby: list[str]) -> DataFrame:
-    """Groups a crosstab by groupby and sums column values by groups
+def association_yval(yval: Series, **kwargs) -> dict[str, float]:
+    """Computes measures of association between feature and quantitative target.
+
+    Parameters
+    ----------
+    yval : DataFrame
+        Values taken by y for each of x's modalities.
+
+    Returns
+    -------
+    dict[str, float]
+        Kruskal-Wallis' H as a dict.
+    """
+    # Kruskal-Wallis' H
+    return {"kruskal": kruskal(*tuple(yval.values))[0]}
+
+
+def yval_grouper(yval: Series, groupby: dict[str:str]) -> Series:
+    grouped_yval = yval.groupby(groupby).sum()
+
+    return grouped_yval
+
+
+def xtab_grouper(xtab: DataFrame, groupby: list[str]) -> DataFrame:
+    """Groups a crosstab by groupby and sums column values by groups (vectorized)
 
     Parameters
     ----------
     xtab : DataFrame
         _description_
     groupby : list[str]
         _description_
@@ -718,95 +862,110 @@
             next_index=next_index,
             all_combinations=all_combinations,
         )
 
     return all_combinations
 
 
+def xtab_combination_formatter(combination: list[list[str]]) -> list[str]:
+    formatted_combination = [
+        value for values in ([group[0]] * len(group) for group in combination) for value in values
+    ]
+
+    return formatted_combination
+
+
+def yval_combination_formatter(combination: list[list[str]]) -> dict[str, str]:
+    formatted_combination = {modal: group[0] for group in combination for modal in group}
+
+    return formatted_combination
+
+
 def get_best_association(
-    xtab: DataFrame,
+    xagg: Union[Series, DataFrame],
     combinations: list[list[str]],
     sort_by: str,
-    xtab_dev: DataFrame = None,
+    *,
+    xagg_dev: Union[Series, DataFrame] = None,
     verbose: bool = False,
+    grouper: Callable = xtab_grouper,
+    combination_formatter: Callable = xtab_combination_formatter,
+    association_measure: Callable = association_xtab,
+    target_rate: Callable = xtab_target_rate,
+    **kwargs,
 ) -> dict[str, Any]:
-    """Computes associations of the xtab for each combination
+    """Computes associations of the tab for each combination
 
     Parameters
     ----------
-    xtab : DataFrame
+    xagg : Union[Series, DataFrame]
         _description_
     combinations : list[list[str]]
         _description_
     sort_by : str
         _description_
-    xtab_dev : DataFrame, optional
+    xagg_dev : Union[Series, DataFrame], optional
         _description_, by default None
     verbose : bool, optional
         _description_, by default False
 
     Returns
     -------
     dict[str, Any]
         _description_
     """
-
     # values to groupby indices with
-    indices_to_groupby = [
-        [value for values in ([group[0]] * len(group) for group in combination) for value in values]
-        for combination in combinations
-    ]
+    indices_to_groupby = [combination_formatter(combination) for combination in combinations]
 
-    # grouping xtab by its indices
-    grouped_xtabs = [
-        vectorized_groupby_sum(xtab, index_to_groupby)
+    # grouping tab by its indices
+    grouped_xaggs = [
+        grouper(xagg, index_to_groupby)
         for index_to_groupby in tqdm(
             indices_to_groupby, disable=not verbose, desc="Grouping modalities   "
         )
     ]
 
-    # computing associations for each xtabs
-    n_obs = xtab.sum().sum()  # number of observation
-    n_mod_y = len(xtab.columns)  # number of modalities and minimum number of modalities
-    associations_xtab = [
-        association_xtab(grouped_xtab, n_obs)
-        for grouped_xtab in tqdm(grouped_xtabs, disable=not verbose, desc="Computing associations")
+    # computing associations for each tabs
+    n_obs = xagg.apply(sum).sum()  # number of observations for xtabs
+    associations_xagg = [
+        association_measure(grouped_xagg, n_obs=n_obs)
+        for grouped_xagg in tqdm(grouped_xaggs, disable=not verbose, desc="Computing associations")
     ]
 
     # adding corresponding combination to the association
-    for combination, index_to_groupby, association, grouped_xtab in zip(
-        combinations, indices_to_groupby, associations_xtab, grouped_xtabs
+    for combination, index_to_groupby, association, grouped_xagg in zip(
+        combinations, indices_to_groupby, associations_xagg, grouped_xaggs
     ):
         association.update(
-            {"combination": combination, "index_to_groupby": index_to_groupby, "xtab": grouped_xtab}
+            {"combination": combination, "index_to_groupby": index_to_groupby, "xagg": grouped_xagg}
         )
 
     # sorting associations according to specified metric
-    associations_xtab = (
-        DataFrame(associations_xtab).sort_values(sort_by, ascending=False).to_dict(orient="records")
+    associations_xagg = (
+        DataFrame(associations_xagg).sort_values(sort_by, ascending=False).to_dict(orient="records")
     )
 
     # case 0: no test sample provided -> not testing for robustness
-    if xtab_dev is None:
-        return associations_xtab[0]
+    if xagg_dev is None:
+        return associations_xagg[0]
 
     # case 1: testing viability on provided test sample
-    for association in tqdm(associations_xtab, disable=not verbose, desc="Testing robustness    "):
+    for association in tqdm(associations_xagg, disable=not verbose, desc="Testing robustness    "):
         # needed parameters
-        index_to_groupby, xtab = (
+        index_to_groupby, xagg = (
             association["index_to_groupby"],
-            association["xtab"],
+            association["xagg"],
         )
 
         # grouping rows of the test crosstab
-        grouped_xtab_dev = vectorized_groupby_sum(xtab_dev, index_to_groupby)
+        grouped_xagg_dev = grouper(xagg_dev, index_to_groupby)
 
         # computing target rate ranks per value
-        train_ranks = xtab_target_rate(xtab).index
-        test_ranks = xtab_target_rate(grouped_xtab_dev).index
+        train_ranks = target_rate(xagg).index
+        test_ranks = target_rate(grouped_xagg_dev).index
 
         # viable on test sample: grouped values have the same ranks in train/test
         if all(train_ranks == test_ranks):
             return association
 
 
 def add_nan_in_combinations(
@@ -871,37 +1030,37 @@
     order_copy = GroupedList(order)
     for combi in combination:
         order_copy.group_list(combi, combi[0])
 
     return order_copy
 
 
-def xtab_apply_order(xtab: DataFrame, order: GroupedList) -> DataFrame:
+def xagg_apply_order(xagg: DataFrame, order: GroupedList) -> DataFrame:
     """Applies an order (combination) to a crosstab
 
     Parameters
     ----------
-    xtab : DataFrame
+    xagg : DataFrame
         Crosstab
     order : GroupedList
         Combination of index to apply to the crosstab
 
     Returns
     -------
     dict[str, Any]
         Orderd crosstab.
     """
     # checking for input values
-    combi_xtab = None
-    if xtab is not None:
+    combi_xagg = None
+    if xagg is not None:
         # grouping modalities in the crosstab
-        groups = list(map(order.get_group, xtab.index))
-        combi_xtab = xtab.groupby(groups, dropna=False, sort=False).sum()
+        groups = list(map(order.get_group, xagg.index))
+        combi_xagg = xagg.groupby(groups, dropna=False, sort=False).sum()
 
-    return combi_xtab
+    return combi_xagg
 
 
 def load_carver(auto_carver_json: dict) -> BaseDiscretizer:
     """Allows one to load an AutoCarver saved as a .json file.
 
     The AutoCarver has to be saved with ``json.dump(f, AutoCarver.to_json())``, otherwise there
     can be no guarantee for it to be restored.
@@ -957,76 +1116,114 @@
 
         # rounding up stats
         stats = stats.round(3)
 
     return stats
 
 
-def prettier_xtab(
-    nice_xtab: DataFrame = None,
+def pretty_yval(yval: Series = None) -> DataFrame:
+    """Prints a continuous yval's statistics
+
+    Parameters
+    ----------
+    yval : Series
+        A series of values of y by modalities of x, by default None
+
+    Returns
+    -------
+    DataFrame
+        Target rate and frequency per modality
+    """
+    # checking for an xtab
+    stats = None
+    if yval is not None:
+        # target rate and frequency statistics per modality
+        stats = DataFrame(
+            {
+                # target rate per modality
+                "target_rate": yval.apply(mean),
+                # frequency per modality
+                "frequency": yval.apply(len) / yval.apply(len).sum(),
+            }
+        )
+
+        # rounding up stats
+        stats = stats.round(3)
+
+    return stats
+
+
+def prettier_xagg(
+    nice_xagg: DataFrame = None,
     caption: str = None,
 ) -> str:
     """Converts a crosstab to the HTML format, adding nice colors
 
     Parameters
     ----------
-    nice_xtab : DataFrame, optional
+    nice_xagg : DataFrame, optional
         Target rate and frequency per modality, by default None
     caption : str, optional
         Title of the HTML table, by default None
 
     Returns
     -------
     str
         HTML format of the crosstab
     """
     """Pretty display of frequency and target rate per modality on the same line."""
     # checking for a provided xtab
-    nicer_xtab = ""
-    if nice_xtab is not None:
+    nicer_xagg = ""
+    if nice_xagg is not None:
         # adding coolwarn color gradient
-        nicer_xtab = nice_xtab.style.background_gradient(cmap="coolwarm")
+        nicer_xagg = nice_xagg.style.background_gradient(cmap="coolwarm")
 
         # printing inline notebook
-        nicer_xtab = nicer_xtab.set_table_attributes("style='display:inline'")
+        nicer_xagg = nicer_xagg.set_table_attributes("style='display:inline'")
 
         # adding custom caption/title
         if caption is not None:
-            nicer_xtab = nicer_xtab.set_caption(caption)
+            nicer_xagg = nicer_xagg.set_caption(caption)
 
         # converting to html
-        nicer_xtab = nicer_xtab._repr_html_()
+        nicer_xagg = nicer_xagg._repr_html_()
 
-    return nicer_xtab
+    return nicer_xagg
 
 
-def print_xtabs(xtab: DataFrame, xtab_dev: DataFrame = None, pretty_print: bool = False) -> None:
+def print_xagg(
+    xagg: DataFrame,
+    printer: Callable,
+    xagg_dev: DataFrame = None,
+    pretty_print: bool = False,
+    **kwargs,
+) -> None:
     """Prints crosstabs' target rates and frequencies per modality, in raw or html format
 
     Parameters
     ----------
-    xtab : DataFrame
+    xagg : DataFrame
         Train crosstab
-    xtab_dev : DataFrame
+    xagg_dev : DataFrame
         Dev crosstab, by default None
     pretty_print : bool, optional
         Whether to output html or not, by default False
     """
     # getting pretty xtabs
-    nice_xtab = pretty_xtab(xtab)
-    nice_xtab_dev = pretty_xtab(xtab_dev)
+    nice_xagg = printer(xagg)
+    nice_xagg_dev = printer(xagg_dev)
 
     # case 0: no pretty hmtl printing
     if not pretty_print:
-        print(nice_xtab, "\n")
+        print(nice_xagg, "\n")
 
     # case 1: pretty html printing
     else:
         # getting prettier xtabs
-        nicer_xtab = prettier_xtab(nice_xtab, caption="X distribution")
-        nicer_xtab_dev = prettier_xtab(nice_xtab_dev, caption="X_dev distribution")
+        nicer_xagg = prettier_xagg(nice_xagg, caption="X distribution")
+        nicer_xagg_dev = prettier_xagg(nice_xagg_dev, caption="X_dev distribution")
 
         # merging outputs
-        nicer_xtabs = nicer_xtab + "    " + nicer_xtab_dev
+        nicer_xaggs = nicer_xagg + "    " + nicer_xagg_dev
 
         # displaying html of colored DataFrame
-        display_html(nicer_xtabs, raw=True)
+        display_html(nicer_xaggs, raw=True)
```

### Comparing `AutoCarver-5.1.9/AutoCarver/converters/converters.py` & `AutoCarver-5.2.0/AutoCarver/converters/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.9/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.2.0/AutoCarver/discretizers/discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.9/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.2.0/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,24 +211,14 @@
             ), f" - [BaseDiscretizer] Missing features from the provided DataFrame: {str(missing_columns)}"
 
             # copying X
             x_copy = X
             if self.copy:
                 x_copy = X.copy()
 
-        # checking for binary target
-        if y is not None:
-            y_values = unique(y)
-            assert (0 in y_values) & (
-                1 in y_values
-            ), " - [BaseDiscretizer] y must be a binary Series (int or float, not object)"
-            assert (
-                len(y_values) == 2
-            ), " - [BaseDiscretizer] y must be a binary Series (int or float, not object)"
-
         return x_copy
 
     def _check_new_values(self, X: DataFrame, features: list[str]) -> None:
         """Checks for new, unexpected values, in X
 
         Parameters
         ----------
```

### Comparing `AutoCarver-5.1.9/AutoCarver/discretizers/utils/grouped_list.py` & `AutoCarver-5.2.0/AutoCarver/discretizers/utils/grouped_list.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.9/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.2.0/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.9/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.2.0/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files 9% similar despite different names*

```diff
@@ -140,68 +140,68 @@
         _description_, by default None
 
     Returns
     -------
     list[float]
         _description_
     """
-    # initialisation de la taille total du dataframe
+    # getting dataset size
     if len_df is None:
         len_df = len(df_feature)
 
-    # initialisation de la liste des quantiles
+    # initiating liust of quantiles
     if quantiles is None:
         quantiles = []
 
-    # calcul du nombre d'occurences de chaque valeur
-    frequencies = (
-        df_feature.value_counts(dropna=False, normalize=False).drop(nan, errors="ignore") / len_df
-    )  # dropping nans to keep them anyways
-    values, frequencies = array(frequencies.index), array(frequencies.values)
-
     # case 1: no observation, all values have been attributed there corresponding modality
     if len(df_feature) == 0:
         return quantiles
 
     # case 2: there are missing values
     if any(isna(df_feature)):
         return find_quantiles(
             df_feature[notna(df_feature)],
             q,
             len_df=len_df,
             quantiles=quantiles,
         )
 
+    # frequencies per known value
+    frequencies = (
+        df_feature.value_counts(dropna=False, normalize=False).drop(nan, errors="ignore") / len_df
+    )
+    values, frequencies = array(frequencies.index), array(frequencies.values)
+
     # case 3 : there are no missing values
     # case 3.1 : there is an over-populated value
     if any(frequencies > 1 / q):
-        # identification de la valeur sur-représentée
+        # identifying over-represented modality
         frequent_value = values[frequencies.argmax()]
 
-        # ajout de la valeur fréquente à la liste des quantiles
+        # adding over-represented modality to the list of quantiles
         quantiles += [frequent_value]
 
-        # calcul des quantiles pour les parties inférieures et supérieures
+        # computing quantiles on smaller and greater values
         quantiles_inf = find_quantiles(df_feature[df_feature < frequent_value], q, len_df=len_df)
         quantiles_sup = find_quantiles(df_feature[df_feature > frequent_value], q, len_df=len_df)
 
         return quantiles_inf + quantiles + quantiles_sup
 
     # case 3.2 : there is no over-populated value
-    # nouveau nombre de quantile en prenant en compte les classes déjà constituées
+    # reducing the size of quantiles by frequencies of over-represented modalities
     new_q = max(round(len(df_feature) / len_df * q), 1)
 
-    # calcul des quantiles sur le dataframe
+    # cutting values into quantiles if there are enough of them
     if new_q > 1:
         quantiles += list(
             quantile(
                 df_feature.values,
                 linspace(0, 1, new_q + 1)[1:-1],
                 method="lower",
             )
         )
 
-    # case when there are no enough observations to compute quantiles
+    # not enough values observed, grouping all remaining values into a quantile
     else:
         quantiles += [max(df_feature.values)]
 
     return quantiles
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `AutoCarver-5.1.9/AutoCarver/discretizers/utils/serialization.py` & `AutoCarver-5.2.0/AutoCarver/discretizers/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.9/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.2.0/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.9/AutoCarver/feature_selection/feature_selector.py` & `AutoCarver-5.2.0/AutoCarver/feature_selection/feature_selector.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.9/AutoCarver/feature_selection/filters/qualitative_filters.py` & `AutoCarver-5.2.0/AutoCarver/feature_selection/filters/qualitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.9/AutoCarver/feature_selection/filters/quantitative_filters.py` & `AutoCarver-5.2.0/AutoCarver/feature_selection/filters/quantitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.9/AutoCarver/feature_selection/measures/base_measures.py` & `AutoCarver-5.2.0/AutoCarver/feature_selection/measures/base_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.9/AutoCarver/feature_selection/measures/qualitative_measures.py` & `AutoCarver-5.2.0/AutoCarver/feature_selection/measures/qualitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.9/AutoCarver/feature_selection/measures/quantitative_measures.py` & `AutoCarver-5.2.0/AutoCarver/feature_selection/measures/quantitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.9/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.2.0/AutoCarver.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.9
+Version: 5.2.0
 Summary: Automatic Discretization of Features with Optimal Target Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
@@ -31,36 +31,14 @@
 </p>
 
 
 # ReadTheDocs
 
 Go check out the brand new package documentation at [ReadTheDocs](https://autocarver.readthedocs.io/en/latest/index.html)!
 
-# AutoCarver
-
-**AutoCarver** is a powerful Python package designed to address the fundamental question of *What's the best processing for my model's features?*
-
-It offers an automated and optimized approach to processing and engineering your data, resulting in improved model performance, enhanced explainability, and reduced feature dimensionality.
-As of today, this set of tools is available for binary classification problems only.
-
-Key Features:
-
-1. **Data Processing and Engineering**: ``AutoCarver`` performs automatic bucketization and carving of a DataFrame's columns to maximize their correlation with a binary target variable. By leveraging advanced techniques, it optimizes the preprocessing steps for your data, leading to enhanced predictive accuracy.
-
-2. **Improved Model Explainability**: ``AutoCarver`` aids in understanding the relationship between the processed features and the target variable. By uncovering meaningful patterns and interactions, it provides valuable insights into the underlying data dynamics, enhancing the interpretability of your binary classification models.
-
-3. **Reduced Feature Dimensionality**: ``AutoCarver`` excels at reducing feature dimensionality, especially in scenarios involving one-hot encoding. It identifies and preserves only the most statistically relevant modalities, ensuring that your models focus on the most informative aspects of the data while eliminating noise and redundancy.
-
-4. **Statistical Accuracy and Relevance**: ``AutoCarver`` incorporates statistical techniques to ensure that the selected modalities have a sufficient number of observations, minimizing the risk of drawing conclusions based on insufficient data. This helps maintain the reliability and validity of your binary classification models.
-
-5. **Robustness Testing**: ``AutoCarver`` goes beyond feature processing by assessing the robustness of the selected modalities. It performs tests to evaluate the stability and consistency of the chosen features across different datasets or subsets, ensuring their reliability in various scenarios.
-
-``AutoCarver`` is a valuable tool for data scientists and practitioners involved in binary classification problems, such as credit scoring, fraud detection, and risk assessment. By leveraging its automated feature processing capabilities, you can unlock the full potential of your data, leading to more accurate predictions, improved model explainability, and better decision-making in your classification tasks.
-
-
 # Install
 
 **AutoCarver** can be installed from [PyPI](https://pypi.org/project/AutoCarver):
 
 ## Minimal install
 
 To install the base features (without vizualization tools), use the following:
@@ -72,7 +50,29 @@
 ## Unabling pretty printing
 
 To enable ``pretty_print`` features (nice colorful html tables in jupyter), use the following:
 
 <pre>
 pip install autocarver[jupyter]
 </pre>
+
+# AutoCarver
+
+**AutoCarver** is a powerful Python package designed to address the fundamental question of *What's the best processing for my model's features?*
+
+It offers an automated and optimized approach to processing and engineering your data, resulting in improved model performance, enhanced explainability, and reduced feature dimensionality.
+As of today, this set of tools is available for binary classification and regression problems only.
+
+Key Features:
+
+1. **Data Processing and Engineering**: **AutoCarver** performs automatic bucketization and carving of a DataFrame's columns to maximize their correlation with a target variable. By leveraging advanced techniques, it optimizes the preprocessing steps for your data, leading to enhanced predictive accuracy.
+
+2. **Improved Model Explainability**: **AutoCarver** aids in understanding the relationship between the processed features and the target variable. By uncovering meaningful patterns and interactions, it provides valuable insights into the underlying data dynamics, enhancing the interpretability of your models.
+
+3. **Reduced Feature Dimensionality**: **AutoCarver** excels at reducing feature dimensionality, especially in scenarios involving one-hot encoding. It identifies and preserves only the most statistically relevant modalities, ensuring that your models focus on the most informative aspects of the data while eliminating noise and redundancy.
+
+4. **Statistical Accuracy and Relevance**: **AutoCarver** incorporates statistical techniques to ensure that the selected modalities have a sufficient number of observations, minimizing the risk of drawing conclusions based on insufficient data. This helps maintain the reliability and validity of your models.
+
+5. **Robustness Testing**: **AutoCarver** goes beyond feature processing by assessing the robustness of the selected modalities. It performs tests to evaluate the stability and consistency of the chosen features across different datasets or subsets, ensuring their reliability in various scenarios.
+
+**AutoCarver** is a valuable tool for data scientists and practitioners involved in binary classification or regression problems, such as credit scoring, fraud detection, and risk assessment. By leveraging its automated feature processing capabilities, you can unlock the full potential of your data, leading to more accurate predictions, improved model explainability, and better decision-making in your classification tasks.
+
```

### Comparing `AutoCarver-5.1.9/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.2.0/AutoCarver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.9/LICENSE` & `AutoCarver-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.9/PKG-INFO` & `AutoCarver-5.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.9
+Version: 5.2.0
 Summary: Automatic Discretization of Features with Optimal Target Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
@@ -31,36 +31,14 @@
 </p>
 
 
 # ReadTheDocs
 
 Go check out the brand new package documentation at [ReadTheDocs](https://autocarver.readthedocs.io/en/latest/index.html)!
 
-# AutoCarver
-
-**AutoCarver** is a powerful Python package designed to address the fundamental question of *What's the best processing for my model's features?*
-
-It offers an automated and optimized approach to processing and engineering your data, resulting in improved model performance, enhanced explainability, and reduced feature dimensionality.
-As of today, this set of tools is available for binary classification problems only.
-
-Key Features:
-
-1. **Data Processing and Engineering**: ``AutoCarver`` performs automatic bucketization and carving of a DataFrame's columns to maximize their correlation with a binary target variable. By leveraging advanced techniques, it optimizes the preprocessing steps for your data, leading to enhanced predictive accuracy.
-
-2. **Improved Model Explainability**: ``AutoCarver`` aids in understanding the relationship between the processed features and the target variable. By uncovering meaningful patterns and interactions, it provides valuable insights into the underlying data dynamics, enhancing the interpretability of your binary classification models.
-
-3. **Reduced Feature Dimensionality**: ``AutoCarver`` excels at reducing feature dimensionality, especially in scenarios involving one-hot encoding. It identifies and preserves only the most statistically relevant modalities, ensuring that your models focus on the most informative aspects of the data while eliminating noise and redundancy.
-
-4. **Statistical Accuracy and Relevance**: ``AutoCarver`` incorporates statistical techniques to ensure that the selected modalities have a sufficient number of observations, minimizing the risk of drawing conclusions based on insufficient data. This helps maintain the reliability and validity of your binary classification models.
-
-5. **Robustness Testing**: ``AutoCarver`` goes beyond feature processing by assessing the robustness of the selected modalities. It performs tests to evaluate the stability and consistency of the chosen features across different datasets or subsets, ensuring their reliability in various scenarios.
-
-``AutoCarver`` is a valuable tool for data scientists and practitioners involved in binary classification problems, such as credit scoring, fraud detection, and risk assessment. By leveraging its automated feature processing capabilities, you can unlock the full potential of your data, leading to more accurate predictions, improved model explainability, and better decision-making in your classification tasks.
-
-
 # Install
 
 **AutoCarver** can be installed from [PyPI](https://pypi.org/project/AutoCarver):
 
 ## Minimal install
 
 To install the base features (without vizualization tools), use the following:
@@ -72,7 +50,29 @@
 ## Unabling pretty printing
 
 To enable ``pretty_print`` features (nice colorful html tables in jupyter), use the following:
 
 <pre>
 pip install autocarver[jupyter]
 </pre>
+
+# AutoCarver
+
+**AutoCarver** is a powerful Python package designed to address the fundamental question of *What's the best processing for my model's features?*
+
+It offers an automated and optimized approach to processing and engineering your data, resulting in improved model performance, enhanced explainability, and reduced feature dimensionality.
+As of today, this set of tools is available for binary classification and regression problems only.
+
+Key Features:
+
+1. **Data Processing and Engineering**: **AutoCarver** performs automatic bucketization and carving of a DataFrame's columns to maximize their correlation with a target variable. By leveraging advanced techniques, it optimizes the preprocessing steps for your data, leading to enhanced predictive accuracy.
+
+2. **Improved Model Explainability**: **AutoCarver** aids in understanding the relationship between the processed features and the target variable. By uncovering meaningful patterns and interactions, it provides valuable insights into the underlying data dynamics, enhancing the interpretability of your models.
+
+3. **Reduced Feature Dimensionality**: **AutoCarver** excels at reducing feature dimensionality, especially in scenarios involving one-hot encoding. It identifies and preserves only the most statistically relevant modalities, ensuring that your models focus on the most informative aspects of the data while eliminating noise and redundancy.
+
+4. **Statistical Accuracy and Relevance**: **AutoCarver** incorporates statistical techniques to ensure that the selected modalities have a sufficient number of observations, minimizing the risk of drawing conclusions based on insufficient data. This helps maintain the reliability and validity of your models.
+
+5. **Robustness Testing**: **AutoCarver** goes beyond feature processing by assessing the robustness of the selected modalities. It performs tests to evaluate the stability and consistency of the chosen features across different datasets or subsets, ensuring their reliability in various scenarios.
+
+**AutoCarver** is a valuable tool for data scientists and practitioners involved in binary classification or regression problems, such as credit scoring, fraud detection, and risk assessment. By leveraging its automated feature processing capabilities, you can unlock the full potential of your data, leading to more accurate predictions, improved model explainability, and better decision-making in your classification tasks.
+
```

### Comparing `AutoCarver-5.1.9/README.md` & `AutoCarver-5.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,36 +8,14 @@
 </p>
 
 
 # ReadTheDocs
 
 Go check out the brand new package documentation at [ReadTheDocs](https://autocarver.readthedocs.io/en/latest/index.html)!
 
-# AutoCarver
-
-**AutoCarver** is a powerful Python package designed to address the fundamental question of *What's the best processing for my model's features?*
-
-It offers an automated and optimized approach to processing and engineering your data, resulting in improved model performance, enhanced explainability, and reduced feature dimensionality.
-As of today, this set of tools is available for binary classification problems only.
-
-Key Features:
-
-1. **Data Processing and Engineering**: ``AutoCarver`` performs automatic bucketization and carving of a DataFrame's columns to maximize their correlation with a binary target variable. By leveraging advanced techniques, it optimizes the preprocessing steps for your data, leading to enhanced predictive accuracy.
-
-2. **Improved Model Explainability**: ``AutoCarver`` aids in understanding the relationship between the processed features and the target variable. By uncovering meaningful patterns and interactions, it provides valuable insights into the underlying data dynamics, enhancing the interpretability of your binary classification models.
-
-3. **Reduced Feature Dimensionality**: ``AutoCarver`` excels at reducing feature dimensionality, especially in scenarios involving one-hot encoding. It identifies and preserves only the most statistically relevant modalities, ensuring that your models focus on the most informative aspects of the data while eliminating noise and redundancy.
-
-4. **Statistical Accuracy and Relevance**: ``AutoCarver`` incorporates statistical techniques to ensure that the selected modalities have a sufficient number of observations, minimizing the risk of drawing conclusions based on insufficient data. This helps maintain the reliability and validity of your binary classification models.
-
-5. **Robustness Testing**: ``AutoCarver`` goes beyond feature processing by assessing the robustness of the selected modalities. It performs tests to evaluate the stability and consistency of the chosen features across different datasets or subsets, ensuring their reliability in various scenarios.
-
-``AutoCarver`` is a valuable tool for data scientists and practitioners involved in binary classification problems, such as credit scoring, fraud detection, and risk assessment. By leveraging its automated feature processing capabilities, you can unlock the full potential of your data, leading to more accurate predictions, improved model explainability, and better decision-making in your classification tasks.
-
-
 # Install
 
 **AutoCarver** can be installed from [PyPI](https://pypi.org/project/AutoCarver):
 
 ## Minimal install
 
 To install the base features (without vizualization tools), use the following:
@@ -49,7 +27,29 @@
 ## Unabling pretty printing
 
 To enable ``pretty_print`` features (nice colorful html tables in jupyter), use the following:
 
 <pre>
 pip install autocarver[jupyter]
 </pre>
+
+# AutoCarver
+
+**AutoCarver** is a powerful Python package designed to address the fundamental question of *What's the best processing for my model's features?*
+
+It offers an automated and optimized approach to processing and engineering your data, resulting in improved model performance, enhanced explainability, and reduced feature dimensionality.
+As of today, this set of tools is available for binary classification and regression problems only.
+
+Key Features:
+
+1. **Data Processing and Engineering**: **AutoCarver** performs automatic bucketization and carving of a DataFrame's columns to maximize their correlation with a target variable. By leveraging advanced techniques, it optimizes the preprocessing steps for your data, leading to enhanced predictive accuracy.
+
+2. **Improved Model Explainability**: **AutoCarver** aids in understanding the relationship between the processed features and the target variable. By uncovering meaningful patterns and interactions, it provides valuable insights into the underlying data dynamics, enhancing the interpretability of your models.
+
+3. **Reduced Feature Dimensionality**: **AutoCarver** excels at reducing feature dimensionality, especially in scenarios involving one-hot encoding. It identifies and preserves only the most statistically relevant modalities, ensuring that your models focus on the most informative aspects of the data while eliminating noise and redundancy.
+
+4. **Statistical Accuracy and Relevance**: **AutoCarver** incorporates statistical techniques to ensure that the selected modalities have a sufficient number of observations, minimizing the risk of drawing conclusions based on insufficient data. This helps maintain the reliability and validity of your models.
+
+5. **Robustness Testing**: **AutoCarver** goes beyond feature processing by assessing the robustness of the selected modalities. It performs tests to evaluate the stability and consistency of the chosen features across different datasets or subsets, ensuring their reliability in various scenarios.
+
+**AutoCarver** is a valuable tool for data scientists and practitioners involved in binary classification or regression problems, such as credit scoring, fraud detection, and risk assessment. By leveraging its automated feature processing capabilities, you can unlock the full potential of your data, leading to more accurate predictions, improved model explainability, and better decision-making in your classification tasks.
+
```

### Comparing `AutoCarver-5.1.9/setup.py` & `AutoCarver-5.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.1.9",
+    version="5.2.0",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Discretization of Features with Optimal Target Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
```

### Comparing `AutoCarver-5.1.9/tests/test_auto_carver.py` & `AutoCarver-5.2.0/tests/test_auto_carver.py`

 * *Files identical despite different names*

