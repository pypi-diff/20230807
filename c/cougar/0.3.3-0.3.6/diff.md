# Comparing `tmp/cougar-0.3.3.tar.gz` & `tmp/cougar-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cougar-0.3.3.tar", last modified: Sun Aug  6 07:27:18 2023, max compression
+gzip compressed data, was "cougar-0.3.6.tar", last modified: Sun Aug  6 13:06:53 2023, max compression
```

## Comparing `cougar-0.3.3.tar` & `cougar-0.3.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 07:27:18.649306 cougar-0.3.3/
--rw-rw-rw-   0        0        0    11558 2023-08-06 07:26:46.000000 cougar-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     1499 2023-08-06 07:27:18.649306 cougar-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-08-06 07:26:46.000000 cougar-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-06 07:27:18.649306 cougar-0.3.3/cougar/
--rw-rw-rw-   0        0        0      290 2023-08-06 07:26:46.000000 cougar-0.3.3/cougar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 07:27:18.649306 cougar-0.3.3/cougar/numpy/
--rw-rw-rw-   0        0        0       27 2023-08-06 07:26:46.000000 cougar-0.3.3/cougar/numpy/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-08-06 07:26:46.000000 cougar-0.3.3/cougar/numpy/functional.py
--rw-rw-rw-   0        0        0     2392 2023-08-06 07:26:46.000000 cougar-0.3.3/cougar/rolling.c
-drwxrwxrwx   0        0        0        0 2023-08-06 07:27:18.649306 cougar-0.3.3/cougar.egg-info/
--rw-rw-rw-   0        0        0     1499 2023-08-06 07:27:17.000000 cougar-0.3.3/cougar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-08-06 07:27:18.000000 cougar-0.3.3/cougar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 07:27:17.000000 cougar-0.3.3/cougar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-06 07:27:17.000000 cougar-0.3.3/cougar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-06 07:27:17.000000 cougar-0.3.3/cougar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1011 2023-08-06 07:26:46.000000 cougar-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 07:27:18.649306 cougar-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1360 2023-08-06 07:27:15.000000 cougar-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-06 07:27:18.649306 cougar-0.3.3/tests/
--rw-rw-rw-   0        0        0        0 2023-08-06 07:26:46.000000 cougar-0.3.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 13:06:53.151121 cougar-0.3.6/
+-rw-rw-rw-   0        0        0    11558 2023-08-06 13:06:21.000000 cougar-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0     1499 2023-08-06 13:06:53.151121 cougar-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-08-06 13:06:21.000000 cougar-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 13:06:53.151121 cougar-0.3.6/cougar/
+-rw-rw-rw-   0        0        0      277 2023-08-06 13:06:50.000000 cougar-0.3.6/cougar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 13:06:53.151121 cougar-0.3.6/cougar/numpy/
+-rw-rw-rw-   0        0        0       27 2023-08-06 13:06:21.000000 cougar-0.3.6/cougar/numpy/__init__.py
+-rw-rw-rw-   0        0        0     1543 2023-08-06 13:06:21.000000 cougar-0.3.6/cougar/numpy/functional.py
+drwxrwxrwx   0        0        0        0 2023-08-06 13:06:53.151121 cougar-0.3.6/cougar/pandas/
+-rw-rw-rw-   0        0        0     4115 2023-08-06 13:06:21.000000 cougar-0.3.6/cougar/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2392 2023-08-06 13:06:21.000000 cougar-0.3.6/cougar/rolling.c
+drwxrwxrwx   0        0        0        0 2023-08-06 13:06:53.151121 cougar-0.3.6/cougar.egg-info/
+-rw-rw-rw-   0        0        0     1499 2023-08-06 13:06:52.000000 cougar-0.3.6/cougar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-08-06 13:06:53.000000 cougar-0.3.6/cougar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 13:06:52.000000 cougar-0.3.6/cougar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-06 13:06:52.000000 cougar-0.3.6/cougar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-06 13:06:52.000000 cougar-0.3.6/cougar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      978 2023-08-06 13:06:50.000000 cougar-0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 13:06:53.151121 cougar-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1360 2023-08-06 13:06:50.000000 cougar-0.3.6/setup.py
```

### Comparing `cougar-0.3.3/LICENSE` & `cougar-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cougar-0.3.3/PKG-INFO` & `cougar-0.3.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cougar
-Version: 0.3.3
+Version: 0.3.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Yunchong Gan
 Author-email: yunchong@pku.edu.cn
 License: UNKNOWN
 Description: # cougar
```

### Comparing `cougar-0.3.3/cougar/numpy/functional.py` & `cougar-0.3.6/cougar/numpy/functional.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def sliding_window(arr: np.ndarray, window: int, axis: int = -1) -> np.ndarray:
     return sliding_window_view(arr, window, axis=axis)
 
 
 def rolling_sum(arr: np.ndarray, window: int, axis: int = -1) -> np.ndarray:
     return pad(
-        sliding_window(arr, window, axis=axis).sum(axis=-1),
+        sliding_window(arr, window, axis=axis).sum(axis=-1).astype(np.float64),
         window - 1,
         axis,
     )
 
 
 def rolling_mean(arr: np.ndarray, window: int, axis: int = -1) -> np.ndarray:
     return pad(
```

### Comparing `cougar-0.3.3/cougar/rolling.c` & `cougar-0.3.6/cougar/rolling.c`

 * *Files identical despite different names*

### Comparing `cougar-0.3.3/cougar.egg-info/PKG-INFO` & `cougar-0.3.6/cougar.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cougar
-Version: 0.3.3
+Version: 0.3.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Yunchong Gan
 Author-email: yunchong@pku.edu.cn
 License: UNKNOWN
 Description: # cougar
```

### Comparing `cougar-0.3.3/pyproject.toml` & `cougar-0.3.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-[tool.poetry]
-name = "cougar"
-version = "0.2.0"
-description = ""
-license = "Apache-2.0"
-authors = ["Yunchong Gan <yunchong@pku.edu.cn>"]
-maintainers = ["Yunchong Gan <yunchong@pku.edu.cn>"]
-readme = "README.md"
-repository = "https://github.com/Phimos/cougar"
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Intended Audience :: Science/Research",
-    "Natural Language :: English",
-    "Operating System :: POSIX :: Linux",
-    "Operating System :: MacOS :: MacOS X",
-    "Operating System :: Microsoft :: Windows",
-    "Programming Language :: C",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11"
-]
-
-[tool.poetry.dependencies]
-python = "^3.7"
-numpy = "^1.21"
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "cougar"
+version = "0.3.6"
+description = ""
+license = "Apache-2.0"
+authors = ["Yunchong Gan <yunchong@pku.edu.cn>"]
+maintainers = ["Yunchong Gan <yunchong@pku.edu.cn>"]
+readme = "README.md"
+repository = "https://github.com/Phimos/cougar"
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Science/Research",
+    "Natural Language :: English",
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: MacOS :: MacOS X",
+    "Operating System :: Microsoft :: Windows",
+    "Programming Language :: C",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11"
+]
+
+[tool.poetry.dependencies]
+python = "^3.7"
+numpy = "^1.21"
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `cougar-0.3.3/setup.py` & `cougar-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import Extension, find_packages, setup
 
 project_dir = Path(__file__).parent.resolve()
 long_description = (project_dir / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="cougar",
-    version="0.3.3",
+    version="0.3.6",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Yunchong Gan",
     author_email="yunchong@pku.edu.cn",
     packages=find_packages(),
     requires=["numpy"],
     install_requires=["numpy"],
```

