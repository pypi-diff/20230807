# Comparing `tmp/rand-omata-0.0.4.tar.gz` & `tmp/rand-omata-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rand-omata-0.0.4.tar", last modified: Mon Aug  7 16:54:35 2023, max compression
+gzip compressed data, was "rand-omata-0.0.5.tar", last modified: Mon Aug  7 17:02:47 2023, max compression
```

## Comparing `rand-omata-0.0.4.tar` & `rand-omata-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 16:54:35.597980 rand-omata-0.0.4/
--rw-rw-rw-   0        0        0       85 2023-08-07 16:50:49.000000 rand-omata-0.0.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0       25 2023-08-07 15:34:04.000000 rand-omata-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      988 2023-08-07 16:54:35.597980 rand-omata-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-08-07 16:50:21.000000 rand-omata-0.0.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-08-07 16:54:35.597980 rand-omata-0.0.4/rand_omata/
--rw-rw-rw-   0        0        0        0 2023-08-07 16:51:31.000000 rand-omata-0.0.4/rand_omata/__init__.py
--rw-rw-rw-   0        0        0     1498 2023-08-07 16:51:34.000000 rand-omata-0.0.4/rand_omata/rand_omata.py
-drwxrwxrwx   0        0        0        0 2023-08-07 16:54:35.597980 rand-omata-0.0.4/rand_omata.egg-info/
--rw-rw-rw-   0        0        0      988 2023-08-07 16:54:35.000000 rand-omata-0.0.4/rand_omata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-08-07 16:54:35.000000 rand-omata-0.0.4/rand_omata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 16:54:35.000000 rand-omata-0.0.4/rand_omata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-08-07 16:54:35.000000 rand-omata-0.0.4/rand_omata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 16:54:35.613602 rand-omata-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      783 2023-08-07 16:54:15.000000 rand-omata-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:02:47.903262 rand-omata-0.0.5/
+-rw-rw-rw-   0        0        0       83 2023-08-07 17:02:34.000000 rand-omata-0.0.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0       25 2023-08-07 17:00:45.000000 rand-omata-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1041 2023-08-07 17:02:47.903262 rand-omata-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-08-07 17:02:29.000000 rand-omata-0.0.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 17:02:47.887639 rand-omata-0.0.5/rand_omata/
+-rw-rw-rw-   0        0        0        0 2023-08-07 16:51:31.000000 rand-omata-0.0.5/rand_omata/__init__.py
+-rw-rw-rw-   0        0        0     1498 2023-08-07 17:02:38.000000 rand-omata-0.0.5/rand_omata/rand_omata.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:02:47.903262 rand-omata-0.0.5/rand_omata.egg-info/
+-rw-rw-rw-   0        0        0     1041 2023-08-07 17:02:47.000000 rand-omata-0.0.5/rand_omata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-08-07 17:02:47.000000 rand-omata-0.0.5/rand_omata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 17:02:47.000000 rand-omata-0.0.5/rand_omata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-07 17:02:47.000000 rand-omata-0.0.5/rand_omata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 17:02:47.903262 rand-omata-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      751 2023-08-07 17:02:19.000000 rand-omata-0.0.5/setup.py
```

### Comparing `rand-omata-0.0.4/PKG-INFO` & `rand-omata-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: rand-omata
-Version: 0.0.4
-Summary: 'It's a matrix generator which can return random data matrix which can be used for data science!/nMore Functions will come later
+Version: 0.0.5
+Summary: 'It's a matrix generator which can return random data matrix which can be used for data science!
 Home-page: https://github.com/Major-Manu/rand-omata.git
 Author: Major Manu
 Author-email: majors00production@gmail.com
 Keywords: matrix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python :: 3
 
-This Project is being made for the sole purpose of generating random data for matrices!
-I have tried this as a simple project to boost my moral and give me the little bit of dopemine which i have been waiting from the start of the project!!!
-I hope somebody will stumbe upon this liberary and use it for their own project!
-I can only hope! 
+#rand-omata
+---
+## Random Data
+---
+### More functions to come soon!
+---
+-This Project is being made for the sole purpose of generating random data for matrices!
+-I have tried this as a simple project to boost my moral and give me the little bit of dopemine which i have been waiting from the start of the project!!!
+-I hope somebody will stumbe upon this liberary and use it for their own project!
+-I can only hope! 
+---
 
 Change Log
 ==========
 
-0.0.4 (07/08/2023)
+0.0.5 (07/08/2023)
 -------------------
-- Second Release
+-Third Release
```

### Comparing `rand-omata-0.0.4/rand_omata/rand_omata.py` & `rand-omata-0.0.5/rand_omata/rand_omata.py`

 * *Files identical despite different names*

### Comparing `rand-omata-0.0.4/rand_omata.egg-info/PKG-INFO` & `rand-omata-0.0.5/rand_omata.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: rand-omata
-Version: 0.0.4
-Summary: 'It's a matrix generator which can return random data matrix which can be used for data science!/nMore Functions will come later
+Version: 0.0.5
+Summary: 'It's a matrix generator which can return random data matrix which can be used for data science!
 Home-page: https://github.com/Major-Manu/rand-omata.git
 Author: Major Manu
 Author-email: majors00production@gmail.com
 Keywords: matrix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python :: 3
 
-This Project is being made for the sole purpose of generating random data for matrices!
-I have tried this as a simple project to boost my moral and give me the little bit of dopemine which i have been waiting from the start of the project!!!
-I hope somebody will stumbe upon this liberary and use it for their own project!
-I can only hope! 
+#rand-omata
+---
+## Random Data
+---
+### More functions to come soon!
+---
+-This Project is being made for the sole purpose of generating random data for matrices!
+-I have tried this as a simple project to boost my moral and give me the little bit of dopemine which i have been waiting from the start of the project!!!
+-I hope somebody will stumbe upon this liberary and use it for their own project!
+-I can only hope! 
+---
 
 Change Log
 ==========
 
-0.0.4 (07/08/2023)
+0.0.5 (07/08/2023)
 -------------------
-- Second Release
+-Third Release
```

### Comparing `rand-omata-0.0.4/setup.py` & `rand-omata-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,16 @@
   'Intended Audience :: Developers',
   'Operating System :: Microsoft :: Windows :: Windows 11',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='rand-omata',
-  version='0.0.4',
-  description="'It's a matrix generator which can return random data matrix which can be used for data science!/nMore Functions will come later",
+  version='0.0.5',
+  description="'It's a matrix generator which can return random data matrix which can be used for data science!",
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='https://github.com/Major-Manu/rand-omata.git',  
   author='Major Manu',
   author_email='majors00production@gmail.com',
   classifiers=classifiers,
   keywords='matrix', 
   packages=find_packages(),
```

