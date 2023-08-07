# Comparing `tmp/DYCodeBase-0.0.1.tar.gz` & `tmp/DYCodeBase-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DYCodeBase-0.0.1.tar", last modified: Mon Aug  7 09:44:54 2023, max compression
+gzip compressed data, was "DYCodeBase-0.0.2.tar", last modified: Mon Aug  7 09:50:26 2023, max compression
```

## Comparing `DYCodeBase-0.0.1.tar` & `DYCodeBase-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 devind    (1000) devind    (1000)        0 2023-08-07 09:44:54.489040 DYCodeBase-0.0.1/
-drwxr-xr-x   0 devind    (1000) devind    (1000)        0 2023-08-07 09:44:54.489040 DYCodeBase-0.0.1/DYCodeBase.egg-info/
--rw-r--r--   0 devind    (1000) devind    (1000)      493 2023-08-07 09:44:54.000000 DYCodeBase-0.0.1/DYCodeBase.egg-info/PKG-INFO
--rw-r--r--   0 devind    (1000) devind    (1000)      269 2023-08-07 09:44:54.000000 DYCodeBase-0.0.1/DYCodeBase.egg-info/SOURCES.txt
--rw-r--r--   0 devind    (1000) devind    (1000)        1 2023-08-07 09:44:54.000000 DYCodeBase-0.0.1/DYCodeBase.egg-info/dependency_links.txt
--rw-r--r--   0 devind    (1000) devind    (1000)       19 2023-08-07 09:44:54.000000 DYCodeBase-0.0.1/DYCodeBase.egg-info/requires.txt
--rw-r--r--   0 devind    (1000) devind    (1000)        6 2023-08-07 09:44:54.000000 DYCodeBase-0.0.1/DYCodeBase.egg-info/top_level.txt
--rw-r--r--   0 devind    (1000) devind    (1000)      493 2023-08-07 09:44:54.489040 DYCodeBase-0.0.1/PKG-INFO
--rw-r--r--   0 devind    (1000) devind    (1000)       71 2023-08-07 09:02:46.000000 DYCodeBase-0.0.1/README.md
-drwxr-xr-x   0 devind    (1000) devind    (1000)        0 2023-08-07 09:44:54.489040 DYCodeBase-0.0.1/model/
--rw-r--r--   0 devind    (1000) devind    (1000)       17 2023-08-07 08:46:25.000000 DYCodeBase-0.0.1/model/__init__.py
-drwxr-xr-x   0 devind    (1000) devind    (1000)        0 2023-08-07 09:44:54.489040 DYCodeBase-0.0.1/model/components/
--rw-r--r--   0 devind    (1000) devind    (1000)       28 2023-08-07 08:46:08.000000 DYCodeBase-0.0.1/model/components/__init__.py
--rw-r--r--   0 devind    (1000) devind    (1000)     2375 2023-08-07 08:43:30.000000 DYCodeBase-0.0.1/model/components/squeeze_excite.py
--rw-r--r--   0 devind    (1000) devind    (1000)       38 2023-08-07 09:44:54.489040 DYCodeBase-0.0.1/setup.cfg
--rw-r--r--   0 devind    (1000) devind    (1000)      960 2023-08-07 09:44:10.000000 DYCodeBase-0.0.1/setup.py
+drwxr-xr-x   0 devind    (1000) devind    (1000)        0 2023-08-07 09:50:26.059039 DYCodeBase-0.0.2/
+drwxr-xr-x   0 devind    (1000) devind    (1000)        0 2023-08-07 09:50:26.059039 DYCodeBase-0.0.2/DYCodeBase.egg-info/
+-rw-r--r--   0 devind    (1000) devind    (1000)      493 2023-08-07 09:50:26.000000 DYCodeBase-0.0.2/DYCodeBase.egg-info/PKG-INFO
+-rw-r--r--   0 devind    (1000) devind    (1000)      269 2023-08-07 09:50:26.000000 DYCodeBase-0.0.2/DYCodeBase.egg-info/SOURCES.txt
+-rw-r--r--   0 devind    (1000) devind    (1000)        1 2023-08-07 09:50:26.000000 DYCodeBase-0.0.2/DYCodeBase.egg-info/dependency_links.txt
+-rw-r--r--   0 devind    (1000) devind    (1000)       11 2023-08-07 09:50:26.000000 DYCodeBase-0.0.2/DYCodeBase.egg-info/requires.txt
+-rw-r--r--   0 devind    (1000) devind    (1000)        6 2023-08-07 09:50:26.000000 DYCodeBase-0.0.2/DYCodeBase.egg-info/top_level.txt
+-rw-r--r--   0 devind    (1000) devind    (1000)      493 2023-08-07 09:50:26.059039 DYCodeBase-0.0.2/PKG-INFO
+-rw-r--r--   0 devind    (1000) devind    (1000)       71 2023-08-07 09:02:46.000000 DYCodeBase-0.0.2/README.md
+drwxr-xr-x   0 devind    (1000) devind    (1000)        0 2023-08-07 09:50:26.059039 DYCodeBase-0.0.2/model/
+-rw-r--r--   0 devind    (1000) devind    (1000)       17 2023-08-07 08:46:25.000000 DYCodeBase-0.0.2/model/__init__.py
+drwxr-xr-x   0 devind    (1000) devind    (1000)        0 2023-08-07 09:50:26.059039 DYCodeBase-0.0.2/model/components/
+-rw-r--r--   0 devind    (1000) devind    (1000)       28 2023-08-07 08:46:08.000000 DYCodeBase-0.0.2/model/components/__init__.py
+-rw-r--r--   0 devind    (1000) devind    (1000)     2375 2023-08-07 08:43:30.000000 DYCodeBase-0.0.2/model/components/squeeze_excite.py
+-rw-r--r--   0 devind    (1000) devind    (1000)       38 2023-08-07 09:50:26.059039 DYCodeBase-0.0.2/setup.cfg
+-rw-r--r--   0 devind    (1000) devind    (1000)      952 2023-08-07 09:48:57.000000 DYCodeBase-0.0.2/setup.py
```

### Comparing `DYCodeBase-0.0.1/model/components/squeeze_excite.py` & `DYCodeBase-0.0.2/model/components/squeeze_excite.py`

 * *Files identical despite different names*

### Comparing `DYCodeBase-0.0.1/setup.py` & `DYCodeBase-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'CodeBase of important Functions'
 LONG_DESCRIPTION = 'Contains Pytorch/ TensorFlow algorithms I have found in a single module'
 
 # Setting up
 setup(
         name="DYCodeBase", 
         version=VERSION,
         author="Devin De Silva",
         author_email="devin@irononetech.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=["tensorflow==2.10.*"], # add any additional packages that 
+        install_requires=["tensorflow"], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         
         keywords=['python', 'codebase'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Developers",
             "Programming Language :: Python :: 3.9",
```

