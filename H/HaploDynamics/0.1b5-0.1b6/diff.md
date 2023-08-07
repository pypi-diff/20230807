# Comparing `tmp/HaploDynamics-0.1b5.tar.gz` & `tmp/HaploDynamics-0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HaploDynamics-0.1b5.tar", last modified: Mon Aug  7 01:34:50 2023, max compression
+gzip compressed data, was "HaploDynamics-0.1b6.tar", last modified: Mon Aug  7 01:44:48 2023, max compression
```

## Comparing `HaploDynamics-0.1b5.tar` & `HaploDynamics-0.1b6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 01:34:50.877431 HaploDynamics-0.1b5/
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 01:34:50.877431 HaploDynamics-0.1b5/HaploDynamics/
--rw-rw-r--   0 remy      (1000) remy      (1000)       60 2023-08-07 01:26:43.000000 HaploDynamics-0.1b5/HaploDynamics/__init__.py
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 01:34:50.877431 HaploDynamics-0.1b5/HaploDynamics.egg-info/
--rw-rw-r--   0 remy      (1000) remy      (1000)     9277 2023-08-07 01:34:50.000000 HaploDynamics-0.1b5/HaploDynamics.egg-info/PKG-INFO
--rw-rw-r--   0 remy      (1000) remy      (1000)      246 2023-08-07 01:34:50.000000 HaploDynamics-0.1b5/HaploDynamics.egg-info/SOURCES.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-07 01:34:50.000000 HaploDynamics-0.1b5/HaploDynamics.egg-info/dependency_links.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)        6 2023-08-07 01:34:50.000000 HaploDynamics-0.1b5/HaploDynamics.egg-info/requires.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)       14 2023-08-07 01:34:50.000000 HaploDynamics-0.1b5/HaploDynamics.egg-info/top_level.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)    35149 2023-08-07 01:26:43.000000 HaploDynamics-0.1b5/LICENSE
--rw-rw-r--   0 remy      (1000) remy      (1000)     9277 2023-08-07 01:34:50.877431 HaploDynamics-0.1b5/PKG-INFO
--rw-rw-r--   0 remy      (1000) remy      (1000)     8393 2023-08-07 01:26:43.000000 HaploDynamics-0.1b5/README.md
--rw-rw-r--   0 remy      (1000) remy      (1000)       79 2023-08-07 01:34:50.877431 HaploDynamics-0.1b5/setup.cfg
--rw-rw-r--   0 remy      (1000) remy      (1000)     1207 2023-08-07 01:33:11.000000 HaploDynamics-0.1b5/setup.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 01:44:48.082907 HaploDynamics-0.1b6/
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 01:44:48.082907 HaploDynamics-0.1b6/HaploDynamics/
+-rw-rw-r--   0 remy      (1000) remy      (1000)       60 2023-08-07 01:26:43.000000 HaploDynamics-0.1b6/HaploDynamics/__init__.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 01:44:48.082907 HaploDynamics-0.1b6/HaploDynamics.egg-info/
+-rw-rw-r--   0 remy      (1000) remy      (1000)     9277 2023-08-07 01:44:48.000000 HaploDynamics-0.1b6/HaploDynamics.egg-info/PKG-INFO
+-rw-rw-r--   0 remy      (1000) remy      (1000)      246 2023-08-07 01:44:48.000000 HaploDynamics-0.1b6/HaploDynamics.egg-info/SOURCES.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-07 01:44:48.000000 HaploDynamics-0.1b6/HaploDynamics.egg-info/dependency_links.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        6 2023-08-07 01:44:48.000000 HaploDynamics-0.1b6/HaploDynamics.egg-info/requires.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)       14 2023-08-07 01:44:48.000000 HaploDynamics-0.1b6/HaploDynamics.egg-info/top_level.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)    35149 2023-08-07 01:26:43.000000 HaploDynamics-0.1b6/LICENSE
+-rw-rw-r--   0 remy      (1000) remy      (1000)     9277 2023-08-07 01:44:48.082907 HaploDynamics-0.1b6/PKG-INFO
+-rw-rw-r--   0 remy      (1000) remy      (1000)     8393 2023-08-07 01:26:43.000000 HaploDynamics-0.1b6/README.md
+-rw-rw-r--   0 remy      (1000) remy      (1000)       79 2023-08-07 01:44:48.082907 HaploDynamics-0.1b6/setup.cfg
+-rw-rw-r--   0 remy      (1000) remy      (1000)     1207 2023-08-07 01:43:33.000000 HaploDynamics-0.1b6/setup.py
```

### Comparing `HaploDynamics-0.1b5/HaploDynamics.egg-info/PKG-INFO` & `HaploDynamics-0.1b6/HaploDynamics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HaploDynamics
-Version: 0.1b5
+Version: 0.1b6
 Summary: A python library to develop genomic data simulators
 Home-page: https://github.com/remytuyeras/HaploDynamics
-Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.5.tar.gz
+Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.6.tar.gz
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
-Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b5 Summary: A python
+Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b6 Summary: A python
 library to develop genomic data simulators Home-page: https://github.com/
 remytuyeras/HaploDynamics Download-URL: https://github.com/remytuyeras/
-HaploDynamics/archive/refs/tags/v0.1-beta.5.tar.gz Author: Remy Tuyeras Author-
+HaploDynamics/archive/refs/tags/v0.1-beta.6.tar.gz Author: Remy Tuyeras Author-
 email: rtuyeras@gmail.com License: gpl-3.0 Keywords:
 Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage
 disequilibrium,Hardy-Weinberg equilibrium Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Intended Audience
 :: Science/Research Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `HaploDynamics-0.1b5/LICENSE` & `HaploDynamics-0.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.1b5/PKG-INFO` & `HaploDynamics-0.1b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HaploDynamics
-Version: 0.1b5
+Version: 0.1b6
 Summary: A python library to develop genomic data simulators
 Home-page: https://github.com/remytuyeras/HaploDynamics
-Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.5.tar.gz
+Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.6.tar.gz
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
-Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b5 Summary: A python
+Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b6 Summary: A python
 library to develop genomic data simulators Home-page: https://github.com/
 remytuyeras/HaploDynamics Download-URL: https://github.com/remytuyeras/
-HaploDynamics/archive/refs/tags/v0.1-beta.5.tar.gz Author: Remy Tuyeras Author-
+HaploDynamics/archive/refs/tags/v0.1-beta.6.tar.gz Author: Remy Tuyeras Author-
 email: rtuyeras@gmail.com License: gpl-3.0 Keywords:
 Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage
 disequilibrium,Hardy-Weinberg equilibrium Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Intended Audience
 :: Science/Research Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `HaploDynamics-0.1b5/README.md` & `HaploDynamics-0.1b6/README.md`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.1b5/setup.py` & `HaploDynamics-0.1b6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name = 'HaploDynamics',
   packages=setuptools.find_packages(include=['HaploDynamics']),
-  version = 'v0.1-beta.5',
+  version = 'v0.1-beta.6',
   license='gpl-3.0',
   author = 'Remy Tuyeras',
   author_email = 'rtuyeras@gmail.com',
   description = 'A python library to develop genomic data simulators',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   url = 'https://github.com/remytuyeras/HaploDynamics',
-  download_url = 'https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.5.tar.gz',
+  download_url = 'https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.6.tar.gz',
   keywords = ['Simulator', 'Genomics', 'Genomic', 'Microarray','SNP chip','VCF', 'Linkage disequilibrium', 'Hardy-Weinberg equilibrium'],
   install_requires=['scipy'],
   classifiers=[
     'Development Status :: 4 - Beta',  #"3 - Alpha", "4 - Beta" or "5 - Production/Stable"
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Topic :: Software Development :: Build Tools',
```

