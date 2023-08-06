# Comparing `tmp/hiveviewer-0.2.4.tar.gz` & `tmp/hiveviewer-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiveviewer-0.2.4.tar", last modified: Fri Aug  4 07:05:20 2023, max compression
+gzip compressed data, was "hiveviewer-0.2.5.tar", last modified: Sun Aug  6 23:27:39 2023, max compression
```

## Comparing `hiveviewer-0.2.4.tar` & `hiveviewer-0.2.5.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.525215 hiveviewer-0.2.4/
--rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.2.4/LICENSE
--rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-04 07:05:20.525065 hiveviewer-0.2.4/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.2.4/README.md
--rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.2.4/pyproject.toml
--rw-r--r--   0 yin        (501) staff       (20)       38 2023-08-04 07:05:20.525260 hiveviewer-0.2.4/setup.cfg
--rw-r--r--   0 yin        (501) staff       (20)     1006 2023-08-04 07:04:54.000000 hiveviewer-0.2.4/setup.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.518757 hiveviewer-0.2.4/src/
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.520251 hiveviewer-0.2.4/src/hiveviewer/
--rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.2.4/src/hiveviewer/__init__.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.521965 hiveviewer-0.2.4/src/hiveviewer/dataloader/
--rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.2.4/src/hiveviewer/dataloader/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     3200 2023-08-04 06:20:30.000000 hiveviewer-0.2.4/src/hiveviewer/dataloader/base.py
--rw-r--r--   0 yin        (501) staff       (20)      885 2023-08-03 06:08:42.000000 hiveviewer-0.2.4/src/hiveviewer/dataloader/load_csv.py
--rw-r--r--   0 yin        (501) staff       (20)      862 2023-08-03 06:10:38.000000 hiveviewer-0.2.4/src/hiveviewer/dataloader/load_excel.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.522414 hiveviewer-0.2.4/src/hiveviewer/evaluation/
--rw-r--r--   0 yin        (501) staff       (20)       61 2023-07-26 06:20:36.000000 hiveviewer-0.2.4/src/hiveviewer/evaluation/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     7803 2023-08-04 07:04:12.000000 hiveviewer-0.2.4/src/hiveviewer/evaluation/calculator.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.523051 hiveviewer-0.2.4/src/hiveviewer/optimization/
--rw-r--r--   0 yin        (501) staff       (20)      128 2023-08-01 02:03:43.000000 hiveviewer-0.2.4/src/hiveviewer/optimization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)      770 2023-08-02 03:43:12.000000 hiveviewer-0.2.4/src/hiveviewer/optimization/base.py
--rw-r--r--   0 yin        (501) staff       (20)     6703 2023-08-04 03:40:54.000000 hiveviewer-0.2.4/src/hiveviewer/optimization/multiple_objective.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.523797 hiveviewer-0.2.4/src/hiveviewer/sampling/
--rw-r--r--   0 yin        (501) staff       (20)      174 2023-07-31 02:06:26.000000 hiveviewer-0.2.4/src/hiveviewer/sampling/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     1068 2023-07-31 03:32:36.000000 hiveviewer-0.2.4/src/hiveviewer/sampling/base.py
--rw-r--r--   0 yin        (501) staff       (20)     1394 2023-08-04 06:40:00.000000 hiveviewer-0.2.4/src/hiveviewer/sampling/frequency_sampler.py
--rw-r--r--   0 yin        (501) staff       (20)     2510 2023-07-30 03:20:30.000000 hiveviewer-0.2.4/src/hiveviewer/sampling/gini_sampler.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.524812 hiveviewer-0.2.4/src/hiveviewer/visualization/
--rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.2.4/src/hiveviewer/visualization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.2.4/src/hiveviewer/visualization/lorenz_curve.py
--rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.2.4/src/hiveviewer/visualization/plot_trisurf.py
--rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.2.4/src/hiveviewer/visualization/venn2.py
--rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.2.4/src/hiveviewer/visualization/venn3.py
--rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.2.4/src/hiveviewer/visualization/venn_base.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.521138 hiveviewer-0.2.4/src/hiveviewer.egg-info/
--rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-04 07:05:20.000000 hiveviewer-0.2.4/src/hiveviewer.egg-info/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)     1013 2023-08-04 07:05:20.000000 hiveviewer-0.2.4/src/hiveviewer.egg-info/SOURCES.txt
--rw-r--r--   0 yin        (501) staff       (20)        1 2023-08-04 07:05:20.000000 hiveviewer-0.2.4/src/hiveviewer.egg-info/dependency_links.txt
--rw-r--r--   0 yin        (501) staff       (20)       82 2023-08-04 07:05:20.000000 hiveviewer-0.2.4/src/hiveviewer.egg-info/requires.txt
--rw-r--r--   0 yin        (501) staff       (20)       11 2023-08-04 07:05:20.000000 hiveviewer-0.2.4/src/hiveviewer.egg-info/top_level.txt
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-06 23:27:39.659930 hiveviewer-0.2.5/
+-rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.2.5/LICENSE
+-rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-06 23:27:39.659778 hiveviewer-0.2.5/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.2.5/README.md
+-rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.2.5/pyproject.toml
+-rw-r--r--   0 yin        (501) staff       (20)       38 2023-08-06 23:27:39.659981 hiveviewer-0.2.5/setup.cfg
+-rw-r--r--   0 yin        (501) staff       (20)     1006 2023-08-06 23:26:53.000000 hiveviewer-0.2.5/setup.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-06 23:27:39.649952 hiveviewer-0.2.5/src/
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-06 23:27:39.651436 hiveviewer-0.2.5/src/hiveviewer/
+-rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.2.5/src/hiveviewer/__init__.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-06 23:27:39.653907 hiveviewer-0.2.5/src/hiveviewer/dataloader/
+-rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.2.5/src/hiveviewer/dataloader/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     3200 2023-08-04 06:20:30.000000 hiveviewer-0.2.5/src/hiveviewer/dataloader/base.py
+-rw-r--r--   0 yin        (501) staff       (20)      885 2023-08-03 06:08:42.000000 hiveviewer-0.2.5/src/hiveviewer/dataloader/load_csv.py
+-rw-r--r--   0 yin        (501) staff       (20)      862 2023-08-03 06:10:38.000000 hiveviewer-0.2.5/src/hiveviewer/dataloader/load_excel.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-06 23:27:39.654513 hiveviewer-0.2.5/src/hiveviewer/evaluation/
+-rw-r--r--   0 yin        (501) staff       (20)       61 2023-07-26 06:20:36.000000 hiveviewer-0.2.5/src/hiveviewer/evaluation/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     7811 2023-08-05 03:12:03.000000 hiveviewer-0.2.5/src/hiveviewer/evaluation/calculator.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-06 23:27:39.655465 hiveviewer-0.2.5/src/hiveviewer/optimization/
+-rw-r--r--   0 yin        (501) staff       (20)      132 2023-08-05 00:45:59.000000 hiveviewer-0.2.5/src/hiveviewer/optimization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)      770 2023-08-02 03:43:12.000000 hiveviewer-0.2.5/src/hiveviewer/optimization/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     6859 2023-08-05 04:42:43.000000 hiveviewer-0.2.5/src/hiveviewer/optimization/multiple_objective.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-06 23:27:39.656657 hiveviewer-0.2.5/src/hiveviewer/sampling/
+-rw-r--r--   0 yin        (501) staff       (20)      174 2023-07-31 02:06:26.000000 hiveviewer-0.2.5/src/hiveviewer/sampling/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     1068 2023-07-31 03:32:36.000000 hiveviewer-0.2.5/src/hiveviewer/sampling/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     1394 2023-08-05 00:52:33.000000 hiveviewer-0.2.5/src/hiveviewer/sampling/frequency_sampler.py
+-rw-r--r--   0 yin        (501) staff       (20)     2510 2023-07-30 03:20:30.000000 hiveviewer-0.2.5/src/hiveviewer/sampling/gini_sampler.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-06 23:27:39.659400 hiveviewer-0.2.5/src/hiveviewer/visualization/
+-rw-r--r--   0 yin        (501) staff       (20)      368 2023-08-05 03:12:02.000000 hiveviewer-0.2.5/src/hiveviewer/visualization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.2.5/src/hiveviewer/visualization/lorenz_curve.py
+-rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.2.5/src/hiveviewer/visualization/plot_trisurf.py
+-rw-r--r--   0 yin        (501) staff       (20)     3654 2023-08-05 04:40:56.000000 hiveviewer-0.2.5/src/hiveviewer/visualization/profolio_curve.py
+-rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.2.5/src/hiveviewer/visualization/venn2.py
+-rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.2.5/src/hiveviewer/visualization/venn3.py
+-rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.2.5/src/hiveviewer/visualization/venn_base.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-06 23:27:39.652733 hiveviewer-0.2.5/src/hiveviewer.egg-info/
+-rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-06 23:27:39.000000 hiveviewer-0.2.5/src/hiveviewer.egg-info/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)     1060 2023-08-06 23:27:39.000000 hiveviewer-0.2.5/src/hiveviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yin        (501) staff       (20)        1 2023-08-06 23:27:39.000000 hiveviewer-0.2.5/src/hiveviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yin        (501) staff       (20)       82 2023-08-06 23:27:39.000000 hiveviewer-0.2.5/src/hiveviewer.egg-info/requires.txt
+-rw-r--r--   0 yin        (501) staff       (20)       11 2023-08-06 23:27:39.000000 hiveviewer-0.2.5/src/hiveviewer.egg-info/top_level.txt
```

### Comparing `hiveviewer-0.2.4/LICENSE` & `hiveviewer-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.4/PKG-INFO` & `hiveviewer-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.2.4
+Version: 0.2.5
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hiveviewer-0.2.4/README.md` & `hiveviewer-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.4/setup.py` & `hiveviewer-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "openpyxl",
         "optuna",
     ],
 )
 
 setup(
     name="hiveviewer",
-    version="0.2.4",
+    version="0.2.5",
     author="Yin Cheng",
     author_email="yin.sjtu@gmail.com",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/yinsn/hiveviewer",
     python_requires=">=3.6",
     description="Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.",
```

### Comparing `hiveviewer-0.2.4/src/hiveviewer/dataloader/base.py` & `hiveviewer-0.2.5/src/hiveviewer/dataloader/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.4/src/hiveviewer/dataloader/load_csv.py` & `hiveviewer-0.2.5/src/hiveviewer/dataloader/load_csv.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.4/src/hiveviewer/dataloader/load_excel.py` & `hiveviewer-0.2.5/src/hiveviewer/dataloader/load_excel.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.4/src/hiveviewer/evaluation/calculator.py` & `hiveviewer-0.2.5/src/hiveviewer/evaluation/calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import List, Optional, Tuple
 
 import numpy as np
 import pandas as pd
 from sklearn.metrics import roc_auc_score
 from tqdm import tqdm
 
-from ..sampling.frequency_sampler import FrequencySampler
-
 
 class Calculator:
     """Calculator class for calculating various metrics."""
 
     def __init__(
         self,
         df: pd.DataFrame,
@@ -111,14 +109,16 @@
         score_column: str,
         slice_from: Optional[float] = None,
         slice_to: Optional[float] = None,
         log_scale: Optional[bool] = True,
         laplace_smoothing: Optional[bool] = True,
     ) -> None:
         """Initialize frequency sampler."""
+        from ..sampling.frequency_sampler import FrequencySampler
+
         self.sampler = FrequencySampler(
             sample_size=sample_size,
             data=self.df[score_column],
             slice_from=slice_from,
             slice_to=slice_to,
             log_scale=log_scale,
             laplace_smoothing=laplace_smoothing,
```

### Comparing `hiveviewer-0.2.4/src/hiveviewer/optimization/base.py` & `hiveviewer-0.2.5/src/hiveviewer/optimization/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.4/src/hiveviewer/optimization/multiple_objective.py` & `hiveviewer-0.2.5/src/hiveviewer/optimization/multiple_objective.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,19 @@
         self.first_order_lower_bound = first_order_lower_bound
         self.first_order_upper_bound = first_order_upper_bound
         self.dirichlet = dirichlet
         if log_file:
             self.build_logger(log_file)
 
     def build_logger(self, log_file: str) -> None:
-        """Build logger to log the results of each trial."""
+        """Build logger for optuna.
+
+        Args:
+            log_file (str): log file path.
+        """
         file_handler = logging.FileHandler(log_file)
         file_handler.setLevel(logging.INFO)
         self.logger = optuna.logging.get_logger("optuna")
         self.logger.addHandler(file_handler)
 
     def add_calculator(
         self,
@@ -65,15 +69,15 @@
         hyperparameter: Optional[float] = None,
         groupby: Optional[str] = None,
     ) -> None:
         """Add calculators to the objective.
 
         Args:
             calculator (Calculator): calculator building blocks.
-            flag (str ["wuauc", "profolio", "logmse"]): type of calculation.
+            flag (str ["wuauc", "profolio", "logmse", ..., ect.]): type of calculator.
             target_column (str): target column to calculate.
         """
         self.calculators.append(calculator)
         self.calculator_flags.append(flag)
         self.target_columns.append(target_column)
         if hyperparameter is not None:
             self.hyperparameters.append(hyperparameter)
@@ -84,16 +88,21 @@
         else:
             self.groupbys.append(None)
 
     def objective(
         self,
         trial: Trial,
     ) -> float:
-        """
-        Calculate the objective value.
+        """Objective function for optuna.
+
+        Args:
+            trial (Trial): optuna trial.
+
+        Returns:
+            float: objective value.
         """
         power_weights: List[float] = []
         first_order_weights: List[float] = []
 
         if self.power:
             if self.dirichlet:
                 for i in range(self.weights_num - 1):
```

### Comparing `hiveviewer-0.2.4/src/hiveviewer/sampling/base.py` & `hiveviewer-0.2.5/src/hiveviewer/sampling/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.4/src/hiveviewer/sampling/frequency_sampler.py` & `hiveviewer-0.2.5/src/hiveviewer/sampling/frequency_sampler.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.4/src/hiveviewer/sampling/gini_sampler.py` & `hiveviewer-0.2.5/src/hiveviewer/sampling/gini_sampler.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.4/src/hiveviewer/visualization/lorenz_curve.py` & `hiveviewer-0.2.5/src/hiveviewer/visualization/lorenz_curve.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.4/src/hiveviewer/visualization/plot_trisurf.py` & `hiveviewer-0.2.5/src/hiveviewer/visualization/plot_trisurf.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.4/src/hiveviewer/visualization/venn2.py` & `hiveviewer-0.2.5/src/hiveviewer/visualization/venn2.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.4/src/hiveviewer/visualization/venn3.py` & `hiveviewer-0.2.5/src/hiveviewer/visualization/venn3.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.4/src/hiveviewer/visualization/venn_base.py` & `hiveviewer-0.2.5/src/hiveviewer/visualization/venn_base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.4/src/hiveviewer.egg-info/PKG-INFO` & `hiveviewer-0.2.5/src/hiveviewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.2.4
+Version: 0.2.5
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hiveviewer-0.2.4/src/hiveviewer.egg-info/SOURCES.txt` & `hiveviewer-0.2.5/src/hiveviewer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,10 +20,11 @@
 src/hiveviewer/sampling/__init__.py
 src/hiveviewer/sampling/base.py
 src/hiveviewer/sampling/frequency_sampler.py
 src/hiveviewer/sampling/gini_sampler.py
 src/hiveviewer/visualization/__init__.py
 src/hiveviewer/visualization/lorenz_curve.py
 src/hiveviewer/visualization/plot_trisurf.py
+src/hiveviewer/visualization/profolio_curve.py
 src/hiveviewer/visualization/venn2.py
 src/hiveviewer/visualization/venn3.py
 src/hiveviewer/visualization/venn_base.py
```

