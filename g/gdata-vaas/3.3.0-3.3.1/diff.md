# Comparing `tmp/gdata-vaas-3.3.0.tar.gz` & `tmp/gdata-vaas-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdata-vaas-3.3.0.tar", last modified: Mon Aug  7 10:10:04 2023, max compression
+gzip compressed data, was "gdata-vaas-3.3.1.tar", last modified: Mon Aug  7 15:10:23 2023, max compression
```

## Comparing `gdata-vaas-3.3.0.tar` & `gdata-vaas-3.3.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 10:10:04.939415 gdata-vaas-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-08-07 10:10:04.939415 gdata-vaas-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-08-07 10:10:04.939415 gdata-vaas-3.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 10:10:04.935415 gdata-vaas-3.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 10:10:04.939415 gdata-vaas-3.3.0/src/gdata_vaas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-08-07 10:10:04.000000 gdata-vaas-3.3.0/src/gdata_vaas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-08-07 10:10:04.000000 gdata-vaas-3.3.0/src/gdata_vaas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-07 10:10:04.000000 gdata-vaas-3.3.0/src/gdata_vaas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-08-07 10:10:04.000000 gdata-vaas-3.3.0/src/gdata_vaas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-08-07 10:10:04.000000 gdata-vaas-3.3.0/src/gdata_vaas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 10:10:04.939415 gdata-vaas-3.3.0/src/vaas/
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/src/vaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      938 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/src/vaas/client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (122)    11419 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/src/vaas/vaas.py
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/src/vaas/vaas_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 10:10:04.939415 gdata-vaas-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/tests/test_client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (122)     9579 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/tests/test_vaas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 15:10:23.684456 gdata-vaas-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-08-07 15:09:43.000000 gdata-vaas-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-08-07 15:10:23.684456 gdata-vaas-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-08-07 15:09:43.000000 gdata-vaas-3.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-08-07 15:09:43.000000 gdata-vaas-3.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      737 2023-08-07 15:10:23.688456 gdata-vaas-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-08-07 15:09:43.000000 gdata-vaas-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 15:10:23.684456 gdata-vaas-3.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 15:10:23.684456 gdata-vaas-3.3.1/src/gdata_vaas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-08-07 15:10:23.000000 gdata-vaas-3.3.1/src/gdata_vaas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-08-07 15:10:23.000000 gdata-vaas-3.3.1/src/gdata_vaas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-07 15:10:23.000000 gdata-vaas-3.3.1/src/gdata_vaas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-08-07 15:10:23.000000 gdata-vaas-3.3.1/src/gdata_vaas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-08-07 15:10:23.000000 gdata-vaas-3.3.1/src/gdata_vaas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 15:10:23.684456 gdata-vaas-3.3.1/src/vaas/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-08-07 15:09:43.000000 gdata-vaas-3.3.1/src/vaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      938 2023-08-07 15:09:43.000000 gdata-vaas-3.3.1/src/vaas/client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11419 2023-08-07 15:09:43.000000 gdata-vaas-3.3.1/src/vaas/vaas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-08-07 15:09:43.000000 gdata-vaas-3.3.1/src/vaas/vaas_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 15:10:23.684456 gdata-vaas-3.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-08-07 15:09:43.000000 gdata-vaas-3.3.1/tests/test_client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9579 2023-08-07 15:09:43.000000 gdata-vaas-3.3.1/tests/test_vaas.py
```

### Comparing `gdata-vaas-3.3.0/LICENSE` & `gdata-vaas-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.3.0/PKG-INFO` & `gdata-vaas-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 3.3.0
+Version: 3.3.1
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata-vaas-3.3.0/README.md` & `gdata-vaas-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.3.0/setup.cfg` & `gdata-vaas-3.3.1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gdata-vaas
-version = 3.3.0
+version = 3.3.1
 author = G DATA CyberDefense AG
 author_email = oem@gdata.de
 description = gdata-vaas is a Python library for the VaaS-API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GDATASoftwareAG/vaas/tree/main/python
 project_urls = 
@@ -13,19 +13,19 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 python_requires = >=3.8
 install_requires = 
-	websockets ==10.4
-	httpx[http2] ==0.24.1
-	pyjwt == 2.3.0
-	authlib ==1.2.1
-	aiofiles==23.1.0
+	websockets>=10.4
+	httpx[http2]>=0.24.1
+	pyjwt>=2.0.0
+	authlib>=1.2.1
+	aiofiles>=23.1.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gdata-vaas-3.3.0/src/gdata_vaas.egg-info/PKG-INFO` & `gdata-vaas-3.3.1/src/gdata_vaas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 3.3.0
+Version: 3.3.1
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata-vaas-3.3.0/src/vaas/__init__.py` & `gdata-vaas-3.3.1/src/vaas/__init__.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.3.0/src/vaas/client_credentials_grant_authenticator.py` & `gdata-vaas-3.3.1/src/vaas/client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.3.0/src/vaas/vaas.py` & `gdata-vaas-3.3.1/src/vaas/vaas.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.3.0/tests/test_client_credentials_grant_authenticator.py` & `gdata-vaas-3.3.1/tests/test_client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.3.0/tests/test_vaas.py` & `gdata-vaas-3.3.1/tests/test_vaas.py`

 * *Files identical despite different names*

