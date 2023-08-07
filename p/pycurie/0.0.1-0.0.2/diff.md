# Comparing `tmp/pycurie-0.0.1.tar.gz` & `tmp/pycurie-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycurie-0.0.1.tar", last modified: Mon Aug  7 20:31:22 2023, max compression
+gzip compressed data, was "pycurie-0.0.2.tar", last modified: Mon Aug  7 20:44:22 2023, max compression
```

## Comparing `pycurie-0.0.1.tar` & `pycurie-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:31:22.618474 pycurie-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-08-07 20:31:22.618474 pycurie-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:31:22.614474 pycurie-0.0.1/curie/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-07 20:31:12.000000 pycurie-0.0.1/curie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-08-07 20:31:12.000000 pycurie-0.0.1/curie/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:31:22.614474 pycurie-0.0.1/curie/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:31:12.000000 pycurie-0.0.1/curie/defaults/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:31:22.614474 pycurie-0.0.1/curie/defaults/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:31:12.000000 pycurie-0.0.1/curie/defaults/jinja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-08-07 20:31:12.000000 pycurie-0.0.1/curie/inca.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-08-07 20:31:12.000000 pycurie-0.0.1/curie/lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-07 20:31:12.000000 pycurie-0.0.1/curie/mk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-07 20:31:12.000000 pycurie-0.0.1/curie/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:31:22.618474 pycurie-0.0.1/curie/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-07 20:31:12.000000 pycurie-0.0.1/curie/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-07 20:31:12.000000 pycurie-0.0.1/curie/utils/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:31:22.618474 pycurie-0.0.1/pycurie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-08-07 20:31:22.000000 pycurie-0.0.1/pycurie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-07 20:31:22.000000 pycurie-0.0.1/pycurie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:31:22.000000 pycurie-0.0.1/pycurie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 20:31:22.000000 pycurie-0.0.1/pycurie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 20:31:22.000000 pycurie-0.0.1/pycurie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 20:31:22.618474 pycurie-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-07 20:31:12.000000 pycurie-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:22.164621 pycurie-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-08-07 20:44:22.164621 pycurie-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:22.164621 pycurie-0.0.2/curie/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:22.164621 pycurie-0.0.2/curie/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/defaults/curie_seed.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:22.164621 pycurie-0.0.2/curie/defaults/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/defaults/jinja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/inca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/mk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/sources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:22.164621 pycurie-0.0.2/curie/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-07 20:44:11.000000 pycurie-0.0.2/curie/utils/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:44:22.164621 pycurie-0.0.2/pycurie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-08-07 20:44:22.000000 pycurie-0.0.2/pycurie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-07 20:44:22.000000 pycurie-0.0.2/pycurie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:44:22.000000 pycurie-0.0.2/pycurie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 20:44:22.000000 pycurie-0.0.2/pycurie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 20:44:22.000000 pycurie-0.0.2/pycurie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 20:44:22.164621 pycurie-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-07 20:44:11.000000 pycurie-0.0.2/setup.py
```

### Comparing `pycurie-0.0.1/PKG-INFO` & `pycurie-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycurie
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/EricDiGi/CurieKetl
 Author: Eric DiGioacchino
 Keywords: etl,data,data engineering,data science,mlops,devops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pycurie-0.0.1/curie/__main__.py` & `pycurie-0.0.2/curie/__main__.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.1/curie/inca.py` & `pycurie-0.0.2/curie/inca.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.1/curie/lab.py` & `pycurie-0.0.2/curie/lab.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.1/curie/mk.py` & `pycurie-0.0.2/curie/mk.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.1/curie/sources.py` & `pycurie-0.0.2/curie/sources.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.1/curie/utils/__init__.py` & `pycurie-0.0.2/curie/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.1/curie/utils/secrets.py` & `pycurie-0.0.2/curie/utils/secrets.py`

 * *Files identical despite different names*

### Comparing `pycurie-0.0.1/pycurie.egg-info/PKG-INFO` & `pycurie-0.0.2/pycurie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycurie
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/EricDiGi/CurieKetl
 Author: Eric DiGioacchino
 Keywords: etl,data,data engineering,data science,mlops,devops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pycurie-0.0.1/setup.py` & `pycurie-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # A simple setup script
 from setuptools import setup, find_packages
 
 setup(name='pycurie',
-      version='0.0.1',
+      version='0.0.02',
       author='Eric DiGioacchino',
       url='https://github.com/EricDiGi/CurieKetl',
       keywords=['etl', 'data', 'data engineering', 'data science', 'mlops', 'devops'],
       classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3"
@@ -14,9 +14,12 @@
         long_description=open('../README.md').read(),
         long_description_content_type='text/markdown',
       packages=find_packages(),
       entry_points={
           'console_scripts': [
               'curie = curie.__main__:main'
           ]
+      },
+      package_data={
+            "curie.defaults": ["*"]
       }
 )
```

