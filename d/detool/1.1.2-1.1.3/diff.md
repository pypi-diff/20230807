# Comparing `tmp/detool-1.1.2.tar.gz` & `tmp/detool-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/detool-1.1.2.tar", last modified: Mon Aug  7 14:31:31 2023, max compression
+gzip compressed data, was "dist/detool-1.1.3.tar", last modified: Mon Aug  7 14:36:25 2023, max compression
```

## Comparing `detool-1.1.2.tar` & `detool-1.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:31:31.000000 detool-1.1.2/
--rw-r--r--   0 admin      (501) staff       (20)     3189 2023-08-07 14:31:31.000000 detool-1.1.2/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     1603 2023-08-07 14:24:35.000000 detool-1.1.2/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:31:31.000000 detool-1.1.2/detool/
--rw-r--r--   0 admin      (501) staff       (20)      385 2023-08-07 14:31:11.000000 detool-1.1.2/detool/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1126 2023-08-07 14:01:03.000000 detool-1.1.2/detool/decr_class_exception.py
--rw-r--r--   0 admin      (501) staff       (20)     1164 2023-08-04 17:06:57.000000 detool-1.1.2/detool/decr_class_log.py
--rw-r--r--   0 admin      (501) staff       (20)     3136 2022-08-02 09:56:30.000000 detool-1.1.2/detool/decr_reids_cache.py
--rw-r--r--   0 admin      (501) staff       (20)      653 2022-06-09 14:51:49.000000 detool-1.1.2/detool/decr_run_times.py
--rw-r--r--   0 admin      (501) staff       (20)      803 2022-06-07 15:08:29.000000 detool-1.1.2/detool/decr_timer.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:31:31.000000 detool-1.1.2/detool.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     3189 2023-08-07 14:31:31.000000 detool-1.1.2/detool.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      315 2023-08-07 14:31:31.000000 detool-1.1.2/detool.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-07 14:31:31.000000 detool-1.1.2/detool.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       51 2023-08-07 14:31:31.000000 detool-1.1.2/detool.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        7 2023-08-07 14:31:31.000000 detool-1.1.2/detool.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-08-07 14:31:31.000000 detool-1.1.2/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1323 2023-08-07 14:31:26.000000 detool-1.1.2/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:36:25.000000 detool-1.1.3/
+-rw-r--r--   0 admin      (501) staff       (20)     3192 2023-08-07 14:36:25.000000 detool-1.1.3/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1606 2023-08-07 14:34:43.000000 detool-1.1.3/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:36:25.000000 detool-1.1.3/detool/
+-rw-r--r--   0 admin      (501) staff       (20)      385 2023-08-07 14:31:11.000000 detool-1.1.3/detool/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1126 2023-08-07 14:01:03.000000 detool-1.1.3/detool/decr_class_exception.py
+-rw-r--r--   0 admin      (501) staff       (20)     1164 2023-08-04 17:06:57.000000 detool-1.1.3/detool/decr_class_log.py
+-rw-r--r--   0 admin      (501) staff       (20)     3136 2022-08-02 09:56:30.000000 detool-1.1.3/detool/decr_reids_cache.py
+-rw-r--r--   0 admin      (501) staff       (20)      653 2022-06-09 14:51:49.000000 detool-1.1.3/detool/decr_run_times.py
+-rw-r--r--   0 admin      (501) staff       (20)      803 2022-06-07 15:08:29.000000 detool-1.1.3/detool/decr_timer.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:36:25.000000 detool-1.1.3/detool.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     3192 2023-08-07 14:36:25.000000 detool-1.1.3/detool.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      315 2023-08-07 14:36:25.000000 detool-1.1.3/detool.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-07 14:36:25.000000 detool-1.1.3/detool.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       51 2023-08-07 14:36:25.000000 detool-1.1.3/detool.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        7 2023-08-07 14:36:25.000000 detool-1.1.3/detool.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-08-07 14:36:25.000000 detool-1.1.3/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1323 2023-08-07 14:36:21.000000 detool-1.1.3/setup.py
```

### Comparing `detool-1.1.2/PKG-INFO` & `detool-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detool
-Version: 1.1.2
+Version: 1.1.3
 Summary: decorator tool collection
 Home-page: UNKNOWN
 Author: abo123456789
 Author-email: abcdef123456chen@sohu.com
 Maintainer: abo123456789
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
@@ -74,15 +74,15 @@
                     raise Exception("class Exception raised")
         
         
             r_exception()
             ClassException().r_exception()
         ```
         
-        #### 5.分析内装饰器
+        #### 5.分析内存装饰器
         ```python
             from detool import profile
         
             @profile
             def t_memory():
                 return [i for i in range(1, 1001)]
```

### Comparing `detool-1.1.2/README.md` & `detool-1.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             raise Exception("class Exception raised")
 
 
     r_exception()
     ClassException().r_exception()
 ```
 
-#### 5.分析内装饰器
+#### 5.分析内存装饰器
 ```python
     from detool import profile
 
     @profile
     def t_memory():
         return [i for i in range(1, 1001)]
```

### Comparing `detool-1.1.2/detool/decr_class_exception.py` & `detool-1.1.3/detool/decr_class_exception.py`

 * *Files identical despite different names*

### Comparing `detool-1.1.2/detool/decr_class_log.py` & `detool-1.1.3/detool/decr_class_log.py`

 * *Files identical despite different names*

### Comparing `detool-1.1.2/detool/decr_reids_cache.py` & `detool-1.1.3/detool/decr_reids_cache.py`

 * *Files identical despite different names*

### Comparing `detool-1.1.2/detool/decr_run_times.py` & `detool-1.1.3/detool/decr_run_times.py`

 * *Files identical despite different names*

### Comparing `detool-1.1.2/detool/decr_timer.py` & `detool-1.1.3/detool/decr_timer.py`

 * *Files identical despite different names*

### Comparing `detool-1.1.2/detool.egg-info/PKG-INFO` & `detool-1.1.3/detool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detool
-Version: 1.1.2
+Version: 1.1.3
 Summary: decorator tool collection
 Home-page: UNKNOWN
 Author: abo123456789
 Author-email: abcdef123456chen@sohu.com
 Maintainer: abo123456789
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
@@ -74,15 +74,15 @@
                     raise Exception("class Exception raised")
         
         
             r_exception()
             ClassException().r_exception()
         ```
         
-        #### 5.分析内装饰器
+        #### 5.分析内存装饰器
         ```python
             from detool import profile
         
             @profile
             def t_memory():
                 return [i for i in range(1, 1001)]
```

### Comparing `detool-1.1.2/setup.py` & `detool-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # @Author cc
 # @TIME 2019/5/25 23:26
 
 from setuptools import setup, find_packages
 
 setup(
     name='detool',
-    version='1.1.2',
+    version='1.1.3',
     description=(
         'decorator tool collection'
     ),
     keywords=("detool", "decorators"),
     long_description_content_type="text/markdown",
     long_description=open('README.md', encoding='utf-8').read(),
     author='abo123456789',
```

