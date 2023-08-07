# Comparing `tmp/pyCryptomusAPI-0.0.5.tar.gz` & `tmp/pyCryptomusAPI-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCryptomusAPI-0.0.5.tar", last modified: Tue Jul 25 20:08:48 2023, max compression
+gzip compressed data, was "pyCryptomusAPI-0.0.6.tar", last modified: Mon Aug  7 16:38:21 2023, max compression
```

## Comparing `pyCryptomusAPI-0.0.5.tar` & `pyCryptomusAPI-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 20:08:48.444679 pyCryptomusAPI-0.0.5/
--rw-rw-rw-   0        0        0     1085 2022-12-10 18:10:42.000000 pyCryptomusAPI-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2174 2023-07-25 20:08:48.443678 pyCryptomusAPI-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1672 2022-12-12 17:35:04.000000 pyCryptomusAPI-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 20:08:48.437700 pyCryptomusAPI-0.0.5/pyCryptomusAPI/
--rw-rw-rw-   0        0        0       20 2022-12-10 22:13:53.000000 pyCryptomusAPI-0.0.5/pyCryptomusAPI/__init__.py
--rw-rw-rw-   0        0        0    17647 2023-07-25 17:39:18.000000 pyCryptomusAPI-0.0.5/pyCryptomusAPI/api.py
--rw-rw-rw-   0        0        0     9897 2023-01-21 14:08:46.000000 pyCryptomusAPI-0.0.5/pyCryptomusAPI/cryto_types.py
--rw-rw-rw-   0        0        0      374 2023-02-14 14:49:00.000000 pyCryptomusAPI-0.0.5/pyCryptomusAPI/private_keys.py
--rw-rw-rw-   0        0        0     2314 2023-02-14 14:48:55.000000 pyCryptomusAPI-0.0.5/pyCryptomusAPI/tests.py
--rw-rw-rw-   0        0        0       95 2023-07-25 17:45:37.000000 pyCryptomusAPI-0.0.5/pyCryptomusAPI/version.py
-drwxrwxrwx   0        0        0        0 2023-07-25 20:08:48.442678 pyCryptomusAPI-0.0.5/pyCryptomusAPI.egg-info/
--rw-rw-rw-   0        0        0     2174 2023-07-25 20:08:48.000000 pyCryptomusAPI-0.0.5/pyCryptomusAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-07-25 20:08:48.000000 pyCryptomusAPI-0.0.5/pyCryptomusAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 20:08:48.000000 pyCryptomusAPI-0.0.5/pyCryptomusAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-25 20:08:48.000000 pyCryptomusAPI-0.0.5/pyCryptomusAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 20:08:48.445677 pyCryptomusAPI-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1053 2022-12-10 18:13:01.000000 pyCryptomusAPI-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:38:21.033697 pyCryptomusAPI-0.0.6/
+-rw-rw-rw-   0        0        0     1085 2022-12-10 18:10:42.000000 pyCryptomusAPI-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       40 2023-08-06 20:01:08.000000 pyCryptomusAPI-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2174 2023-08-07 16:38:21.033697 pyCryptomusAPI-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1672 2022-12-12 17:35:04.000000 pyCryptomusAPI-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 16:38:21.018087 pyCryptomusAPI-0.0.6/pyCryptomusAPI/
+-rw-rw-rw-   0        0        0       20 2022-12-10 22:13:53.000000 pyCryptomusAPI-0.0.6/pyCryptomusAPI/__init__.py
+-rw-rw-rw-   0        0        0    17647 2023-07-25 17:39:18.000000 pyCryptomusAPI-0.0.6/pyCryptomusAPI/api.py
+-rw-rw-rw-   0        0        0     9897 2023-01-21 14:08:46.000000 pyCryptomusAPI-0.0.6/pyCryptomusAPI/cryto_types.py
+-rw-rw-rw-   0        0        0     2314 2023-02-14 14:48:55.000000 pyCryptomusAPI-0.0.6/pyCryptomusAPI/tests.py
+-rw-rw-rw-   0        0        0       95 2023-08-06 20:15:09.000000 pyCryptomusAPI-0.0.6/pyCryptomusAPI/version.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:38:21.033697 pyCryptomusAPI-0.0.6/pyCryptomusAPI.egg-info/
+-rw-rw-rw-   0        0        0     2174 2023-08-07 16:38:20.000000 pyCryptomusAPI-0.0.6/pyCryptomusAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-08-07 16:38:20.000000 pyCryptomusAPI-0.0.6/pyCryptomusAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 16:38:20.000000 pyCryptomusAPI-0.0.6/pyCryptomusAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-08-07 16:38:20.000000 pyCryptomusAPI-0.0.6/pyCryptomusAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 16:38:21.033697 pyCryptomusAPI-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-08-07 16:33:36.000000 pyCryptomusAPI-0.0.6/setup.py
```

### Comparing `pyCryptomusAPI-0.0.5/LICENSE` & `pyCryptomusAPI-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.5/PKG-INFO` & `pyCryptomusAPI-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCryptomusAPI
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python implementation of Cryptomus (https://cryptomus.com) pubilc API
 Home-page: https://github.com/Badiboy/pyCryptomusAPI
 Author: Badiboy
 License: MIT license
 Keywords: Crypto Pay API Cryptomus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyCryptomusAPI-0.0.5/README.md` & `pyCryptomusAPI-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.5/pyCryptomusAPI/api.py` & `pyCryptomusAPI-0.0.6/pyCryptomusAPI/api.py`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.5/pyCryptomusAPI/cryto_types.py` & `pyCryptomusAPI-0.0.6/pyCryptomusAPI/cryto_types.py`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.5/pyCryptomusAPI/tests.py` & `pyCryptomusAPI-0.0.6/pyCryptomusAPI/tests.py`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.5/pyCryptomusAPI.egg-info/PKG-INFO` & `pyCryptomusAPI-0.0.6/pyCryptomusAPI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCryptomusAPI
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python implementation of Cryptomus (https://cryptomus.com) pubilc API
 Home-page: https://github.com/Badiboy/pyCryptomusAPI
 Author: Badiboy
 License: MIT license
 Keywords: Crypto Pay API Cryptomus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyCryptomusAPI-0.0.5/setup.py` & `pyCryptomusAPI-0.0.6/setup.py`

 * *Files identical despite different names*

