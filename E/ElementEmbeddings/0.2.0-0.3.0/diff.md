# Comparing `tmp/ElementEmbeddings-0.2.0.tar.gz` & `tmp/ElementEmbeddings-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElementEmbeddings-0.2.0.tar", last modified: Fri Jul  7 16:35:27 2023, max compression
+gzip compressed data, was "ElementEmbeddings-0.3.0.tar", last modified: Mon Aug  7 07:59:54 2023, max compression
```

## Comparing `ElementEmbeddings-0.2.0.tar` & `ElementEmbeddings-0.3.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.996227 ElementEmbeddings-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-07 16:35:26.996227 ElementEmbeddings-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 16:35:26.996227 ElementEmbeddings-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.988227 ElementEmbeddings-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.992227 ElementEmbeddings-0.2.0/src/ElementEmbeddings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-07 16:35:26.000000 ElementEmbeddings-0.2.0/src/ElementEmbeddings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-07 16:35:26.000000 ElementEmbeddings-0.2.0/src/ElementEmbeddings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:35:26.000000 ElementEmbeddings-0.2.0/src/ElementEmbeddings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-07 16:35:26.000000 ElementEmbeddings-0.2.0/src/ElementEmbeddings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 16:35:26.000000 ElementEmbeddings-0.2.0/src/ElementEmbeddings.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.992227 ElementEmbeddings-0.2.0/src/elementembeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)    33496 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.996227 ElementEmbeddings-0.2.0/src/elementembeddings/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.996227 ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/element_group.json
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/element_symbols.json
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/ordered_periodic.txt
--rw-r--r--   0 runner    (1001) docker     (123)   199959 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/periodic-table-lookup-symbols.json
--rw-r--r--   0 runner    (1001) docker     (123)   259692 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/periodic-table-lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/magpie.csv
--rw-r--r--   0 runner    (1001) docker     (123)    44406 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/magpie_sc.json
--rw-r--r--   0 runner    (1001) docker     (123)   476891 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/mat2vec.csv
--rw-r--r--   0 runner    (1001) docker     (123)   449163 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/matscholar-embedding.json
--rw-r--r--   0 runner    (1001) docker     (123)    32012 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/megnet16.json
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/mod_petti.json
--rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/oliynyk.json
--rw-r--r--   0 runner    (1001) docker     (123)    77531 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/oliynyk_sc.json
--rw-r--r--   0 runner    (1001) docker     (123)   487394 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/random_200.csv
--rw-r--r--   0 runner    (1001) docker     (123)   488226 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/random_200_new.csv
--rw-r--r--   0 runner    (1001) docker     (123)   356292 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/skipatom_20201009_induced.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.996227 ElementEmbeddings-0.2.0/src/elementembeddings/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/tests/test_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/tests/test_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.996227 ElementEmbeddings-0.2.0/src/elementembeddings/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/utils/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:59:54.919901 ElementEmbeddings-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-08-07 07:59:54.919901 ElementEmbeddings-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 07:59:54.919901 ElementEmbeddings-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:59:54.907900 ElementEmbeddings-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:59:54.911901 ElementEmbeddings-0.3.0/src/ElementEmbeddings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-08-07 07:59:54.000000 ElementEmbeddings-0.3.0/src/ElementEmbeddings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-07 07:59:54.000000 ElementEmbeddings-0.3.0/src/ElementEmbeddings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 07:59:54.000000 ElementEmbeddings-0.3.0/src/ElementEmbeddings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-07 07:59:54.000000 ElementEmbeddings-0.3.0/src/ElementEmbeddings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 07:59:54.000000 ElementEmbeddings-0.3.0/src/ElementEmbeddings.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:59:54.911901 ElementEmbeddings-0.3.0/src/elementembeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30857 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:59:54.907900 ElementEmbeddings-0.3.0/src/elementembeddings/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:59:54.911901 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_data/element_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_data/element_symbols.json
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_data/ordered_periodic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   199959 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_data/periodic-table-lookup-symbols.json
+-rw-r--r--   0 runner    (1001) docker     (123)   259692 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_data/periodic-table-lookup.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:59:54.915901 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/atomic.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/magpie.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    44406 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/magpie_sc.json
+-rw-r--r--   0 runner    (1001) docker     (123)   476891 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/mat2vec.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   449163 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/matscholar-embedding.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32012 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/megnet16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/mod_petti.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15299 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/oliynyk.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    77531 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/oliynyk_sc.json
+-rw-r--r--   0 runner    (1001) docker     (123)   487394 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/random_200.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   488226 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/random_200_new.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   356292 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/skipatom_20201009_induced.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:59:54.919901 ElementEmbeddings-0.3.0/src/elementembeddings/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/tests/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/tests/test_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:59:54.919901 ElementEmbeddings-0.3.0/src/elementembeddings/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-07 07:59:39.000000 ElementEmbeddings-0.3.0/src/elementembeddings/utils/math.py
```

### Comparing `ElementEmbeddings-0.2.0/LICENSE.md` & `ElementEmbeddings-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/setup.py` & `ElementEmbeddings-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup script for AtomicEmbeddings."""
 import os
 
 from setuptools import find_namespace_packages, setup
 
 module_dir = os.path.dirname(os.path.abspath(__file__))
 
-VERSION = "0.2.0"
+VERSION = "0.3.0"
 DESCRIPTION = "Element Embeddings"
 with open(os.path.join(module_dir, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 
 # Setting up
 setup(
@@ -19,46 +19,47 @@
     author_email="anthony.onwuli16@imperial.ac.uk",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     package_data={
-        "elementembeddings.data": ["*.json", "*.csv"],
+        "elementembeddings.data.element_representations": ["*.json", "*.csv"],
         "elementembeddings.data.element_data": ["*.json", "*.txt"],
     },
     test_suite="elementembeddings.tests.test",
     install_requires=[
         "numpy==1.23.3",
         "scipy==1.10.1",
         "pymatgen>2022.9.21",
-        "seaborn==0.12.1",
+        "seaborn==0.12.2",
         "matplotlib==3.7.1",
         "scikit-learn==1.3.0",
         "umap-learn==0.5.3",
         "adjustText==0.8",
     ],
     extras_require={
         "dev": [
-            "pre-commit==2.20.0",
+            "pre-commit==3.3.3",
             "black==23.3.0",
             "isort==5.12.0",
             "pytest==7.2.1",
             "pytest-subtests==0.10.0",
             "nbqa==1.5.3",
             "pyupgrade==3.3.1",
             "flake8==6.0.0",
-            "autopep8==2.0.1",
+            "autopep8==2.0.2",
             "pytest-cov==4.1.0",
         ],
         "docs": [
             "mkdocs==1.4.3",
             "mkdocs-material==9.1.17",
             "mkdocstrings ==0.21.2",
-            "mkdocstrings-python == 1.0.0",
+            "mkdocstrings-python == 1.2.1",
+            "mike ==1.1.2",
         ],
     },
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/composition.py` & `ElementEmbeddings-0.3.0/src/elementembeddings/composition.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 This module provides a class for handling compositional embeddings.
 
 Typical usage example:
     Fe2O3_magpie = CompositionalEmbedding("Fe2O3", "magpie")
 """
 import collections
 import re
-from typing import Dict, Union
+from typing import Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
+from scipy.stats import energy_distance, wasserstein_distance
+from sklearn.metrics import DistanceMetric
 from tqdm import tqdm
 
 from .core import Embedding
+from .utils.math import cosine_distance
 
 tqdm.pandas()
 # Modified from pymatgen.core.Compositions
 
 
 def formula_parser(formula: str) -> Dict[str, float]:
     # TO-DO: Add validation to check composition contains real elements.
@@ -208,15 +211,15 @@
         "maxpool": "_maxpool_feature_vector",
         "range": "_range_feature_vector",
         "sum": "_sum_feature_vector",
         "geometric_mean": "_geometric_mean_feature_vector",
         "harmonic_mean": "_harmonic_mean_feature_vector",
     }
 
-    def feature_vector(self, stats: Union[str, list] = ["mean"]):
+    def feature_vector(self, stats: Union[str, list] = "mean"):
         """
         Compute a feature vector.
 
         The feature vector is a concatenation of
         the statistics specified in the stats argument.
 
         Args:
@@ -248,43 +251,115 @@
                 "are not valid statistics."
             )
         feature_vector = []
         for s in stats:
             feature_vector.append(getattr(self, self._stats_functions_dict[s])())
         return np.concatenate(feature_vector)
 
+    def distance(
+        self,
+        comp_other,
+        distance_metric: str = "euclidean",
+        stats: Union[str, List[str]] = "mean",
+    ):
+        """
+        Compute the distance between two compositions.
+
+        Args:
+            comp_other (Union[str, CompositionalEmbedding]): The other composition.
+            distance_metric (str): The metric to be used. The default is 'euclidean'.
+
+        Returns:
+            float: The distance between the two CompositionalEmbedding objects.
+        """
+        if isinstance(comp_other, str):
+            comp_other = CompositionalEmbedding(comp_other, self.embedding)
+        if not isinstance(comp_other, CompositionalEmbedding):
+            raise ValueError(
+                "comp_other must be a string or a CompositionalEmbedding object."
+            )
+        if self.embedding_name != comp_other.embedding_name:
+            raise ValueError(
+                "The two CompositionalEmbedding objects must have the same embedding."
+            )
+        return _composition_distance(
+            self, comp_other, self.embedding, distance_metric, stats
+        )
+
     def __repr__(self):
         return (
             f"CompositionalEmbedding(formula={self.formula}, "
-            f"embedding={self.embedding})"
+            f"embedding={self.embedding_name})"
         )
 
     def __str__(self):
         return (
             f"CompositionalEmbedding(formula={self.formula}, "
-            f"embedding={self.embedding})"
+            f"embedding={self.embedding_name})"
         )
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
-            return self.formula == other.formula and self.embedding == other.embedding
+            return (
+                self.formula == other.formula
+                and self.embedding_name == other.embedding_name
+            )
         else:
             return False
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __hash__(self):
         return hash((self.formula, self.embedding))
 
 
+def _composition_distance(
+    comp1: Union[str, CompositionalEmbedding],
+    comp2: Union[str, CompositionalEmbedding],
+    embedding: Optional[Union[str, Embedding]] = None,
+    distance_metric: str = "euclidean",
+    stats: Union[str, List[str]] = "mean",
+) -> float:
+    """Compute the distance between two compositions."""
+    if not isinstance(comp1, CompositionalEmbedding):
+        comp1 = CompositionalEmbedding(comp1, embedding=embedding)
+    if not isinstance(comp2, CompositionalEmbedding):
+        comp2 = CompositionalEmbedding(comp2, embedding=embedding)
+    assert comp1.embedding_name == comp2.embedding_name
+
+    comp1_vec = comp1.feature_vector(stats=stats)
+    comp2_vec = comp2.feature_vector(stats=stats)
+
+    scikit_metrics = ["euclidean", "manhattan", "chebyshev"]
+
+    scipy_metrics = {"wasserstein": wasserstein_distance, "energy": energy_distance}
+
+    # valid_metrics = scikit_metrics + list(scipy_metrics.keys()) + ["cosine"]
+
+    if distance_metric in scikit_metrics:
+        distance = DistanceMetric.get_metric(distance_metric)
+
+        return distance.pairwise(
+            comp1_vec.reshape(1, -1),
+            comp2_vec.reshape(1, -1),
+        )[
+            0
+        ][0]
+
+    elif distance_metric in scipy_metrics.keys():
+        return scipy_metrics[distance_metric](comp1_vec, comp2_vec)
+    elif distance_metric == "cosine_distance":
+        return cosine_distance(comp1_vec, comp2_vec)
+
+
 def composition_featuriser(
     data: Union[pd.DataFrame, pd.Series, CompositionalEmbedding, list],
     embedding: Union[Embedding, str] = "magpie",
-    stats: Union[str, list] = ["mean"],
+    stats: Union[str, list] = "mean",
     inplace: bool = False,
 ) -> pd.DataFrame:
     """
     Compute a feature vector for a composition.
 
     The feature vector is based on the statistics specified
     in the stats argument.
@@ -299,40 +374,38 @@
         inplace (bool, optional): Whether to perform the operation in place on the data.
         The default is False.
 
     Returns:
         Union[pd.DataFrame,list]: A pandas DataFrame containing the feature vector,
         or a list of feature vectors is returned
     """
+    if isinstance(stats, str):
+        stats = [stats]
+    if isinstance(data, pd.Series):
+        data = data.to_frame(name="formula")
     if isinstance(data, pd.DataFrame):
         if not inplace:
             data = data.copy()
         if "formula" not in data.columns:
             raise ValueError(
                 "The data must contain a column named 'formula' to featurise."
             )
-        data["composition"] = data["formula"].progress_apply(
-            lambda x: CompositionalEmbedding(x, embedding)
-        )
-        data["feature_vector"] = data["composition"].progress_apply(
-            lambda x: x.feature_vector(stats)
-        )
-        data.drop("composition", axis=1, inplace=True)
-        return data
-    elif isinstance(data, pd.Series):
-        if not inplace:
-            data = data.copy()
-        data["composition"] = data["formula"].progress_apply(
-            lambda x: CompositionalEmbedding(x, embedding)
-        )
-        data["feature_vector"] = data["composition"].progress_apply(
-            lambda x: x.feature_vector(stats)
-        )
-        data.drop("composition", axis=1, inplace=True)
-        return data
+        print("Featurising compositions...")
+        comps = [
+            CompositionalEmbedding(x, embedding) for x in tqdm(data["formula"].tolist())
+        ]
+        print("Computing feature vectors...")
+        fvs = [x.feature_vector(stats) for x in tqdm(comps)]
+        feature_names = comps[0].embedding.feature_labels
+        feature_names = [
+            f"{stat}_{feature}" for stat in stats for feature in feature_names
+        ]
+        data_new = pd.concat([data, pd.DataFrame(fvs, columns=feature_names)], axis=1)
+        # data.columns = []
+        return data_new
     elif isinstance(data, list):
         comps = [CompositionalEmbedding(x, embedding) for x in data]
         return [x.feature_vector(stats) for x in tqdm(comps)]
 
     elif isinstance(data, CompositionalEmbedding):
         return data.feature_vector(stats)
     else:
```

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/core.py` & `ElementEmbeddings-0.3.0/src/elementembeddings/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,18 @@
 
 import fnmatch
 import json
 import random
 import warnings
 from itertools import combinations_with_replacement
 from os import path
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Union
 
-import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import seaborn as sns
-from numpy.linalg import norm
 from pymatgen.core import Element
 from scipy.stats import energy_distance, pearsonr, spearmanr, wasserstein_distance
 from sklearn import decomposition
 from sklearn.manifold import TSNE
 from sklearn.metrics import DistanceMetric
 from sklearn.preprocessing import StandardScaler
 from umap import UMAP
@@ -46,38 +43,84 @@
     To load an embedding distributed from the package use the load_data() method.
 
     Works like a standard python dictionary. The keys are {element: vector} pairs.
 
     Adds a few convenience methods related to elemental representations.
     """
 
-    def __init__(self, embeddings: dict, embedding_name: Optional[str] = None):
+    def __init__(
+        self,
+        embeddings: dict,
+        embedding_name: Optional[str] = None,
+        feature_labels: Optional[List[str]] = None,
+    ):
         """Initialise the Embedding class.
 
         Args:
             embeddings (dict): A {element_symbol: vector} dictionary
             embedding_name (str): The name of the elemental representation
+            feature_labels (list(str)): A list of feature labels
         """
         self.embeddings = embeddings
         self.embedding_name = embedding_name
+        self.feature_labels = feature_labels
+        if not self._is_standardised():
+            warnings.warn(
+                "Embedding is not standardised. "
+                "It is recommended that you standardise your embeddings before use. "
+                "Use the standardise() method to standardise your embeddings."
+            )
+            self.is_standardised = False
+        else:
+            self.is_standardised = True
 
         # Grab a random value from the embedding vector
         _rand_embed = random.choice(list(self.embeddings.values()))
         # Convert embeddings to numpy array if not already a numpy array
         if not isinstance(_rand_embed, np.ndarray):
             self.embeddings = {
                 ele: np.array(self.embeddings[ele]) for ele in self.embeddings
             }
+
         # Determines if the embedding vector has a length attribute
         # (i.e. is not a scalar int or float)
-        # If the 'vector' is a scalar/float, the representation is linear (dim=1)
+        # If the 'vector' is a scalar/float, the representation is linear
+        # A linear representation gets converted to a one-hot vector
         if hasattr(_rand_embed, "__len__") and (not isinstance(_rand_embed, str)):
+            self.embedding_type: str = "vector"
             self.dim: int = len(random.choice(list(self.embeddings.values())))
         else:
-            self.dim: int = int(1)
+            self.embedding_type: str = "linear"
+
+        # Create one-hot vectors for a scalar representation
+        if self.embedding_type == "linear":
+            sorted_embedding = sorted(self.embeddings.items(), key=lambda x: x[1])
+            elements = np.loadtxt(
+                f"{data_directory}/element_data/ordered_periodic.txt", dtype=str
+            )
+            if self.embedding_name == "mod_petti":
+                sorted_embedding = {
+                    el: num for el, num in sorted_embedding if el in elements[:103]
+                }
+            else:
+                sorted_embedding = {
+                    el: num for el, num in sorted_embedding if el in elements[:118]
+                }
+            self.feature_labels = list(sorted_embedding.keys())
+            self.embeddings = {}
+
+            for el, num in sorted_embedding.items():
+                self.embeddings[el] = np.zeros(len(sorted_embedding))
+                self.embeddings[el][num] = 1
+            self.dim = len(random.choice(list(self.embeddings.values())))
+
+        if not self.feature_labels:
+            self.feature_labels = list(range(self.dim))
+        else:
+            self.feature_labels = self.feature_labels
 
         # Dummy initialisation for results
         self._data = []
         self._pca_data = None  # type: Optional[np.ndarray]
         self._tsne_data = None  # type: Optional[np.ndarray]
         self._umap_data = None  # type: Optional[np.ndarray]
 
@@ -96,14 +139,15 @@
         | Matscholar              | matscholar   |
         | Megnet (16 dimensions)  | megnet16     |
         | Modified pettifor scale | mod_petti    |
         | Oliynyk                 | oliynyk      |
         | Oliynyk (scaled)        | oliynyk_sc   |
         | Random (200 dimensions) | random_200   |
         | SkipAtom                | skipatom     |
+        | Atomic Number           | atomic       |
 
 
         Args:
             embedding_name (str): The str_name of an embedding file.
 
         Returns:
             Embedding :class:`Embedding` instance.
@@ -111,110 +155,105 @@
         _cbfv_files = {
             "magpie": "magpie.csv",
             "magpie_sc": "magpie_sc.json",
             "mat2vec": "mat2vec.csv",
             "matscholar": "matscholar-embedding.json",
             "megnet16": "megnet16.json",
             "mod_petti": "mod_petti.json",
-            "oliynyk": "oliynyk.json",
+            "oliynyk": "oliynyk.csv",
             "oliynyk_sc": "oliynyk_sc.json",
             "random_200": "random_200_new.csv",
             "skipatom": "skipatom_20201009_induced.csv",
+            "atomic": "atomic.json",
         }
-        _cbfv_names = list(_cbfv_files.keys())
-        _cbfv_names_others = [
-            i
-            for i in _cbfv_names
-            if i not in ["skipatom", "random_200", "megnet16", "magpie", "mat2vec"]
-        ]
-
-        # Get the embeddings
-        if embedding_name in _cbfv_files:
-            if embedding_name in ["skipatom", "random_200", "magpie", "mat2vec"]:
-                _csv = path.join(data_directory, _cbfv_files[embedding_name])
-                df = pd.read_csv(_csv)
-                # Convert df to a dictionary of (ele:embeddings) pairs
-                elements = list(df["element"])
-                df.drop(["element"], axis=1, inplace=True)
-                embeds_array = df.to_numpy()
-                embedding_data = {
-                    elements[i]: embeds_array[i] for i in range(len(embeds_array))
-                }
 
-            elif embedding_name == "megnet16":
-                megnet16_json = path.join(data_directory, _cbfv_files["megnet16"])
-                with open(megnet16_json) as f:
-                    embedding_data = json.load(f)
-                # Remove 'Null' key from megnet embedding
-                del embedding_data["Null"]
-
-            elif embedding_name in _cbfv_names_others:
-                _json = path.join(data_directory, _cbfv_files[embedding_name])
-                with open(_json) as f:
-                    embedding_data = json.load(f)
-        else:
-            raise (
-                ValueError(
-                    f"{embedding_name} not in the data directory or not in directory."
-                )
+        if _cbfv_files[embedding_name].endswith(".csv"):
+            return Embedding.from_csv(
+                path.join(
+                    data_directory,
+                    "element_representations",
+                    _cbfv_files[embedding_name],
+                ),
+                embedding_name,
+            )
+        elif "megnet" in _cbfv_files[embedding_name]:
+            return Embedding.from_json(
+                path.join(
+                    data_directory,
+                    "element_representations",
+                    _cbfv_files[embedding_name],
+                ),
+                embedding_name,
+            ).remove_elements(["Null"])
+        elif _cbfv_files[embedding_name].endswith(".json"):
+            return Embedding.from_json(
+                path.join(
+                    data_directory,
+                    "element_representations",
+                    _cbfv_files[embedding_name],
+                ),
+                embedding_name,
             )
-        return Embedding(embedding_data, embedding_name)
 
     @staticmethod
-    def from_json(embedding_json):
+    def from_json(embedding_json, embedding_name: Optional[str] = None):
         """
         Create an instance of the Embedding class from a json file.
 
         Args:
             embedding_json (str): Filepath of the json file
+            embedding_name (str): The name of the elemental representation
         """
         # Need to add validation handling for JSONs in different formats
         with open(embedding_json) as f:
             embedding_data = json.load(f)
-        return Embedding(embedding_data)
+        return Embedding(embedding_data, embedding_name)
 
     @staticmethod
-    def from_csv(embedding_csv):
+    def from_csv(embedding_csv, embedding_name: Optional[str] = None):
         """
         Create an instance of the Embedding class from a csv file.
 
         The first column of the csv file must contain the elements and be named element.
 
         Args:
             embedding_csv (str): Filepath of the csv file
+            embedding_name (str): The name of the elemental representation
+
         """
         # Need to add validation handling for csv files
         df = pd.read_csv(embedding_csv)
         elements = list(df["element"])
         df.drop(["element"], axis=1, inplace=True)
+        feature_labels = list(df.columns)
         embeds_array = df.to_numpy()
         embedding_data = {
             elements[i]: embeds_array[i] for i in range(len(embeds_array))
         }
-        return Embedding(embedding_data)
+        return Embedding(embedding_data, embedding_name, feature_labels)
 
     def as_dataframe(self, columns: str = "components") -> pd.DataFrame:
         """
         Return the embedding as a pandas Dataframe.
 
         The first column is the elements and each other
         column represents a component of the embedding.
 
         Args:
             columns (str): A string to specify if the columns are the vector components
-            and the index is the elements (`columns='components')
+            and the index is the elements (`columns='components'`)
             or the columns are the elements (`columns='elements'`).
 
         Returns:
             df (pandas.DataFrame): A pandas dataframe object
 
 
         """
         embedding = self.embeddings
-        df = pd.DataFrame(embedding)
+        df = pd.DataFrame(embedding, index=self.feature_labels)
         if columns == "components":
             return df.T
         elif columns == "elements":
             return df
         else:
             raise (
                 ValueError(
@@ -285,14 +324,49 @@
             if isinstance(elements, str):
                 del embeddings_copy[elements]
             elif isinstance(elements, list):
                 for el in elements:
                     del embeddings_copy[el]
             return Embedding(embeddings_copy, self.embedding_name)
 
+    def _is_standardised(self):
+        """Check if the embeddings are standardised.
+
+        Mean must be 0 and standard deviation must be 1.
+        """
+        return np.isclose(
+            np.mean(np.array(list(self.embeddings.values()))), 0
+        ) and np.isclose(np.std(np.array(list(self.embeddings.values()))), 1)
+
+    def standardise(self, inplace: bool = False):
+        """Standardise the embeddings.
+
+        Mean is 0 and standard deviation is 1.
+
+        """
+        if self._is_standardised():
+            warnings.warn(
+                "Embedding is already standardised. "
+                "Returning None and not changing the embedding."
+            )
+            return None
+        else:
+            embeddings_copy = self.embeddings.copy()
+            embeddings_array = np.array(list(embeddings_copy.values()))
+            embeddings_array = StandardScaler().fit_transform(embeddings_array)
+            for el, emb in zip(embeddings_copy.keys(), embeddings_array):
+                embeddings_copy[el] = emb
+
+            if inplace:
+                self.embeddings = embeddings_copy
+                self.is_standardised = True
+                return None
+            else:
+                return Embedding(embeddings_copy, self.embedding_name)
+
     def citation(self) -> List[str]:
         """Return a citation for the embedding."""
         if self.embedding_name in ["magpie", "magpie_sc"]:
             citation = [
                 "@article{ward2016general,"
                 "title={A general-purpose machine learning framework for "
                 "predicting properties of inorganic materials},"
@@ -429,63 +503,14 @@
 
     def create_pairs(self):
         """Create all possible pairs of elements."""
         ele_list = self.element_list
         ele_pairs = combinations_with_replacement(ele_list, 2)
         return ele_pairs
 
-    def stats_correlation_df(self) -> pd.DataFrame:
-        """Return a pandas.DataFrame with correlation metrics.
-
-         The columns of returned dataframe are:
-        [element_1, element_2, pearson_corr, euclid_dist].
-        """
-        warnings.warn(
-            "This method is deprecated and will be removed in a future release. ",
-            DeprecationWarning,
-        )
-        ele_pairs = self.create_pairs()
-        table = []
-        for ele1, ele2 in ele_pairs:
-            pearson = pearsonr(self.embeddings[ele1], self.embeddings[ele2])
-            dist = norm(self.embeddings[ele1] - self.embeddings[ele2])
-
-            table.append((ele1, ele2, pearson[0], dist))
-            if ele1 != ele2:
-                table.append((ele2, ele1, pearson[0], dist))
-
-        corr_df = pd.DataFrame(
-            table,
-            columns=[
-                "ele_1",
-                "ele_2",
-                "pearson_corr",
-                "euclid_dist",
-            ],
-        )
-
-        mend_1 = [(Element(ele).mendeleev_no, ele) for ele in corr_df["ele_1"]]
-        mend_2 = [(Element(ele).mendeleev_no, ele) for ele in corr_df["ele_2"]]
-
-        corr_df["mend_1"] = mend_1
-        corr_df["mend_2"] = mend_2
-
-        corr_df = corr_df[
-            [
-                "ele_1",
-                "ele_2",
-                "mend_1",
-                "mend_2",
-                "euclid_dist",
-                "pearson_corr",
-            ]
-        ]
-
-        return corr_df
-
     def compute_correlation_metric(
         self, ele1: str, ele2: str, metric: str = "pearson"
     ) -> float:
         """
         Compute the correlation/similarity metric between two vectors.
 
         Allowed metrics:
@@ -573,31 +598,14 @@
         else:
             print(
                 "Invalid distance metric."
                 f"Use one of the following metrics:{valid_metrics}"
             )
             raise ValueError
 
-    def pearson_pivot_table(self) -> pd.DataFrame:
-        """
-        Return a pandas.DataFrame style pivot object.
-
-        The index and column are the mendeleev number of the element pairs
-        and the values being the pearson correlation metrics.
-        """
-        warnings.warn(
-            "This method is deprecated and will be removed in a future release. ",
-            DeprecationWarning,
-        )
-        corr_df = self.correlation_df()
-        pearson_pivot = corr_df.pivot_table(
-            values="pearson_corr", index="mend_1", columns="mend_2"
-        )
-        return pearson_pivot
-
     def distance_df(self, metric: str = "euclidean") -> pd.DataFrame:
         """
         Return a dataframe with columns ["ele_1", "ele_2", metric].
 
         Allowed metrics:
 
         * euclidean
@@ -731,227 +739,89 @@
             return correlation_pivot
         elif sortby == "atomic_number":
             correlation_pivot = corr_df.pivot_table(
                 values=metric, index="Z_1", columns="Z_2"
             )
             return correlation_pivot
 
-    def plot_pearson_correlation(self, figsize: Tuple[int, int] = (24, 24), **kwargs):
-        """
-        Plot the heatmap of the pearson correlation values.
+    def calculate_PC(self, n_components: int = 2, standardise: bool = True, **kwargs):
+        """Calculate the principal componenets (PC) of the embeddings.
 
         Args:
-            figsize (tuple): A tuple of (width, height).
-            **kwargs: Other keyword arguments to be passed to sns.heatmap
-
-        Returns:
-            ax (matplotlib Axes): An Axes object with the heatmap
-
+            n_components (int): The number of components to project the embeddings to.
+            standardise (bool): Whether to standardise the embeddings before projecting.
+            **kwargs: Other keyword arguments to be passed to PCA.
         """
-        warnings.warn(
-            "This method is deprecated and will be removed in a future release. ",
-            DeprecationWarning,
-        )
-        pearson_pivot = self.pearson_pivot_table()
-
-        plt.figure(figsize=figsize)
-        ax = sns.heatmap(
-            pearson_pivot, cmap="bwr", square=True, linecolor="k", **kwargs
-        )
-
-        return ax
-
-    def plot_distance_correlation(
-        self, metric: str = "euclidean", figsize: Tuple[int, int] = (24, 24), **kwargs
-    ):
-        """
-        Plot the heatmap of the pairwise distance metrics.
-
-        Args:
-            metric (str): A valid distance metric
-            figsize (tuple): A tuple of (width, height)
-
-        Returns:
-            ax (matplotlib.axes.Axes): An Axes object with the heatmap
-
-        """
-        warnings.warn(
-            "This method is deprecated and will be removed in a future release. ",
-            DeprecationWarning,
-        )
-        distance_pivot = self.distance_pivot_table(metric=metric)
-
-        plt.figure(figsize=figsize)
-        ax = sns.heatmap(
-            distance_pivot, cmap="bwr", square=True, linecolor="k", **kwargs
-        )
-
-        return ax
-
-    def calculate_PC(self, n_components: int = 2, scale: bool = True, **kwargs):
-        """Calculate the principal componenets (PC) of the embeddings."""
-        if scale:
-            embeddings_array = StandardScaler().fit_transform(
-                np.array(list(self.embeddings.values()))
-            )
+        if standardise:
+            if self.is_standardised:
+                embeddings_array = np.array(list(self.embeddings.values()))
+            else:
+                self.standardise(inplace=True)
+                embeddings_array = np.array(list(self.embeddings.values()))
         else:
+            warnings.warn(
+                """It is recommended to scale the embeddings
+                before projecting with PCA.
+                To do so, set `standardise=True`."""
+            )
             embeddings_array = np.array(list(self.embeddings.values()))
 
         pca = decomposition.PCA(
             n_components=n_components, **kwargs
         )  # project to N dimensions
         pca.fit(embeddings_array)
         self._pca_data = pca.transform(embeddings_array)
         return self._pca_data
 
-    def calculate_tSNE(self, n_components: int = 2, scale: bool = True, **kwargs):
-        """Calculate t-SNE components."""
-        if scale:
-            embeddings_array = StandardScaler().fit_transform(
-                np.array(list(self.embeddings.values()))
-            )
+    def calculate_tSNE(self, n_components: int = 2, standardise: bool = True, **kwargs):
+        """Calculate t-SNE components.
+
+        Args:
+            n_components (int): The number of components to project the embeddings to.
+            standardise (bool): Whether to standardise the embeddings before projecting.
+            **kwargs: Other keyword arguments to be passed to t-SNE.
+        """
+        if standardise:
+            if self.is_standardised:
+                embeddings_array = np.array(list(self.embeddings.values()))
+            else:
+                self.standardise(inplace=True)
+                embeddings_array = np.array(list(self.embeddings.values()))
         else:
+            warnings.warn(
+                """It is recommended to scale the embeddings
+                before projecting with t-SNE.
+                To do so, set `standardise=True`."""
+            )
             embeddings_array = np.array(list(self.embeddings.values()))
 
         tsne = TSNE(n_components=n_components, **kwargs)
         tsne_result = tsne.fit_transform(embeddings_array)
         self._tsne_data = tsne_result
         return self._tsne_data
 
-    def calculate_UMAP(self, n_components: int = 2, scale: bool = True, **kwargs):
-        """Calculate UMAP embeddings."""
-        if scale:
-            embeddings_array = StandardScaler().fit_transform(
-                np.array(list(self.embeddings.values()))
-            )
+    def calculate_UMAP(self, n_components: int = 2, standardise: bool = True, **kwargs):
+        """Calculate UMAP embeddings.
+
+        Args:
+            n_components (int): The number of components to project the embeddings to.
+            standardise (bool): Whether to scale the embeddings before projecting.
+            **kwargs: Other keyword arguments to be passed to UMAP.
+        """
+        if standardise:
+            if self.is_standardised:
+                embeddings_array = np.array(list(self.embeddings.values()))
+            else:
+                self.standardise(inplace=True)
+                embeddings_array = np.array(list(self.embeddings.values()))
         else:
+            warnings.warn(
+                """It is recommended to scale the embeddings
+                before projecting with UMAP.
+                To do so, set `standardise=True`."""
+            )
             embeddings_array = np.array(list(self.embeddings.values()))
 
         umap = UMAP(n_components=n_components, **kwargs)
         umap_result = umap.fit_transform(embeddings_array)
         self._umap_data = umap_result
         return self._umap_data
-
-    def plot_PCA_2D(
-        self,
-        figsize: Tuple[int, int] = (16, 12),
-        points_hue: str = "group",
-        points_size: int = 200,
-        **kwargs,
-    ):
-        """Plot a PCA plot of the atomic embedding.
-
-        Args:
-            figsize (tuple): A tuple of (width, height)
-            points_size (float): The marker size
-
-        Returns:
-            ax (matplotlib.axes.Axes): An Axes object with the PCA plot
-
-        """
-        warnings.warn(
-            "This method is deprecated and will be removed in a future release. ",
-            DeprecationWarning,
-        )
-        embeddings_array = np.array(list(self.embeddings.values()))
-        element_array = np.array(self.element_list)
-
-        pca = decomposition.PCA(n_components=2)  # project to 2 dimensions
-
-        pca.fit(embeddings_array)
-        X = pca.transform(embeddings_array)
-
-        pca_dim1 = X[:, 0]
-        pca_dim2 = X[:, 1]
-
-        # Create a dataframe to store the dimensions, labels and group info for the PCA
-        pca_df = pd.DataFrame(
-            {
-                "pca_dim1": pca_dim1,
-                "pca_dim2": pca_dim2,
-                "element": element_array,
-                "group": list(self.element_groups_dict.values()),
-            }
-        )
-        fig, ax = plt.subplots(figsize=figsize)
-
-        sns.scatterplot(
-            x="pca_dim1",
-            y="pca_dim2",
-            data=pca_df,
-            hue=points_hue,
-            s=points_size,
-            **kwargs,
-            ax=ax,
-        )
-
-        plt.xlabel("Dimension 1")
-        plt.ylabel("Dimension 2")
-
-        for i in range(len(X)):
-            plt.text(x=pca_dim1[i], y=pca_dim2[i], s=element_array[i])
-
-        return plt
-
-    def plot_tSNE(
-        self,
-        n_components: str = 2,
-        figsize: Tuple[int, int] = (16, 12),
-        points_hue: str = "group",
-        points_size: int = 200,
-        **kwargs,
-    ):
-        """Plot a t-SNE plot of the atomic embedding.
-
-        Args:
-            n_components (int): Number of t-SNE components to plot.
-            figsize (tuple): A tuple of (width, height)
-            points_size (float): The marker size
-
-        Returns:
-            ax (matplotlib.axes.Axes): An Axes object with the PCA plot
-
-
-        """
-        warnings.warn(
-            "This method is deprecated and will be removed in a future release. ",
-            DeprecationWarning,
-        )
-        embeddings_array = np.array(list(self.embeddings.values()))
-        element_array = np.array(self.element_list)
-
-        tsne = TSNE(n_components)
-        tsne_result = tsne.fit_transform(embeddings_array)
-
-        tsne_df = pd.DataFrame(
-            {
-                "tsne_dim1": tsne_result[:, 0],
-                "tsne_dim2": tsne_result[:, 1],
-                "element": element_array,
-                "group": list(self.element_groups_dict.values()),
-            }
-        )
-        # Create the t-SNE plot
-        fig, ax = plt.subplots(figsize=figsize)
-        sns.scatterplot(
-            x="tsne_dim1",
-            y="tsne_dim2",
-            data=tsne_df,
-            hue=points_hue,
-            s=points_size,
-            ax=ax,
-        )
-        # lim = (tsne_result.min()-5, tsne_result.max()+5)
-        # ax.set_xlim(lim)
-        # ax.set_ylim(lim)
-        plt.xlabel("Dimension 1")
-        plt.ylabel("Dimension 2")
-
-        # Label the points
-        for i in range(tsne_df.shape[0]):
-            plt.text(
-                x=tsne_df["tsne_dim1"][i],
-                y=tsne_df["tsne_dim2"][i],
-                s=tsne_df["element"][i],
-            )
-
-        return plt
```

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/element_group.json` & `ElementEmbeddings-0.3.0/src/elementembeddings/data/element_data/element_group.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/element_symbols.json` & `ElementEmbeddings-0.3.0/src/elementembeddings/data/element_data/element_symbols.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/periodic-table-lookup-symbols.json` & `ElementEmbeddings-0.3.0/src/elementembeddings/data/element_data/periodic-table-lookup-symbols.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/periodic-table-lookup.json` & `ElementEmbeddings-0.3.0/src/elementembeddings/data/element_data/periodic-table-lookup.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/data/magpie.csv` & `ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/magpie.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/data/magpie_sc.json` & `ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/magpie_sc.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/data/mat2vec.csv` & `ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/mat2vec.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/data/matscholar-embedding.json` & `ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/matscholar-embedding.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/data/megnet16.json` & `ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/megnet16.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/data/mod_petti.json` & `ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/mod_petti.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/data/oliynyk_sc.json` & `ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/oliynyk_sc.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/data/random_200.csv` & `ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/random_200.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/data/random_200_new.csv` & `ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/random_200_new.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/data/skipatom_20201009_induced.csv` & `ElementEmbeddings-0.3.0/src/elementembeddings/data/element_representations/skipatom_20201009_induced.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/plotter.py` & `ElementEmbeddings-0.3.0/src/elementembeddings/plotter.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,67 +90,80 @@
 
 def dimension_plotter(
     embedding: Embedding,
     ax: Optional[plt.axes] = None,
     n_components: int = 2,
     reducer: str = "umap",
     adjusttext: bool = True,
-    **kwargs,
+    reducer_params: Optional[dict] = None,
+    scatter_params: Optional[dict] = None,
 ):
     """Plot the reduced dimensions of the embeddings.
 
     Args:
         embedding (Embedding): The embedding to be plotted.
         ax (plt.axes, optional): The axes to plot on, by default None
         n_components (int): The number of components to reduce to, by default 2
         reducer (str): The dimensionality reduction algorithm to use, by default "umap"
         adjust_text (bool): Whether to avoid overlap of the text labels, by default True
-        **kwargs:  Additional keyword arguments to pass to the
-          dimensionality reduction algorithm.
+        reducer_params (dict, optional): Additional keyword arguments to pass to
+        the reducer, by default None
+        scatter_params (dict, optional): Additional keyword arguments to pass to
+        the scatterplot, by default None
 
     """
+    if reducer_params is None:
+        reducer_params = {}
     if reducer == "umap":
         if (
             embedding._umap_data is not None
             and embedding._umap_data.shape[1] == n_components
         ):
             reduced = embedding._umap_data
         else:
-            reduced = embedding.calculate_UMAP(n_components=n_components, **kwargs)
+            reduced = embedding.calculate_UMAP(
+                n_components=n_components, **reducer_params
+            )
     elif reducer == "tsne":
         if (
             embedding._tsne_data is not None
             and embedding._tsne_data.shape[1] == n_components
         ):
             reduced = embedding._tsne_data
         else:
-            reduced = embedding.calculate_tSNE(n_components=n_components, **kwargs)
+            reduced = embedding.calculate_tSNE(
+                n_components=n_components, **reducer_params
+            )
     elif reducer == "pca":
         if (
             embedding._pca_data is not None
             and embedding._pca_data.shape[1] == n_components
         ):
             reduced = embedding._pca_data
         else:
-            reduced = embedding.calculate_PC(n_components=n_components, **kwargs)
+            reduced = embedding.calculate_PC(
+                n_components=n_components, **reducer_params
+            )
     else:
         raise ValueError("Unrecognised reducer.")
 
     if reduced.shape[1] == 2:
         df = pd.DataFrame(
             {
                 "x": reduced[:, 0],
                 "y": reduced[:, 1],
                 "element": np.array(embedding.element_list),
                 "Group": list(embedding.element_groups_dict.values()),
             }
         )
         if not ax:
             fig, ax = plt.subplots()
-        sns.scatterplot(data=df, x="x", y="y", hue="Group", ax=ax, **kwargs)
+        if scatter_params is None:
+            scatter_params = {}
+        sns.scatterplot(data=df, x="x", y="y", hue="Group", ax=ax, **scatter_params)
         ax.set_xlabel("Dimension 1")
         ax.set_ylabel("Dimension 2")
         texts = [
             ax.text(df["x"][i], df["y"][i], df["element"][i], fontsize=12)
             for i in range(len(df))
         ]
         if adjusttext:
```

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/tests/test_core.py` & `ElementEmbeddings-0.3.0/src/elementembeddings/tests/test_core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Test the core module of AtomicEmbeddings."""
+import copy
 import os
 import unittest
 
-import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 from elementembeddings.core import Embedding
 
 test_files_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "files")
 TEST_EMBEDDING_CSV = os.path.join(test_files_dir, "test_embedding.csv")
@@ -21,38 +21,106 @@
     def setUpClass(cls):
         """Set up the test."""
         cls.test_skipatom = Embedding.load_data("skipatom")
         cls.test_megnet16 = Embedding.load_data("megnet16")
         cls.test_matscholar = Embedding.load_data("matscholar")
         cls.test_mod_petti = Embedding.load_data("mod_petti")
         cls.test_magpie = Embedding.load_data("magpie")
+        cls.test_atomic = Embedding.load_data("atomic")
+        cls.test_magpie_sc = Embedding.load_data("magpie_sc")
 
     def test_Embedding_attributes(self):
         """Test attributes of the loaded embeddings."""
         assert self.test_skipatom.dim == 200
         assert self.test_skipatom.embedding_name == "skipatom"
+        assert self.test_skipatom.embedding_type == "vector"
         assert self.test_megnet16.dim == 16
         assert self.test_megnet16.embedding_name == "megnet16"
+        assert self.test_megnet16.embedding_type == "vector"
         assert self.test_matscholar.dim == 200
         assert self.test_matscholar.embedding_name == "matscholar"
-        assert self.test_mod_petti.dim == 1
+        assert self.test_matscholar.embedding_type == "vector"
+        assert self.test_mod_petti.dim == 103
         assert self.test_mod_petti.embedding_name == "mod_petti"
+        assert self.test_mod_petti.embedding_type == "linear"
         assert isinstance(self.test_skipatom.citation(), list)
         assert isinstance(self.test_megnet16.citation(), list)
         assert isinstance(self.test_matscholar.citation(), list)
         assert isinstance(self.test_mod_petti.citation(), list)
 
+    def test_Embedding_standardised(self):
+        """Test that the Embedding class can check if the data is standardised."""
+        assert self.test_magpie.is_standardised is False
+        assert self.test_magpie_sc.is_standardised is True
+
+    def test_Embedding_standardisation(self):
+        """Test the standardisation method of the Embedding class."""
+        assert self.test_magpie.is_standardised is False
+        assert self.test_magpie.standardise().is_standardised is True
+        assert self.test_skipatom.is_standardised is False
+        assert self.test_skipatom.standardise().is_standardised is True
+        assert self.test_skipatom.standardise().standardise() is None
+        assert copy.deepcopy(self.test_magpie).standardise(inplace=True) is None
+
     def test_Embedding_file_input(self):
         """Test that the Embedding class can load custom data."""
         embedding_csv = Embedding.from_csv(TEST_EMBEDDING_CSV)
         embedding_json = Embedding.from_json(TEST_EMBEDDING_JSON)
         assert embedding_csv.dim == 10
         assert embedding_json.dim == 10
 
-    def test_Embeddings_class_magpie(self):
+    def test_Embedding_class_mod_petti(self):
+        """Test that the Embedding class can load the mod_petti data."""
+        mod_petti = self.test_mod_petti
+        # Check if the embeddings attribute is a dict
+        assert isinstance(mod_petti.embeddings, dict)
+        # Check if the embedding vector is a numpy array
+        assert isinstance(mod_petti.embeddings["H"], np.ndarray)
+        # Check if H is present in the embedding keys
+        assert "H" in mod_petti.embeddings.keys()
+        # Check dimensions
+        assert mod_petti.dim == 103
+        # Check embedding type
+        assert mod_petti.embedding_type == "linear"
+        # Check that a list is returned
+        assert isinstance(mod_petti.element_list, list)
+        # Check the the dimensons of the embedding vector
+        assert mod_petti.embeddings["H"].shape == (103,)
+        # Check that the embedding vector is not all zeros
+        assert not np.all(mod_petti.embeddings["H"] == 0)
+        # Check the the embedding vector for H is correct
+        test_H = np.zeros(103)
+        test_H[-1] = 1
+        assert np.all(mod_petti.embeddings["H"] == test_H)
+
+    def test_Embedding_class_atomic(self):
+        """Test that the Embedding class can load the atomic data."""
+        atomic = self.test_atomic
+        # Check if the embeddings attribute is a dict
+        assert isinstance(atomic.embeddings, dict)
+        # Check if the embedding vector is a numpy array
+        assert isinstance(atomic.embeddings["H"], np.ndarray)
+        # Check if H is present in the embedding keys
+        assert "H" in atomic.embeddings.keys()
+        # Check dimensions
+        assert atomic.dim == 118
+        # Check embedding type
+        assert atomic.embedding_type == "linear"
+        # Check that a list is returned
+        assert isinstance(atomic.element_list, list)
+        # Check the the dimensons of the embedding vector
+        assert atomic.embeddings["H"].shape == (118,)
+        # Check that the embedding vector is not all zeros
+        assert not np.all(atomic.embeddings["H"] == 0)
+        # Check the the embedding vector for H is correct
+        test_H = np.zeros(118)
+        test_H[0] = 1
+        assert np.all(atomic.embeddings["H"] == test_H)
+
+    def test_Embedding_class_magpie(self):
         """Test that the Embedding class can load the magpie data."""
         magpie = self.test_magpie
         # Check if the embeddings attribute is a dict
         assert isinstance(magpie.embeddings, dict)
         # Check if the embedding vector is a numpy array
         assert isinstance(magpie.embeddings["H"], np.ndarray)
         # Check if H is present in the embedding keys
@@ -352,19 +420,14 @@
             "Z_2",
             "euclidean",
         ]
         assert isinstance(self.test_magpie.distance_pivot_table(), pd.DataFrame)
         assert isinstance(
             self.test_magpie.distance_pivot_table(sortby="atomic_number"), pd.DataFrame
         )
-        assert isinstance(self.test_magpie.plot_distance_correlation(), plt.Axes)
-        assert isinstance(
-            self.test_magpie.plot_distance_correlation(metric="euclidean"), plt.Axes
-        )
-        assert isinstance(self.test_magpie.stats_correlation_df(), pd.DataFrame)
 
     def test_remove_elements(self):
         """Test the remove_elements function."""
         assert isinstance(self.test_skipatom.remove_elements("H"), Embedding)
         assert isinstance(self.test_skipatom.remove_elements(["H", "Li"]), Embedding)
         self.assertIsNone(self.test_skipatom.remove_elements("H", inplace=True))
         self.assertFalse(self.test_skipatom._is_el_in_embedding("H"))
```

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/tests/test_plotter.py` & `ElementEmbeddings-0.3.0/src/elementembeddings/tests/test_plotter.py`

 * *Files 26% similar despite different names*

```diff
@@ -92,7 +92,41 @@
         self.assertRaises(
             ValueError,
             dimension_plotter,
             self.test_skipatom,
             n_components=4,
             reducer="pca",
         )
+
+    def test_kwargs_plotter(self):
+        """Test that the dimension_plotter function works with kwargs."""
+        pca_params = {"svd_solver": "full", "random_state": 42}
+        tsne_params = {"n_iter": 1000, "random_state": 42, "perplexity": 100}
+        umap_params = {"n_neighbors": 15, "random_state": 42}
+        scatter_params = {"s": 1}
+        skipatom_pca_plot = dimension_plotter(
+            self.test_skipatom,
+            n_components=2,
+            reducer="pca",
+            adjusttext=False,
+            reducer_params=pca_params,
+            scatter_params=scatter_params,
+        )
+        assert isinstance(skipatom_pca_plot, plt.Axes)
+        skipatom_tsne_plot = dimension_plotter(
+            self.test_skipatom,
+            n_components=2,
+            reducer="tsne",
+            adjusttext=False,
+            scatter_params=scatter_params,
+            reducer_params=tsne_params,
+        )
+        assert isinstance(skipatom_tsne_plot, plt.Axes)
+        skipatom_umap_plot = dimension_plotter(
+            self.test_skipatom,
+            n_components=2,
+            reducer="umap",
+            adjusttext=False,
+            scatter_params=scatter_params,
+            reducer_params=umap_params,
+        )
+        assert isinstance(skipatom_umap_plot, plt.Axes)
```

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/tests/test_utils.py` & `ElementEmbeddings-0.3.0/src/elementembeddings/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.2.0/src/elementembeddings/utils/math.py` & `ElementEmbeddings-0.3.0/src/elementembeddings/utils/math.py`

 * *Files identical despite different names*

