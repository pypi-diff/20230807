# Comparing `tmp/py-worksdone-utils-1.0.7.tar.gz` & `tmp/py-worksdone-utils-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-worksdone-utils-1.0.7.tar", last modified: Fri Aug  4 13:20:48 2023, max compression
+gzip compressed data, was "py-worksdone-utils-1.0.8.tar", last modified: Mon Aug  7 07:36:58 2023, max compression
```

## Comparing `py-worksdone-utils-1.0.7.tar` & `py-worksdone-utils-1.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 13:20:48.588519 py-worksdone-utils-1.0.7/
--rw-r--r--   0 erne      (1000) erne      (1000)      420 2023-08-04 13:20:48.588519 py-worksdone-utils-1.0.7/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)     6386 2023-07-20 13:12:23.000000 py-worksdone-utils-1.0.7/README.md
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 13:20:48.588519 py-worksdone-utils-1.0.7/py_worksdone_utils.egg-info/
--rw-r--r--   0 erne      (1000) erne      (1000)      420 2023-08-04 13:20:48.000000 py-worksdone-utils-1.0.7/py_worksdone_utils.egg-info/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)      520 2023-08-04 13:20:48.000000 py-worksdone-utils-1.0.7/py_worksdone_utils.egg-info/SOURCES.txt
--rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-08-04 13:20:48.000000 py-worksdone-utils-1.0.7/py_worksdone_utils.egg-info/dependency_links.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       23 2023-08-04 13:20:48.000000 py-worksdone-utils-1.0.7/py_worksdone_utils.egg-info/requires.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       17 2023-08-04 13:20:48.000000 py-worksdone-utils-1.0.7/py_worksdone_utils.egg-info/top_level.txt
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 13:20:48.588519 py-worksdone-utils-1.0.7/pyworksdoneutils/
--rw-r--r--   0 erne      (1000) erne      (1000)        2 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.7/pyworksdoneutils/__init__.py
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 13:20:48.588519 py-worksdone-utils-1.0.7/pyworksdoneutils/keycloak/
--rw-r--r--   0 erne      (1000) erne      (1000)        0 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.7/pyworksdoneutils/keycloak/__init__.py
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 13:20:48.588519 py-worksdone-utils-1.0.7/pyworksdoneutils/keycloak/flask/
--rw-r--r--   0 erne      (1000) erne      (1000)       82 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.7/pyworksdoneutils/keycloak/flask/__init__.py
--rw-r--r--   0 erne      (1000) erne      (1000)     3932 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.7/pyworksdoneutils/keycloak/flask/_decorators.py
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 13:20:48.588519 py-worksdone-utils-1.0.7/pyworksdoneutils/sqlalchemy/
--rw-r--r--   0 erne      (1000) erne      (1000)        0 2023-08-04 12:23:57.000000 py-worksdone-utils-1.0.7/pyworksdoneutils/sqlalchemy/__init__.py
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-04 13:20:48.588519 py-worksdone-utils-1.0.7/pyworksdoneutils/sqlalchemy/flask/
--rw-r--r--   0 erne      (1000) erne      (1000)       37 2023-08-04 12:25:58.000000 py-worksdone-utils-1.0.7/pyworksdoneutils/sqlalchemy/flask/__init__.py
--rw-r--r--   0 erne      (1000) erne      (1000)     1169 2023-08-04 13:20:22.000000 py-worksdone-utils-1.0.7/pyworksdoneutils/sqlalchemy/flask/_decorators.py
--rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-08-04 13:20:48.588519 py-worksdone-utils-1.0.7/setup.cfg
--rw-r--r--   0 erne      (1000) erne      (1000)      647 2023-08-04 13:20:44.000000 py-worksdone-utils-1.0.7/setup.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-07 07:36:58.048226 py-worksdone-utils-1.0.8/
+-rw-r--r--   0 erne      (1000) erne      (1000)      420 2023-08-07 07:36:58.038226 py-worksdone-utils-1.0.8/PKG-INFO
+-rw-r--r--   0 erne      (1000) erne      (1000)     6386 2023-07-20 13:12:23.000000 py-worksdone-utils-1.0.8/README.md
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-07 07:36:58.038226 py-worksdone-utils-1.0.8/py_worksdone_utils.egg-info/
+-rw-r--r--   0 erne      (1000) erne      (1000)      420 2023-08-07 07:36:58.000000 py-worksdone-utils-1.0.8/py_worksdone_utils.egg-info/PKG-INFO
+-rw-r--r--   0 erne      (1000) erne      (1000)      520 2023-08-07 07:36:58.000000 py-worksdone-utils-1.0.8/py_worksdone_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-08-07 07:36:58.000000 py-worksdone-utils-1.0.8/py_worksdone_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       23 2023-08-07 07:36:58.000000 py-worksdone-utils-1.0.8/py_worksdone_utils.egg-info/requires.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       17 2023-08-07 07:36:58.000000 py-worksdone-utils-1.0.8/py_worksdone_utils.egg-info/top_level.txt
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-07 07:36:58.038226 py-worksdone-utils-1.0.8/pyworksdoneutils/
+-rw-r--r--   0 erne      (1000) erne      (1000)        2 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.8/pyworksdoneutils/__init__.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-07 07:36:58.038226 py-worksdone-utils-1.0.8/pyworksdoneutils/keycloak/
+-rw-r--r--   0 erne      (1000) erne      (1000)        0 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.8/pyworksdoneutils/keycloak/__init__.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-07 07:36:58.038226 py-worksdone-utils-1.0.8/pyworksdoneutils/keycloak/flask/
+-rw-r--r--   0 erne      (1000) erne      (1000)       82 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.8/pyworksdoneutils/keycloak/flask/__init__.py
+-rw-r--r--   0 erne      (1000) erne      (1000)     3932 2023-08-04 12:23:01.000000 py-worksdone-utils-1.0.8/pyworksdoneutils/keycloak/flask/_decorators.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-07 07:36:58.038226 py-worksdone-utils-1.0.8/pyworksdoneutils/sqlalchemy/
+-rw-r--r--   0 erne      (1000) erne      (1000)        0 2023-08-04 12:23:57.000000 py-worksdone-utils-1.0.8/pyworksdoneutils/sqlalchemy/__init__.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-08-07 07:36:58.038226 py-worksdone-utils-1.0.8/pyworksdoneutils/sqlalchemy/flask/
+-rw-r--r--   0 erne      (1000) erne      (1000)       37 2023-08-04 12:25:58.000000 py-worksdone-utils-1.0.8/pyworksdoneutils/sqlalchemy/flask/__init__.py
+-rw-r--r--   0 erne      (1000) erne      (1000)     1039 2023-08-07 07:36:46.000000 py-worksdone-utils-1.0.8/pyworksdoneutils/sqlalchemy/flask/_decorators.py
+-rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-08-07 07:36:58.048226 py-worksdone-utils-1.0.8/setup.cfg
+-rw-r--r--   0 erne      (1000) erne      (1000)      647 2023-08-07 07:36:55.000000 py-worksdone-utils-1.0.8/setup.py
```

### Comparing `py-worksdone-utils-1.0.7/README.md` & `py-worksdone-utils-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `py-worksdone-utils-1.0.7/py_worksdone_utils.egg-info/SOURCES.txt` & `py-worksdone-utils-1.0.8/py_worksdone_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-worksdone-utils-1.0.7/pyworksdoneutils/keycloak/flask/_decorators.py` & `py-worksdone-utils-1.0.8/pyworksdoneutils/keycloak/flask/_decorators.py`

 * *Files identical despite different names*

### Comparing `py-worksdone-utils-1.0.7/setup.py` & `py-worksdone-utils-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
     name="py-worksdone-utils",
-    version="1.0.7",
+    version="1.0.8",
     author="KE",
     author_email="",
     description="Utilities with Keycloak",
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["python-keycloak==3.3.0"],
     keywords=["python", "decorator", "token", "keycloak"],
```

