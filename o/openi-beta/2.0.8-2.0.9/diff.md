# Comparing `tmp/openi-beta-2.0.8.tar.gz` & `tmp/openi-beta-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-2.0.8.tar", last modified: Mon Aug  7 01:56:15 2023, max compression
+gzip compressed data, was "openi-beta-2.0.9.tar", last modified: Mon Aug  7 06:40:06 2023, max compression
```

## Comparing `openi-beta-2.0.8.tar` & `openi-beta-2.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 01:56:15.343454 openi-beta-2.0.8/
--rw-rw-rw-   0        0        0     2086 2023-08-07 01:56:15.342449 openi-beta-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1440 2023-08-07 01:38:11.000000 openi-beta-2.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-08-07 01:56:15.343454 openi-beta-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-08-07 01:39:47.000000 openi-beta-2.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-07 01:56:15.307411 openi-beta-2.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-08-07 01:56:15.312202 openi-beta-2.0.8/src/openi/
--rw-rw-rw-   0        0        0      194 2023-08-07 01:38:11.000000 openi-beta-2.0.8/src/openi/__init__.py
--rw-rw-rw-   0        0        0     6456 2023-08-07 01:38:11.000000 openi-beta-2.0.8/src/openi/apis.py
--rw-rw-rw-   0        0        0     5238 2023-08-07 01:38:11.000000 openi-beta-2.0.8/src/openi/cli.py
-drwxrwxrwx   0        0        0        0 2023-08-07 01:56:15.314327 openi-beta-2.0.8/src/openi/dataset/
--rw-rw-rw-   0        0        0      109 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/dataset/__init__.py
--rw-rw-rw-   0        0        0     2752 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/dataset/dataset_file.py
--rw-rw-rw-   0        0        0     2671 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/dataset/download.py
--rw-rw-rw-   0        0        0     4392 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/dataset/upload.py
--rw-rw-rw-   0        0        0     3029 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/login.py
--rw-rw-rw-   0        0        0     4078 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/settings.py
-drwxrwxrwx   0        0        0        0 2023-08-07 01:56:15.316939 openi-beta-2.0.8/src/openi/utils/
--rw-rw-rw-   0        0        0       50 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/utils/__init__.py
--rw-rw-rw-   0        0        0     1400 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/utils/file_utils.py
--rw-rw-rw-   0        0        0      723 2023-08-07 01:38:12.000000 openi-beta-2.0.8/src/openi/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-08-07 01:56:15.342449 openi-beta-2.0.8/src/openi_beta.egg-info/
--rw-rw-rw-   0        0        0     2086 2023-08-07 01:56:15.000000 openi-beta-2.0.8/src/openi_beta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-08-07 01:56:15.000000 openi-beta-2.0.8/src/openi_beta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 01:56:15.000000 openi-beta-2.0.8/src/openi_beta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-08-07 01:56:15.000000 openi-beta-2.0.8/src/openi_beta.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-08-07 01:56:15.000000 openi-beta-2.0.8/src/openi_beta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-07 01:56:15.000000 openi-beta-2.0.8/src/openi_beta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 06:40:06.484149 openi-beta-2.0.9/
+-rw-rw-rw-   0        0        0     2086 2023-08-07 06:40:06.482937 openi-beta-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1440 2023-08-07 01:38:11.000000 openi-beta-2.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-07 06:40:06.484149 openi-beta-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-08-07 06:39:56.000000 openi-beta-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:40:06.438978 openi-beta-2.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 06:40:06.449301 openi-beta-2.0.9/src/openi/
+-rw-rw-rw-   0        0        0      146 2023-08-07 06:39:52.000000 openi-beta-2.0.9/src/openi/__init__.py
+-rw-rw-rw-   0        0        0     6456 2023-08-07 01:38:11.000000 openi-beta-2.0.9/src/openi/apis.py
+-rw-rw-rw-   0        0        0     5238 2023-08-07 01:38:11.000000 openi-beta-2.0.9/src/openi/cli.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:40:06.452559 openi-beta-2.0.9/src/openi/dataset/
+-rw-rw-rw-   0        0        0      109 2023-08-07 01:38:12.000000 openi-beta-2.0.9/src/openi/dataset/__init__.py
+-rw-rw-rw-   0        0        0     2752 2023-08-07 01:38:12.000000 openi-beta-2.0.9/src/openi/dataset/dataset_file.py
+-rw-rw-rw-   0        0        0     2671 2023-08-07 01:38:12.000000 openi-beta-2.0.9/src/openi/dataset/download.py
+-rw-rw-rw-   0        0        0     4392 2023-08-07 01:38:12.000000 openi-beta-2.0.9/src/openi/dataset/upload.py
+-rw-rw-rw-   0        0        0     3029 2023-08-07 01:38:12.000000 openi-beta-2.0.9/src/openi/login.py
+-rw-rw-rw-   0        0        0     4078 2023-08-07 01:38:12.000000 openi-beta-2.0.9/src/openi/settings.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:40:06.454794 openi-beta-2.0.9/src/openi/utils/
+-rw-rw-rw-   0        0        0       50 2023-08-07 01:38:12.000000 openi-beta-2.0.9/src/openi/utils/__init__.py
+-rw-rw-rw-   0        0        0     1400 2023-08-07 01:38:12.000000 openi-beta-2.0.9/src/openi/utils/file_utils.py
+-rw-rw-rw-   0        0        0      723 2023-08-07 01:38:12.000000 openi-beta-2.0.9/src/openi/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:40:06.481932 openi-beta-2.0.9/src/openi_beta.egg-info/
+-rw-rw-rw-   0        0        0     2086 2023-08-07 06:40:06.000000 openi-beta-2.0.9/src/openi_beta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-08-07 06:40:06.000000 openi-beta-2.0.9/src/openi_beta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 06:40:06.000000 openi-beta-2.0.9/src/openi_beta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-08-07 06:40:06.000000 openi-beta-2.0.9/src/openi_beta.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-08-07 06:40:06.000000 openi-beta-2.0.9/src/openi_beta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-07 06:40:06.000000 openi-beta-2.0.9/src/openi_beta.egg-info/top_level.txt
```

### Comparing `openi-beta-2.0.8/PKG-INFO` & `openi-beta-2.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 2.0.8
+Version: 2.0.9
 Summary: Beta package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-2.0.8/README.md` & `openi-beta-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.8/setup.py` & `openi-beta-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="openi-beta",
-    version="2.0.8",
+    version="2.0.9",
     description="Beta package for openi pypi",
     package_dir={"": "src"},
     packages=find_packages("src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi",
     author="chenzh05",
```

### Comparing `openi-beta-2.0.8/src/openi/apis.py` & `openi-beta-2.0.9/src/openi/apis.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.8/src/openi/cli.py` & `openi-beta-2.0.9/src/openi/cli.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.8/src/openi/dataset/dataset_file.py` & `openi-beta-2.0.9/src/openi/dataset/dataset_file.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.8/src/openi/dataset/download.py` & `openi-beta-2.0.9/src/openi/dataset/download.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.8/src/openi/dataset/upload.py` & `openi-beta-2.0.9/src/openi/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.8/src/openi/login.py` & `openi-beta-2.0.9/src/openi/login.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.8/src/openi/settings.py` & `openi-beta-2.0.9/src/openi/settings.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.8/src/openi/utils/file_utils.py` & `openi-beta-2.0.9/src/openi/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.8/src/openi/utils/logger.py` & `openi-beta-2.0.9/src/openi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.8/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-2.0.9/src/openi_beta.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 2.0.8
+Version: 2.0.9
 Summary: Beta package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-2.0.8/src/openi_beta.egg-info/SOURCES.txt` & `openi-beta-2.0.9/src/openi_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

