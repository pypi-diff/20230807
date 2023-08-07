# Comparing `tmp/HaploDynamics-0.1b7.tar.gz` & `tmp/HaploDynamics-0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HaploDynamics-0.1b7.tar", last modified: Mon Aug  7 02:14:29 2023, max compression
+gzip compressed data, was "HaploDynamics-0.1b9.tar", last modified: Mon Aug  7 02:23:37 2023, max compression
```

## Comparing `HaploDynamics-0.1b7.tar` & `HaploDynamics-0.1b9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:14:29.014267 HaploDynamics-0.1b7/
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:14:29.014267 HaploDynamics-0.1b7/HaploDynamics/
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:14:29.014267 HaploDynamics-0.1b7/HaploDynamics/Framework/
--rw-rw-r--   0 remy      (1000) remy      (1000)       22 2023-08-07 02:13:05.000000 HaploDynamics-0.1b7/HaploDynamics/Framework/__init__.py
--rw-rw-r--   0 remy      (1000) remy      (1000)       67 2023-08-07 02:13:05.000000 HaploDynamics-0.1b7/HaploDynamics/Framework/future.py
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:14:29.014267 HaploDynamics-0.1b7/HaploDynamics/HaploDX/
--rw-rw-r--   0 remy      (1000) remy      (1000)    17508 2023-08-07 02:13:05.000000 HaploDynamics-0.1b7/HaploDynamics/HaploDX/HaploDX.py
--rw-rw-r--   0 remy      (1000) remy      (1000)       23 2023-08-07 02:13:05.000000 HaploDynamics-0.1b7/HaploDynamics/HaploDX/__init__.py
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:14:29.014267 HaploDynamics-0.1b7/HaploDynamics.egg-info/
--rw-rw-r--   0 remy      (1000) remy      (1000)     9277 2023-08-07 02:14:28.000000 HaploDynamics-0.1b7/HaploDynamics.egg-info/PKG-INFO
--rw-rw-r--   0 remy      (1000) remy      (1000)      357 2023-08-07 02:14:28.000000 HaploDynamics-0.1b7/HaploDynamics.egg-info/SOURCES.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-07 02:14:28.000000 HaploDynamics-0.1b7/HaploDynamics.egg-info/dependency_links.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)        6 2023-08-07 02:14:28.000000 HaploDynamics-0.1b7/HaploDynamics.egg-info/requires.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)       14 2023-08-07 02:14:28.000000 HaploDynamics-0.1b7/HaploDynamics.egg-info/top_level.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)    35149 2023-08-07 02:13:05.000000 HaploDynamics-0.1b7/LICENSE
--rw-rw-r--   0 remy      (1000) remy      (1000)     9277 2023-08-07 02:14:29.014267 HaploDynamics-0.1b7/PKG-INFO
--rw-rw-r--   0 remy      (1000) remy      (1000)     8393 2023-08-07 02:13:05.000000 HaploDynamics-0.1b7/README.md
--rw-rw-r--   0 remy      (1000) remy      (1000)       79 2023-08-07 02:14:29.014267 HaploDynamics-0.1b7/setup.cfg
--rw-rw-r--   0 remy      (1000) remy      (1000)     1241 2023-08-07 02:13:05.000000 HaploDynamics-0.1b7/setup.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:23:37.812746 HaploDynamics-0.1b9/
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:23:37.812746 HaploDynamics-0.1b9/HaploDynamics/
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:23:37.812746 HaploDynamics-0.1b9/HaploDynamics/Framework/
+-rw-rw-r--   0 remy      (1000) remy      (1000)       22 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/HaploDynamics/Framework/__init__.py
+-rw-rw-r--   0 remy      (1000) remy      (1000)       67 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/HaploDynamics/Framework/future.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:23:37.812746 HaploDynamics-0.1b9/HaploDynamics/HaploDX/
+-rw-rw-r--   0 remy      (1000) remy      (1000)    17508 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/HaploDynamics/HaploDX/HaploDX.py
+-rw-rw-r--   0 remy      (1000) remy      (1000)       23 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/HaploDynamics/HaploDX/__init__.py
+-rw-rw-r--   0 remy      (1000) remy      (1000)       60 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/HaploDynamics/__init__.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:23:37.812746 HaploDynamics-0.1b9/HaploDynamics.egg-info/
+-rw-rw-r--   0 remy      (1000) remy      (1000)     9277 2023-08-07 02:23:37.000000 HaploDynamics-0.1b9/HaploDynamics.egg-info/PKG-INFO
+-rw-rw-r--   0 remy      (1000) remy      (1000)      383 2023-08-07 02:23:37.000000 HaploDynamics-0.1b9/HaploDynamics.egg-info/SOURCES.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-07 02:23:37.000000 HaploDynamics-0.1b9/HaploDynamics.egg-info/dependency_links.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        6 2023-08-07 02:23:37.000000 HaploDynamics-0.1b9/HaploDynamics.egg-info/requires.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)       14 2023-08-07 02:23:37.000000 HaploDynamics-0.1b9/HaploDynamics.egg-info/top_level.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)    35149 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/LICENSE
+-rw-rw-r--   0 remy      (1000) remy      (1000)     9277 2023-08-07 02:23:37.816745 HaploDynamics-0.1b9/PKG-INFO
+-rw-rw-r--   0 remy      (1000) remy      (1000)     8393 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/README.md
+-rw-rw-r--   0 remy      (1000) remy      (1000)       79 2023-08-07 02:23:37.816745 HaploDynamics-0.1b9/setup.cfg
+-rw-rw-r--   0 remy      (1000) remy      (1000)     1257 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/setup.py
```

### Comparing `HaploDynamics-0.1b7/HaploDynamics/HaploDX/HaploDX.py` & `HaploDynamics-0.1b9/HaploDynamics/HaploDX/HaploDX.py`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.1b7/HaploDynamics.egg-info/PKG-INFO` & `HaploDynamics-0.1b9/HaploDynamics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HaploDynamics
-Version: 0.1b7
+Version: 0.1b9
 Summary: A python library to develop genomic data simulators
 Home-page: https://github.com/remytuyeras/HaploDynamics
-Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.7.tar.gz
+Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.9.tar.gz
 Author: Remy Tuyeras
 Author-email: rtuyeras@gmail.com
 License: gpl-3.0
 Keywords: Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage disequilibrium,Hardy-Weinberg equilibrium
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b7 Summary: A python
+Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b9 Summary: A python
 library to develop genomic data simulators Home-page: https://github.com/
 remytuyeras/HaploDynamics Download-URL: https://github.com/remytuyeras/
-HaploDynamics/archive/refs/tags/v0.1-beta.7.tar.gz Author: Remy Tuyeras Author-
+HaploDynamics/archive/refs/tags/v0.1-beta.9.tar.gz Author: Remy Tuyeras Author-
 email: rtuyeras@gmail.com License: gpl-3.0 Keywords:
 Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage
 disequilibrium,Hardy-Weinberg equilibrium Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Intended Audience
 :: Science/Research Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `HaploDynamics-0.1b7/LICENSE` & `HaploDynamics-0.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.1b7/PKG-INFO` & `HaploDynamics-0.1b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HaploDynamics
-Version: 0.1b7
+Version: 0.1b9
 Summary: A python library to develop genomic data simulators
 Home-page: https://github.com/remytuyeras/HaploDynamics
-Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.7.tar.gz
+Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.9.tar.gz
 Author: Remy Tuyeras
 Author-email: rtuyeras@gmail.com
 License: gpl-3.0
 Keywords: Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage disequilibrium,Hardy-Weinberg equilibrium
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b7 Summary: A python
+Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b9 Summary: A python
 library to develop genomic data simulators Home-page: https://github.com/
 remytuyeras/HaploDynamics Download-URL: https://github.com/remytuyeras/
-HaploDynamics/archive/refs/tags/v0.1-beta.7.tar.gz Author: Remy Tuyeras Author-
+HaploDynamics/archive/refs/tags/v0.1-beta.9.tar.gz Author: Remy Tuyeras Author-
 email: rtuyeras@gmail.com License: gpl-3.0 Keywords:
 Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage
 disequilibrium,Hardy-Weinberg equilibrium Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Intended Audience
 :: Science/Research Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `HaploDynamics-0.1b7/README.md` & `HaploDynamics-0.1b9/README.md`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.1b7/setup.py` & `HaploDynamics-0.1b9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name = 'HaploDynamics',
-  packages=setuptools.find_packages(include=['HaploDynamics.HaploDX','HaploDynamics.Framework']),
-  version = 'v0.1-beta.7',
+  packages=setuptools.find_packages(include=['HaploDynamics','HaploDynamics.HaploDX','HaploDynamics.Framework']),
+  version = 'v0.1-beta.9',
   license='gpl-3.0',
   author = 'Remy Tuyeras',
   author_email = 'rtuyeras@gmail.com',
   description = 'A python library to develop genomic data simulators',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   url = 'https://github.com/remytuyeras/HaploDynamics',
-  download_url = 'https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.7.tar.gz',
+  download_url = 'https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.9.tar.gz',
   keywords = ['Simulator', 'Genomics', 'Genomic', 'Microarray','SNP chip','VCF', 'Linkage disequilibrium', 'Hardy-Weinberg equilibrium'],
   install_requires=['scipy'],
   classifiers=[
     'Development Status :: 4 - Beta',  #"3 - Alpha", "4 - Beta" or "5 - Production/Stable"
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Topic :: Software Development :: Build Tools',
```

