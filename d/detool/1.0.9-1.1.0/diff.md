# Comparing `tmp/detool-1.0.9.tar.gz` & `tmp/detool-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/detool-1.0.9.tar", last modified: Mon Aug  7 14:07:04 2023, max compression
+gzip compressed data, was "dist/detool-1.1.0.tar", last modified: Mon Aug  7 14:10:54 2023, max compression
```

## Comparing `detool-1.0.9.tar` & `detool-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:07:04.000000 detool-1.0.9/
--rw-r--r--   0 admin      (501) staff       (20)     2932 2023-08-07 14:07:04.000000 detool-1.0.9/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:07:04.000000 detool-1.0.9/detool.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     2932 2023-08-07 14:07:04.000000 detool-1.0.9/detool.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      315 2023-08-07 14:07:04.000000 detool-1.0.9/detool.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)       27 2023-08-07 14:07:04.000000 detool-1.0.9/detool.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        7 2023-08-07 14:07:04.000000 detool-1.0.9/detool.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-07 14:07:04.000000 detool-1.0.9/detool.egg-info/dependency_links.txt
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:07:04.000000 detool-1.0.9/detool/
--rw-r--r--   0 admin      (501) staff       (20)      653 2022-06-09 14:51:49.000000 detool-1.0.9/detool/decr_run_times.py
--rw-r--r--   0 admin      (501) staff       (20)      803 2022-06-07 15:08:29.000000 detool-1.0.9/detool/decr_timer.py
--rw-r--r--   0 admin      (501) staff       (20)     1126 2023-08-07 14:01:03.000000 detool-1.0.9/detool/decr_class_exception.py
--rw-r--r--   0 admin      (501) staff       (20)      348 2023-08-07 14:06:24.000000 detool-1.0.9/detool/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1164 2023-08-04 17:06:57.000000 detool-1.0.9/detool/decr_class_log.py
--rw-r--r--   0 admin      (501) staff       (20)     3136 2022-08-02 09:56:30.000000 detool-1.0.9/detool/decr_reids_cache.py
--rw-r--r--   0 admin      (501) staff       (20)     1434 2023-08-07 14:06:24.000000 detool-1.0.9/README.md
--rw-r--r--   0 admin      (501) staff       (20)     1288 2023-08-07 14:07:00.000000 detool-1.0.9/setup.py
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-08-07 14:07:04.000000 detool-1.0.9/setup.cfg
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:10:54.000000 detool-1.1.0/
+-rw-r--r--   0 admin      (501) staff       (20)     2932 2023-08-07 14:10:54.000000 detool-1.1.0/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1434 2023-08-07 14:10:32.000000 detool-1.1.0/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:10:54.000000 detool-1.1.0/detool/
+-rw-r--r--   0 admin      (501) staff       (20)      348 2023-08-07 14:06:24.000000 detool-1.1.0/detool/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1126 2023-08-07 14:01:03.000000 detool-1.1.0/detool/decr_class_exception.py
+-rw-r--r--   0 admin      (501) staff       (20)     1164 2023-08-04 17:06:57.000000 detool-1.1.0/detool/decr_class_log.py
+-rw-r--r--   0 admin      (501) staff       (20)     3136 2022-08-02 09:56:30.000000 detool-1.1.0/detool/decr_reids_cache.py
+-rw-r--r--   0 admin      (501) staff       (20)      653 2022-06-09 14:51:49.000000 detool-1.1.0/detool/decr_run_times.py
+-rw-r--r--   0 admin      (501) staff       (20)      803 2022-06-07 15:08:29.000000 detool-1.1.0/detool/decr_timer.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:10:54.000000 detool-1.1.0/detool.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     2932 2023-08-07 14:10:54.000000 detool-1.1.0/detool.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      315 2023-08-07 14:10:54.000000 detool-1.1.0/detool.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-07 14:10:54.000000 detool-1.1.0/detool.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       27 2023-08-07 14:10:54.000000 detool-1.1.0/detool.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        7 2023-08-07 14:10:54.000000 detool-1.1.0/detool.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-08-07 14:10:54.000000 detool-1.1.0/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1288 2023-08-07 14:10:32.000000 detool-1.1.0/setup.py
```

### Comparing `detool-1.0.9/PKG-INFO` & `detool-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detool
-Version: 1.0.9
+Version: 1.1.0
 Summary: decorator tool collection
 Home-page: UNKNOWN
 Author: abo123456789
 Author-email: abcdef123456chen@sohu.com
 Maintainer: abo123456789
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
@@ -55,15 +55,15 @@
             @log_decorator
             def calculate(a, b):
                 return a + b
         
             Cal(3).sum(a=3, b=6)
         ```
         
-        #### 3.异常捕获装饰器
+        #### 4.异常捕获装饰器
         ```python
             from detool import class_exception_decorator,exception_decorator
         
             @exception_decorator
             def r_exception():
                 raise Exception("function Exception raised")
```

### Comparing `detool-1.0.9/detool.egg-info/PKG-INFO` & `detool-1.1.0/detool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detool
-Version: 1.0.9
+Version: 1.1.0
 Summary: decorator tool collection
 Home-page: UNKNOWN
 Author: abo123456789
 Author-email: abcdef123456chen@sohu.com
 Maintainer: abo123456789
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
@@ -55,15 +55,15 @@
             @log_decorator
             def calculate(a, b):
                 return a + b
         
             Cal(3).sum(a=3, b=6)
         ```
         
-        #### 3.异常捕获装饰器
+        #### 4.异常捕获装饰器
         ```python
             from detool import class_exception_decorator,exception_decorator
         
             @exception_decorator
             def r_exception():
                 raise Exception("function Exception raised")
```

### Comparing `detool-1.0.9/detool/decr_run_times.py` & `detool-1.1.0/detool/decr_run_times.py`

 * *Files identical despite different names*

### Comparing `detool-1.0.9/detool/decr_timer.py` & `detool-1.1.0/detool/decr_timer.py`

 * *Files identical despite different names*

### Comparing `detool-1.0.9/detool/decr_class_exception.py` & `detool-1.1.0/detool/decr_class_exception.py`

 * *Files identical despite different names*

### Comparing `detool-1.0.9/detool/decr_class_log.py` & `detool-1.1.0/detool/decr_class_log.py`

 * *Files identical despite different names*

### Comparing `detool-1.0.9/detool/decr_reids_cache.py` & `detool-1.1.0/detool/decr_reids_cache.py`

 * *Files identical despite different names*

### Comparing `detool-1.0.9/README.md` & `detool-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     @log_decorator
     def calculate(a, b):
         return a + b
 
     Cal(3).sum(a=3, b=6)
 ```
 
-#### 3.异常捕获装饰器
+#### 4.异常捕获装饰器
 ```python
     from detool import class_exception_decorator,exception_decorator
 
     @exception_decorator
     def r_exception():
         raise Exception("function Exception raised")
```

### Comparing `detool-1.0.9/setup.py` & `detool-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # @Author cc
 # @TIME 2019/5/25 23:26
 
 from setuptools import setup, find_packages
 
 setup(
     name='detool',
-    version='1.0.9',
+    version='1.1.0',
     description=(
         'decorator tool collection'
     ),
     keywords=("detool", "decorators"),
     long_description_content_type="text/markdown",
     long_description=open('README.md', encoding='utf-8').read(),
     author='abo123456789',
```

