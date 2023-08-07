# Comparing `tmp/detool-1.0.8.tar.gz` & `tmp/detool-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/detool-1.0.8.tar", last modified: Fri Aug  4 17:07:33 2023, max compression
+gzip compressed data, was "dist/detool-1.0.9.tar", last modified: Mon Aug  7 14:07:04 2023, max compression
```

## Comparing `detool-1.0.8.tar` & `detool-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-04 17:07:33.000000 detool-1.0.8/
--rw-r--r--   0 admin      (501) staff       (20)     2349 2023-08-04 17:07:33.000000 detool-1.0.8/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-04 17:07:33.000000 detool-1.0.8/detool.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     2349 2023-08-04 17:07:32.000000 detool-1.0.8/detool.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      284 2023-08-04 17:07:33.000000 detool-1.0.8/detool.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)       27 2023-08-04 17:07:32.000000 detool-1.0.8/detool.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        7 2023-08-04 17:07:32.000000 detool-1.0.8/detool.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-04 17:07:32.000000 detool-1.0.8/detool.egg-info/dependency_links.txt
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-04 17:07:33.000000 detool-1.0.8/detool/
--rw-r--r--   0 admin      (501) staff       (20)      653 2022-06-09 14:51:49.000000 detool-1.0.8/detool/decr_run_times.py
--rw-r--r--   0 admin      (501) staff       (20)      803 2022-06-07 15:08:29.000000 detool-1.0.8/detool/decr_timer.py
--rw-r--r--   0 admin      (501) staff       (20)      267 2023-08-04 17:06:57.000000 detool-1.0.8/detool/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1164 2023-08-04 17:06:57.000000 detool-1.0.8/detool/decr_class_log.py
--rw-r--r--   0 admin      (501) staff       (20)     3136 2022-08-02 09:56:30.000000 detool-1.0.8/detool/decr_reids_cache.py
--rw-r--r--   0 admin      (501) staff       (20)     1011 2023-08-04 17:06:57.000000 detool-1.0.8/README.md
--rw-r--r--   0 admin      (501) staff       (20)     1288 2023-08-04 17:06:57.000000 detool-1.0.8/setup.py
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-08-04 17:07:33.000000 detool-1.0.8/setup.cfg
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:07:04.000000 detool-1.0.9/
+-rw-r--r--   0 admin      (501) staff       (20)     2932 2023-08-07 14:07:04.000000 detool-1.0.9/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:07:04.000000 detool-1.0.9/detool.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     2932 2023-08-07 14:07:04.000000 detool-1.0.9/detool.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      315 2023-08-07 14:07:04.000000 detool-1.0.9/detool.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)       27 2023-08-07 14:07:04.000000 detool-1.0.9/detool.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        7 2023-08-07 14:07:04.000000 detool-1.0.9/detool.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-07 14:07:04.000000 detool-1.0.9/detool.egg-info/dependency_links.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-07 14:07:04.000000 detool-1.0.9/detool/
+-rw-r--r--   0 admin      (501) staff       (20)      653 2022-06-09 14:51:49.000000 detool-1.0.9/detool/decr_run_times.py
+-rw-r--r--   0 admin      (501) staff       (20)      803 2022-06-07 15:08:29.000000 detool-1.0.9/detool/decr_timer.py
+-rw-r--r--   0 admin      (501) staff       (20)     1126 2023-08-07 14:01:03.000000 detool-1.0.9/detool/decr_class_exception.py
+-rw-r--r--   0 admin      (501) staff       (20)      348 2023-08-07 14:06:24.000000 detool-1.0.9/detool/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1164 2023-08-04 17:06:57.000000 detool-1.0.9/detool/decr_class_log.py
+-rw-r--r--   0 admin      (501) staff       (20)     3136 2022-08-02 09:56:30.000000 detool-1.0.9/detool/decr_reids_cache.py
+-rw-r--r--   0 admin      (501) staff       (20)     1434 2023-08-07 14:06:24.000000 detool-1.0.9/README.md
+-rw-r--r--   0 admin      (501) staff       (20)     1288 2023-08-07 14:07:00.000000 detool-1.0.9/setup.py
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-08-07 14:07:04.000000 detool-1.0.9/setup.cfg
```

### Comparing `detool-1.0.8/PKG-INFO` & `detool-1.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detool
-Version: 1.0.8
+Version: 1.0.9
 Summary: decorator tool collection
 Home-page: UNKNOWN
 Author: abo123456789
 Author-email: abcdef123456chen@sohu.com
 Maintainer: abo123456789
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
@@ -54,14 +54,34 @@
                     return a + b
             @log_decorator
             def calculate(a, b):
                 return a + b
         
             Cal(3).sum(a=3, b=6)
         ```
+        
+        #### 3.异常捕获装饰器
+        ```python
+            from detool import class_exception_decorator,exception_decorator
+        
+            @exception_decorator
+            def r_exception():
+                raise Exception("function Exception raised")
+        
+        
+            @class_exception_decorator
+            class ClassException(object):
+                def r_exception(self):
+                    raise Exception("class Exception raised")
+        
+        
+            r_exception()
+            ClassException().r_exception()
+        ```
+        
 Keywords: detool,decorators
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `detool-1.0.8/detool.egg-info/PKG-INFO` & `detool-1.0.9/detool.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detool
-Version: 1.0.8
+Version: 1.0.9
 Summary: decorator tool collection
 Home-page: UNKNOWN
 Author: abo123456789
 Author-email: abcdef123456chen@sohu.com
 Maintainer: abo123456789
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
@@ -54,14 +54,34 @@
                     return a + b
             @log_decorator
             def calculate(a, b):
                 return a + b
         
             Cal(3).sum(a=3, b=6)
         ```
+        
+        #### 3.异常捕获装饰器
+        ```python
+            from detool import class_exception_decorator,exception_decorator
+        
+            @exception_decorator
+            def r_exception():
+                raise Exception("function Exception raised")
+        
+        
+            @class_exception_decorator
+            class ClassException(object):
+                def r_exception(self):
+                    raise Exception("class Exception raised")
+        
+        
+            r_exception()
+            ClassException().r_exception()
+        ```
+        
 Keywords: detool,decorators
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `detool-1.0.8/detool/decr_run_times.py` & `detool-1.0.9/detool/decr_run_times.py`

 * *Files identical despite different names*

### Comparing `detool-1.0.8/detool/decr_timer.py` & `detool-1.0.9/detool/decr_timer.py`

 * *Files identical despite different names*

### Comparing `detool-1.0.8/detool/decr_class_log.py` & `detool-1.0.9/detool/decr_class_log.py`

 * *Files identical despite different names*

### Comparing `detool-1.0.8/detool/decr_reids_cache.py` & `detool-1.0.9/detool/decr_reids_cache.py`

 * *Files identical despite different names*

### Comparing `detool-1.0.8/setup.py` & `detool-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # @Author cc
 # @TIME 2019/5/25 23:26
 
 from setuptools import setup, find_packages
 
 setup(
     name='detool',
-    version='1.0.8',
+    version='1.0.9',
     description=(
         'decorator tool collection'
     ),
     keywords=("detool", "decorators"),
     long_description_content_type="text/markdown",
     long_description=open('README.md', encoding='utf-8').read(),
     author='abo123456789',
```

