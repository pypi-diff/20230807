# Comparing `tmp/dandelion-eu-0.3.2.tar.gz` & `tmp/dandelion-eu-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dandelion-eu-0.3.2.tar", last modified: Mon Sep  2 10:47:13 2019, max compression
+gzip compressed data, was "dandelion-eu-0.3.3.tar", last modified: Mon Aug  7 10:58:24 2023, max compression
```

## Comparing `dandelion-eu-0.3.2.tar` & `dandelion-eu-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 berardi    (501) staff       (20)        0 2019-09-02 10:47:13.000000 dandelion-eu-0.3.2/
--rw-r--r--   0 berardi    (501) staff       (20)     3182 2019-09-02 10:47:13.000000 dandelion-eu-0.3.2/PKG-INFO
--rw-r--r--   0 berardi    (501) staff       (20)     1429 2019-09-02 10:46:34.000000 dandelion-eu-0.3.2/README.rst
-drwxr-xr-x   0 berardi    (501) staff       (20)        0 2019-09-02 10:47:13.000000 dandelion-eu-0.3.2/dandelion/
--rw-r--r--   0 berardi    (501) staff       (20)      229 2019-09-02 10:46:13.000000 dandelion-eu-0.3.2/dandelion/__init__.py
--rw-r--r--   0 berardi    (501) staff       (20)     4314 2019-09-02 10:12:39.000000 dandelion-eu-0.3.2/dandelion/base.py
-drwxr-xr-x   0 berardi    (501) staff       (20)        0 2019-09-02 10:47:13.000000 dandelion-eu-0.3.2/dandelion/cache/
--rw-r--r--   0 berardi    (501) staff       (20)       84 2019-07-26 15:22:32.000000 dandelion-eu-0.3.2/dandelion/cache/__init__.py
--rw-r--r--   0 berardi    (501) staff       (20)      699 2019-09-02 10:12:39.000000 dandelion-eu-0.3.2/dandelion/cache/base.py
--rw-r--r--   0 berardi    (501) staff       (20)      911 2019-07-26 15:22:32.000000 dandelion-eu-0.3.2/dandelion/cache/file.py
--rw-r--r--   0 berardi    (501) staff       (20)     5302 2019-07-26 15:22:32.000000 dandelion-eu-0.3.2/dandelion/datagem.py
--rw-r--r--   0 berardi    (501) staff       (20)      897 2019-09-02 10:12:39.000000 dandelion-eu-0.3.2/dandelion/datatxt.py
--rw-r--r--   0 berardi    (501) staff       (20)      240 2019-07-26 15:22:32.000000 dandelion-eu-0.3.2/dandelion/utils.py
-drwxr-xr-x   0 berardi    (501) staff       (20)        0 2019-09-02 10:47:13.000000 dandelion-eu-0.3.2/dandelion_eu.egg-info/
--rw-r--r--   0 berardi    (501) staff       (20)     3182 2019-09-02 10:47:13.000000 dandelion-eu-0.3.2/dandelion_eu.egg-info/PKG-INFO
--rw-r--r--   0 berardi    (501) staff       (20)      385 2019-09-02 10:47:13.000000 dandelion-eu-0.3.2/dandelion_eu.egg-info/SOURCES.txt
--rw-r--r--   0 berardi    (501) staff       (20)        1 2019-09-02 10:47:13.000000 dandelion-eu-0.3.2/dandelion_eu.egg-info/dependency_links.txt
--rw-r--r--   0 berardi    (501) staff       (20)       13 2019-09-02 10:47:13.000000 dandelion-eu-0.3.2/dandelion_eu.egg-info/requires.txt
--rw-r--r--   0 berardi    (501) staff       (20)       10 2019-09-02 10:47:13.000000 dandelion-eu-0.3.2/dandelion_eu.egg-info/top_level.txt
--rw-r--r--   0 berardi    (501) staff       (20)       79 2019-09-02 10:47:13.000000 dandelion-eu-0.3.2/setup.cfg
--rw-r--r--   0 berardi    (501) staff       (20)     1850 2019-09-02 10:41:22.000000 dandelion-eu-0.3.2/setup.py
+drwxr-xr-x   0 berardi    (501) staff       (20)        0 2023-08-07 10:58:24.734990 dandelion-eu-0.3.3/
+-rw-r--r--   0 berardi    (501) staff       (20)    18052 2019-07-26 15:22:32.000000 dandelion-eu-0.3.3/LICENSE
+-rw-r--r--   0 berardi    (501) staff       (20)     2796 2023-08-07 10:58:24.735179 dandelion-eu-0.3.3/PKG-INFO
+-rw-r--r--   0 berardi    (501) staff       (20)     1429 2023-08-07 10:29:43.000000 dandelion-eu-0.3.3/README.rst
+drwxr-xr-x   0 berardi    (501) staff       (20)        0 2023-08-07 10:58:24.730362 dandelion-eu-0.3.3/dandelion/
+-rw-r--r--   0 berardi    (501) staff       (20)      229 2023-08-07 10:29:30.000000 dandelion-eu-0.3.3/dandelion/__init__.py
+-rw-r--r--   0 berardi    (501) staff       (20)     4314 2023-08-07 10:29:43.000000 dandelion-eu-0.3.3/dandelion/base.py
+drwxr-xr-x   0 berardi    (501) staff       (20)        0 2023-08-07 10:58:24.731847 dandelion-eu-0.3.3/dandelion/cache/
+-rw-r--r--   0 berardi    (501) staff       (20)       84 2019-07-26 15:22:32.000000 dandelion-eu-0.3.3/dandelion/cache/__init__.py
+-rw-r--r--   0 berardi    (501) staff       (20)      699 2019-09-02 10:12:39.000000 dandelion-eu-0.3.3/dandelion/cache/base.py
+-rw-r--r--   0 berardi    (501) staff       (20)      911 2019-07-26 15:22:32.000000 dandelion-eu-0.3.3/dandelion/cache/file.py
+-rw-r--r--   0 berardi    (501) staff       (20)     5302 2019-07-26 15:22:32.000000 dandelion-eu-0.3.3/dandelion/datagem.py
+-rw-r--r--   0 berardi    (501) staff       (20)      897 2019-09-02 10:12:39.000000 dandelion-eu-0.3.3/dandelion/datatxt.py
+-rw-r--r--   0 berardi    (501) staff       (20)      240 2019-07-26 15:22:32.000000 dandelion-eu-0.3.3/dandelion/utils.py
+drwxr-xr-x   0 berardi    (501) staff       (20)        0 2023-08-07 10:58:24.734571 dandelion-eu-0.3.3/dandelion_eu.egg-info/
+-rw-r--r--   0 berardi    (501) staff       (20)     2796 2023-08-07 10:58:24.000000 dandelion-eu-0.3.3/dandelion_eu.egg-info/PKG-INFO
+-rw-r--r--   0 berardi    (501) staff       (20)      393 2023-08-07 10:58:24.000000 dandelion-eu-0.3.3/dandelion_eu.egg-info/SOURCES.txt
+-rw-r--r--   0 berardi    (501) staff       (20)        1 2023-08-07 10:58:24.000000 dandelion-eu-0.3.3/dandelion_eu.egg-info/dependency_links.txt
+-rw-r--r--   0 berardi    (501) staff       (20)       13 2023-08-07 10:58:24.000000 dandelion-eu-0.3.3/dandelion_eu.egg-info/requires.txt
+-rw-r--r--   0 berardi    (501) staff       (20)       10 2023-08-07 10:58:24.000000 dandelion-eu-0.3.3/dandelion_eu.egg-info/top_level.txt
+-rw-r--r--   0 berardi    (501) staff       (20)       79 2023-08-07 10:58:24.735873 dandelion-eu-0.3.3/setup.cfg
+-rw-r--r--   0 berardi    (501) staff       (20)     1850 2019-09-02 10:41:22.000000 dandelion-eu-0.3.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dandelion-eu-0.3.2/PKG-INFO` & `dandelion-eu-0.3.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dandelion-eu
-Version: 0.3.2
+Version: 0.3.3
 Summary: Connect to the dandelion.eu API in a very pythonic way!
 Home-page: https://github.com/giacbrd/python-dandelion-eu
+Download-URL: https://github.com/giacbrd/python-dandelion-eu/tarball/0.3.3
 Author: SpazioDati s.r.l.
 Author-email: berardi@spaziodati.eu
-License: UNKNOWN
-Download-URL: https://github.com/giacbrd/python-dandelion-eu/tarball/0.3.2
-Description: .. image:: https://travis-ci.org/giacbrd/python-dandelion-eu.svg?branch=master
-          :target: https://travis-ci.org/giacbrd/python-dandelion-eu
-        
-        .. image:: https://coveralls.io/repos/SpazioDati/python-dandelion-eu/badge.png?branch=master
-          :target: https://coveralls.io/r/SpazioDati/python-dandelion-eu?branch=master
-        
-        .. image:: https://img.shields.io/pypi/v/dandelion-eu
-            :target: https://pypi.python.org/pypi/dandelion-eu/
-            :alt: Latest PyPI version
-        
-        .. _PyPI: https://pypi.python.org/pypi/dandelion-eu/
-        .. _ReadTheDocs: http://python-dandelion-eu.readthedocs.org/
-        .. _dandelion: https://dandelion.eu/accounts/register/?next=/
-        .. _dandelion.eu: http://dandelion.eu/
-        
-        python-dandelion-eu
-        ===================
-        
-        Bring the power of the dandelion.eu_ semantic to your python applications and scripts!
-        Semantic in python couldn't be easier.
-        
-        
-        .. code-block:: py
-        
-            >>> from dandelion import DataTXT
-            >>> datatxt = DataTXT(token='YOUR_TOKEN')
-            >>> response = datatxt.nex('The doctor says an apple is better than an orange')
-            >>> for annotation in response.annotations:
-                  print(annotation)
-            ...
-        
-        Register on dandelion_ to obtain your authentication token and enrich your application with our semantic intelligence.
-        
-        Installation
-        ------------
-        
-        ``dandelion-eu`` is available on PyPI_ install it simply with::
-        
-            pip install dandelion-eu
-        
-        
-        Documentation
-        -------------
-        
-        Documentation is available on ReadTheDocs_.
-        
 Keywords: api,dandelion
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Italian
 Classifier: Natural Language :: Spanish
@@ -72,7 +24,54 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/giacbrd/python-dandelion-eu.svg?branch=master
+  :target: https://travis-ci.org/giacbrd/python-dandelion-eu
+
+.. image:: https://coveralls.io/repos/SpazioDati/python-dandelion-eu/badge.png?branch=master
+  :target: https://coveralls.io/r/SpazioDati/python-dandelion-eu?branch=master
+
+.. image:: https://img.shields.io/pypi/v/dandelion-eu
+    :target: https://pypi.python.org/pypi/dandelion-eu/
+    :alt: Latest PyPI version
+
+.. _PyPI: https://pypi.python.org/pypi/dandelion-eu/
+.. _ReadTheDocs: http://python-dandelion-eu.readthedocs.org/
+.. _dandelion: https://dandelion.eu/accounts/register/?next=/
+.. _dandelion.eu: http://dandelion.eu/
+
+python-dandelion-eu
+===================
+
+Bring the power of the dandelion.eu_ semantic to your python applications and scripts!
+Semantic in python couldn't be easier.
+
+
+.. code-block:: py
+
+    >>> from dandelion import DataTXT
+    >>> datatxt = DataTXT(token='YOUR_TOKEN')
+    >>> response = datatxt.nex('The doctor says an apple is better than an orange')
+    >>> for annotation in response.annotations:
+          print(annotation)
+    ...
+
+Register on dandelion_ to obtain your authentication token and enrich your application with our semantic intelligence.
+
+Installation
+------------
+
+``dandelion-eu`` is available on PyPI_ install it simply with::
+
+    pip install dandelion-eu
+
+
+Documentation
+-------------
+
+Documentation is available on ReadTheDocs_.
```

### Comparing `dandelion-eu-0.3.2/README.rst` & `dandelion-eu-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `dandelion-eu-0.3.2/dandelion/base.py` & `dandelion-eu-0.3.3/dandelion/base.py`

 * *Files identical despite different names*

### Comparing `dandelion-eu-0.3.2/dandelion/cache/base.py` & `dandelion-eu-0.3.3/dandelion/cache/base.py`

 * *Files identical despite different names*

### Comparing `dandelion-eu-0.3.2/dandelion/cache/file.py` & `dandelion-eu-0.3.3/dandelion/cache/file.py`

 * *Files identical despite different names*

### Comparing `dandelion-eu-0.3.2/dandelion/datagem.py` & `dandelion-eu-0.3.3/dandelion/datagem.py`

 * *Files identical despite different names*

### Comparing `dandelion-eu-0.3.2/dandelion/datatxt.py` & `dandelion-eu-0.3.3/dandelion/datatxt.py`

 * *Files identical despite different names*

### Comparing `dandelion-eu-0.3.2/dandelion_eu.egg-info/PKG-INFO` & `dandelion-eu-0.3.3/dandelion_eu.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dandelion-eu
-Version: 0.3.2
+Version: 0.3.3
 Summary: Connect to the dandelion.eu API in a very pythonic way!
 Home-page: https://github.com/giacbrd/python-dandelion-eu
+Download-URL: https://github.com/giacbrd/python-dandelion-eu/tarball/0.3.3
 Author: SpazioDati s.r.l.
 Author-email: berardi@spaziodati.eu
-License: UNKNOWN
-Download-URL: https://github.com/giacbrd/python-dandelion-eu/tarball/0.3.2
-Description: .. image:: https://travis-ci.org/giacbrd/python-dandelion-eu.svg?branch=master
-          :target: https://travis-ci.org/giacbrd/python-dandelion-eu
-        
-        .. image:: https://coveralls.io/repos/SpazioDati/python-dandelion-eu/badge.png?branch=master
-          :target: https://coveralls.io/r/SpazioDati/python-dandelion-eu?branch=master
-        
-        .. image:: https://img.shields.io/pypi/v/dandelion-eu
-            :target: https://pypi.python.org/pypi/dandelion-eu/
-            :alt: Latest PyPI version
-        
-        .. _PyPI: https://pypi.python.org/pypi/dandelion-eu/
-        .. _ReadTheDocs: http://python-dandelion-eu.readthedocs.org/
-        .. _dandelion: https://dandelion.eu/accounts/register/?next=/
-        .. _dandelion.eu: http://dandelion.eu/
-        
-        python-dandelion-eu
-        ===================
-        
-        Bring the power of the dandelion.eu_ semantic to your python applications and scripts!
-        Semantic in python couldn't be easier.
-        
-        
-        .. code-block:: py
-        
-            >>> from dandelion import DataTXT
-            >>> datatxt = DataTXT(token='YOUR_TOKEN')
-            >>> response = datatxt.nex('The doctor says an apple is better than an orange')
-            >>> for annotation in response.annotations:
-                  print(annotation)
-            ...
-        
-        Register on dandelion_ to obtain your authentication token and enrich your application with our semantic intelligence.
-        
-        Installation
-        ------------
-        
-        ``dandelion-eu`` is available on PyPI_ install it simply with::
-        
-            pip install dandelion-eu
-        
-        
-        Documentation
-        -------------
-        
-        Documentation is available on ReadTheDocs_.
-        
 Keywords: api,dandelion
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Italian
 Classifier: Natural Language :: Spanish
@@ -72,7 +24,54 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/giacbrd/python-dandelion-eu.svg?branch=master
+  :target: https://travis-ci.org/giacbrd/python-dandelion-eu
+
+.. image:: https://coveralls.io/repos/SpazioDati/python-dandelion-eu/badge.png?branch=master
+  :target: https://coveralls.io/r/SpazioDati/python-dandelion-eu?branch=master
+
+.. image:: https://img.shields.io/pypi/v/dandelion-eu
+    :target: https://pypi.python.org/pypi/dandelion-eu/
+    :alt: Latest PyPI version
+
+.. _PyPI: https://pypi.python.org/pypi/dandelion-eu/
+.. _ReadTheDocs: http://python-dandelion-eu.readthedocs.org/
+.. _dandelion: https://dandelion.eu/accounts/register/?next=/
+.. _dandelion.eu: http://dandelion.eu/
+
+python-dandelion-eu
+===================
+
+Bring the power of the dandelion.eu_ semantic to your python applications and scripts!
+Semantic in python couldn't be easier.
+
+
+.. code-block:: py
+
+    >>> from dandelion import DataTXT
+    >>> datatxt = DataTXT(token='YOUR_TOKEN')
+    >>> response = datatxt.nex('The doctor says an apple is better than an orange')
+    >>> for annotation in response.annotations:
+          print(annotation)
+    ...
+
+Register on dandelion_ to obtain your authentication token and enrich your application with our semantic intelligence.
+
+Installation
+------------
+
+``dandelion-eu`` is available on PyPI_ install it simply with::
+
+    pip install dandelion-eu
+
+
+Documentation
+-------------
+
+Documentation is available on ReadTheDocs_.
```

### Comparing `dandelion-eu-0.3.2/setup.py` & `dandelion-eu-0.3.3/setup.py`

 * *Files identical despite different names*

