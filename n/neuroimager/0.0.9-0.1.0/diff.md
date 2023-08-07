# Comparing `tmp/neuroimager-0.0.9.tar.gz` & `tmp/neuroimager-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroimager-0.0.9.tar", last modified: Thu Aug  3 14:53:56 2023, max compression
+gzip compressed data, was "neuroimager-0.1.0.tar", last modified: Mon Aug  7 03:34:22 2023, max compression
```

## Comparing `neuroimager-0.0.9.tar` & `neuroimager-0.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.322424 neuroimager-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 14:53:46.000000 neuroimager-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-08-03 14:53:56.322424 neuroimager-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-08-03 14:53:46.000000 neuroimager-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.310424 neuroimager-0.0.9/neuroimager/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.318424 neuroimager-0.0.9/neuroimager/pipes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/pipes/brainage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/pipes/cca.py
--rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/pipes/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/pipes/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    39138 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/pipes/hmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    30640 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/pipes/task_fmri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.318424 neuroimager-0.0.9/neuroimager/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/plotting/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/plotting/styler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.318424 neuroimager-0.0.9/neuroimager/preproc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/preproc/decompose.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/preproc/prep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.318424 neuroimager-0.0.9/neuroimager/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/stats/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/stats/perm_ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.322424 neuroimager-0.0.9/neuroimager/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/utils/atlas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/utils/fc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/utils/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-03 14:53:46.000000 neuroimager-0.0.9/neuroimager/utils/rbload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:53:56.314424 neuroimager-0.0.9/neuroimager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-08-03 14:53:56.000000 neuroimager-0.0.9/neuroimager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-03 14:53:56.000000 neuroimager-0.0.9/neuroimager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:53:56.000000 neuroimager-0.0.9/neuroimager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 14:53:56.000000 neuroimager-0.0.9/neuroimager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 14:53:56.000000 neuroimager-0.0.9/neuroimager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:53:56.322424 neuroimager-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-03 14:53:46.000000 neuroimager-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:34:22.351490 neuroimager-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 03:34:02.000000 neuroimager-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-08-07 03:34:22.351490 neuroimager-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-08-07 03:34:02.000000 neuroimager-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:34:22.347489 neuroimager-0.1.0/neuroimager/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:34:22.347489 neuroimager-0.1.0/neuroimager/pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/pipes/brainage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/pipes/cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/pipes/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/pipes/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39138 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/pipes/hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30640 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/pipes/task_fmri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:34:22.347489 neuroimager-0.1.0/neuroimager/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/plotting/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/plotting/styler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:34:22.347489 neuroimager-0.1.0/neuroimager/preproc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/preproc/decompose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/preproc/prep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:34:22.347489 neuroimager-0.1.0/neuroimager/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/stats/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/stats/perm_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:34:22.351490 neuroimager-0.1.0/neuroimager/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/utils/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/utils/fc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/utils/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-07 03:34:03.000000 neuroimager-0.1.0/neuroimager/utils/rbload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:34:22.347489 neuroimager-0.1.0/neuroimager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-08-07 03:34:22.000000 neuroimager-0.1.0/neuroimager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-07 03:34:22.000000 neuroimager-0.1.0/neuroimager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 03:34:22.000000 neuroimager-0.1.0/neuroimager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-07 03:34:22.000000 neuroimager-0.1.0/neuroimager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 03:34:22.000000 neuroimager-0.1.0/neuroimager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 03:34:22.351490 neuroimager-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-07 03:34:03.000000 neuroimager-0.1.0/setup.py
```

### Comparing `neuroimager-0.0.9/LICENSE` & `neuroimager-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/PKG-INFO` & `neuroimager-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroimager
-Version: 0.0.9
+Version: 0.1.0
 Summary: A collection of utilities used for MRI data analysis
 Home-page: https://github.com/Wetiqe/neuroimager
 Author: Wetiqe
 Author-email: jzni132134@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neuroimager-0.0.9/README.md` & `neuroimager-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/pipes/brainage.py` & `neuroimager-0.1.0/neuroimager/pipes/brainage.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/pipes/explore.py` & `neuroimager-0.1.0/neuroimager/pipes/explore.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/pipes/graph.py` & `neuroimager-0.1.0/neuroimager/pipes/graph.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/pipes/hmm.py` & `neuroimager-0.1.0/neuroimager/pipes/hmm.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/pipes/task_fmri.py` & `neuroimager-0.1.0/neuroimager/pipes/task_fmri.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/plotting/plot.py` & `neuroimager-0.1.0/neuroimager/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/plotting/styler.py` & `neuroimager-0.1.0/neuroimager/plotting/styler.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/preproc/decompose.py` & `neuroimager-0.1.0/neuroimager/preproc/decompose.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/preproc/prep.py` & `neuroimager-0.1.0/neuroimager/preproc/prep.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/stats/correlation.py` & `neuroimager-0.1.0/neuroimager/stats/correlation.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/stats/perm_ttest.py` & `neuroimager-0.1.0/neuroimager/stats/perm_ttest.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/utils/__init__.py` & `neuroimager-0.1.0/neuroimager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/utils/atlas.py` & `neuroimager-0.1.0/neuroimager/utils/atlas.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/utils/fc.py` & `neuroimager-0.1.0/neuroimager/utils/fc.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/utils/ml.py` & `neuroimager-0.1.0/neuroimager/utils/ml.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager/utils/rbload.py` & `neuroimager-0.1.0/neuroimager/utils/rbload.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/neuroimager.egg-info/PKG-INFO` & `neuroimager-0.1.0/neuroimager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroimager
-Version: 0.0.9
+Version: 0.1.0
 Summary: A collection of utilities used for MRI data analysis
 Home-page: https://github.com/Wetiqe/neuroimager
 Author: Wetiqe
 Author-email: jzni132134@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neuroimager-0.0.9/neuroimager.egg-info/SOURCES.txt` & `neuroimager-0.1.0/neuroimager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.9/setup.py` & `neuroimager-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 current_dir = os.path.abspath(os.path.dirname(__file__))
 # Read the contents of your README file
 with open(os.path.join(current_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="neuroimager",
-    version="0.0.9",
+    version="0.1.0",
     description="A collection of utilities used for MRI data analysis",
     author="Wetiqe",
     author_email="jzni132134@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Wetiqe/neuroimager",
     packages=find_packages(),
```

