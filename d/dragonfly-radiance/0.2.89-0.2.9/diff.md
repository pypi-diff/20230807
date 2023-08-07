# Comparing `tmp/dragonfly-radiance-0.2.89.tar.gz` & `tmp/dragonfly-radiance-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dragonfly-radiance-0.2.89.tar", last modified: Mon Aug  7 20:00:15 2023, max compression
+gzip compressed data, was "dist/dragonfly-radiance-0.2.9.tar", last modified: Mon Mar  6 15:17:33 2023, max compression
```

## Comparing `dragonfly-radiance-0.2.89.tar` & `dragonfly-radiance-0.2.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:00:15.000000 dragonfly-radiance-0.2.89/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-08-07 20:00:15.000000 dragonfly-radiance-0.2.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:00:15.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/_extend_dragonfly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:00:15.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)    25643 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/gridpar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:00:15.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/properties/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/properties/building.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/properties/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/properties/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/properties/room2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/dragonfly_radiance/properties/story.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:00:15.000000 dragonfly-radiance-0.2.89/dragonfly_radiance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-08-07 20:00:15.000000 dragonfly-radiance-0.2.89/dragonfly_radiance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-07 20:00:15.000000 dragonfly-radiance-0.2.89/dragonfly_radiance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:00:15.000000 dragonfly-radiance-0.2.89/dragonfly_radiance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 20:00:15.000000 dragonfly-radiance-0.2.89/dragonfly_radiance.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-07 20:00:15.000000 dragonfly-radiance-0.2.89/dragonfly_radiance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-07 20:00:15.000000 dragonfly-radiance-0.2.89/dragonfly_radiance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-07 20:00:15.000000 dragonfly-radiance-0.2.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-07 19:58:42.000000 dragonfly-radiance-0.2.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:17:33.000000 dragonfly-radiance-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-06 15:17:33.000000 dragonfly-radiance-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:17:33.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/_extend_dragonfly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:17:33.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25643 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/gridpar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:17:33.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/properties/building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/properties/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/properties/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/properties/room2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/dragonfly_radiance/properties/story.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:17:33.000000 dragonfly-radiance-0.2.9/dragonfly_radiance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-06 15:17:33.000000 dragonfly-radiance-0.2.9/dragonfly_radiance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-06 15:17:33.000000 dragonfly-radiance-0.2.9/dragonfly_radiance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 15:17:33.000000 dragonfly-radiance-0.2.9/dragonfly_radiance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-06 15:17:33.000000 dragonfly-radiance-0.2.9/dragonfly_radiance.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-06 15:17:33.000000 dragonfly-radiance-0.2.9/dragonfly_radiance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-06 15:17:33.000000 dragonfly-radiance-0.2.9/dragonfly_radiance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-06 15:17:33.000000 dragonfly-radiance-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-03-06 15:16:10.000000 dragonfly-radiance-0.2.9/setup.py
```

### Comparing `dragonfly-radiance-0.2.89/LICENSE` & `dragonfly-radiance-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.2.89/PKG-INFO` & `dragonfly-radiance-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfly-radiance
-Version: 0.2.89
+Version: 0.2.9
 Summary: Dragonfly extension for radiance simulation.
 Home-page: https://github.com/ladybug-tools/dragonfly-radiance
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dragonfly-radiance-0.2.89/README.md` & `dragonfly-radiance-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.2.89/dev-requirements.txt` & `dragonfly-radiance-0.2.9/dev-requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 coverage==5.5
 coveralls==1.7.0;python_version<'3.0'
 coveralls==2.2.0;python_version>='3.6'
 pytest==4.6.9;python_version<'3.0'
 pytest==6.2.4;python_version>='3.6'
 pytest-cov==2.12.0
 Sphinx==1.8.5;python_version<'3.0'
-Sphinx==5.3.0;python_version>='3.6'
+Sphinx==3.3.1;python_version>='3.6'
 docutils==0.17;python_version>='3.6'
 sphinx-bootstrap-theme==0.8.1
-sphinxcontrib-fulltoc==1.2.0
 sphinxcontrib-websupport==1.1.2;python_version<'3.0'
 sphinxcontrib-websupport==1.2.4;python_version>='3.6'
-sphinx-click==4.4.0
+sphinxcontrib-fulltoc==1.2.0
+sphinx-click==2.7.1
 twine==1.13.0;python_version<'3.0'
 twine==3.4.1;python_version>='3.6'
 wheel==0.38.1
 setuptools==44.1.0;python_version<'3.0'
 setuptools==65.5.1;python_version>='3.6'
 importlib-metadata==2.0.0;python_version<'3.0'
-importlib-metadata==4.8.0;python_version>='3.6'
+importlib-metadata==4.3.1;python_version>='3.6'
 jinja2==3.0.3;python_version>='3.6'
 markupsafe==2.0.1;python_version>='3.6'
```

### Comparing `dragonfly-radiance-0.2.89/dragonfly_radiance/_extend_dragonfly.py` & `dragonfly-radiance-0.2.9/dragonfly_radiance/_extend_dragonfly.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.2.89/dragonfly_radiance/cli/translate.py` & `dragonfly-radiance-0.2.9/dragonfly_radiance/cli/translate.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.2.89/dragonfly_radiance/gridpar.py` & `dragonfly-radiance-0.2.9/dragonfly_radiance/gridpar.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.2.89/dragonfly_radiance/properties/context.py` & `dragonfly-radiance-0.2.9/dragonfly_radiance/properties/context.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.2.89/dragonfly_radiance/properties/model.py` & `dragonfly-radiance-0.2.9/dragonfly_radiance/properties/model.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.2.89/dragonfly_radiance/properties/room2d.py` & `dragonfly-radiance-0.2.9/dragonfly_radiance/properties/room2d.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.2.89/dragonfly_radiance/properties/story.py` & `dragonfly-radiance-0.2.9/dragonfly_radiance/properties/story.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.2.89/dragonfly_radiance.egg-info/PKG-INFO` & `dragonfly-radiance-0.2.9/dragonfly_radiance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfly-radiance
-Version: 0.2.89
+Version: 0.2.9
 Summary: Dragonfly extension for radiance simulation.
 Home-page: https://github.com/ladybug-tools/dragonfly-radiance
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dragonfly-radiance-0.2.89/dragonfly_radiance.egg-info/SOURCES.txt` & `dragonfly-radiance-0.2.9/dragonfly_radiance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.2.89/setup.py` & `dragonfly-radiance-0.2.9/setup.py`

 * *Files identical despite different names*

