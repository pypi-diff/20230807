# Comparing `tmp/jianglab-0.7.9.tar.gz` & `tmp/jianglab-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.7.9.tar", last modified: Mon Aug  7 16:53:27 2023, max compression
+gzip compressed data, was "jianglab-0.8.0.tar", last modified: Mon Aug  7 17:14:06 2023, max compression
```

## Comparing `jianglab-0.7.9.tar` & `jianglab-0.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 16:53:27.983167 jianglab-0.7.9/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-07 16:53:27.982823 jianglab-0.7.9/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.7.9/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 16:53:27.979373 jianglab-0.7.9/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.7.9/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    50332 2023-08-07 16:53:14.000000 jianglab-0.7.9/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.7.9/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 16:53:27.982248 jianglab-0.7.9/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-07 16:53:27.000000 jianglab-0.7.9/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-07 16:53:27.000000 jianglab-0.7.9/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-07 16:53:27.000000 jianglab-0.7.9/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      168 2023-08-07 16:53:27.000000 jianglab-0.7.9/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-07 16:53:27.000000 jianglab-0.7.9/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-07 16:53:27.983306 jianglab-0.7.9/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1162 2023-08-07 16:53:18.000000 jianglab-0.7.9/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 17:14:06.792295 jianglab-0.8.0/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-07 17:14:06.791972 jianglab-0.8.0/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.8.0/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 17:14:06.788652 jianglab-0.8.0/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.8.0/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    50330 2023-08-07 17:13:50.000000 jianglab-0.8.0/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.8.0/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-07 17:14:06.791479 jianglab-0.8.0/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-07 17:14:06.000000 jianglab-0.8.0/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-07 17:14:06.000000 jianglab-0.8.0/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-07 17:14:06.000000 jianglab-0.8.0/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      168 2023-08-07 17:14:06.000000 jianglab-0.8.0/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-07 17:14:06.000000 jianglab-0.8.0/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-07 17:14:06.792416 jianglab-0.8.0/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1162 2023-08-07 17:13:57.000000 jianglab-0.8.0/setup.py
```

### Comparing `jianglab-0.7.9/PKG-INFO` & `jianglab-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.7.9
+Version: 0.8.0
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.7.9/README.md` & `jianglab-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.7.9/jianglab/common_functions.py` & `jianglab-0.8.0/jianglab/common_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1230,13 +1230,13 @@
     if recursive:
         files = glob.glob(location + '/**/*', recursive=True)
     else:
         files = glob.glob(location + '/*', recursive=False)
     final_files = []
     for keyword in keyword_list:
         final_files.append([f for f in files if keyword in f])
-        final_files = final_files[0]
-        print(final_files)
+    final_files = final_files[0]
+        #print(final_files)
     for exclude_word in exclude_list:
-        print(exclude_word)
+        #print(exclude_word)
         final_files = [f for f in final_files if exclude_word not in f]
     return final_files
```

### Comparing `jianglab-0.7.9/jianglab.egg-info/PKG-INFO` & `jianglab-0.8.0/jianglab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.7.9
+Version: 0.8.0
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.7.9/setup.py` & `jianglab-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.7.9',
+    version='0.8.0',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

