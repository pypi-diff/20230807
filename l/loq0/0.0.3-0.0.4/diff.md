# Comparing `tmp/loq0-0.0.3.tar.gz` & `tmp/loq0-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loq0-0.0.3.tar", last modified: Sun Aug  6 14:18:10 2023, max compression
+gzip compressed data, was "loq0-0.0.4.tar", last modified: Sun Aug  6 16:45:17 2023, max compression
```

## Comparing `loq0-0.0.3.tar` & `loq0-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 seo_hyun   (501) staff       (20)        0 2023-08-06 14:18:10.471774 loq0-0.0.3/
--rw-r--r--   0 seo_hyun   (501) staff       (20)      393 2023-08-06 14:18:10.471626 loq0-0.0.3/PKG-INFO
-drwxr-xr-x   0 seo_hyun   (501) staff       (20)        0 2023-08-06 14:18:10.471416 loq0-0.0.3/loq0.egg-info/
--rw-r--r--   0 seo_hyun   (501) staff       (20)      393 2023-08-06 14:18:10.000000 loq0-0.0.3/loq0.egg-info/PKG-INFO
--rw-r--r--   0 seo_hyun   (501) staff       (20)      120 2023-08-06 14:18:10.000000 loq0-0.0.3/loq0.egg-info/SOURCES.txt
--rw-r--r--   0 seo_hyun   (501) staff       (20)        1 2023-08-06 14:18:10.000000 loq0-0.0.3/loq0.egg-info/dependency_links.txt
--rw-r--r--   0 seo_hyun   (501) staff       (20)        1 2023-08-06 14:18:10.000000 loq0-0.0.3/loq0.egg-info/top_level.txt
--rw-r--r--   0 seo_hyun   (501) staff       (20)       38 2023-08-06 14:18:10.471823 loq0-0.0.3/setup.cfg
--rw-r--r--   0 seo_hyun   (501) staff       (20)      547 2023-08-06 14:17:54.000000 loq0-0.0.3/setup.py
+drwxr-xr-x   0 seo_hyun   (501) staff       (20)        0 2023-08-06 16:45:17.158375 loq0-0.0.4/
+-rw-r--r--   0 seo_hyun   (501) staff       (20)      393 2023-08-06 16:45:17.158218 loq0-0.0.4/PKG-INFO
+drwxr-xr-x   0 seo_hyun   (501) staff       (20)        0 2023-08-06 16:45:17.157994 loq0-0.0.4/loq0.egg-info/
+-rw-r--r--   0 seo_hyun   (501) staff       (20)      393 2023-08-06 16:45:17.000000 loq0-0.0.4/loq0.egg-info/PKG-INFO
+-rw-r--r--   0 seo_hyun   (501) staff       (20)      120 2023-08-06 16:45:17.000000 loq0-0.0.4/loq0.egg-info/SOURCES.txt
+-rw-r--r--   0 seo_hyun   (501) staff       (20)        1 2023-08-06 16:45:17.000000 loq0-0.0.4/loq0.egg-info/dependency_links.txt
+-rw-r--r--   0 seo_hyun   (501) staff       (20)        1 2023-08-06 16:45:17.000000 loq0-0.0.4/loq0.egg-info/top_level.txt
+-rw-r--r--   0 seo_hyun   (501) staff       (20)       38 2023-08-06 16:45:17.158422 loq0-0.0.4/setup.cfg
+-rw-r--r--   0 seo_hyun   (501) staff       (20)      550 2023-08-06 16:45:01.000000 loq0-0.0.4/setup.py
```

### Comparing `loq0-0.0.3/setup.py` & `loq0-0.0.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 setuptools.setup(
     name="loq0",
-    version="0.0.3",
+    version="0.0.4",
     author="seorii",
     author_email="me@seorii.page",
     description="League of Quoridor",
     long_description="League of Quoridor",
     long_description_content_type="text/markdown",
     url="https://github.com/dastyinc/loq0",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages('.'),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

