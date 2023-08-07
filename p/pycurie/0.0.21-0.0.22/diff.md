# Comparing `tmp/pycurie-0.0.21.tar.gz` & `tmp/pycurie-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycurie-0.0.21.tar", last modified: Mon Aug  7 20:54:16 2023, max compression
+gzip compressed data, was "pycurie-0.0.22.tar", last modified: Mon Aug  7 20:58:21 2023, max compression
```

## Comparing `pycurie-0.0.21.tar` & `pycurie-0.0.22.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:16.774313 pycurie-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-08-07 20:54:16.774313 pycurie-0.0.21/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:16.770313 pycurie-0.0.21/curie/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:16.770313 pycurie-0.0.21/curie/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/defaults/curie_seed.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:16.770313 pycurie-0.0.21/curie/defaults/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/defaults/jinja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/defaults/jinja/docs-settings.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/defaults/jinja/pipeline-bp.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/defaults/jinja/pipeline.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/inca.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/mk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:16.774313 pycurie-0.0.21/curie/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-07 20:54:08.000000 pycurie-0.0.21/curie/utils/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:54:16.774313 pycurie-0.0.21/pycurie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-08-07 20:54:16.000000 pycurie-0.0.21/pycurie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-07 20:54:16.000000 pycurie-0.0.21/pycurie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:54:16.000000 pycurie-0.0.21/pycurie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 20:54:16.000000 pycurie-0.0.21/pycurie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 20:54:16.000000 pycurie-0.0.21/pycurie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 20:54:16.774313 pycurie-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-07 20:54:08.000000 pycurie-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:58:21.473647 pycurie-0.0.22/
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-08-07 20:58:21.473647 pycurie-0.0.22/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:58:21.469647 pycurie-0.0.22/curie/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-07 20:58:10.000000 pycurie-0.0.22/curie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-08-07 20:58:10.000000 pycurie-0.0.22/curie/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:58:21.469647 pycurie-0.0.22/curie/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:58:10.000000 pycurie-0.0.22/curie/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-08-07 20:58:10.000000 pycurie-0.0.22/curie/defaults/curie_seed.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:58:21.469647 pycurie-0.0.22/curie/defaults/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:58:10.000000 pycurie-0.0.22/curie/defaults/jinja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-08-07 20:58:10.000000 pycurie-0.0.22/curie/defaults/jinja/docs-settings.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-08-07 20:58:10.000000 pycurie-0.0.22/curie/defaults/jinja/pipeline-bp.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-07 20:58:10.000000 pycurie-0.0.22/curie/defaults/jinja/pipeline.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-08-07 20:58:10.000000 pycurie-0.0.22/curie/inca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-08-07 20:58:10.000000 pycurie-0.0.22/curie/lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-07 20:58:10.000000 pycurie-0.0.22/curie/mk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-07 20:58:10.000000 pycurie-0.0.22/curie/sources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:58:21.469647 pycurie-0.0.22/curie/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-07 20:58:10.000000 pycurie-0.0.22/curie/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-07 20:58:10.000000 pycurie-0.0.22/curie/utils/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:58:21.469647 pycurie-0.0.22/pycurie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-08-07 20:58:21.000000 pycurie-0.0.22/pycurie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-07 20:58:21.000000 pycurie-0.0.22/pycurie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:58:21.000000 pycurie-0.0.22/pycurie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 20:58:21.000000 pycurie-0.0.22/pycurie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 20:58:21.000000 pycurie-0.0.22/pycurie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 20:58:21.473647 pycurie-0.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-07 20:58:10.000000 pycurie-0.0.22/setup.py
```

### Comparing `pycurie-0.0.21/PKG-INFO` & `pycurie-0.0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycurie
-Version: 0.0.21
+Version: 0.0.22
 Home-page: https://github.com/EricDiGi/CurieKetl
 Author: Eric DiGioacchino
 Keywords: etl,data,data engineering,data science,mlops,devops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pycurie-0.0.21/curie/__main__.py` & `pycurie-0.0.22/curie/__main__.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.21/curie/defaults/curie_seed.zip` & `pycurie-0.0.22/curie/defaults/curie_seed.zip`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.21/curie/defaults/jinja/docs-settings.yaml.j2` & `pycurie-0.0.22/curie/defaults/jinja/docs-settings.yaml.j2`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.21/curie/defaults/jinja/pipeline-bp.md.j2` & `pycurie-0.0.22/curie/defaults/jinja/pipeline-bp.md.j2`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.21/curie/defaults/jinja/pipeline.md.j2` & `pycurie-0.0.22/curie/defaults/jinja/pipeline.md.j2`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.21/curie/inca.py` & `pycurie-0.0.22/curie/inca.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.21/curie/lab.py` & `pycurie-0.0.22/curie/lab.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.21/curie/mk.py` & `pycurie-0.0.22/curie/mk.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.21/curie/sources.py` & `pycurie-0.0.22/curie/sources.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.21/curie/utils/__init__.py` & `pycurie-0.0.22/curie/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.21/curie/utils/secrets.py` & `pycurie-0.0.22/curie/utils/secrets.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.21/pycurie.egg-info/PKG-INFO` & `pycurie-0.0.22/pycurie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycurie
-Version: 0.0.21
+Version: 0.0.22
 Home-page: https://github.com/EricDiGi/CurieKetl
 Author: Eric DiGioacchino
 Keywords: etl,data,data engineering,data science,mlops,devops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pycurie-0.0.21/pycurie.egg-info/SOURCES.txt` & `pycurie-0.0.22/pycurie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.21/setup.py` & `pycurie-0.0.22/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # A simple setup script
 from setuptools import setup, find_packages
 
 setup(name='pycurie',
-      version='0.0.21',
+      version='0.0.22',
       author='Eric DiGioacchino',
       url='https://github.com/EricDiGi/CurieKetl',
       keywords=['etl', 'data', 'data engineering', 'data science', 'mlops', 'devops'],
       classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3"
@@ -17,10 +17,10 @@
       entry_points={
           'console_scripts': [
               'curie = curie.__main__:main'
           ]
       },
       package_data={
             "curie.defaults": ["*"],
-            "curie.defaults.jinja": ["*"]
+            "curie.defaults.jinja": ["*.md.j2", "*.yaml.j2"]
       }
 )
```

