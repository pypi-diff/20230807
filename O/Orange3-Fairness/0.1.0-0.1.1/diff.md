# Comparing `tmp/Orange3-Fairness-0.1.0.tar.gz` & `tmp/Orange3-Fairness-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orange3-Fairness-0.1.0.tar", last modified: Mon Jul 31 15:51:47 2023, max compression
+gzip compressed data, was "Orange3-Fairness-0.1.1.tar", last modified: Mon Aug  7 08:22:22 2023, max compression
```

## Comparing `Orange3-Fairness-0.1.0.tar` & `Orange3-Fairness-0.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 15:51:47.901450 Orange3-Fairness-0.1.0/
--rw-rw-rw-   0        0        0    35823 2023-06-23 10:08:27.000000 Orange3-Fairness-0.1.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-31 15:51:47.864140 Orange3-Fairness-0.1.0/Orange3_Fairness.egg-info/
--rw-rw-rw-   0        0        0      816 2023-07-31 15:51:47.000000 Orange3-Fairness-0.1.0/Orange3_Fairness.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1819 2023-07-31 15:51:47.000000 Orange3-Fairness-0.1.0/Orange3_Fairness.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 15:51:47.000000 Orange3-Fairness-0.1.0/Orange3_Fairness.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2023-07-31 15:51:47.000000 Orange3-Fairness-0.1.0/Orange3_Fairness.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-07-31 15:51:47.000000 Orange3-Fairness-0.1.0/Orange3_Fairness.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-31 15:51:47.000000 Orange3-Fairness-0.1.0/Orange3_Fairness.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      816 2023-07-31 15:51:47.900453 Orange3-Fairness-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-07-26 08:35:04.000000 Orange3-Fairness-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 15:51:47.865140 Orange3-Fairness-0.1.0/orangecontrib/
--rw-rw-rw-   0        0        0      165 2023-07-14 09:07:13.000000 Orange3-Fairness-0.1.0/orangecontrib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:51:47.866140 Orange3-Fairness-0.1.0/orangecontrib/fairness/
--rw-rw-rw-   0        0        0       31 2023-07-14 08:54:04.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:51:47.867140 Orange3-Fairness-0.1.0/orangecontrib/fairness/evaluation/
--rw-rw-rw-   0        0        0       22 2023-07-14 08:54:04.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/evaluation/__init__.py
--rw-rw-rw-   0        0        0     2730 2023-07-14 09:12:43.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/evaluation/scoring.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:51:47.870139 Orange3-Fairness-0.1.0/orangecontrib/fairness/modeling/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:54:04.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/modeling/__init__.py
--rw-rw-rw-   0        0        0    12467 2023-07-27 10:26:48.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/modeling/adversarial.py
--rw-rw-rw-   0        0        0     4990 2023-07-27 11:36:07.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/modeling/postprocessing.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:51:47.880242 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/
--rw-rw-rw-   0        0        0     1132 2023-07-14 09:34:41.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:51:47.889345 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/icons/
--rw-rw-rw-   0        0        0     5385 2023-07-25 17:20:31.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/icons/adversarial_debiasing.svg
--rw-rw-rw-   0        0        0     1300 2023-07-25 17:36:15.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/icons/as_fairness.svg
--rw-rw-rw-   0        0        0      903 2023-07-25 17:38:13.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/icons/combine_preprocessors.svg
--rw-rw-rw-   0        0        0      485 2023-07-25 17:38:42.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/icons/dataset_bias.svg
--rw-rw-rw-   0        0        0     2003 2023-07-25 17:33:06.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/icons/eq_odds_postprocessing.svg
--rw-rw-rw-   0        0        0      799 2023-07-25 17:40:49.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/icons/reweighing.svg
--rw-rw-rw-   0        0        0      614 2023-07-25 17:41:02.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/icons/weighted_log_reg.svg
--rw-rw-rw-   0        0        0     9698 2023-07-31 14:34:37.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/owadversarialdebiasing.py
--rw-rw-rw-   0        0        0    11637 2023-07-27 09:43:30.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/owasfairness.py
--rw-rw-rw-   0        0        0     1866 2023-07-25 17:03:23.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/owcombinepreprocessors.py
--rw-rw-rw-   0        0        0     2083 2023-07-25 17:03:32.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/owdatasetbias.py
--rw-rw-rw-   0        0        0     3418 2023-07-31 14:45:45.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/owequalizedodds.py
--rw-rw-rw-   0        0        0     4794 2023-07-25 17:03:58.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/owreweighing.py
--rw-rw-rw-   0        0        0     7095 2023-07-25 17:16:41.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/owweightedlogisticregression.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:51:47.899453 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/tests/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:54:04.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/tests/__init__.py
--rw-rw-rw-   0        0        0     6677 2023-07-28 14:11:25.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/tests/test_owadversarialdebiasing.py
--rw-rw-rw-   0        0        0     2928 2023-07-24 13:13:13.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/tests/test_owasfairness.py
--rw-rw-rw-   0        0        0     2712 2023-07-24 13:17:11.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/tests/test_owdatasetbias.py
--rw-rw-rw-   0        0        0     6422 2023-07-28 09:20:23.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/tests/test_owequalizedodds.py
--rw-rw-rw-   0        0        0     4925 2023-07-25 12:13:29.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/tests/test_owreweighing.py
--rw-rw-rw-   0        0        0     1407 2023-07-24 13:17:00.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/tests/utils.py
--rw-rw-rw-   0        0        0     9934 2023-07-31 14:49:30.000000 Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/utils.py
--rw-rw-rw-   0        0        0       42 2023-07-31 15:51:47.901450 Orange3-Fairness-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1376 2023-07-31 15:51:40.000000 Orange3-Fairness-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:22:22.506056 Orange3-Fairness-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-06-23 10:08:27.000000 Orange3-Fairness-0.1.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-08-07 08:22:22.463054 Orange3-Fairness-0.1.1/Orange3_Fairness.egg-info/
+-rw-rw-rw-   0        0        0      816 2023-08-07 08:22:22.000000 Orange3-Fairness-0.1.1/Orange3_Fairness.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1819 2023-08-07 08:22:22.000000 Orange3-Fairness-0.1.1/Orange3_Fairness.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 08:22:22.000000 Orange3-Fairness-0.1.1/Orange3_Fairness.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-08-07 08:22:22.000000 Orange3-Fairness-0.1.1/Orange3_Fairness.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-08-07 08:22:22.000000 Orange3-Fairness-0.1.1/Orange3_Fairness.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-07 08:22:22.000000 Orange3-Fairness-0.1.1/Orange3_Fairness.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      816 2023-08-07 08:22:22.505055 Orange3-Fairness-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-07-31 15:57:22.000000 Orange3-Fairness-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 08:22:22.464052 Orange3-Fairness-0.1.1/orangecontrib/
+-rw-rw-rw-   0        0        0      165 2023-07-14 09:07:13.000000 Orange3-Fairness-0.1.1/orangecontrib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:22:22.465053 Orange3-Fairness-0.1.1/orangecontrib/fairness/
+-rw-rw-rw-   0        0        0       31 2023-07-14 08:54:04.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:22:22.467052 Orange3-Fairness-0.1.1/orangecontrib/fairness/evaluation/
+-rw-rw-rw-   0        0        0       22 2023-07-14 08:54:04.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     3149 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/evaluation/scoring.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:22:22.471052 Orange3-Fairness-0.1.1/orangecontrib/fairness/modeling/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:54:04.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/modeling/__init__.py
+-rw-rw-rw-   0        0        0     6723 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/modeling/adversarial.py
+-rw-rw-rw-   0        0        0     5355 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/modeling/postprocessing.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:22:22.483054 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/
+-rw-rw-rw-   0        0        0     1132 2023-07-14 09:34:41.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:22:22.494053 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/icons/
+-rw-rw-rw-   0        0        0     5385 2023-07-25 17:20:31.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/icons/adversarial_debiasing.svg
+-rw-rw-rw-   0        0        0     1300 2023-07-25 17:36:15.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/icons/as_fairness.svg
+-rw-rw-rw-   0        0        0      903 2023-07-25 17:38:13.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/icons/combine_preprocessors.svg
+-rw-rw-rw-   0        0        0      485 2023-07-25 17:38:42.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/icons/dataset_bias.svg
+-rw-rw-rw-   0        0        0     2003 2023-07-25 17:33:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/icons/eq_odds_postprocessing.svg
+-rw-rw-rw-   0        0        0      799 2023-07-25 17:40:49.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/icons/reweighing.svg
+-rw-rw-rw-   0        0        0      614 2023-07-25 17:41:02.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/icons/weighted_log_reg.svg
+-rw-rw-rw-   0        0        0    10315 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/owadversarialdebiasing.py
+-rw-rw-rw-   0        0        0    12556 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/owasfairness.py
+-rw-rw-rw-   0        0        0     2298 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/owcombinepreprocessors.py
+-rw-rw-rw-   0        0        0     2410 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/owdatasetbias.py
+-rw-rw-rw-   0        0        0     6284 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/owequalizedodds.py
+-rw-rw-rw-   0        0        0     4825 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/owreweighing.py
+-rw-rw-rw-   0        0        0     1606 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/owweightedlogisticregression.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:22:22.504054 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:54:04.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/tests/__init__.py
+-rw-rw-rw-   0        0        0     6677 2023-07-28 14:11:25.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/tests/test_owadversarialdebiasing.py
+-rw-rw-rw-   0        0        0     2928 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/tests/test_owasfairness.py
+-rw-rw-rw-   0        0        0     2712 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/tests/test_owdatasetbias.py
+-rw-rw-rw-   0        0        0     6420 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/tests/test_owequalizedodds.py
+-rw-rw-rw-   0        0        0     4925 2023-07-25 12:13:29.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/tests/test_owreweighing.py
+-rw-rw-rw-   0        0        0     1407 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/tests/utils.py
+-rw-rw-rw-   0        0        0    12289 2023-08-07 07:57:06.000000 Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/utils.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 08:22:22.506056 Orange3-Fairness-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1448 2023-08-07 08:21:16.000000 Orange3-Fairness-0.1.1/setup.py
```

### Comparing `Orange3-Fairness-0.1.0/LICENSE` & `Orange3-Fairness-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Orange3-Fairness-0.1.0/Orange3_Fairness.egg-info/PKG-INFO` & `Orange3-Fairness-0.1.1/Orange3_Fairness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orange3-Fairness
-Version: 0.1.0
+Version: 0.1.1
 Summary: Orange3 add-on for fairness-aware machine learning.
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: contact@orange.biolab.si
 Maintainer: Zan Mervic
 License: GPL3+
 Keywords: orange3 add-on,orange3 fairness
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `Orange3-Fairness-0.1.0/Orange3_Fairness.egg-info/SOURCES.txt` & `Orange3-Fairness-0.1.1/Orange3_Fairness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Fairness-0.1.0/PKG-INFO` & `Orange3-Fairness-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orange3-Fairness
-Version: 0.1.0
+Version: 0.1.1
 Summary: Orange3 add-on for fairness-aware machine learning.
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: contact@orange.biolab.si
 Maintainer: Zan Mervic
 License: GPL3+
 Keywords: orange3 add-on,orange3 fairness
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/evaluation/scoring.py` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/evaluation/scoring.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,97 @@
 from abc import abstractmethod
 from Orange.data import DiscreteVariable, ContinuousVariable, Domain
 from Orange.evaluation.scoring import Score
 
 from aif360.metrics import ClassificationMetric
 
-from orangecontrib.fairness.widgets.utils import table_to_standard_dataset, contains_fairness_attributes
+from orangecontrib.fairness.widgets.utils import (
+    table_to_standard_dataset,
+    contains_fairness_attributes,
+)
 
 
 __all__ = [
     "StatisticalParityDifference",
     "EqualOpportunityDifference",
     "AverageOddsDifference",
     "DisparateImpact",
 ]
 
 
 class FairnessScorer(Score, abstract=True):
+    """Abstract class which will allow fairness scores to be calculated and displayed in certain widgets"""
+
     class_types = (
         DiscreteVariable,
         ContinuousVariable,
     )
 
-    # This is a static method, it is called by the Orange framework to check if the scorer is compatible with the domain of the data
     @staticmethod
     def is_compatible(domain: Domain) -> bool:
+        """Checks if the scorer is compatible with the domain of the data. If not the scores will not be computed."""
         return contains_fairness_attributes(domain)
 
-    # This method is called by the Orange framework, together with the metric method it computes the specific score
     def compute_score(self, results):
+        """Method that creates a ClassificationMetric object used to compute fairness scores"""
+        dataset, privileged_groups, unprivileged_groups = table_to_standard_dataset(
+            results.data
+        )
 
-        dataset, privileged_groups, unprivileged_groups = table_to_standard_dataset(results.data)
-        # We need to subset the created dataset so that it will match the shape/order of the predictions if some of the data was used multiple times
+        # We need to subset the created dataset so that it will match the shape/order 
+        # This is needed when/if some of the rows in the data were used multiple times
         dataset = dataset.subset(results.row_indices)
         dataset_pred = dataset.copy()
         dataset_pred.labels = results.predicted
+
         classification_metric = ClassificationMetric(
             dataset,
             dataset_pred,
             unprivileged_groups=unprivileged_groups,
             privileged_groups=privileged_groups,
         )
         return [self.metric(classification_metric)]
 
-    # This indicates that the metric method needs to be implemented by the subclasses
     @abstractmethod
     def metric(self, classification_metric):
+        """Method that needs to be implemented by the subclasses of the FairnessScorer."""
         pass
 
 
 class StatisticalParityDifference(FairnessScorer):
+    """Class for Statistical Parity Difference fairness scoring."""
+
     name = "SPD"
     long_name = "Statistical Parity Difference"
 
-    def metric(self, classificationMetric):
-        return classificationMetric.statistical_parity_difference()
+    def metric(self, classification_metric):
+        return classification_metric.statistical_parity_difference()
 
 
 class EqualOpportunityDifference(FairnessScorer):
+    """Class for Equal Opportunity Difference fairness scoring."""
+
     name = "EOD"
     long_name = "Equal Opportunity Difference"
 
-    def metric(self, classificationMetric):
-        return classificationMetric.equal_opportunity_difference()
+    def metric(self, classification_metric):
+        return classification_metric.equal_opportunity_difference()
 
 
 class AverageOddsDifference(FairnessScorer):
+    """Class for Average Odds Difference fairness scoring."""
+
     name = "AOD"
     long_name = "Average Odds Difference"
 
-    def metric(self, classificationMetric):
-        return classificationMetric.average_odds_difference()
+    def metric(self, classification_metric):
+        return classification_metric.average_odds_difference()
 
 
 class DisparateImpact(FairnessScorer):
+    """Class for Disparate Impact fairness scoring."""
+
     name = "DI"
     long_name = "Disparate Impact"
 
-    def metric(self, classificationMetric):
-        return classificationMetric.disparate_impact()
+    def metric(self, classification_metric):
+        return classification_metric.disparate_impact()
```

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/modeling/postprocessing.py` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/modeling/postprocessing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,120 +1,126 @@
 import numpy as np
 
 from Orange.base import Learner, Model
 from Orange.data import Table
 
 from aif360.algorithms.postprocessing import EqOddsPostprocessing
 
-
 from orangecontrib.fairness.widgets.utils import (
     table_to_standard_dataset,
     contains_fairness_attributes,
     MISSING_FAIRNESS_ATTRIBUTES,
 )
 
 
 class PostprocessingModel(Model):
+    """Model created and fitted by the PostprocessingLearner, which is used to predict on new data and to postprocess the predictions"""
     def __init__(self, model, postprocessor, learner):
         super().__init__()
         self.model = model
         self.postprocessor = postprocessor
         self.learner = learner
         self.params = vars()
 
     def predict(self, data):
+        """Function used to preprocess, predict and postprocess on new data"""
         if isinstance(data, Table):
-            # Normalize the data
             data = self.learner.preprocess(data)
             # Get the predictions and scores from the model
-            predictions, scores = self.model.predict_storage(data)
+            predictions, scores = self.model(data, ret=Model.ValueProbs)
 
-            # For creating the standard dataset we need to know the encoding the table uses for the class variable, the encoding is ordinal and is the same as the order of values in the domain
+            # For creating the standard dataset we need to know the encoding the table uses for the class variable
+            # This can be found in the domain and is the same as the order of values of the class variable in the domain
+            # This is why we need to add it back to the domain if it was removed
             if not data.domain.class_var:
                 data.domain.class_var = self.original_domain.class_var
             standard_dataset, _, _ = table_to_standard_dataset(data)
             standard_dataset_pred = standard_dataset.copy(deepcopy=True)
             standard_dataset_pred.labels = predictions.reshape(-1, 1)
 
             # Postprocess the predictions
             standard_dataset_pred_transf = self.postprocessor.predict(
                 standard_dataset_pred
             )
 
-            # Return the postprocessed predictions and the scores
             return np.squeeze(standard_dataset_pred_transf.labels, axis=1), scores
 
     def predict_storage(self, data):
         if isinstance(data, Table):
             return self.predict(data)
         else:
             raise TypeError("Data is not of type Table")
 
     def __call__(self, data, ret=Model.Value):
         return self.predict_storage(data)
 
 
 class PostprocessingLearner(Learner):
+    """Learner subclass used to create and fit the model and postprocessor and create the PostprocessingModel"""
     __returns__ = PostprocessingModel
 
     def __init__(self, learner, preprocessors=None, repeatable=None):
         super().__init__(preprocessors=preprocessors)
         self.learner = learner
+        self.callback = None
         self.seed = 42 if repeatable else None
         self.params = vars()
 
     def incompatibility_reason(self, domain):
+        """Function used to check if the domain contains the fairness attributes"""
         if not contains_fairness_attributes(domain):
             return MISSING_FAIRNESS_ATTRIBUTES
 
+    # Fit storage and fit functions were modified to use a Table/Storage object
+    # This is because it's the easiest way to get the domain, and meta attributes
+    # TODO: Should I use the X,Y,W format instead of the table format ? (Same for the model)
     def fit_storage(self, data):
         if isinstance(data, Table):
             self.fit(data)
         else:
             raise TypeError("Data is not of type Table")
 
     def _fit_model(self, data):
         if type(self).fit is Learner.fit:
             return self.fit_storage(data)
         else:
             return self.fit(data)
 
     def fit(self, data):
+        """Function used to preprocess the data, fit the model and the postprocessor"""
         if isinstance(data, Table):
             if not contains_fairness_attributes(data.domain):
                 raise ValueError(MISSING_FAIRNESS_ATTRIBUTES)
-            # Normalize the data
             data = self.preprocess(data)
 
-            # Fit the model TODO: Split the data into train and test data so we can fit the postprocessor on the test data to avoid data leakage
-            # The reason why we use _fit_model here (or predict_storage later) instead of __call__ is because we don't want the learner/model to apply its own preprocessing
-            # The resaon why we use _fit_model here instead of fit_storage is because fit_storage is not implemented for all learners and causes an error
-            model = self.learner._fit_model(data) #<------------ This line causes the error
-            # Because I use fit_storage instead of __call__ I need to set the original domain manually (this is needed for the postprocessor to be compatible with adversarial debiasing)
-            model.original_domain = data.domain
-            predictions, _ = model.predict_storage(
-                data
-            )  # Returns the predictions and the scores
+            # Fit the model to the data
+            # TODO: Split the data into train and test data so we can fit the postprocessor on the test data to avoid data leakage
+            model = self.learner(data, self.callback)
+            # Get the predictions from the model, which will be used to fit the postprocessor
+            predictions = model(data)
 
             # Get the predictions which will be used to fit the postprocessor
             (
                 standard_dataset,
                 privileged_groups,
                 unprivileged_groups,
             ) = table_to_standard_dataset(data)
             standard_dataset_pred = standard_dataset.copy(deepcopy=True)
             standard_dataset_pred.labels = predictions
-            # Fit the postprocessor
+
+            # Create and fit the postprocessor to the predictions
             postprocessor = EqOddsPostprocessing(
                 unprivileged_groups=unprivileged_groups,
                 privileged_groups=privileged_groups,
                 seed=self.seed,
             )
             postprocessor.fit(standard_dataset, standard_dataset_pred)
             return PostprocessingModel(model, postprocessor, self)
         else:
             raise TypeError("Data is not of type Table")
 
-    def __call__(self, data):
+    def __call__(self, data, progress_callback=None):
+        self.callback = progress_callback
+        self.learner.callback = progress_callback
         model = super().__call__(data)
         model.params = self.params
         return model
```

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/__init__.py` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/icons/adversarial_debiasing.svg` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/icons/adversarial_debiasing.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/icons/as_fairness.svg` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/icons/as_fairness.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/icons/combine_preprocessors.svg` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/icons/combine_preprocessors.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/icons/eq_odds_postprocessing.svg` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/icons/eq_odds_postprocessing.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/icons/reweighing.svg` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/icons/reweighing.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/icons/weighted_log_reg.svg` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/icons/weighted_log_reg.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/owadversarialdebiasing.py` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/owadversarialdebiasing.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,63 +8,74 @@
 from Orange.base import Model
 from Orange.widgets.widget import Msg
 
 from AnyQt.QtWidgets import QFormLayout, QLabel
 from AnyQt.QtCore import Qt
 
 from orangecontrib.fairness.modeling.adversarial import AdversarialDebiasingLearner
-from orangecontrib.fairness.widgets.utils import check_fairness_data, check_for_fairness_learner_or_preprocessor
+from orangecontrib.fairness.widgets.utils import (
+    check_fairness_data,
+    check_for_fairness_learner_or_preprocessor,
+)
 
 
 class InterruptException(Exception):
+    """A dummy exception used to interrupt the training process."""
     pass
 
 
 class AdversarialDebiasingRunner:
+    """A class used to run the AdversarialDebiasingLearner in a separate thread and display progress using the callback."""
+
     @staticmethod
     def run(
         learner: AdversarialDebiasingLearner, data: Table, state: TaskState
     ) -> Model:
         if data is None:
             return None
 
-        def callback(i: float, msg: str = None) -> bool:
-            state.set_progress_value(i)
-            # if msg:
-            #     state.set_status(msg)
+        def callback(progress: float, msg: str = None) -> bool:
+            state.set_progress_value(progress)
             if state.is_interruption_requested():
                 raise InterruptException
 
         model = learner(data, progress_callback=callback)
         return model
 
 
 class OWAdversarialDebiasing(ConcurrentWidgetMixin, OWBaseLearner):
+    """A widget used to customize and create the AdversarialDebiasing Learner and/or Model"""
+
     name = "Adversarial Debiasing"
     description = "Adversarial Debiasing classification algorithm with or without fairness constraints."
     icon = "icons/adversarial_debiasing.svg"
-    # priority = 10
+    priority = 30
 
-    # For inputs and outputs we use the same as in OWBaseLearner superclass
     class Inputs(OWBaseLearner.Inputs):
+        """Inputs for the widgets, which are the same as for the super class (Data, Preprocessor)"""
+
         pass
 
     class Outputs(OWBaseLearner.Outputs):
+        """Outputs for the widgets, which are the same as for the super class (Learner, Model)"""
+
         pass
 
-    # Changing the ignored preprocessors message slightly to fit the new widget
-    # This message is shown when the user specifies custom preprocessors
     class Information(OWBaseLearner.Information):
-        ignored_preprocessors = Msg(            
+        """Information shown to the user when the user specifies custom preprocessors"""
+
+        # This was slightly changed from the original to fit the new widget better
+        ignored_preprocessors = Msg(
             "Ignoring default preprocessing. \n"
             "Default preprocessing (scailing), has been replaced with user-specified "
             "preprocessors. Problems may occur if these are inadequate"
-            "for the given data.")
+            "for the given data."
+        )
 
-    # Here we define the learner we want to use, in this case it is the AdversarialDebiasingLearner
+    # We define the learner we want to use
     LEARNER = AdversarialDebiasingLearner
 
     # We define the list of lambdas for the slider
     lambdas = list(
         chain(
             [0],
             [x / 10000 for x in range(1, 10)],
@@ -87,16 +98,16 @@
     lambda_index = Setting(1)
     repeatable = Setting(False)
 
     def __init__(self):
         ConcurrentWidgetMixin.__init__(self)
         OWBaseLearner.__init__(self)
 
-    # We define the UI for the widget
     def add_main_layout(self):
+        """Defines the main UI layout of the widget"""
         form = QFormLayout()
         form.setFieldGrowthPolicy(form.AllNonFixedFieldsGrow)
         form.setLabelAlignment(Qt.AlignLeft)
 
         gui.widgetBox(self.controlArea, True, orientation=form)
         # Spin box for the number of neurons in hidden layers
         form.addRow(
@@ -166,15 +177,14 @@
             minValue=0,
             maxValue=len(self.lambdas) - 1,
             callback=lambda: (self.set_lambda(), self.settings_changed()),
             createLabel=False,
         )
         form.addRow(self.reg_label)
         form.addRow(self.slider)
-        # form.addRow(self.reg_label, self.slider)
         # Checkbox for the replicable training
         form.addRow(
             gui.checkBox(
                 None,
                 self,
                 "repeatable",
                 label="Replicable training",
@@ -183,89 +193,95 @@
             )
         )
         self.set_lambda()
         self._debias_changed()
 
     # ---------Methods related to UI------------
 
-    # Responsible for the text of the lambda slider
     def set_lambda(self):
+        """Responsible for the text of the adversary loss weight slider"""
         self.strength_D = self.lambdas[self.lambda_index]
-        self.reg_label.setText("Adversary Loss Weight, λ={}:".format(self.strength_D))
+        self.reg_label.setText(f"Adversary Loss Weight, λ={self.strength_D}:")
 
-    # Responsible for getting the lambda value from the index of the slider
     @property
     def selected_lambda(self):
+        """Responsible for getting the lambda value from the index of the slider value"""
         return self.lambdas[self.lambda_index]
-    
-    # Responsible for enabling/disabling the slider
+
     def _debias_changed(self):
+        """Responsible for enabling/disabling the slider"""
         self.slider.setEnabled(self.debias)
         self.apply()
 
     # ---------Methods related to inputs--------------
 
     @Inputs.data
     @check_fairness_data
     def set_data(self, data):
+        """
+        Function which is called when the user inputs data, it first checks if the
+        data is valid, cancels the current task and then calls the superclass method.
+        """
         self.cancel()
         super().set_data(data)
 
     @Inputs.preprocessor
     @check_for_fairness_learner_or_preprocessor
     def set_preprocessor(self, preprocessor):
+        """
+        Function which is called when the user inputs a preprocessor, it first checks if the
+        preprocessor is valid, cancels the current task and then calls the superclass method.
+        """
         self.cancel()
         super().set_preprocessor(preprocessor)
 
-    #----------Methods related to the learner/model--------------
+    # ----------Methods related to the learner/model--------------
 
-    # Responsible for creating the learner with the parameters we want
-    # It is called in the superclass by the update_learner method
     def create_learner(self):
+        """
+        Responsible for creating the learner with the parameters we want
+        It is called in the superclass by the update_learner method
+        """
         kwargs = {
             "classifier_num_hidden_units": self.hidden_layers_neurons,
             "num_epochs": self.number_of_epochs,
             "batch_size": self.batch_size,
             "debias": self.debias,
             "adversary_loss_weight": 0,
         }
         if self.repeatable:
             kwargs["seed"] = 42
         if self.debias:
             kwargs["adversary_loss_weight"] = self.selected_lambda
         return self.LEARNER(**kwargs, preprocessors=self.preprocessors)
 
-
-    # This method is called when the input data is changed
-    # it is responsible for fitting the learner and sending the created model to the output
-    # There is also a update_learner method which is called in the apply method of the superclass (along with update_model)
     def update_model(self):
+        """Responsible for starting a new thread, fitting the learner and sending the created model to the output"""
+        # This method is called along with the update_learner method in the apply method of the superclass
+
         self.cancel()
-        # This method will run the run_task method in a separate thread and pass the learner and data as arguments
         if self.data is not None:
             self.start(AdversarialDebiasingRunner.run, self.learner, self.data)
         else:
             self.Outputs.model.send(None)
 
-
     def get_learner_parameters(self):
         parameters = [
             ("Neurons in hidden layers", self.hidden_layers_neurons),
             ("Number of epochs", self.number_of_epochs),
             ("Batch size", self.batch_size),
             ("Use debiasing", self.debias),
         ]
 
         if self.debias:
             parameters.append(("Adversary Loss Weight", self.selected_lambda))
 
         return parameters
 
-    #-----------Methods related to threading and output-------------
-
+    # -----------Methods related to threading and output-------------
 
     def on_partial_result(self, _):
         pass
 
     def on_done(self, result: Model):
         assert isinstance(result, Model) or result is None
         self.model = result
```

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/owasfairness.py` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/owasfairness.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,57 +5,60 @@
 from Orange.widgets.widget import Input, Output, OWWidget
 from Orange.widgets.utils.itemmodels import DomainModel, PyListModel
 from Orange.data import Table, Domain, DiscreteVariable
 from Orange.preprocess import RemoveNaNRows
 
 from Orange.widgets.utils.widgetpreview import WidgetPreview
 
-from orangecontrib.fairness.widgets.utils import check_for_missing_rows
+from orangecontrib.fairness.widgets.utils import check_for_missing_rows, check_data_structure
 
 
 class OWAsFairness(OWWidget):
-    # Define the name and other details of the widget
+    """
+    Converts a dataset to a fairness dataset with marked favorable class values, 
+    protected attributes and priviliged protected attribute values.
+    """
     name = "As Fairness Data"
     description = "Converts a dataset to a fairness dataset with marked favorable class values, protected attributes and priviliged protected attribute values."
     icon = 'icons/as_fairness.svg'
-    # priority = 0
+    priority = 0
 
     want_main_area = False
     resizing_enabled = False
 
-    # Define inputs and outputs
     class Inputs:
+        """Define the inputs to the widgets"""
         data = Input("Data", Table)
 
     class Outputs:
+        """Define the outputs to the widgets"""
         data = Output("Data", Table)
 
-    # Settings: The favorable_class, protected_attribute, and privileged_values are instance variables that are declared as ContextSetting. A ContextSetting is a special type of Setting that Orange remembers for each different context (i.e., input data domain).
+    # Settings: The favorable_class, protected_attribute, and privileged_values are instance variables that are declared as ContextSetting.
+    # A ContextSetting is a special type of Setting that Orange remembers for each different context (i.e., input data domain).
     settingsHandler = DomainContextHandler(
         match_values=DomainContextHandler.MATCH_VALUES_ALL
     )
     protected_attribute = ContextSetting(None)
     favorable_class_value = ContextSetting("")
-    privileged_PA_values = ContextSetting([])
+    privileged_pa_values = ContextSetting([])
     auto_commit: bool = Setting(
         True, schema_only=True
     )  # schema_only -> The setting is saved within the workflow but the default never changes.
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-
         self._data: Optional[Table] = None
-
         favorable_class_items_model = PyListModel(
             iterable=[]
         )  # Here we don't want to display the different attributes/features but the values of the attribute so I couldn't use the DomainModel which stores the features, so I used the PyListModel which can store any type in an iterable
         protected_attribute_model = DomainModel(
             valid_types=(DiscreteVariable,)
         )  # DomainModel stores the domain of the input data and allows us to select a attribute from it. It is tied to the gui.comboBox widget. And Can be accesed by self.controls.protected_attribute.model()
-        privileged_PA_values_model = PyListModel(iterable=[])
+        privileged_pa_values_model = PyListModel(iterable=[])
 
         # Create a box for each of the three variables and populate them with comboboxes and listboxes.
         box = gui.vBox(self.controlArea, "Favorable Class Value", margin=0)
         gui.comboBox(
             box,
             self,
             "favorable_class_value",
@@ -76,34 +79,39 @@
 
         box = gui.vBox(
             self.controlArea, "Privileged Protected Attribute Values", margin=0
         )
         var_list = gui.listView(
             box,
             self,
-            "privileged_PA_values",
-            model=privileged_PA_values_model,
+            "privileged_pa_values",
+            model=privileged_pa_values_model,
             callback=self.commit.deferred,
         )
         var_list.setSelectionMode(var_list.ExtendedSelection)
 
         # A Commit/AutoCommit button which controls if a new signal is sent whenever the user changes the value of a variable or only when the user commits the changes
         self.commit_button = gui.auto_commit(
             self.controlArea, self, "auto_commit", "&Commit", box=False
         )
 
     @Inputs.data
     @check_for_missing_rows
+    @check_data_structure
     def set_data(self, data: Table) -> None:
+        """
+        Function called when new data is received on the input. It is responsible for filling 
+        the widget comboboxes and listboxes with the values contained in the input data.
+        """
         self.closeContext()
         self._data = None
         domain: Optional[Domain] = None
 
         if data is not None:
-            # First impute the data, by removing all rows with missing values
+            # Remove all rows with missing values from the data, because the fairness algorithms can't handle missing values.
             data = RemoveNaNRows()(data)
 
             # Create a table with the same data but a different domain
             self._data = data.transform(data.domain)
             # Copy the attributes from the original data to the new data
             self._data.attributes = data.attributes.copy()
 
@@ -117,105 +125,113 @@
             # Clear the old values of the favorable_class_items_model PyListModel
             if self.controls.favorable_class_value.model():
                 self.controls.favorable_class_value.model().clear()
             # Fill the favorable_class_items_model PyListModel with the values of the class variable of the input data.
             for value in data.domain.class_vars[0].values:
                 self.controls.favorable_class_value.model().append(value)
 
-            # Clear the old values of the privileged_PA_values_model PyListModel
-            if self.controls.privileged_PA_values.model():
-                self.controls.privileged_PA_values.model().clear()
-            # Fill the privileged_PA_values_model PyListModel with the values of the protected attribute variable of the input data.
+            # Clear the old values of the privileged_pa_values_model PyListModel
+            if self.controls.privileged_pa_values.model():
+                self.controls.privileged_pa_values.model().clear()
+            # Fill the privileged_pa_values_model PyListModel with the values of the protected attribute variable of the input data.
             for value in self.controls.protected_attribute.model()[0].values:
-                self.controls.privileged_PA_values.model().append(value)
+                self.controls.privileged_pa_values.model().append(value)
 
             # Set the selected variables to the first variable in the list of variables (in the comboboxes or listboxes)
             self.protected_attribute = (
                 self.controls.protected_attribute.model()[0]
                 if len(self.controls.protected_attribute.model())
                 else None
             )
             self.favorable_class_value = (
                 self.controls.favorable_class_value.model()[0]
                 if len(self.controls.favorable_class_value.model())
                 else None
             )
-            self.privileged_PA_values = (
-                [self.controls.privileged_PA_values.model()[0]]
-                if len(self.controls.privileged_PA_values.model())
+            self.privileged_pa_values = (
+                [self.controls.privileged_pa_values.model()[0]]
+                if len(self.controls.privileged_pa_values.model())
                 else []
             )
 
             # If atleast one value for each variable is selected, then open the context for the widget using the new domain
             # This means that these settings will be remembered the next time the widget receives the same input data.
             # If the input data allready has a known domain, then the saved settings will be used.
             if (
                 self.protected_attribute is not None
                 and self.favorable_class_value is not None
-                and len(self.controls.privileged_PA_values.model()) > 0
+                and len(self.controls.privileged_pa_values.model()) > 0
             ):
                 self.openContext(domain)
 
         # Apply the changes and send the data to the output
-        self.commit.now()  # In the set_data we always have a commit.now() instead of a commit.deferred() because we want to apply the changes as soon as the input data changes.
+        # Here we have commit.now() instead of a commit.deferred() because we want to apply the changes as soon as the input data changes.
+        self.commit.now()
 
     def openContext(self, *a):
+        """
+        Call the openContext function of the parent class and then check if the protected
+        attribute variable or the privileged_pa_values_model PyListModel need to be changed.
+        """
         super().openContext(*a)
-    
-        # Check if the privileged_PA_values match the values of the protected attribute variable
+
+        # Check if the privileged_pa_values match the values of the protected attribute variable
         # This is needed because when loading a old workflow, the domain sometimes doesn't change the protected_attribute
-        if not set(self.privileged_PA_values).issubset(set(self.protected_attribute.values)):
-            self.change_values(clear_PA_values=True)
-        # Check if the self.controls.privileged_PA_values.model matches the values of the protected attribute variable
+        if not set(self.privileged_pa_values).issubset(set(self.protected_attribute.values)):
+            self.change_values(clear_pa_values=True)
+        # Check if the self.controls.privileged_pa_values.model matches the values of the protected attribute variable
         # This is needed when loading an old workflow the displayed values might not match the values of the protected attribute variable
-        elif not set(self.controls.privileged_PA_values.model()).issubset(
+        elif not set(self.controls.privileged_pa_values.model()).issubset(
             set(self.protected_attribute.values)
         ):
-            self.change_values(clear_PA_values=False)
+            self.change_values(clear_pa_values=False)
 
 
+    def change_values(self, clear_pa_values=True) -> None:
+        """
+        This function is normally called when the user changes the protected attribute variable
+        It changes the values of the privileged_pa_values_model PyListModel (the list of displayed privileged PA values) 
+        and the selected privileged PA values (self.privileged_pa_values) to match the values of the new protected attribute variable.
+        """
 
-
-
-    # This function is normally called when the user changes the protected attribute variable
-    # It changes the values of the privileged_PA_values_model PyListModel (the list of displayed privileged PA values) and the selected privileged PA values (self.privileged_PA_values)
-    def change_values(self, clear_PA_values=True) -> None:
         # Change the list of displayed privileged PA values
-        self.controls.privileged_PA_values.model().clear()
+        self.controls.privileged_pa_values.model().clear()
         # Fill the list with the values of the new protected attribute variable
         for value in self.protected_attribute.values:
-            self.controls.privileged_PA_values.model().append(value)
+            self.controls.privileged_pa_values.model().append(value)
 
-        # Change the selected privileged PA values            
-        if clear_PA_values:
-            self.privileged_PA_values = (
-                [self.controls.privileged_PA_values.model()[0]]
-                if len(self.controls.privileged_PA_values.model())
+        # Change the selected privileged PA values
+        if clear_pa_values:
+            self.privileged_pa_values = (
+                [self.controls.privileged_pa_values.model()[0]]
+                if len(self.controls.privileged_pa_values.model())
                 else []
             )
 
+
     # Adding the protected attribute and favorable class value as attributes to the data domain
     def as_fairness_data(self, data: Table) -> Optional[Table]:
+        """This function adds the protected attribute and favorable class value as attributes to the data domain"""
         if (
             not self.protected_attribute
             or not self.favorable_class_value
-            or not self.privileged_PA_values
+            or not self.privileged_pa_values
             or not data
         ):
             return None
 
         old_domain = data.domain
 
         # Create the new attribute or copy the old ones
         new_attributes = []
         for attribute in old_domain.attributes:
-            # If the attribute is the protected attribute, then create a new attribute with the same values but add the privileged_PA_values attribute
+            # If the attribute is the protected attribute, then create a new attribute with the same values but add the privileged_pa_values attribute
             if attribute.name == self.protected_attribute.name:
                 new_attr = attribute.copy()
-                new_attr.attributes["privileged_PA_values"] = self.privileged_PA_values
+                new_attr.attributes["privileged_pa_values"] = self.privileged_pa_values
             # Else just copy the attribute
             else:
                 new_attr = attribute
             new_attributes.append(new_attr)
 
         # Create new class_var
         new_class_var = old_domain.class_var.copy()
@@ -223,18 +239,20 @@
 
         new_domain = Domain(new_attributes, new_class_var, old_domain.metas)
 
         # Create a new table with the new domain
         new_data = data.transform(new_domain)
         return new_data
 
-    # This function is called when the user changes the value of the comboboxes or listboxes
-    # It changes the data attributes and outputs the data
     @gui.deferred  # The defered allows us to only call the function once the user has stopped changing the values of the comboboxes or listboxes and "Applies" the changes
     def commit(self) -> None:
+        """
+        This function is called when the user changes the value of the comboboxes or listboxes.
+        It changes the data attributes and outputs the data
+        """
         data = None
         if self._data is not None:
             data = self.as_fairness_data(self._data)
         self.Outputs.data.send(data)
 
 
 if __name__ == "__main__":
```

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/owcombinepreprocessors.py` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/owcombinepreprocessors.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,57 +2,60 @@
 
 from Orange.widgets import gui
 from Orange.widgets.widget import Input, Output, OWWidget
 from Orange.preprocess.preprocess import Preprocess, PreprocessorList
 
 
 class OWCombinePreprocessors(OWWidget):
+    """Widget for combining 2 preprocessors into one so it can be used as input for other widgets."""
+
     name = "Combine Preprocessors"
     description = "Combine multiple preprocessors into one."
     icon = "icons/combine_preprocessors.svg"
-    # priority = 0
+    priority = 60
 
     want_control_area = False
     resizing_enabled = False
 
     class Inputs:
+        """Input for the widget - two preprocessors or preprocessor lists."""
+
         first_preprocessor = Input("First Preprocessor", Preprocess)
         second_preprocessor = Input("Second Preprocessor", Preprocess)
 
     class Outputs:
+        """Output for the widget - combined preprocessor."""
+
         preprocessor = Output("Preprocessor", Preprocess)
 
     def __init__(self):
         self.preprocessor_list = []
         self.first_preprocessor = None
         self.second_preprocessor = None
-        
+
         super().__init__()
 
         box = gui.vBox(self.mainArea, "Info")
         gui.widgetLabel(
             box,
             "This widgets allows you to combine two preprocessors into one and use it as input for other widgets.",
         )
 
-
     @Inputs.first_preprocessor
     def set_first_preprocessor(self, preprocessor: Optional[Preprocess]) -> None:
+        """Storing the preprocessor entered in the first input."""
         self.first_preprocessor = preprocessor
 
     @Inputs.second_preprocessor
     def set_second_preprocessor(self, preprocessor: Optional[Preprocess]) -> None:
+        """Storing the preprocessor entered in the second input."""
         self.second_preprocessor = preprocessor
-        
 
     def handleNewSignals(self):
+        """Combining the two preprocessors into one and sending it as output."""
         self.preprocessor_list = []
         if self.first_preprocessor is not None:
             self.preprocessor_list.append(self.first_preprocessor)
         if self.second_preprocessor is not None:
             self.preprocessor_list.append(self.second_preprocessor)
 
         self.Outputs.preprocessor.send(PreprocessorList(self.preprocessor_list))
-        
-
-
-
```

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/owdatasetbias.py` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/owdatasetbias.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,35 +6,41 @@
 
 from aif360.metrics import BinaryLabelDatasetMetric
 
 from orangecontrib.fairness.widgets.utils import table_to_standard_dataset, check_fairness_data
 
 
 class OWDatasetBias(OWWidget):
+    """
+    Widget for computing the fairness metrics (bias) of a dataset.
+    More specifically, it computes the disparate impact and statistical parity difference metrics for the dataset.
+    """
     name = "Dataset Bias"
     description = "Computes the bias of a dataset. More specifically, it computes the disparate impact and statistical parity difference metrics for the dataset."
     icon = "icons/dataset_bias.svg"
-    # priority = 0
+    priority = 10
 
     want_control_area = False
     resizing_enabled = False
 
     class Inputs:
+        """Input for the widget - dataset."""
         data = Input("Data", Table)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         box = gui.vBox(self.mainArea, "Bias")
         self.disparate_impact_label = gui.label(box, self, "No data detected.")
         self.statistical_parity_difference_label = gui.label(box, self, "")
 
     @Inputs.data
     @check_fairness_data
     def set_data(self, data: Optional[Table]) -> None:
+        """Computes the bias of the dataset and displays it on the widget."""
         if (
             not data
         ):
             self.disparate_impact_label.setText("No data detected.")
             self.statistical_parity_difference_label.setText("")
             return
```

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/owequalizedodds.py` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/tests/test_owdatasetbias.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,65 @@
-from Orange.base import Learner
-from Orange.data import Table
-from Orange.widgets.settings import Setting
-from Orange.widgets.utils.owlearnerwidget import OWBaseLearner
-from Orange.widgets.widget import Input
-from Orange.widgets import gui
-
-from AnyQt.QtWidgets import QFormLayout
-from AnyQt.QtCore import Qt
-
-from orangecontrib.fairness.modeling.postprocessing import PostprocessingLearner
-from orangecontrib.fairness.widgets.utils import check_fairness_data, check_for_fairness_learner_or_preprocessor
-
-
-class OWEqualizedOdds(OWBaseLearner):
-    name = "Equalized Odds Postprocessing"
-    description = "Postprocessing fairness algorithm which changes the predictions of a classifier to satisfy equalized odds."
-    icon = "icons/eq_odds_postprocessing.svg"
-    # priority = 10
-
-    LEARNER = PostprocessingLearner
-    repeatable = Setting(True)
-
-    class Inputs(OWBaseLearner.Inputs):
-        learner = Input("Learner", Learner)
-
-    def __init__(self):
-        self.normal_learner: Learner = None
-        super().__init__()
-
-    def add_main_layout(self):
-        form = QFormLayout()
-        form.setFieldGrowthPolicy(form.AllNonFixedFieldsGrow)
-        form.setLabelAlignment(Qt.AlignLeft)
-        gui.widgetBox(self.controlArea, True, orientation=form)
-        form.addRow(
-            gui.checkBox(
-                None,
-                self,
-                "repeatable",
-                label="Replicable training",
-                callback=self.settings_changed,
-                attribute=Qt.WA_LayoutUsesWidgetRect,
-            )
+import os
+import unittest
+
+from Orange.data.table import Table
+from Orange.widgets.tests.base import WidgetTest
+from Orange.widgets.tests.utils import simulate
+from Orange.widgets.utils.itemmodels import select_rows
+
+from orangecontrib.fairness.widgets.owasfairness import OWAsFairness
+from orangecontrib.fairness.widgets.owdatasetbias import OWDatasetBias
+from orangecontrib.fairness.widgets.tests.utils import as_fairness_setup
+
+
+class TestOWDatasetBias(WidgetTest):
+    def setUp(self) -> None:
+        self.test_data_path = "https://datasets.biolab.si/core/adult.tab"
+        self.widget = self.create_widget(OWDatasetBias)
+        self.as_fairness = self.create_widget(OWAsFairness)
+
+        self.assertEqual(self.widget.disparate_impact_label.text(), "No data detected.")
+        self.assertEqual(self.widget.statistical_parity_difference_label.text(), "")
+
+    def test_no_data(self):
+        """Check that the widget doesn't crash on empty data"""
+        self.send_signal(self.widget.Inputs.data, None)
+        self.assertEqual(self.widget.disparate_impact_label.text(), "No data detected.")
+        self.assertEqual(self.widget.statistical_parity_difference_label.text(), "")
+
+    def test_incorrect_input_data(self):
+        """Check that the widget displays an error message when the input data does not have the 'AsFairness' attributes"""
+        test_data = Table(self.test_data_path)
+        self.send_signal(self.widget.Inputs.data, test_data)
+        self.assertTrue(self.widget.Error.missing_fairness_data.is_shown())
+
+    def test_input_as_fairness_data(self):
+        """Check that the widget works with data from the as fairness widget"""
+        test_data = as_fairness_setup(self)
+        self.send_signal(
+            self.as_fairness.Inputs.data,
+            test_data,
+        )
+        simulate.combobox_activate_item(
+            self.as_fairness.controls.favorable_class_value, ">50K"
+        )
+        simulate.combobox_activate_item(
+            self.as_fairness.controls.protected_attribute, "sex"
         )
+        select_rows(self.as_fairness.controls.privileged_pa_values, [1])
+        output_data = self.get_output(self.as_fairness.Outputs.data)
 
-    @Inputs.data
-    @check_fairness_data
-    def set_data(self, data: Table):
-        super().set_data(data)
-
-
-    @Inputs.learner
-    @check_for_fairness_learner_or_preprocessor
-    def set_learner(self, learner: Learner):
-        self.normal_learner = learner
-        if learner is not None:
-            self.learner_name = f"Equalized Odds: {learner.name}"
-
-    @Inputs.preprocessor
-    @check_for_fairness_learner_or_preprocessor
-    def set_preprocessor(self, preprocessor):
-        super().set_preprocessor(preprocessor)
-
-
-    def create_learner(self):
-        if not self.normal_learner:
-            return None
-        return self.LEARNER(
-            self.normal_learner,
-            preprocessors=self.preprocessors,
-            repeatable=self.repeatable,
+        self.send_signal(self.widget.Inputs.data, output_data)
+        self.assertTrue(
+            self.widget.disparate_impact_label.text().startswith(
+                "Disparate Impact (ideal = 1):"
+            )
+        )
+        self.assertTrue(
+            self.widget.statistical_parity_difference_label.text().startswith(
+                "Statistical Parity Difference (ideal = 0):"
+            )
         )
-    
-    def handleNewSignals(self):
-        if not self.normal_learner:
-            return
-        self.update_learner() 
-        if self.data is not None:
-            self.update_model()
 
 
 if __name__ == "__main__":
-    import sys
-    from AnyQt.QtWidgets import QApplication
-    from Orange.classification.logistic_regression import LogisticRegressionLearner
-    from Orange.widgets.evaluate.owpredictions import OWPredictions
-    from Orange.widgets.utils.widgetpreview import WidgetPreview
-
-    WidgetPreview(OWEqualizedOdds).run()
-
-    a = QApplication(sys.argv)
-    table = Table("orangedemo/tests/datasets/adult_race_all.pkl")
-    widget = OWEqualizedOdds()
-    widget.set_data(table)
-    widget.set_learner(LogisticRegressionLearner())
-    learner = widget.create_learner()
-    model = learner(table)
-
-    predictions_widget = OWPredictions()
-    predictions_widget.set_data(table)
-    predictions_widget.insert_predictor(0, model)
-    predictions_widget.handleNewSignals()
+    unittest.main()
```

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/owreweighing.py` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/owreweighing.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,116 +3,132 @@
 from Orange.widgets import gui
 from Orange.widgets.widget import Input, Output, OWWidget
 from Orange.data import Table, Domain, ContinuousVariable
 from Orange.preprocess import preprocess
 
 from aif360.algorithms.preprocessing import Reweighing as ReweighingAlgorithm
 
-from orangecontrib.fairness.widgets.utils import table_to_standard_dataset, check_fairness_data
+from orangecontrib.fairness.widgets.utils import (
+    table_to_standard_dataset,
+    check_fairness_data,
+)
 
 
 class MzCom:
-    # The __init__ method is called when the class is created and can have as many arguments as you want. MzCom(model) creates an instance of the class
-    # The __call__ method is called when the class is called, it must only have one argument, which is the data. MzCom(model)(data) calls the __call__ method of the class
+    """A class used to compute the weights of the rows of a dataset using a allready fitted reweighing algorithm"""
+
     def __init__(self, model, original_domain=None):
         self.original_domain = original_domain
         self.model = model
 
     def __call__(self, data):
-        # For creating a standard dataset we need the "Favorable class values" domain attribute, which may not be present in the data so we need to add it
+        # For creating the standard dataset we need to know the encoding the table uses for the class variable
+        # This can be found in the domain and is the same as the order of values of the class variable in the domain
+        # This is why we need to add it back to the domain if it was removed
         if not data.domain.class_var:
-                data.domain.class_var = self.original_domain.class_var
+            data.domain.class_var = self.original_domain.class_var
         data, _, _ = table_to_standard_dataset(data)
-        # Call the transform method of the model
         data = self.model.transform(data)
-        # Return the weights
         return data.instance_weights
 
     # TODO: Check if this is ok
     InheritEq = True
 
 
-class ReweighingModel():
-    # This class doesn't need an __init__ method because it doesn't need any arguments when it is created
-    # The __call__ method creates an instance of the ReweighingAlgorithm, fits it to the data and returns it
+class ReweighingModel:
+    """A class used to create a ReweighingAlgoritm instance, fitting it to the data and returning it"""
+
     def __call__(self, data):
         (
-            standardDataset,
+            standard_dataset,
             privileged_groups,
             unprivileged_groups,
         ) = table_to_standard_dataset(data)
         reweighing = ReweighingAlgorithm(unprivileged_groups, privileged_groups)
-        reweighing = reweighing.fit(standardDataset)
+        reweighing = reweighing.fit(standard_dataset)
         return reweighing
 
 
 class ReweighingTransform(preprocess.Preprocess):
-    # The __call__ method applies the reweighing algorithm to the data and returns the data with the weights
+    """
+    A class used to add a new column/variable to the data with the weights of the rows of the data computed
+    by the fitted reweighing algorithm stored in the MzCom class instance as a compute_value function
+    """
+
     def __call__(self, data):
-        # Create an instalce of the ReweighingModel, and call the __call__ method with the data as argument
         model = ReweighingModel()(data)
-        # Create a new variable "weights" with the compute_value function, the compute_value function is the MzCom class, which when called calls the transform method of the model
-        weights = ContinuousVariable("weights", compute_value=MzCom(model, original_domain=data.domain))
+        weights = ContinuousVariable(
+            "weights", compute_value=MzCom(model, original_domain=data.domain)
+        )
         # Alternative for the compute_value: compute_value=lambda data, model=model: transf(data, model)
 
         # Add the variable "weights" to the domain of the data
         new_data = data.transform(
             Domain(
                 data.domain.attributes,
                 data.domain.class_vars,
                 data.domain.metas + (weights,),
             )
         )
         return new_data
 
 
 class OWReweighing(OWWidget):
+    """
+    A class used to create a widget for the reweighing algorithm,
+    which can be used to transform a dataset or as a preprocessor for a model.
+    """
+
     name = "Reweighing"
     description = "Applies the reweighing algorithm to a dataset, which adjusts the weights of rows."
-    icon = 'icons/reweighing.svg'
-    # priority = 0
+    icon = "icons/reweighing.svg"
+    priority = 20
 
     want_control_area = False
     resizing_enabled = False
 
-    # Define the inputs and outputs of the widget
     class Inputs:
+        """The inputs of the widget - the dataset"""
+
         data = Input("Data", Table)
 
     class Outputs:
+        """The outputs of the widget - the preprocessed dataset and the preprocessor"""
+
         data = Output("Preprocessed Data", Table)
         preprocessor = Output("Preprocessor", preprocess.Preprocess, dynamic=False)
 
-    # Define the initial state of the widget (constructor)
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.preprocessor = ReweighingTransform()
         self.Outputs.preprocessor.send(self.preprocessor)
 
         box = gui.vBox(self.mainArea, "Info")
         gui.widgetLabel(
             box,
             "This widget applies the reweighing algorithm to a dataset, which adjusts the weights of rows.\nThe input data must have the additional 'AsFairness' attributes and be without any missing values.",
         )
 
         self._data: Optional[Table] = None
 
-    # Define what should happen when the input data is received
     @Inputs.data
     @check_fairness_data
     def set_data(self, data: Optional[Table]) -> None:
+        """Handling the input data by saving it"""
         if not data:
             return
 
         self._data = data
 
     def handleNewSignals(self):
+        """Handling any new signals by applying the reweighing algorithm to the data"""
         self.apply()
 
     def apply(self):
+        """Fitting the reweighing algorithm to the data and sending the preprocessed data and the preprocessor to the output"""
         if self._data is None:
             return
 
         preprocessed_data = self.preprocessor(self._data)
 
         self.Outputs.data.send(preprocessed_data)
         self.Outputs.preprocessor.send(self.preprocessor)
```

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/tests/test_owadversarialdebiasing.py` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/tests/test_owadversarialdebiasing.py`

 * *Files identical despite different names*

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/tests/test_owasfairness.py` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/tests/test_owasfairness.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             self.widget.Inputs.data,
             test_data,
         )
 
         self.assertTrue(self.widget.controls.protected_attribute.count() > 0)
         self.assertTrue(self.widget.controls.favorable_class_value.count() > 0)
         self.assertTrue(
-            self.widget.controls.privileged_PA_values.model().rowCount() > 0
+            self.widget.controls.privileged_pa_values.model().rowCount() > 0
         )
 
     def test_selection(self):
         """Check that the selection works properly"""
         test_data = Table(self.test_data_path)
         self.send_signal(
             self.widget.Inputs.data,
@@ -44,37 +44,37 @@
             self.widget.controls.favorable_class_value, ">50K"
         )
         self.assertEqual(self.widget.favorable_class_value, ">50K")
 
         simulate.combobox_activate_item(self.widget.controls.protected_attribute, "sex")
         self.assertEqual(self.widget.protected_attribute.name, "sex")
 
-        select_rows(self.widget.controls.privileged_PA_values, [1])
-        self.assertEqual(self.widget.privileged_PA_values, ["Male"])
+        select_rows(self.widget.controls.privileged_pa_values, [1])
+        self.assertEqual(self.widget.privileged_pa_values, ["Male"])
 
     def test_output(self):
         """Check that the selection is properly set"""
         test_data = Table(self.test_data_path)
         self.send_signal(
             self.widget.Inputs.data,
             test_data,
         )
 
         simulate.combobox_activate_item(
             self.widget.controls.favorable_class_value, ">50K"
         )
         simulate.combobox_activate_item(self.widget.controls.protected_attribute, "sex")
-        select_rows(self.widget.controls.privileged_PA_values, [1])
+        select_rows(self.widget.controls.privileged_pa_values, [1])
 
         output_data = self.get_output(self.widget.Outputs.data)
 
         self.assertTrue(output_data is not None)
         self.assertTrue("favorable_class_value" in output_data.domain.class_var.attributes)
-        contains_PA_values = False
+        contains_pa_values = False
         for attr in output_data.domain.attributes:
-            if "privileged_PA_values" in attr.attributes:
-                        contains_PA_values = True
-        self.assertTrue(contains_PA_values)
+            if "privileged_pa_values" in attr.attributes:
+                        contains_pa_values = True
+        self.assertTrue(contains_pa_values)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/tests/test_owequalizedodds.py` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/tests/test_owequalizedodds.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 
 class TestOWEqualizedOdds(WidgetTest):
     def setUp(self) -> None:
         self.test_data_path = "https://datasets.biolab.si/core/adult.tab"
         self.widget = self.create_widget(OWEqualizedOdds)
         self.as_fairness = self.create_widget(OWAsFairness)
         self.predictions = self.create_widget(OWPredictions)
-        self.cross_validation = self.create_widget(OWTestAndScore)
+        self.test_and_score = self.create_widget(OWTestAndScore)
 
     def test_no_data(self):
         """Check that the widget doesn't crash on empty data"""
         self.send_signal(self.widget.Inputs.data, None)
 
     def test_compatibility_with_predictions(self):
         """Check that the widget works with the predictions widget"""
         test_data = as_fairness_setup(self)
         self.send_signal(self.widget.Inputs.data, test_data)
-        self.send_signal(self.widget.Inputs.learner, LogisticRegressionLearner())
+        self.send_signal(self.widget.Inputs.input_learner, LogisticRegressionLearner())
         learner = self.widget.create_learner()
         model = learner(test_data)
 
         self.send_signal(
             self.predictions.Inputs.data, test_data, widget=self.predictions
         )
         self.send_signal(
@@ -49,42 +49,42 @@
         self.assertIsNotNone(predictions)
         self.assertIsNotNone(results)
 
     def test_compatibility_with_test_and_score(self):
         """Check that the widget works with the test and score widget"""
         test_data = as_fairness_setup(self)
         self.send_signal(self.widget.Inputs.data, test_data)
-        self.send_signal(self.widget.Inputs.learner, LogisticRegressionLearner())
+        self.send_signal(self.widget.Inputs.input_learner, LogisticRegressionLearner())
         learner = self.widget.create_learner()
 
         self.send_signal(
-            self.cross_validation.Inputs.train_data,
+            self.test_and_score.Inputs.train_data,
             test_data,
-            widget=self.cross_validation,
+            widget=self.test_and_score,
         )
         self.send_signal(
-            self.cross_validation.Inputs.learner, learner, widget=self.cross_validation
+            self.test_and_score.Inputs.learner, learner, widget=self.test_and_score
         )
-        self.wait_until_finished(self.cross_validation, timeout=10000)
+        self.wait_until_finished(self.test_and_score, timeout=20000)
         predictions = self.get_output(
-            self.cross_validation.Outputs.predictions, widget=self.cross_validation
+            self.test_and_score.Outputs.predictions, widget=self.test_and_score
         )
         results = self.get_output(
-            self.cross_validation.Outputs.evaluations_results,
-            widget=self.cross_validation,
+            self.test_and_score.Outputs.evaluations_results,
+            widget=self.test_and_score,
         )
 
         self.assertIsNotNone(predictions)
         self.assertIsNotNone(results)
 
     def test_effecitveness(self):
         """Check that the widget works with the predictions widget"""
         test_data = as_fairness_setup(self)
         self.send_signal(self.widget.Inputs.data, test_data)
-        self.send_signal(self.widget.Inputs.learner, LogisticRegressionLearner())
+        self.send_signal(self.widget.Inputs.input_learner, LogisticRegressionLearner())
         learner = self.widget.create_learner()
         model = learner(test_data)
 
         # Predictions with postprocessing
         self.send_signal(
             self.predictions.Inputs.data, test_data, widget=self.predictions
         )
```

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/tests/test_owreweighing.py` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/tests/test_owreweighing.py`

 * *Files identical despite different names*

### Comparing `Orange3-Fairness-0.1.0/orangecontrib/fairness/widgets/tests/utils.py` & `Orange3-Fairness-0.1.1/orangecontrib/fairness/widgets/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     )
     simulate.combobox_activate_item(
         self.as_fairness.controls.favorable_class_value, ">50K"
     )
     simulate.combobox_activate_item(
         self.as_fairness.controls.protected_attribute, "sex"
     )
-    select_rows(self.as_fairness.controls.privileged_PA_values, [1])
+    select_rows(self.as_fairness.controls.privileged_pa_values, [1])
     output_data = self.get_output(self.as_fairness.Outputs.data)
     return output_data
 
 
 def print_metrics(results, bias=True):
     print(f"ROC AUC: {scoring.AUC(results)}")
     print(f"CA: {scoring.CA(results)}")
```

### Comparing `Orange3-Fairness-0.1.0/setup.py` & `Orange3-Fairness-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup, find_packages
 from os import path
 
-LONG_DESCRIPTION = open(
-    path.join(path.dirname(__file__), "README.pypi"), "r", encoding="utf-8"
-).read()
+try:
+    LONG_DESCRIPTION = open(
+        path.join(path.dirname(__file__), "README.pypi"), "r", encoding="utf-8"
+    ).read()
+except FileNotFoundError:
+    LONG_DESCRIPTION = ""
 
 setup(
     name="Orange3-Fairness",
-    version="0.1.0",
+    version="0.1.1",
     author="Bioinformatics Laboratory, FRI UL",
     author_email="contact@orange.biolab.si",
     maintainer="Zan Mervic",
     description="Orange3 add-on for fairness-aware machine learning.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/x-rst',
     license="GPL3+",
```

