# Comparing `tmp/cougar-0.3.7.tar.gz` & `tmp/cougar-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cougar-0.3.7.tar", last modified: Mon Aug  7 12:35:40 2023, max compression
+gzip compressed data, was "cougar-0.4.0.tar", last modified: Mon Aug  7 15:16:47 2023, max compression
```

## Comparing `cougar-0.3.7.tar` & `cougar-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 12:35:40.654823 cougar-0.3.7/
--rw-rw-rw-   0        0        0    11558 2023-08-07 12:33:46.000000 cougar-0.3.7/LICENSE
--rw-rw-rw-   0        0        0     1252 2023-08-07 12:35:40.654823 cougar-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-08-07 12:33:46.000000 cougar-0.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 12:35:40.654823 cougar-0.3.7/cougar/
--rw-rw-rw-   0        0        0      277 2023-08-07 12:35:36.000000 cougar-0.3.7/cougar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:35:40.654823 cougar-0.3.7/cougar/numpy/
--rw-rw-rw-   0        0        0       27 2023-08-07 12:33:46.000000 cougar-0.3.7/cougar/numpy/__init__.py
--rw-rw-rw-   0        0        0     1619 2023-08-07 12:33:46.000000 cougar-0.3.7/cougar/numpy/functional.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:35:40.654823 cougar-0.3.7/cougar/pandas/
--rw-rw-rw-   0        0        0     4115 2023-08-07 12:33:46.000000 cougar-0.3.7/cougar/pandas/__init__.py
--rw-rw-rw-   0        0        0     2392 2023-08-07 12:33:46.000000 cougar-0.3.7/cougar/rolling.c
-drwxrwxrwx   0        0        0        0 2023-08-07 12:35:40.654823 cougar-0.3.7/cougar.egg-info/
--rw-rw-rw-   0        0        0     1252 2023-08-07 12:35:40.000000 cougar-0.3.7/cougar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-08-07 12:35:40.000000 cougar-0.3.7/cougar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 12:35:40.000000 cougar-0.3.7/cougar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-07 12:35:40.000000 cougar-0.3.7/cougar.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-07 12:35:40.000000 cougar-0.3.7/cougar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      978 2023-08-07 12:35:36.000000 cougar-0.3.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-07 12:35:40.654823 cougar-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1360 2023-08-07 12:35:36.000000 cougar-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:16:47.616146 cougar-0.4.0/
+-rw-rw-rw-   0        0        0    11558 2023-08-07 15:16:02.000000 cougar-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1598 2023-08-07 15:16:47.616146 cougar-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2023-08-07 15:16:02.000000 cougar-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 15:16:47.616146 cougar-0.4.0/cougar/
+-rw-rw-rw-   0        0        0      277 2023-08-07 15:16:42.000000 cougar-0.4.0/cougar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:16:47.616146 cougar-0.4.0/cougar/numpy/
+-rw-rw-rw-   0        0        0       27 2023-08-07 15:16:02.000000 cougar-0.4.0/cougar/numpy/__init__.py
+-rw-rw-rw-   0        0        0     1619 2023-08-07 15:16:02.000000 cougar-0.4.0/cougar/numpy/functional.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:16:47.616146 cougar-0.4.0/cougar/pandas/
+-rw-rw-rw-   0        0        0     4115 2023-08-07 15:16:02.000000 cougar-0.4.0/cougar/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2392 2023-08-07 15:16:02.000000 cougar-0.4.0/cougar/rolling.c
+drwxrwxrwx   0        0        0        0 2023-08-07 15:16:47.616146 cougar-0.4.0/cougar.egg-info/
+-rw-rw-rw-   0        0        0     1598 2023-08-07 15:16:47.000000 cougar-0.4.0/cougar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-08-07 15:16:47.000000 cougar-0.4.0/cougar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 15:16:47.000000 cougar-0.4.0/cougar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-07 15:16:47.000000 cougar-0.4.0/cougar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 15:16:47.000000 cougar-0.4.0/cougar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      978 2023-08-07 15:16:42.000000 cougar-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 15:16:47.616146 cougar-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1360 2023-08-07 15:16:42.000000 cougar-0.4.0/setup.py
```

### Comparing `cougar-0.3.7/LICENSE` & `cougar-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cougar-0.3.7/PKG-INFO` & `cougar-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cougar
-Version: 0.3.7
+Version: 0.4.0
 Author: Yunchong Gan
 Author-email: yunchong@pku.edu.cn
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
@@ -37,10 +37,23 @@
 import numpy as np
 import cougar as cg
 
 arr = np.random.rand(1_000_000)
 cg.rolling_mean(arr, 1_000)
 ```
 
+## Supported Methods
+
+| Method   | Time Complexity |
+| -------- | --------------- |
+| sum      | O(1)            |
+| mean     | O(1)            |
+| min      | O(1)            |
+| max      | O(1)            |
+| argmin   | O(1)            |
+| argmax   | O(1)            |
+| rank     | O(log n)        |
+| quantile | O(log n)        |
+
 ## Benchmark
 
 todo
```

### Comparing `cougar-0.3.7/cougar/numpy/functional.py` & `cougar-0.4.0/cougar/numpy/functional.py`

 * *Files identical despite different names*

### Comparing `cougar-0.3.7/cougar/pandas/__init__.py` & `cougar-0.4.0/cougar/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `cougar-0.3.7/cougar/rolling.c` & `cougar-0.4.0/cougar/rolling.c`

 * *Files identical despite different names*

### Comparing `cougar-0.3.7/cougar.egg-info/PKG-INFO` & `cougar-0.4.0/cougar.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cougar
-Version: 0.3.7
+Version: 0.4.0
 Author: Yunchong Gan
 Author-email: yunchong@pku.edu.cn
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
@@ -37,10 +37,23 @@
 import numpy as np
 import cougar as cg
 
 arr = np.random.rand(1_000_000)
 cg.rolling_mean(arr, 1_000)
 ```
 
+## Supported Methods
+
+| Method   | Time Complexity |
+| -------- | --------------- |
+| sum      | O(1)            |
+| mean     | O(1)            |
+| min      | O(1)            |
+| max      | O(1)            |
+| argmin   | O(1)            |
+| argmax   | O(1)            |
+| rank     | O(log n)        |
+| quantile | O(log n)        |
+
 ## Benchmark
 
 todo
```

### Comparing `cougar-0.3.7/pyproject.toml` & `cougar-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cougar"
-version = "0.3.7"
+version = "0.4.0"
 description = ""
 license = "Apache-2.0"
 authors = ["Yunchong Gan <yunchong@pku.edu.cn>"]
 maintainers = ["Yunchong Gan <yunchong@pku.edu.cn>"]
 readme = "README.md"
 repository = "https://github.com/Phimos/cougar"
 classifiers = [
```

### Comparing `cougar-0.3.7/setup.py` & `cougar-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import Extension, find_packages, setup
 
 project_dir = Path(__file__).parent.resolve()
 long_description = (project_dir / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="cougar",
-    version="0.3.7",
+    version="0.4.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Yunchong Gan",
     author_email="yunchong@pku.edu.cn",
     packages=find_packages(),
     requires=["numpy"],
     install_requires=["numpy"],
```

