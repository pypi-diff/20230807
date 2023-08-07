# Comparing `tmp/sakib_helpers-0.0.2.tar.gz` & `tmp/sakib_helpers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sakib_helpers-0.0.2.tar", last modified: Sat Aug  5 02:55:31 2023, max compression
+gzip compressed data, was "sakib_helpers-0.0.3.tar", last modified: Mon Aug  7 03:10:28 2023, max compression
```

## Comparing `sakib_helpers-0.0.2.tar` & `sakib_helpers-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 02:55:31.413962 sakib_helpers-0.0.2/
--rw-rw-rw-   0        0        0     1085 2023-08-02 02:13:53.000000 sakib_helpers-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1619 2023-08-05 02:55:31.413962 sakib_helpers-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      956 2023-08-02 02:13:35.000000 sakib_helpers-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 02:55:31.351030 sakib_helpers-0.0.2/sakib_helpers/
--rw-rw-rw-   0        0        0        0 2023-08-02 02:03:25.000000 sakib_helpers-0.0.2/sakib_helpers/__init__.py
--rw-rw-rw-   0        0        0      205 2023-08-02 02:12:47.000000 sakib_helpers-0.0.2/sakib_helpers/helpers.py
-drwxrwxrwx   0        0        0        0 2023-08-05 02:55:31.398323 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/
--rw-rw-rw-   0        0        0        0 2023-08-03 03:08:38.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/__init__.py
--rw-rw-rw-   0        0        0       66 2023-08-03 03:08:38.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/admin.py
--rw-rw-rw-   0        0        0      184 2023-08-05 02:52:34.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/apps.py
-drwxrwxrwx   0        0        0        0 2023-08-05 02:55:31.413962 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/migrations/
--rw-rw-rw-   0        0        0        0 2023-08-03 03:08:38.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2023-08-03 03:08:38.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/models.py
-drwxrwxrwx   0        0        0        0 2023-08-05 02:55:31.413962 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/templatetags/
--rw-rw-rw-   0        0        0        0 2023-08-03 03:11:05.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/templatetags/__init__.py
--rw-rw-rw-   0        0        0      357 2023-08-03 03:15:10.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/templatetags/sakib_helpers.py
--rw-rw-rw-   0        0        0       63 2023-08-03 03:08:38.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/tests.py
--rw-rw-rw-   0        0        0       66 2023-08-03 03:08:38.000000 sakib_helpers-0.0.2/sakib_helpers/sakib_helpers_app/views.py
-drwxrwxrwx   0        0        0        0 2023-08-05 02:55:31.392311 sakib_helpers-0.0.2/sakib_helpers.egg-info/
--rw-rw-rw-   0        0        0     1619 2023-08-05 02:55:31.000000 sakib_helpers-0.0.2/sakib_helpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      720 2023-08-05 02:55:31.000000 sakib_helpers-0.0.2/sakib_helpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 02:55:31.000000 sakib_helpers-0.0.2/sakib_helpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-05 02:55:31.000000 sakib_helpers-0.0.2/sakib_helpers.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-08-05 02:55:31.000000 sakib_helpers-0.0.2/sakib_helpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-05 02:55:31.000000 sakib_helpers-0.0.2/sakib_helpers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 02:55:31.413962 sakib_helpers-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3121 2023-08-05 02:55:24.000000 sakib_helpers-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 03:10:28.410688 sakib_helpers-0.0.3/
+-rw-rw-rw-   0        0        0     1085 2023-08-02 02:13:53.000000 sakib_helpers-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1619 2023-08-07 03:10:28.408671 sakib_helpers-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      956 2023-08-02 02:13:35.000000 sakib_helpers-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 03:10:28.238829 sakib_helpers-0.0.3/sakib_helpers/
+-rw-rw-rw-   0        0        0        0 2023-08-02 02:03:25.000000 sakib_helpers-0.0.3/sakib_helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 03:10:28.389542 sakib_helpers-0.0.3/sakib_helpers/app/
+-rw-rw-rw-   0        0        0        0 2023-08-03 03:08:38.000000 sakib_helpers-0.0.3/sakib_helpers/app/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-08-03 03:08:38.000000 sakib_helpers-0.0.3/sakib_helpers/app/admin.py
+-rw-rw-rw-   0        0        0      158 2023-08-07 02:55:47.000000 sakib_helpers-0.0.3/sakib_helpers/app/apps.py
+drwxrwxrwx   0        0        0        0 2023-08-07 03:10:28.393545 sakib_helpers-0.0.3/sakib_helpers/app/migrations/
+-rw-rw-rw-   0        0        0        0 2023-08-03 03:08:38.000000 sakib_helpers-0.0.3/sakib_helpers/app/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-08-03 03:08:38.000000 sakib_helpers-0.0.3/sakib_helpers/app/models.py
+drwxrwxrwx   0        0        0        0 2023-08-07 03:10:28.402121 sakib_helpers-0.0.3/sakib_helpers/app/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-08-03 03:11:05.000000 sakib_helpers-0.0.3/sakib_helpers/app/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     1280 2023-08-07 02:59:37.000000 sakib_helpers-0.0.3/sakib_helpers/app/templatetags/sakib_helpers.py
+-rw-rw-rw-   0        0        0       63 2023-08-03 03:08:38.000000 sakib_helpers-0.0.3/sakib_helpers/app/tests.py
+-rw-rw-rw-   0        0        0       66 2023-08-03 03:08:38.000000 sakib_helpers-0.0.3/sakib_helpers/app/views.py
+-rw-rw-rw-   0        0        0     3942 2023-08-07 03:09:27.000000 sakib_helpers-0.0.3/sakib_helpers/helpers.py
+drwxrwxrwx   0        0        0        0 2023-08-07 03:10:28.360865 sakib_helpers-0.0.3/sakib_helpers.egg-info/
+-rw-rw-rw-   0        0        0     1619 2023-08-07 03:10:27.000000 sakib_helpers-0.0.3/sakib_helpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2023-08-07 03:10:28.000000 sakib_helpers-0.0.3/sakib_helpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 03:10:27.000000 sakib_helpers-0.0.3/sakib_helpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 03:10:27.000000 sakib_helpers-0.0.3/sakib_helpers.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-08-07 03:10:27.000000 sakib_helpers-0.0.3/sakib_helpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-07 03:10:27.000000 sakib_helpers-0.0.3/sakib_helpers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 03:10:28.411683 sakib_helpers-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2987 2023-08-07 03:10:11.000000 sakib_helpers-0.0.3/setup.py
```

### Comparing `sakib_helpers-0.0.2/LICENSE` & `sakib_helpers-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sakib_helpers-0.0.2/PKG-INFO` & `sakib_helpers-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sakib_helpers
-Version: 0.0.2
+Version: 0.0.3
 Summary: python helper functions/methods
 Home-page: https://w3code.tech
 Author: Sakib Malik
 Author-email: maliksakib347@gmail.com
 Project-URL: Docs, https://w3code.tech
 Keywords: arithmetic,math,mathematics,python tutorial
 Classifier: Development Status :: 1 - Planning
```

### Comparing `sakib_helpers-0.0.2/README.md` & `sakib_helpers-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sakib_helpers-0.0.2/sakib_helpers.egg-info/PKG-INFO` & `sakib_helpers-0.0.3/sakib_helpers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sakib-helpers
-Version: 0.0.2
+Version: 0.0.3
 Summary: python helper functions/methods
 Home-page: https://w3code.tech
 Author: Sakib Malik
 Author-email: maliksakib347@gmail.com
 Project-URL: Docs, https://w3code.tech
 Keywords: arithmetic,math,mathematics,python tutorial
 Classifier: Development Status :: 1 - Planning
```

### Comparing `sakib_helpers-0.0.2/sakib_helpers.egg-info/SOURCES.txt` & `sakib_helpers-0.0.3/sakib_helpers.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 sakib_helpers/helpers.py
 sakib_helpers.egg-info/PKG-INFO
 sakib_helpers.egg-info/SOURCES.txt
 sakib_helpers.egg-info/dependency_links.txt
 sakib_helpers.egg-info/not-zip-safe
 sakib_helpers.egg-info/requires.txt
 sakib_helpers.egg-info/top_level.txt
-sakib_helpers/sakib_helpers_app/__init__.py
-sakib_helpers/sakib_helpers_app/admin.py
-sakib_helpers/sakib_helpers_app/apps.py
-sakib_helpers/sakib_helpers_app/models.py
-sakib_helpers/sakib_helpers_app/tests.py
-sakib_helpers/sakib_helpers_app/views.py
-sakib_helpers/sakib_helpers_app/migrations/__init__.py
-sakib_helpers/sakib_helpers_app/templatetags/__init__.py
-sakib_helpers/sakib_helpers_app/templatetags/sakib_helpers.py
+sakib_helpers/app/__init__.py
+sakib_helpers/app/admin.py
+sakib_helpers/app/apps.py
+sakib_helpers/app/models.py
+sakib_helpers/app/tests.py
+sakib_helpers/app/views.py
+sakib_helpers/app/migrations/__init__.py
+sakib_helpers/app/templatetags/__init__.py
+sakib_helpers/app/templatetags/sakib_helpers.py
```

### Comparing `sakib_helpers-0.0.2/setup.py` & `sakib_helpers-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 import sys
 from io import open
 
 
 CURRENT_PYTHON = sys.version_info[:2]
 REQUIRED_PYTHON = (3, 6)
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'python helper functions/methods'
-LONG_DESCRIPTION = 'In this package have more helpful packages used in django and python. This package is developed by sakib malik.'
 
 
 def read(f):
     return open(f, 'r', encoding='utf-8').read()
 
 
 # This check and everything above must remain compatible with Python 2.7.
```

