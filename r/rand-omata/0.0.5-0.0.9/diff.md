# Comparing `tmp/rand-omata-0.0.5.tar.gz` & `tmp/rand-omata-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rand-omata-0.0.5.tar", last modified: Mon Aug  7 17:02:47 2023, max compression
+gzip compressed data, was "rand-omata-0.0.9.tar", last modified: Mon Aug  7 17:17:10 2023, max compression
```

## Comparing `rand-omata-0.0.5.tar` & `rand-omata-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 17:02:47.903262 rand-omata-0.0.5/
--rw-rw-rw-   0        0        0       83 2023-08-07 17:02:34.000000 rand-omata-0.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0       25 2023-08-07 17:00:45.000000 rand-omata-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1041 2023-08-07 17:02:47.903262 rand-omata-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-08-07 17:02:29.000000 rand-omata-0.0.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-08-07 17:02:47.887639 rand-omata-0.0.5/rand_omata/
--rw-rw-rw-   0        0        0        0 2023-08-07 16:51:31.000000 rand-omata-0.0.5/rand_omata/__init__.py
--rw-rw-rw-   0        0        0     1498 2023-08-07 17:02:38.000000 rand-omata-0.0.5/rand_omata/rand_omata.py
-drwxrwxrwx   0        0        0        0 2023-08-07 17:02:47.903262 rand-omata-0.0.5/rand_omata.egg-info/
--rw-rw-rw-   0        0        0     1041 2023-08-07 17:02:47.000000 rand-omata-0.0.5/rand_omata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-08-07 17:02:47.000000 rand-omata-0.0.5/rand_omata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 17:02:47.000000 rand-omata-0.0.5/rand_omata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-08-07 17:02:47.000000 rand-omata-0.0.5/rand_omata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 17:02:47.903262 rand-omata-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      751 2023-08-07 17:02:19.000000 rand-omata-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:17:10.902969 rand-omata-0.0.9/
+-rw-rw-rw-   0        0        0      519 2023-08-07 17:16:53.000000 rand-omata-0.0.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0       25 2023-08-07 17:00:45.000000 rand-omata-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1392 2023-08-07 17:17:10.902969 rand-omata-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-08-07 17:16:28.000000 rand-omata-0.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 17:17:10.887342 rand-omata-0.0.9/rand_omata/
+-rw-rw-rw-   0        0        0        0 2023-08-07 16:51:31.000000 rand-omata-0.0.9/rand_omata/__init__.py
+-rw-rw-rw-   0        0        0     1498 2023-08-07 17:02:38.000000 rand-omata-0.0.9/rand_omata/rand_omata.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:17:10.902969 rand-omata-0.0.9/rand_omata.egg-info/
+-rw-rw-rw-   0        0        0     1392 2023-08-07 17:17:10.000000 rand-omata-0.0.9/rand_omata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-08-07 17:17:10.000000 rand-omata-0.0.9/rand_omata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 17:17:10.000000 rand-omata-0.0.9/rand_omata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-07 17:17:10.000000 rand-omata-0.0.9/rand_omata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 17:17:10.902969 rand-omata-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      751 2023-08-07 17:16:40.000000 rand-omata-0.0.9/setup.py
```

### Comparing `rand-omata-0.0.5/PKG-INFO` & `rand-omata-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: rand-omata
-Version: 0.0.5
+Version: 0.0.9
 Summary: 'It's a matrix generator which can return random data matrix which can be used for data science!
 Home-page: https://github.com/Major-Manu/rand-omata.git
 Author: Major Manu
 Author-email: majors00production@gmail.com
 Keywords: matrix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python :: 3
 
+This Project is being made for the sole purpose of generating random data for matrices! 
+I have tried this as a simple project to boost my moral and give me the little bit of dopemine which i have been waiting from the start of the project!!! 
+I hope somebody will stumbe upon this liberary and use it for their own project! 
+I can only hope!
+
+Change Log
+==========
+
 #rand-omata
 ---
 ## Random Data
 ---
 ### More functions to come soon!
 ---
 -This Project is being made for the sole purpose of generating random data for matrices!
 -I have tried this as a simple project to boost my moral and give me the little bit of dopemine which i have been waiting from the start of the project!!!
 -I hope somebody will stumbe upon this liberary and use it for their own project!
 -I can only hope! 
 ---
 
-Change Log
-==========
 
 0.0.5 (07/08/2023)
 -------------------
 -Third Release
```

### Comparing `rand-omata-0.0.5/rand_omata/rand_omata.py` & `rand-omata-0.0.9/rand_omata/rand_omata.py`

 * *Files identical despite different names*

### Comparing `rand-omata-0.0.5/rand_omata.egg-info/PKG-INFO` & `rand-omata-0.0.9/rand_omata.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: rand-omata
-Version: 0.0.5
+Version: 0.0.9
 Summary: 'It's a matrix generator which can return random data matrix which can be used for data science!
 Home-page: https://github.com/Major-Manu/rand-omata.git
 Author: Major Manu
 Author-email: majors00production@gmail.com
 Keywords: matrix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python :: 3
 
+This Project is being made for the sole purpose of generating random data for matrices! 
+I have tried this as a simple project to boost my moral and give me the little bit of dopemine which i have been waiting from the start of the project!!! 
+I hope somebody will stumbe upon this liberary and use it for their own project! 
+I can only hope!
+
+Change Log
+==========
+
 #rand-omata
 ---
 ## Random Data
 ---
 ### More functions to come soon!
 ---
 -This Project is being made for the sole purpose of generating random data for matrices!
 -I have tried this as a simple project to boost my moral and give me the little bit of dopemine which i have been waiting from the start of the project!!!
 -I hope somebody will stumbe upon this liberary and use it for their own project!
 -I can only hope! 
 ---
 
-Change Log
-==========
 
 0.0.5 (07/08/2023)
 -------------------
 -Third Release
```

### Comparing `rand-omata-0.0.5/setup.py` & `rand-omata-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   'Intended Audience :: Developers',
   'Operating System :: Microsoft :: Windows :: Windows 11',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='rand-omata',
-  version='0.0.5',
+  version='0.0.9',
   description="'It's a matrix generator which can return random data matrix which can be used for data science!",
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='https://github.com/Major-Manu/rand-omata.git',  
   author='Major Manu',
   author_email='majors00production@gmail.com',
   classifiers=classifiers,
   keywords='matrix',
```

