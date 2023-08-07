# Comparing `tmp/jourdanhub-0.0.1.tar.gz` & `tmp/jourdanhub-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jourdanhub-0.0.1.tar", last modified: Mon Aug  7 15:27:00 2023, max compression
+gzip compressed data, was "jourdanhub-0.0.2.tar", last modified: Mon Aug  7 16:00:20 2023, max compression
```

## Comparing `jourdanhub-0.0.1.tar` & `jourdanhub-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 15:27:00.269582 jourdanhub-0.0.1/
--rw-rw-rw-   0        0        0      225 2023-08-07 12:11:20.000000 jourdanhub-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      647 2023-08-07 15:27:00.269582 jourdanhub-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-08-07 15:23:12.000000 jourdanhub-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 15:27:00.247583 jourdanhub-0.0.1/jourdanhub/
--rw-rw-rw-   0        0        0       36 2023-08-07 12:18:23.000000 jourdanhub-0.0.1/jourdanhub/__init__.py
--rw-rw-rw-   0        0        0       63 2023-08-07 12:06:01.000000 jourdanhub-0.0.1/jourdanhub/__main__.py
--rw-rw-rw-   0        0        0       23 2023-08-07 12:21:30.000000 jourdanhub-0.0.1/jourdanhub/_version.py
--rw-rw-rw-   0        0        0      657 2023-08-07 14:11:31.000000 jourdanhub-0.0.1/jourdanhub/app.py
--rw-rw-rw-   0        0        0      788 2023-08-07 12:06:01.000000 jourdanhub-0.0.1/jourdanhub/userapi_handler.py
-drwxrwxrwx   0        0        0        0 2023-08-07 15:27:00.268587 jourdanhub-0.0.1/jourdanhub.egg-info/
--rw-rw-rw-   0        0        0      647 2023-08-07 15:26:59.000000 jourdanhub-0.0.1/jourdanhub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-08-07 15:26:59.000000 jourdanhub-0.0.1/jourdanhub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 15:26:59.000000 jourdanhub-0.0.1/jourdanhub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-08-07 15:26:59.000000 jourdanhub-0.0.1/jourdanhub.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-08-07 14:12:30.000000 jourdanhub-0.0.1/jourdanhub.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-08-07 15:26:59.000000 jourdanhub-0.0.1/jourdanhub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-07 15:26:59.000000 jourdanhub-0.0.1/jourdanhub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      130 2023-08-07 12:11:10.000000 jourdanhub-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-08-07 15:27:00.271582 jourdanhub-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1327 2023-08-07 15:26:32.000000 jourdanhub-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:00:20.748430 jourdanhub-0.0.2/
+-rw-rw-rw-   0        0        0      225 2023-08-07 12:11:20.000000 jourdanhub-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      647 2023-08-07 16:00:20.749433 jourdanhub-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-08-07 15:23:12.000000 jourdanhub-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 16:00:20.706825 jourdanhub-0.0.2/jourdanhub/
+-rw-rw-rw-   0        0        0       36 2023-08-07 12:18:23.000000 jourdanhub-0.0.2/jourdanhub/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-08-07 12:06:01.000000 jourdanhub-0.0.2/jourdanhub/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-08-07 16:00:17.000000 jourdanhub-0.0.2/jourdanhub/_version.py
+-rw-rw-rw-   0        0        0      657 2023-08-07 14:11:31.000000 jourdanhub-0.0.2/jourdanhub/app.py
+-rw-rw-rw-   0        0        0      788 2023-08-07 12:06:01.000000 jourdanhub-0.0.2/jourdanhub/userapi_handler.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:00:20.747435 jourdanhub-0.0.2/jourdanhub.egg-info/
+-rw-rw-rw-   0        0        0      647 2023-08-07 16:00:20.000000 jourdanhub-0.0.2/jourdanhub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-08-07 16:00:20.000000 jourdanhub-0.0.2/jourdanhub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 16:00:20.000000 jourdanhub-0.0.2/jourdanhub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-08-07 16:00:20.000000 jourdanhub-0.0.2/jourdanhub.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 16:00:20.000000 jourdanhub-0.0.2/jourdanhub.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-08-07 16:00:20.000000 jourdanhub-0.0.2/jourdanhub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-07 16:00:20.000000 jourdanhub-0.0.2/jourdanhub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      130 2023-08-07 12:11:10.000000 jourdanhub-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-08-07 16:00:20.762430 jourdanhub-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1327 2023-08-07 16:00:01.000000 jourdanhub-0.0.2/setup.py
```

### Comparing `jourdanhub-0.0.1/PKG-INFO` & `jourdanhub-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jourdanhub
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wrapper for JupyterHub
 Home-page: https://github.com/carlosjourdan/jourdanhub
 Author: Carlos Jourdan
 License: AGPL-3.0
 Keywords: JupyterHub,SWAN,CERN
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `jourdanhub-0.0.1/jourdanhub/app.py` & `jourdanhub-0.0.2/jourdanhub/app.py`

 * *Files identical despite different names*

### Comparing `jourdanhub-0.0.1/jourdanhub/userapi_handler.py` & `jourdanhub-0.0.2/jourdanhub/userapi_handler.py`

 * *Files identical despite different names*

### Comparing `jourdanhub-0.0.1/jourdanhub.egg-info/PKG-INFO` & `jourdanhub-0.0.2/jourdanhub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jourdanhub
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wrapper for JupyterHub
 Home-page: https://github.com/carlosjourdan/jourdanhub
 Author: Carlos Jourdan
 License: AGPL-3.0
 Keywords: JupyterHub,SWAN,CERN
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `jourdanhub-0.0.1/setup.py` & `jourdanhub-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     url="https://github.com/carlosjourdan/jourdanhub",
     author="Carlos Jourdan",
     description="Wrapper for JupyterHub",
     long_description= long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
-          'jupyterhub~=3.0.0'
+          'jupyterhub~=4.0.1'
     ],
     zip_safe=False,
     include_package_data=True,
     license="AGPL-3.0",
     platforms="Linux, Mac OS X",
     keywords=["JupyterHub", "SWAN", "CERN"],
     entry_points={
```

