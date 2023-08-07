# Comparing `tmp/zi_api_auth_client-2.0.0.tar.gz` & `tmp/zi_api_auth_client-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zi_api_auth_client-2.0.0.tar", last modified: Fri Jan 13 01:32:31 2023, max compression
+gzip compressed data, was "zi_api_auth_client-2.0.1.tar", last modified: Mon Aug  7 17:40:00 2023, max compression
```

## Comparing `zi_api_auth_client-2.0.0.tar` & `zi_api_auth_client-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 harsh.singh   (503) staff       (20)        0 2023-01-13 01:32:31.865584 zi_api_auth_client-2.0.0/
--rw-r--r--   0 harsh.singh   (503) staff       (20)     1077 2023-01-13 01:30:29.000000 zi_api_auth_client-2.0.0/LICENSE.txt
--rw-r--r--   0 harsh.singh   (503) staff       (20)     2097 2023-01-13 01:32:31.865208 zi_api_auth_client-2.0.0/PKG-INFO
--rw-r--r--   0 harsh.singh   (503) staff       (20)     1683 2023-01-13 01:30:29.000000 zi_api_auth_client-2.0.0/README.md
--rw-r--r--   0 harsh.singh   (503) staff       (20)       38 2023-01-13 01:32:31.865713 zi_api_auth_client-2.0.0/setup.cfg
--rw-r--r--   0 harsh.singh   (503) staff       (20)     1078 2023-01-13 01:30:29.000000 zi_api_auth_client-2.0.0/setup.py
-drwxr-xr-x   0 harsh.singh   (503) staff       (20)        0 2023-01-13 01:32:31.862903 zi_api_auth_client-2.0.0/zi_api_auth_client/
--rw-r--r--   0 harsh.singh   (503) staff       (20)      368 2023-01-13 01:30:29.000000 zi_api_auth_client-2.0.0/zi_api_auth_client/__init__.py
--rw-r--r--   0 harsh.singh   (503) staff       (20)     2364 2023-01-13 01:30:29.000000 zi_api_auth_client-2.0.0/zi_api_auth_client/zi_api_auth_client.py
-drwxr-xr-x   0 harsh.singh   (503) staff       (20)        0 2023-01-13 01:32:31.864820 zi_api_auth_client-2.0.0/zi_api_auth_client.egg-info/
--rw-r--r--   0 harsh.singh   (503) staff       (20)     2097 2023-01-13 01:32:31.000000 zi_api_auth_client-2.0.0/zi_api_auth_client.egg-info/PKG-INFO
--rw-r--r--   0 harsh.singh   (503) staff       (20)      311 2023-01-13 01:32:31.000000 zi_api_auth_client-2.0.0/zi_api_auth_client.egg-info/SOURCES.txt
--rw-r--r--   0 harsh.singh   (503) staff       (20)        1 2023-01-13 01:32:31.000000 zi_api_auth_client-2.0.0/zi_api_auth_client.egg-info/dependency_links.txt
--rw-r--r--   0 harsh.singh   (503) staff       (20)       51 2023-01-13 01:32:31.000000 zi_api_auth_client-2.0.0/zi_api_auth_client.egg-info/requires.txt
--rw-r--r--   0 harsh.singh   (503) staff       (20)       19 2023-01-13 01:32:31.000000 zi_api_auth_client-2.0.0/zi_api_auth_client.egg-info/top_level.txt
+drwxr-xr-x   0 harsh.singh   (503) staff       (20)        0 2023-08-07 17:40:00.515678 zi_api_auth_client-2.0.1/
+-rw-r--r--   0 harsh.singh   (503) staff       (20)     1077 2023-01-13 01:30:29.000000 zi_api_auth_client-2.0.1/LICENSE.txt
+-rw-r--r--   0 harsh.singh   (503) staff       (20)     2097 2023-08-07 17:40:00.515375 zi_api_auth_client-2.0.1/PKG-INFO
+-rw-r--r--   0 harsh.singh   (503) staff       (20)     1683 2023-01-13 01:30:29.000000 zi_api_auth_client-2.0.1/README.md
+-rw-r--r--   0 harsh.singh   (503) staff       (20)       38 2023-08-07 17:40:00.515767 zi_api_auth_client-2.0.1/setup.cfg
+-rw-r--r--   0 harsh.singh   (503) staff       (20)     1078 2023-08-07 17:35:03.000000 zi_api_auth_client-2.0.1/setup.py
+drwxr-xr-x   0 harsh.singh   (503) staff       (20)        0 2023-08-07 17:40:00.512985 zi_api_auth_client-2.0.1/zi_api_auth_client/
+-rw-r--r--   0 harsh.singh   (503) staff       (20)      368 2023-08-07 16:13:51.000000 zi_api_auth_client-2.0.1/zi_api_auth_client/__init__.py
+-rw-r--r--   0 harsh.singh   (503) staff       (20)     2364 2023-01-13 01:30:29.000000 zi_api_auth_client-2.0.1/zi_api_auth_client/zi_api_auth_client.py
+drwxr-xr-x   0 harsh.singh   (503) staff       (20)        0 2023-08-07 17:40:00.514979 zi_api_auth_client-2.0.1/zi_api_auth_client.egg-info/
+-rw-r--r--   0 harsh.singh   (503) staff       (20)     2097 2023-08-07 17:40:00.000000 zi_api_auth_client-2.0.1/zi_api_auth_client.egg-info/PKG-INFO
+-rw-r--r--   0 harsh.singh   (503) staff       (20)      311 2023-08-07 17:40:00.000000 zi_api_auth_client-2.0.1/zi_api_auth_client.egg-info/SOURCES.txt
+-rw-r--r--   0 harsh.singh   (503) staff       (20)        1 2023-08-07 17:40:00.000000 zi_api_auth_client-2.0.1/zi_api_auth_client.egg-info/dependency_links.txt
+-rw-r--r--   0 harsh.singh   (503) staff       (20)       51 2023-08-07 17:40:00.000000 zi_api_auth_client-2.0.1/zi_api_auth_client.egg-info/requires.txt
+-rw-r--r--   0 harsh.singh   (503) staff       (20)       19 2023-08-07 17:40:00.000000 zi_api_auth_client-2.0.1/zi_api_auth_client.egg-info/top_level.txt
```

### Comparing `zi_api_auth_client-2.0.0/LICENSE.txt` & `zi_api_auth_client-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zi_api_auth_client-2.0.0/PKG-INFO` & `zi_api_auth_client-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zi_api_auth_client
-Version: 2.0.0
+Version: 2.0.1
 Summary: A library that supports username-password and PKI authentication methods for enterprise-api
 Home-page: https://github.com/Zoominfo/api-auth-python-client
 Author: Krishna Teja Dinavahi
 Author-email: krishnateja.dinavahi@zoominfo.com
 License: MIT
 Keywords: ZoomInfo enterprise-api pki-auth
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zi_api_auth_client-2.0.0/README.md` & `zi_api_auth_client-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `zi_api_auth_client-2.0.0/setup.py` & `zi_api_auth_client-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 # reading long description from file
 with open('DESCRIPTION.txt') as file:
     long_description = file.read()
 
 # external packages requirements
-REQUIREMENTS = ['PyJWT==2.6.0', 'requests==2.28.1', 'cryptography==38.0.4']
+REQUIREMENTS = ['PyJWT==2.6.0', 'requests==2.28.1', 'cryptography==41.0.3']
 
 CLASSIFIERS = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 
 # calling the setup function
 setuptools.setup(name='zi_api_auth_client',
-                 version='2.0.0',
+                 version='2.0.1',
                  description='A library that supports username-password and PKI authentication methods for enterprise-api',
                  long_description=long_description,
                  url='https://github.com/Zoominfo/api-auth-python-client',
                  author='Krishna Teja Dinavahi',
                  author_email='krishnateja.dinavahi@zoominfo.com',
                  license='MIT',
                  classifiers=CLASSIFIERS,
```

### Comparing `zi_api_auth_client-2.0.0/zi_api_auth_client/zi_api_auth_client.py` & `zi_api_auth_client-2.0.1/zi_api_auth_client/zi_api_auth_client.py`

 * *Files identical despite different names*

### Comparing `zi_api_auth_client-2.0.0/zi_api_auth_client.egg-info/PKG-INFO` & `zi_api_auth_client-2.0.1/zi_api_auth_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zi-api-auth-client
-Version: 2.0.0
+Version: 2.0.1
 Summary: A library that supports username-password and PKI authentication methods for enterprise-api
 Home-page: https://github.com/Zoominfo/api-auth-python-client
 Author: Krishna Teja Dinavahi
 Author-email: krishnateja.dinavahi@zoominfo.com
 License: MIT
 Keywords: ZoomInfo enterprise-api pki-auth
 Classifier: License :: OSI Approved :: MIT License
```

