# Comparing `tmp/cougar-0.3.6.tar.gz` & `tmp/cougar-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cougar-0.3.6.tar", last modified: Sun Aug  6 13:06:53 2023, max compression
+gzip compressed data, was "cougar-0.3.7.tar", last modified: Mon Aug  7 12:35:40 2023, max compression
```

## Comparing `cougar-0.3.6.tar` & `cougar-0.3.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 13:06:53.151121 cougar-0.3.6/
--rw-rw-rw-   0        0        0    11558 2023-08-06 13:06:21.000000 cougar-0.3.6/LICENSE
--rw-rw-rw-   0        0        0     1499 2023-08-06 13:06:53.151121 cougar-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-08-06 13:06:21.000000 cougar-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-06 13:06:53.151121 cougar-0.3.6/cougar/
--rw-rw-rw-   0        0        0      277 2023-08-06 13:06:50.000000 cougar-0.3.6/cougar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 13:06:53.151121 cougar-0.3.6/cougar/numpy/
--rw-rw-rw-   0        0        0       27 2023-08-06 13:06:21.000000 cougar-0.3.6/cougar/numpy/__init__.py
--rw-rw-rw-   0        0        0     1543 2023-08-06 13:06:21.000000 cougar-0.3.6/cougar/numpy/functional.py
-drwxrwxrwx   0        0        0        0 2023-08-06 13:06:53.151121 cougar-0.3.6/cougar/pandas/
--rw-rw-rw-   0        0        0     4115 2023-08-06 13:06:21.000000 cougar-0.3.6/cougar/pandas/__init__.py
--rw-rw-rw-   0        0        0     2392 2023-08-06 13:06:21.000000 cougar-0.3.6/cougar/rolling.c
-drwxrwxrwx   0        0        0        0 2023-08-06 13:06:53.151121 cougar-0.3.6/cougar.egg-info/
--rw-rw-rw-   0        0        0     1499 2023-08-06 13:06:52.000000 cougar-0.3.6/cougar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-08-06 13:06:53.000000 cougar-0.3.6/cougar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 13:06:52.000000 cougar-0.3.6/cougar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-06 13:06:52.000000 cougar-0.3.6/cougar.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-06 13:06:52.000000 cougar-0.3.6/cougar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      978 2023-08-06 13:06:50.000000 cougar-0.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 13:06:53.151121 cougar-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1360 2023-08-06 13:06:50.000000 cougar-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:35:40.654823 cougar-0.3.7/
+-rw-rw-rw-   0        0        0    11558 2023-08-07 12:33:46.000000 cougar-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0     1252 2023-08-07 12:35:40.654823 cougar-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-08-07 12:33:46.000000 cougar-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 12:35:40.654823 cougar-0.3.7/cougar/
+-rw-rw-rw-   0        0        0      277 2023-08-07 12:35:36.000000 cougar-0.3.7/cougar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:35:40.654823 cougar-0.3.7/cougar/numpy/
+-rw-rw-rw-   0        0        0       27 2023-08-07 12:33:46.000000 cougar-0.3.7/cougar/numpy/__init__.py
+-rw-rw-rw-   0        0        0     1619 2023-08-07 12:33:46.000000 cougar-0.3.7/cougar/numpy/functional.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:35:40.654823 cougar-0.3.7/cougar/pandas/
+-rw-rw-rw-   0        0        0     4115 2023-08-07 12:33:46.000000 cougar-0.3.7/cougar/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2392 2023-08-07 12:33:46.000000 cougar-0.3.7/cougar/rolling.c
+drwxrwxrwx   0        0        0        0 2023-08-07 12:35:40.654823 cougar-0.3.7/cougar.egg-info/
+-rw-rw-rw-   0        0        0     1252 2023-08-07 12:35:40.000000 cougar-0.3.7/cougar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-08-07 12:35:40.000000 cougar-0.3.7/cougar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 12:35:40.000000 cougar-0.3.7/cougar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-07 12:35:40.000000 cougar-0.3.7/cougar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 12:35:40.000000 cougar-0.3.7/cougar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      978 2023-08-07 12:35:36.000000 cougar-0.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 12:35:40.654823 cougar-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1360 2023-08-07 12:35:36.000000 cougar-0.3.7/setup.py
```

### Comparing `cougar-0.3.6/LICENSE` & `cougar-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cougar-0.3.6/PKG-INFO` & `cougar-0.3.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,12 @@
 Metadata-Version: 2.1
 Name: cougar
-Version: 0.3.6
-Summary: UNKNOWN
-Home-page: UNKNOWN
+Version: 0.3.7
 Author: Yunchong Gan
 Author-email: yunchong@pku.edu.cn
-License: UNKNOWN
-Description: # cougar
-        
-        A python C-extension for rolling window aggregations. Try to support more methods than `bottleneck` and run faster than `pandas`. Currently this is only a weekend project, feel free to contribute.
-        
-        
-        ## Installation
-        
-        ```bash
-        pip install cougar
-        ```
-        
-        ## Usage
-        
-        ```python
-        import numpy as np
-        import cougar as cg
-        
-        arr = np.random.rand(1_000_000)
-        cg.rolling_mean(arr, 1_000)
-        ```
-        
-        ## Benchmark
-        
-        todo
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: C
@@ -42,7 +14,33 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires: numpy
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# cougar
+
+A python C-extension for rolling window aggregations. Try to support more methods than `bottleneck` and run faster than `pandas`. Currently this is only a weekend project, feel free to contribute.
+
+
+## Installation
+
+```bash
+pip install cougar
+```
+
+## Usage
+
+```python
+import numpy as np
+import cougar as cg
+
+arr = np.random.rand(1_000_000)
+cg.rolling_mean(arr, 1_000)
+```
+
+## Benchmark
+
+todo
```

### Comparing `cougar-0.3.6/cougar/numpy/functional.py` & `cougar-0.3.7/cougar/numpy/functional.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,35 +20,35 @@
         window - 1,
         axis,
     )
 
 
 def rolling_mean(arr: np.ndarray, window: int, axis: int = -1) -> np.ndarray:
     return pad(
-        sliding_window(arr, window, axis=axis).mean(axis=-1),
+        sliding_window(arr, window, axis=axis).mean(axis=-1).astype(np.float64),
         window - 1,
         axis,
     )
 
 
 def rolling_std(arr: np.ndarray, window: int, axis: int = -1) -> np.ndarray:
     return pad(
-        sliding_window(arr, window, axis=axis).std(axis=-1),
+        sliding_window(arr, window, axis=axis).std(axis=-1).astype(np.float64),
         window - 1,
         axis,
     )
 
 
 def rolling_max(arr: np.ndarray, window: int, axis: int = -1) -> np.ndarray:
     return pad(
-        sliding_window(arr, window, axis=axis).max(axis=-1),
+        sliding_window(arr, window, axis=axis).max(axis=-1).astype(np.float64),
         window - 1,
         axis,
     )
 
 
 def rolling_min(arr: np.ndarray, window: int, axis: int = -1) -> np.ndarray:
     return pad(
-        sliding_window(arr, window, axis=axis).min(axis=-1),
+        sliding_window(arr, window, axis=axis).min(axis=-1).astype(np.float64),
         window - 1,
         axis,
     )
```

### Comparing `cougar-0.3.6/cougar/pandas/__init__.py` & `cougar-0.3.7/cougar/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `cougar-0.3.6/cougar/rolling.c` & `cougar-0.3.7/cougar/rolling.c`

 * *Files identical despite different names*

### Comparing `cougar-0.3.6/cougar.egg-info/PKG-INFO` & `cougar-0.3.7/cougar.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,12 @@
 Metadata-Version: 2.1
 Name: cougar
-Version: 0.3.6
-Summary: UNKNOWN
-Home-page: UNKNOWN
+Version: 0.3.7
 Author: Yunchong Gan
 Author-email: yunchong@pku.edu.cn
-License: UNKNOWN
-Description: # cougar
-        
-        A python C-extension for rolling window aggregations. Try to support more methods than `bottleneck` and run faster than `pandas`. Currently this is only a weekend project, feel free to contribute.
-        
-        
-        ## Installation
-        
-        ```bash
-        pip install cougar
-        ```
-        
-        ## Usage
-        
-        ```python
-        import numpy as np
-        import cougar as cg
-        
-        arr = np.random.rand(1_000_000)
-        cg.rolling_mean(arr, 1_000)
-        ```
-        
-        ## Benchmark
-        
-        todo
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: C
@@ -42,7 +14,33 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires: numpy
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# cougar
+
+A python C-extension for rolling window aggregations. Try to support more methods than `bottleneck` and run faster than `pandas`. Currently this is only a weekend project, feel free to contribute.
+
+
+## Installation
+
+```bash
+pip install cougar
+```
+
+## Usage
+
+```python
+import numpy as np
+import cougar as cg
+
+arr = np.random.rand(1_000_000)
+cg.rolling_mean(arr, 1_000)
+```
+
+## Benchmark
+
+todo
```

### Comparing `cougar-0.3.6/pyproject.toml` & `cougar-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cougar"
-version = "0.3.6"
+version = "0.3.7"
 description = ""
 license = "Apache-2.0"
 authors = ["Yunchong Gan <yunchong@pku.edu.cn>"]
 maintainers = ["Yunchong Gan <yunchong@pku.edu.cn>"]
 readme = "README.md"
 repository = "https://github.com/Phimos/cougar"
 classifiers = [
```

### Comparing `cougar-0.3.6/setup.py` & `cougar-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import Extension, find_packages, setup
 
 project_dir = Path(__file__).parent.resolve()
 long_description = (project_dir / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="cougar",
-    version="0.3.6",
+    version="0.3.7",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Yunchong Gan",
     author_email="yunchong@pku.edu.cn",
     packages=find_packages(),
     requires=["numpy"],
     install_requires=["numpy"],
```

