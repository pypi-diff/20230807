# Comparing `tmp/jianglab-0.7.8.tar.gz` & `tmp/jianglab-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.7.8.tar", last modified: Mon Aug  7 16:50:46 2023, max compression
+gzip compressed data, was "jianglab-0.7.9.tar", last modified: Mon Aug  7 16:53:27 2023, max compression
```

## Comparing `jianglab-0.7.8.tar` & `jianglab-0.7.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 16:50:46.619622 jianglab-0.7.8/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-07 16:50:46.619301 jianglab-0.7.8/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.7.8/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 16:50:46.616533 jianglab-0.7.8/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.7.8/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    50337 2023-08-07 16:50:24.000000 jianglab-0.7.8/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.7.8/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 16:50:46.618823 jianglab-0.7.8/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-07 16:50:46.000000 jianglab-0.7.8/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-07 16:50:46.000000 jianglab-0.7.8/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-07 16:50:46.000000 jianglab-0.7.8/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      168 2023-08-07 16:50:46.000000 jianglab-0.7.8/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-07 16:50:46.000000 jianglab-0.7.8/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-07 16:50:46.619739 jianglab-0.7.8/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1162 2023-08-07 16:50:41.000000 jianglab-0.7.8/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 16:53:27.983167 jianglab-0.7.9/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-07 16:53:27.982823 jianglab-0.7.9/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.7.9/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 16:53:27.979373 jianglab-0.7.9/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.7.9/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    50332 2023-08-07 16:53:14.000000 jianglab-0.7.9/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.7.9/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 16:53:27.982248 jianglab-0.7.9/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-07 16:53:27.000000 jianglab-0.7.9/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-07 16:53:27.000000 jianglab-0.7.9/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-07 16:53:27.000000 jianglab-0.7.9/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      168 2023-08-07 16:53:27.000000 jianglab-0.7.9/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-07 16:53:27.000000 jianglab-0.7.9/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-07 16:53:27.983306 jianglab-0.7.9/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1162 2023-08-07 16:53:18.000000 jianglab-0.7.9/setup.py
```

### Comparing `jianglab-0.7.8/PKG-INFO` & `jianglab-0.7.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.7.8
+Version: 0.7.9
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.7.8/README.md` & `jianglab-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.7.8/jianglab/common_functions.py` & `jianglab-0.7.9/jianglab/common_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1215,15 +1215,15 @@
 #     else:
 #         files = glob.glob(location + '/*', recursive=False)
 #     files = [f for f in files if keyword1 in f]
 #     if keyword2 != "":
 #         files = [f for f in files if keyword2 in f]
 #     return files
 
-def search_file_in_location_list(location, keyword_list=[], exclude_list = [], recursive=True):
+def search_file_in_location(location, keyword_list=[], exclude_list = [], recursive=True):
     """Search for a file in a given location. 
     If recursive is True, the search will be recursive.
     search files that contain both keywords in their name."""
     if type(keyword_list) == str:
         keyword_list = [keyword_list]
     if type(exclude_list) == str:
         exclude_list = [exclude_list]
```

### Comparing `jianglab-0.7.8/jianglab.egg-info/PKG-INFO` & `jianglab-0.7.9/jianglab.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.7.8
+Version: 0.7.9
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.7.8/setup.py` & `jianglab-0.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.7.8',
+    version='0.7.9',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

