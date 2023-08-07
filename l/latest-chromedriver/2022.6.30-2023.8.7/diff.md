# Comparing `tmp/latest-chromedriver-2022.6.30.tar.gz` & `tmp/latest-chromedriver-2023.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latest-chromedriver-2022.6.30.tar", last modified: Thu Jun 30 08:41:49 2022, max compression
+gzip compressed data, was "latest-chromedriver-2023.8.7.tar", last modified: Mon Aug  7 09:03:00 2023, max compression
```

## Comparing `latest-chromedriver-2022.6.30.tar` & `latest-chromedriver-2023.8.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-06-30 08:41:49.827019 latest-chromedriver-2022.6.30/
--rw-rw-rw-   0        0        0     1096 2022-06-23 08:33:50.000000 latest-chromedriver-2022.6.30/LICENSE
--rw-rw-rw-   0        0        0     3374 2022-06-30 08:41:49.826021 latest-chromedriver-2022.6.30/PKG-INFO
--rw-rw-rw-   0        0        0     2558 2022-06-28 12:28:36.000000 latest-chromedriver-2022.6.30/README.md
-drwxrwxrwx   0        0        0        0 2022-06-30 08:41:49.770117 latest-chromedriver-2022.6.30/latest_chromedriver/
--rw-rw-rw-   0        0        0      236 2022-06-30 08:41:46.000000 latest-chromedriver-2022.6.30/latest_chromedriver/__init__.py
--rw-rw-rw-   0        0        0      256 2022-06-23 08:33:50.000000 latest-chromedriver-2022.6.30/latest_chromedriver/__main__.py
--rw-rw-rw-   0        0        0     3671 2022-06-27 07:06:09.000000 latest-chromedriver-2022.6.30/latest_chromedriver/chrome_info.py
--rw-rw-rw-   0        0        0     3568 2022-06-27 07:47:07.000000 latest-chromedriver-2022.6.30/latest_chromedriver/download_driver.py
--rw-rw-rw-   0        0        0     2339 2022-06-27 07:35:28.000000 latest-chromedriver-2022.6.30/latest_chromedriver/enviroment.py
--rw-rw-rw-   0        0        0      461 2022-06-24 06:08:12.000000 latest-chromedriver-2022.6.30/latest_chromedriver/version.py
-drwxrwxrwx   0        0        0        0 2022-06-30 08:41:49.822031 latest-chromedriver-2022.6.30/latest_chromedriver.egg-info/
--rw-rw-rw-   0        0        0     3374 2022-06-30 08:41:49.000000 latest-chromedriver-2022.6.30/latest_chromedriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2022-06-30 08:41:49.000000 latest-chromedriver-2022.6.30/latest_chromedriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-30 08:41:49.000000 latest-chromedriver-2022.6.30/latest_chromedriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2022-06-30 08:41:49.000000 latest-chromedriver-2022.6.30/latest_chromedriver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2022-06-30 08:41:49.000000 latest-chromedriver-2022.6.30/latest_chromedriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2022-06-30 08:41:49.000000 latest-chromedriver-2022.6.30/latest_chromedriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-30 08:41:49.827019 latest-chromedriver-2022.6.30/setup.cfg
--rw-rw-rw-   0        0        0     1860 2022-06-30 08:41:46.000000 latest-chromedriver-2022.6.30/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:03:00.853449 latest-chromedriver-2023.8.7/
+-rw-rw-rw-   0        0        0     1096 2022-06-23 08:33:50.000000 latest-chromedriver-2023.8.7/LICENSE
+-rw-rw-rw-   0        0        0     3373 2023-08-07 09:03:00.852486 latest-chromedriver-2023.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2558 2022-06-28 12:28:36.000000 latest-chromedriver-2023.8.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 09:03:00.827521 latest-chromedriver-2023.8.7/latest_chromedriver/
+-rw-rw-rw-   0        0        0      236 2023-08-07 09:02:57.000000 latest-chromedriver-2023.8.7/latest_chromedriver/__init__.py
+-rw-rw-rw-   0        0        0      256 2022-06-23 08:33:50.000000 latest-chromedriver-2023.8.7/latest_chromedriver/__main__.py
+-rw-rw-rw-   0        0        0     3671 2022-06-27 07:06:09.000000 latest-chromedriver-2023.8.7/latest_chromedriver/chrome_info.py
+-rw-rw-rw-   0        0        0     6523 2023-08-07 09:02:07.000000 latest-chromedriver-2023.8.7/latest_chromedriver/download_driver.py
+-rw-rw-rw-   0        0        0     2339 2022-06-27 07:35:28.000000 latest-chromedriver-2023.8.7/latest_chromedriver/enviroment.py
+-rw-rw-rw-   0        0        0      461 2022-06-24 06:08:12.000000 latest-chromedriver-2023.8.7/latest_chromedriver/version.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:03:00.846470 latest-chromedriver-2023.8.7/latest_chromedriver.egg-info/
+-rw-rw-rw-   0        0        0     3373 2023-08-07 09:03:00.000000 latest-chromedriver-2023.8.7/latest_chromedriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-08-07 09:03:00.000000 latest-chromedriver-2023.8.7/latest_chromedriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 09:03:00.000000 latest-chromedriver-2023.8.7/latest_chromedriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-08-07 09:03:00.000000 latest-chromedriver-2023.8.7/latest_chromedriver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-08-07 09:03:00.000000 latest-chromedriver-2023.8.7/latest_chromedriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-07 09:03:00.000000 latest-chromedriver-2023.8.7/latest_chromedriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 09:03:00.853449 latest-chromedriver-2023.8.7/setup.cfg
+-rw-rw-rw-   0        0        0     1860 2023-08-07 09:02:57.000000 latest-chromedriver-2023.8.7/setup.py
```

### Comparing `latest-chromedriver-2022.6.30/LICENSE` & `latest-chromedriver-2023.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `latest-chromedriver-2022.6.30/PKG-INFO` & `latest-chromedriver-2023.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latest-chromedriver
-Version: 2022.6.30
+Version: 2023.8.7
 Summary: A small package to find the correct chromedriver version in windows machines
 Home-page: https://github.com/hargikas/auto-chromedriver/
 Author: Charalampos Gkikas
 Author-email: hargikas@gmail.com
 License: MIT
 Project-URL: Say Thanks!, https://saythanks.io/to/hargikas
 Project-URL: Source, https://github.com/hargikas/auto-chromedriver/
```

### Comparing `latest-chromedriver-2022.6.30/README.md` & `latest-chromedriver-2023.8.7/README.md`

 * *Files identical despite different names*

### Comparing `latest-chromedriver-2022.6.30/latest_chromedriver/chrome_info.py` & `latest-chromedriver-2023.8.7/latest_chromedriver/chrome_info.py`

 * *Files identical despite different names*

### Comparing `latest-chromedriver-2022.6.30/latest_chromedriver/enviroment.py` & `latest-chromedriver-2023.8.7/latest_chromedriver/enviroment.py`

 * *Files identical despite different names*

### Comparing `latest-chromedriver-2022.6.30/latest_chromedriver.egg-info/PKG-INFO` & `latest-chromedriver-2023.8.7/latest_chromedriver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latest-chromedriver
-Version: 2022.6.30
+Version: 2023.8.7
 Summary: A small package to find the correct chromedriver version in windows machines
 Home-page: https://github.com/hargikas/auto-chromedriver/
 Author: Charalampos Gkikas
 Author-email: hargikas@gmail.com
 License: MIT
 Project-URL: Say Thanks!, https://saythanks.io/to/hargikas
 Project-URL: Source, https://github.com/hargikas/auto-chromedriver/
```

### Comparing `latest-chromedriver-2022.6.30/setup.py` & `latest-chromedriver-2023.8.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 import datetime
 
-__version__ = '2022.06.30'
+__version__ = '2023.08.07'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="latest-chromedriver",
     version=__version__,
```

