# Comparing `tmp/pycurie-0.0.2.tar.gz` & `tmp/pycurie-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycurie-0.0.2.tar", last modified: Mon Aug  7 20:44:22 2023, max compression
+gzip compressed data, was "pycurie-0.0.21.tar", last modified: Mon Aug  7 20:54:16 2023, max compression
```

## Comparing `pycurie-0.0.2.tar` & `pycurie-0.0.21.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:22.164621 pycurie-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-08-07 20:44:22.164621 pycurie-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:22.164621 pycurie-0.0.2/curie/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:22.164621 pycurie-0.0.2/curie/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/defaults/curie_seed.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:22.164621 pycurie-0.0.2/curie/defaults/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/defaults/jinja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/inca.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/mk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:22.164621 pycurie-0.0.2/curie/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/utils/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:22.164621 pycurie-0.0.2/pycurie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-08-07 20:44:22.000000 pycurie-0.0.2/pycurie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-07 20:44:22.000000 pycurie-0.0.2/pycurie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:44:22.000000 pycurie-0.0.2/pycurie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 20:44:22.000000 pycurie-0.0.2/pycurie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 20:44:22.000000 pycurie-0.0.2/pycurie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 20:44:22.164621 pycurie-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-07 20:44:11.000000 pycurie-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:16.774313 pycurie-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-08-07 20:54:16.774313 pycurie-0.0.21/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:16.770313 pycurie-0.0.21/curie/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:16.770313 pycurie-0.0.21/curie/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/defaults/curie_seed.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:16.770313 pycurie-0.0.21/curie/defaults/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/defaults/jinja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/defaults/jinja/docs-settings.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/defaults/jinja/pipeline-bp.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/defaults/jinja/pipeline.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/inca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/mk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/sources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:16.774313 pycurie-0.0.21/curie/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/utils/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:16.774313 pycurie-0.0.21/pycurie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-08-07 20:54:16.000000 pycurie-0.0.21/pycurie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-07 20:54:16.000000 pycurie-0.0.21/pycurie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:54:16.000000 pycurie-0.0.21/pycurie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 20:54:16.000000 pycurie-0.0.21/pycurie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 20:54:16.000000 pycurie-0.0.21/pycurie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 20:54:16.774313 pycurie-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-07 20:54:08.000000 pycurie-0.0.21/setup.py
```

### Comparing `pycurie-0.0.2/PKG-INFO` & `pycurie-0.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycurie
-Version: 0.0.2
+Version: 0.0.21
 Home-page: https://github.com/EricDiGi/CurieKetl
 Author: Eric DiGioacchino
 Keywords: etl,data,data engineering,data science,mlops,devops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pycurie-0.0.2/curie/__main__.py` & `pycurie-0.0.21/curie/__main__.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.2/curie/defaults/curie_seed.zip` & `pycurie-0.0.21/curie/defaults/curie_seed.zip`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.2/curie/inca.py` & `pycurie-0.0.21/curie/inca.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.2/curie/lab.py` & `pycurie-0.0.21/curie/lab.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.2/curie/mk.py` & `pycurie-0.0.21/curie/mk.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.2/curie/sources.py` & `pycurie-0.0.21/curie/sources.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.2/curie/utils/__init__.py` & `pycurie-0.0.21/curie/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.2/curie/utils/secrets.py` & `pycurie-0.0.21/curie/utils/secrets.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.2/pycurie.egg-info/PKG-INFO` & `pycurie-0.0.21/pycurie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycurie
-Version: 0.0.2
+Version: 0.0.21
 Home-page: https://github.com/EricDiGi/CurieKetl
 Author: Eric DiGioacchino
 Keywords: etl,data,data engineering,data science,mlops,devops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pycurie-0.0.2/setup.py` & `pycurie-0.0.21/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # A simple setup script
 from setuptools import setup, find_packages
 
 setup(name='pycurie',
-      version='0.0.02',
+      version='0.0.21',
       author='Eric DiGioacchino',
       url='https://github.com/EricDiGi/CurieKetl',
       keywords=['etl', 'data', 'data engineering', 'data science', 'mlops', 'devops'],
       classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3"
@@ -16,10 +16,11 @@
       packages=find_packages(),
       entry_points={
           'console_scripts': [
               'curie = curie.__main__:main'
           ]
       },
       package_data={
-            "curie.defaults": ["*"]
+            "curie.defaults": ["*"],
+            "curie.defaults.jinja": ["*"]
       }
 )
```

