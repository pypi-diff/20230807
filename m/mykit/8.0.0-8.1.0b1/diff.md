# Comparing `tmp/mykit-8.0.0.tar.gz` & `tmp/mykit-8.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-vek498fw/mykit-8.0.0.tar", last modified: Sun Aug  6 20:00:55 2023, max compression
+gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-dvghywvd/mykit-8.1.0b1.tar", last modified: Mon Aug  7 15:58:13 2023, max compression
```

## Comparing `mykit-8.0.0.tar` & `mykit-8.1.0b1.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:55.000000 mykit-8.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-06 20:00:46.000000 mykit-8.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-06 20:00:55.000000 mykit-8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-06 20:00:46.000000 mykit-8.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit/app/
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit/app/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/app/architecture/eventdriven.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/app/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/app/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit/app/complex/
--rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/app/complex/biplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/app/complex/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/app/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/app/slider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit/kit/
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/kit/color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit/kit/fast_visualizations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit/kit/fast_visualizations/static/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/kit/fast_visualizations/static/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/kit/ffmpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit/kit/keycrate/
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/kit/keycrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/kit/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit/kit/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/kit/neuralnet/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/kit/neuralnet/genetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/kit/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/kit/pLog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/kit/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/kit/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/kit/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit/rec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/rec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:46.000000 mykit-8.0.0/mykit/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 20:00:55.000000 mykit-8.0.0/mykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-06 20:00:46.000000 mykit-8.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-06 20:00:55.000000 mykit-8.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-06 20:00:46.000000 mykit-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.000000 mykit-8.1.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-07 15:58:06.000000 mykit-8.1.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-08-07 15:58:13.000000 mykit-8.1.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-07 15:58:06.000000 mykit-8.1.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit/app/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/app/architecture/eventdriven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/app/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/app/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit/app/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/app/complex/biplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/app/complex/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/app/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/app/slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit/ghactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/ghactions/eLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/ghactions/set_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/kit/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit/kit/fast_visualizations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit/kit/fast_visualizations/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/kit/fast_visualizations/static/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/kit/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit/kit/keycrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/kit/keycrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/kit/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit/kit/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/kit/neuralnet/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/kit/neuralnet/genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/kit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/kit/pLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/kit/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/kit/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/kit/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit/rec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/rec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:06.000000 mykit-8.1.0b1/mykit/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 15:58:13.000000 mykit-8.1.0b1/mykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-07 15:58:07.000000 mykit-8.1.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-07 15:58:13.000000 mykit-8.1.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-07 15:58:06.000000 mykit-8.1.0b1/setup.py
```

### Comparing `mykit-8.0.0/LICENSE` & `mykit-8.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/PKG-INFO` & `mykit-8.1.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 8.0.0
+Version: 8.1.0b1
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/mykit/docs
 Project-URL: Report bugs, https://github.com/nvfp/mykit/issues
```

### Comparing `mykit-8.0.0/README.md` & `mykit-8.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/__init__.py` & `mykit-8.1.0b1/mykit/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/__main__.py` & `mykit-8.1.0b1/mykit/__main__.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/app/__init__.py` & `mykit-8.1.0b1/mykit/app/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/app/architecture/eventdriven.py` & `mykit-8.1.0b1/mykit/app/architecture/eventdriven.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/app/arrow.py` & `mykit-8.1.0b1/mykit/app/arrow.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/app/button.py` & `mykit-8.1.0b1/mykit/app/button.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/app/complex/biplot.py` & `mykit-8.1.0b1/mykit/app/complex/biplot.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/app/complex/plot.py` & `mykit-8.1.0b1/mykit/app/complex/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/app/label.py` & `mykit-8.1.0b1/mykit/app/label.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/app/slider.py` & `mykit-8.1.0b1/mykit/app/slider.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/kit/color.py` & `mykit-8.1.0b1/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/kit/fast_visualizations/static/plot.py` & `mykit-8.1.0b1/mykit/kit/fast_visualizations/static/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/kit/ffmpeg.py` & `mykit-8.1.0b1/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/kit/keycrate/__init__.py` & `mykit-8.1.0b1/mykit/kit/keycrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/kit/math.py` & `mykit-8.1.0b1/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/kit/neuralnet/dense.py` & `mykit-8.1.0b1/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/kit/neuralnet/genetic.py` & `mykit-8.1.0b1/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/kit/noise.py` & `mykit-8.1.0b1/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/kit/pLog.py` & `mykit-8.1.0b1/mykit/kit/pLog.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/kit/path.py` & `mykit-8.1.0b1/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/kit/text.py` & `mykit-8.1.0b1/mykit/kit/text.py`

 * *Files 21% similar despite different names*

```diff
@@ -152,8 +152,55 @@
     if precision > 0:
         n_format = n_format.rstrip('0').rstrip('.')
     
     GAP = ''
     if suffix != '':
         GAP = ' '*gap
 
-    return sign + n_format + GAP + suffix
+    return sign + n_format + GAP + suffix
+
+
+def num_round(number:int, /, keep:int=2, add_commas:bool=True) -> str:
+    """
+    Rounding number (see demo below).
+
+    ---
+    
+    ## Params
+    - `number`: The input number; floats are also accepted.
+    - `keep`: number of the non-zero part (see demo below)
+    - `add_commas`: separated the thousands with commas
+
+    ## Demo
+    >>> num_round(12345, 1)  # 10,000
+    >>> num_round(12345, 2)  # 12,000
+    >>> num_round(12345, 3)  # 12,300
+    >>> num_round(12385, 3)  # 12,400
+
+    ## Docs
+    - `keep` value is clamped to a minimum of 1.
+    """
+
+    ## Handle float
+    number = round(number)
+
+    ## Handle negative number
+    sign = ''
+    if number < 0:
+        number = abs(number)
+        sign = '-'
+
+    ## Clamp
+    keep = min(len(str(number)), max(1, keep))
+    
+    ## Rounding
+    power = len(str(number)) - keep
+    scale = int( _math.pow(10, power) )
+    rounded = round(number/scale)*scale
+
+    ## Stringify
+    if add_commas:
+        rounded = f'{rounded:,}'
+    else:
+        rounded = str(rounded)
+
+    return sign + rounded
```

### Comparing `mykit-8.0.0/mykit/kit/time.py` & `mykit-8.1.0b1/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit/kit/utils.py` & `mykit-8.1.0b1/mykit/kit/utils.py`

 * *Files identical despite different names*

### Comparing `mykit-8.0.0/mykit.egg-info/PKG-INFO` & `mykit-8.1.0b1/mykit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 8.0.0
+Version: 8.1.0b1
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/mykit/docs
 Project-URL: Report bugs, https://github.com/nvfp/mykit/issues
```

### Comparing `mykit-8.0.0/mykit.egg-info/SOURCES.txt` & `mykit-8.1.0b1/mykit.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 mykit/app/arrow.py
 mykit/app/button.py
 mykit/app/label.py
 mykit/app/slider.py
 mykit/app/architecture/eventdriven.py
 mykit/app/complex/biplot.py
 mykit/app/complex/plot.py
+mykit/ghactions/eLog.py
+mykit/ghactions/set_output.py
 mykit/kit/color.py
 mykit/kit/ffmpeg.py
 mykit/kit/math.py
 mykit/kit/noise.py
 mykit/kit/pLog.py
 mykit/kit/path.py
 mykit/kit/text.py
```

### Comparing `mykit-8.0.0/pyproject.toml` & `mykit-8.1.0b1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "8.0.0"
+version = "8.1.0b1"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

