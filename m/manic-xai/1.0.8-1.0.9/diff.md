# Comparing `tmp/manic-xai-1.0.8.tar.gz` & `tmp/manic-xai-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manic-xai-1.0.8.tar", last modified: Wed Aug  2 20:42:57 2023, max compression
+gzip compressed data, was "manic-xai-1.0.9.tar", last modified: Wed Aug  2 20:44:11 2023, max compression
```

## Comparing `manic-xai-1.0.8.tar` & `manic-xai-1.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:42:57.005525 manic-xai-1.0.8/
--rw-r--r--   0 craigpirie   (501) staff       (20)     1064 2023-07-26 15:54:10.000000 manic-xai-1.0.8/LICENSE
--rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-08-02 20:42:57.005057 manic-xai-1.0.8/PKG-INFO
--rw-r--r--   0 craigpirie   (501) staff       (20)     2721 2023-07-26 17:17:12.000000 manic-xai-1.0.8/README.md
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:42:56.995941 manic-xai-1.0.8/manic/
--rw-r--r--   0 craigpirie   (501) staff       (20)     2845 2023-08-01 23:21:50.000000 manic-xai-1.0.8/manic/Baseline.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     6369 2023-08-02 20:20:39.000000 manic-xai-1.0.8/manic/Crossover.py
--rw-r--r--   0 craigpirie   (501) staff       (20)    10944 2023-08-02 17:39:33.000000 manic-xai-1.0.8/manic/Disagreement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     6987 2023-08-01 23:28:50.000000 manic-xai-1.0.8/manic/Evaluation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     6644 2023-08-02 20:15:27.000000 manic-xai-1.0.8/manic/GeneticAlgorithm.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     7248 2023-08-02 20:37:56.000000 manic-xai-1.0.8/manic/Manic.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     5614 2023-08-01 23:32:04.000000 manic-xai-1.0.8/manic/Mutation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1563 2023-08-02 17:56:19.000000 manic-xai-1.0.8/manic/Replacement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     7213 2023-08-02 17:44:55.000000 manic-xai-1.0.8/manic/Selection.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1824 2023-08-01 22:52:00.000000 manic-xai-1.0.8/manic/Termination.py
--rw-r--r--   0 craigpirie   (501) staff       (20)    10672 2023-08-02 20:09:42.000000 manic-xai-1.0.8/manic/Utility.py
--rw-r--r--   0 craigpirie   (501) staff       (20)      496 2023-08-02 20:42:12.000000 manic-xai-1.0.8/manic/__init__.py
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:42:57.001396 manic-xai-1.0.8/manic/__tests__/
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 23:28:48.000000 manic-xai-1.0.8/manic/__tests__/__init__.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:16.000000 manic-xai-1.0.8/manic/__tests__/test_baseline.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1905 2023-07-28 17:41:26.000000 manic-xai-1.0.8/manic/__tests__/test_crossover.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     5034 2023-07-28 16:53:03.000000 manic-xai-1.0.8/manic/__tests__/test_disagreement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:35.000000 manic-xai-1.0.8/manic/__tests__/test_evaluation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-31 01:59:12.000000 manic-xai-1.0.8/manic/__tests__/test_genetic_algorithm.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     1269 2023-07-26 17:02:40.000000 manic-xai-1.0.8/manic/__tests__/test_manic.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     4387 2023-07-28 14:27:49.000000 manic-xai-1.0.8/manic/__tests__/test_mutation.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-08-01 22:24:47.000000 manic-xai-1.0.8/manic/__tests__/test_replacement.py
--rw-r--r--   0 craigpirie   (501) staff       (20)     9470 2023-07-28 15:04:45.000000 manic-xai-1.0.8/manic/__tests__/test_selection.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:43.000000 manic-xai-1.0.8/manic/__tests__/test_termination.py
--rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:46:05.000000 manic-xai-1.0.8/manic/__tests__/test_utility.py
-drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:42:57.004475 manic-xai-1.0.8/manic_xai.egg-info/
--rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-08-02 20:42:56.000000 manic-xai-1.0.8/manic_xai.egg-info/PKG-INFO
--rw-r--r--   0 craigpirie   (501) staff       (20)      834 2023-08-02 20:42:56.000000 manic-xai-1.0.8/manic_xai.egg-info/SOURCES.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)        1 2023-08-02 20:42:56.000000 manic-xai-1.0.8/manic_xai.egg-info/dependency_links.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)       69 2023-08-02 20:42:56.000000 manic-xai-1.0.8/manic_xai.egg-info/requires.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)        6 2023-08-02 20:42:56.000000 manic-xai-1.0.8/manic_xai.egg-info/top_level.txt
--rw-r--r--   0 craigpirie   (501) staff       (20)       38 2023-08-02 20:42:57.005661 manic-xai-1.0.8/setup.cfg
--rw-r--r--   0 craigpirie   (501) staff       (20)     1041 2023-08-02 20:42:53.000000 manic-xai-1.0.8/setup.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:44:11.422202 manic-xai-1.0.9/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1064 2023-07-26 15:54:10.000000 manic-xai-1.0.9/LICENSE
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-08-02 20:44:11.421716 manic-xai-1.0.9/PKG-INFO
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2721 2023-07-26 17:17:12.000000 manic-xai-1.0.9/README.md
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:44:11.413063 manic-xai-1.0.9/manic/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     2845 2023-08-01 23:21:50.000000 manic-xai-1.0.9/manic/Baseline.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     6369 2023-08-02 20:20:39.000000 manic-xai-1.0.9/manic/Crossover.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)    10944 2023-08-02 17:39:33.000000 manic-xai-1.0.9/manic/Disagreement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     6987 2023-08-01 23:28:50.000000 manic-xai-1.0.9/manic/Evaluation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     6644 2023-08-02 20:15:27.000000 manic-xai-1.0.9/manic/GeneticAlgorithm.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     7248 2023-08-02 20:37:56.000000 manic-xai-1.0.9/manic/Manic.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5614 2023-08-01 23:32:04.000000 manic-xai-1.0.9/manic/Mutation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1563 2023-08-02 17:56:19.000000 manic-xai-1.0.9/manic/Replacement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     7213 2023-08-02 17:44:55.000000 manic-xai-1.0.9/manic/Selection.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1824 2023-08-01 22:52:00.000000 manic-xai-1.0.9/manic/Termination.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)    10672 2023-08-02 20:09:42.000000 manic-xai-1.0.9/manic/Utility.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)      496 2023-08-02 20:42:12.000000 manic-xai-1.0.9/manic/__init__.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:44:11.418657 manic-xai-1.0.9/manic/__tests__/
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-27 23:28:48.000000 manic-xai-1.0.9/manic/__tests__/__init__.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:16.000000 manic-xai-1.0.9/manic/__tests__/test_baseline.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1905 2023-07-28 17:41:26.000000 manic-xai-1.0.9/manic/__tests__/test_crossover.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     5034 2023-07-28 16:53:03.000000 manic-xai-1.0.9/manic/__tests__/test_disagreement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:35.000000 manic-xai-1.0.9/manic/__tests__/test_evaluation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-31 01:59:12.000000 manic-xai-1.0.9/manic/__tests__/test_genetic_algorithm.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1269 2023-07-26 17:02:40.000000 manic-xai-1.0.9/manic/__tests__/test_manic.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     4387 2023-07-28 14:27:49.000000 manic-xai-1.0.9/manic/__tests__/test_mutation.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-08-01 22:24:47.000000 manic-xai-1.0.9/manic/__tests__/test_replacement.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)     9470 2023-07-28 15:04:45.000000 manic-xai-1.0.9/manic/__tests__/test_selection.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:45:43.000000 manic-xai-1.0.9/manic/__tests__/test_termination.py
+-rw-r--r--   0 craigpirie   (501) staff       (20)        0 2023-07-28 17:46:05.000000 manic-xai-1.0.9/manic/__tests__/test_utility.py
+drwxr-xr-x   0 craigpirie   (501) staff       (20)        0 2023-08-02 20:44:11.421095 manic-xai-1.0.9/manic_xai.egg-info/
+-rw-r--r--   0 craigpirie   (501) staff       (20)     3261 2023-08-02 20:44:11.000000 manic-xai-1.0.9/manic_xai.egg-info/PKG-INFO
+-rw-r--r--   0 craigpirie   (501) staff       (20)      834 2023-08-02 20:44:11.000000 manic-xai-1.0.9/manic_xai.egg-info/SOURCES.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)        1 2023-08-02 20:44:11.000000 manic-xai-1.0.9/manic_xai.egg-info/dependency_links.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)       69 2023-08-02 20:44:11.000000 manic-xai-1.0.9/manic_xai.egg-info/requires.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)        6 2023-08-02 20:44:11.000000 manic-xai-1.0.9/manic_xai.egg-info/top_level.txt
+-rw-r--r--   0 craigpirie   (501) staff       (20)       38 2023-08-02 20:44:11.422416 manic-xai-1.0.9/setup.cfg
+-rw-r--r--   0 craigpirie   (501) staff       (20)     1041 2023-08-02 20:43:55.000000 manic-xai-1.0.9/setup.py
```

### Comparing `manic-xai-1.0.8/LICENSE` & `manic-xai-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/PKG-INFO` & `manic-xai-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manic-xai
-Version: 1.0.8
+Version: 1.0.9
 Summary: Genetic Algorithm for Generating Metacounterfactual Explanations
 Home-page: https://github.com/craigybaeb/MANIC
 Author: Craig Pirie
 Author-email: c.pirie11@rgu.ac.uk
 Keywords: manic,metacounterfactual,counterfactual,xai,explanation,aggregation,disagreement,agreement
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `manic-xai-1.0.8/README.md` & `manic-xai-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/Baseline.py` & `manic-xai-1.0.9/manic/Baseline.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/Crossover.py` & `manic-xai-1.0.9/manic/Crossover.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/Disagreement.py` & `manic-xai-1.0.9/manic/Disagreement.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/Evaluation.py` & `manic-xai-1.0.9/manic/Evaluation.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/GeneticAlgorithm.py` & `manic-xai-1.0.9/manic/GeneticAlgorithm.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/Manic.py` & `manic-xai-1.0.9/manic/Manic.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/Mutation.py` & `manic-xai-1.0.9/manic/Mutation.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/Replacement.py` & `manic-xai-1.0.9/manic/Replacement.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/Selection.py` & `manic-xai-1.0.9/manic/Selection.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/Termination.py` & `manic-xai-1.0.9/manic/Termination.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/Utility.py` & `manic-xai-1.0.9/manic/Utility.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/__tests__/test_crossover.py` & `manic-xai-1.0.9/manic/__tests__/test_crossover.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/__tests__/test_disagreement.py` & `manic-xai-1.0.9/manic/__tests__/test_disagreement.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/__tests__/test_manic.py` & `manic-xai-1.0.9/manic/__tests__/test_manic.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/__tests__/test_mutation.py` & `manic-xai-1.0.9/manic/__tests__/test_mutation.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic/__tests__/test_selection.py` & `manic-xai-1.0.9/manic/__tests__/test_selection.py`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/manic_xai.egg-info/PKG-INFO` & `manic-xai-1.0.9/manic_xai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manic-xai
-Version: 1.0.8
+Version: 1.0.9
 Summary: Genetic Algorithm for Generating Metacounterfactual Explanations
 Home-page: https://github.com/craigybaeb/MANIC
 Author: Craig Pirie
 Author-email: c.pirie11@rgu.ac.uk
 Keywords: manic,metacounterfactual,counterfactual,xai,explanation,aggregation,disagreement,agreement
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `manic-xai-1.0.8/manic_xai.egg-info/SOURCES.txt` & `manic-xai-1.0.9/manic_xai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manic-xai-1.0.8/setup.py` & `manic-xai-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="manic-xai",
-    version='1.0.8',
+    version='1.0.9',
     author="Craig Pirie",
     author_email="c.pirie11@rgu.ac.uk",
     description="Genetic Algorithm for Generating Metacounterfactual Explanations",
     url = "https://github.com/craigybaeb/MANIC",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

