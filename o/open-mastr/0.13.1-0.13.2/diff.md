# Comparing `tmp/open_mastr-0.13.1.tar.gz` & `tmp/open_mastr-0.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_mastr-0.13.1.tar", last modified: Tue Apr 11 08:53:57 2023, max compression
+gzip compressed data, was "open_mastr-0.13.2.tar", last modified: Mon Aug  7 11:38:05 2023, max compression
```

## Comparing `open_mastr-0.13.1.tar` & `open_mastr-0.13.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.817996 open_mastr-0.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34521 2023-04-11 08:53:46.000000 open_mastr-0.13.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-04-11 08:53:57.817996 open_mastr-0.13.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-04-11 08:53:46.000000 open_mastr-0.13.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.813996 open_mastr-0.13.1/open_mastr/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/mastr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.813996 open_mastr-0.13.1/open_mastr/soap_api/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48271 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.813996 open_mastr-0.13.1/open_mastr/soap_api/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/metadata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15770 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/metadata/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/metadata/description.py
--rw-r--r--   0 runner    (1001) docker     (123)    41853 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.813996 open_mastr-0.13.1/open_mastr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.813996 open_mastr-0.13.1/open_mastr/utils/config/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/config/logging.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.817996 open_mastr-0.13.1/open_mastr/xml_download/
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/xml_download/colums_to_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/xml_download/utils_cleansing_bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/xml_download/utils_download_bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/xml_download/utils_write_to_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.813996 open_mastr-0.13.1/open_mastr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-04-11 08:53:57.000000 open_mastr-0.13.1/open_mastr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-11 08:53:57.000000 open_mastr-0.13.1/open_mastr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:53:57.000000 open_mastr-0.13.1/open_mastr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 08:53:57.000000 open_mastr-0.13.1/open_mastr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 08:53:57.000000 open_mastr-0.13.1/open_mastr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-11 08:53:57.817996 open_mastr-0.13.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-11 08:53:47.000000 open_mastr-0.13.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.817996 open_mastr-0.13.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-11 08:53:47.000000 open_mastr-0.13.1/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-04-11 08:53:47.000000 open_mastr-0.13.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-11 08:53:47.000000 open_mastr-0.13.1/tests/test_mastr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:38:05.409882 open_mastr-0.13.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34521 2023-08-07 11:37:53.000000 open_mastr-0.13.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-08-07 11:38:05.409882 open_mastr-0.13.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-08-07 11:37:53.000000 open_mastr-0.13.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:38:05.405882 open_mastr-0.13.2/open_mastr/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/mastr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:38:05.409882 open_mastr-0.13.2/open_mastr/soap_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/soap_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48271 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/soap_api/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:38:05.409882 open_mastr-0.13.2/open_mastr/soap_api/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/soap_api/metadata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/soap_api/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15770 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/soap_api/metadata/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/soap_api/metadata/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41853 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/soap_api/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/soap_api/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/soap_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:38:05.409882 open_mastr-0.13.2/open_mastr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:38:05.409882 open_mastr-0.13.2/open_mastr/utils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/utils/config/logging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/utils/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/utils/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/utils/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:38:05.409882 open_mastr-0.13.2/open_mastr/xml_download/
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/xml_download/colums_to_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/xml_download/utils_cleansing_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/xml_download/utils_download_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-08-07 11:37:53.000000 open_mastr-0.13.2/open_mastr/xml_download/utils_write_to_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:38:05.405882 open_mastr-0.13.2/open_mastr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-08-07 11:38:05.000000 open_mastr-0.13.2/open_mastr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-07 11:38:05.000000 open_mastr-0.13.2/open_mastr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:38:05.000000 open_mastr-0.13.2/open_mastr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-07 11:38:05.000000 open_mastr-0.13.2/open_mastr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 11:38:05.000000 open_mastr-0.13.2/open_mastr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-07 11:38:05.409882 open_mastr-0.13.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-08-07 11:37:53.000000 open_mastr-0.13.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:38:05.409882 open_mastr-0.13.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-07 11:37:53.000000 open_mastr-0.13.2/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-08-07 11:37:53.000000 open_mastr-0.13.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-07 11:37:53.000000 open_mastr-0.13.2/tests/test_mastr.py
```

### Comparing `open_mastr-0.13.1/LICENSE.md` & `open_mastr-0.13.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/PKG-INFO` & `open_mastr-0.13.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: open_mastr
-Version: 0.13.1
+Version: 0.13.2
 Summary: A package that provides an interface for downloading and processing the data of the Marktstammdatenregister (MaStR)
 Home-page: https://github.com/OpenEnergyPlatform/open-MaStR
-Download-URL: https://github.com/OpenEnergyPlatform/open-MaStR/archive/refs/tags/v0.13.1.tar.gz
+Download-URL: https://github.com/OpenEnergyPlatform/open-MaStR/archive/refs/tags/v0.13.2.tar.gz
 Author: Open Energy Family
 Author-email: datenzentrum@rl-institut.de
 Maintainer: Ludwig Hülk
 Maintainer-email: datenzentrum@rl-institut.de
 Project-URL: Documentation, https://open-mastr.readthedocs.io/
 Project-URL: Changelog, https://open-mastr.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/OpenEnergyPlatform/open-MaStR/issues
```

### Comparing `open_mastr-0.13.1/README.rst` & `open_mastr-0.13.2/README.rst`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/mastr.py` & `open_mastr-0.13.2/open_mastr/mastr.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/soap_api/download.py` & `open_mastr-0.13.2/open_mastr/soap_api/download.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/soap_api/metadata/LICENSE` & `open_mastr-0.13.2/open_mastr/soap_api/metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/soap_api/metadata/create.py` & `open_mastr-0.13.2/open_mastr/soap_api/metadata/create.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/soap_api/metadata/description.py` & `open_mastr-0.13.2/open_mastr/soap_api/metadata/description.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/soap_api/mirror.py` & `open_mastr-0.13.2/open_mastr/soap_api/mirror.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/soap_api/parallel.py` & `open_mastr-0.13.2/open_mastr/soap_api/parallel.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/soap_api/utils.py` & `open_mastr-0.13.2/open_mastr/soap_api/utils.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/utils/config.py` & `open_mastr-0.13.2/open_mastr/utils/config.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/utils/constants.py` & `open_mastr-0.13.2/open_mastr/utils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,16 @@
 # Map bulk data to bulk download tables (xml file names)
 BULK_INCLUDE_TABLES_MAP = {
     "wind": ["anlageneegwind", "einheitenwind"],
     "solar": ["anlageneegsolar", "einheitensolar"],
     "biomass": ["anlageneegbiomasse", "einheitenbiomasse"],
     "hydro": ["anlageneegwasser", "einheitenwasser"],
     "gsgk": [
-        "anlageneeggeosolarthermiegrubenklaerschlammdruckentspannung",
-        "einheitengeosolarthermiegrubenklaerschlammdruckentspannung",
+        "anlageneeggeothermiegrubengasdruckentspannung",
+        "einheitengeothermiegrubengasdruckentspannung",
     ],
     "combustion": ["anlagenkwk", "einheitenverbrennung"],
     "nuclear": ["einheitenkernkraft"],
     "storage": ["anlageneegspeicher", "anlagenstromspeicher", "einheitenstromspeicher"],
     "gas": [
         "anlagengasspeicher",
         "einheitengaserzeuger",
```

### Comparing `open_mastr-0.13.1/open_mastr/utils/credentials.py` & `open_mastr-0.13.2/open_mastr/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/utils/docs.py` & `open_mastr-0.13.2/open_mastr/utils/docs.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/utils/helpers.py` & `open_mastr-0.13.2/open_mastr/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/utils/orm.py` & `open_mastr-0.13.2/open_mastr/utils/orm.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/xml_download/colums_to_replace.py` & `open_mastr-0.13.2/open_mastr/xml_download/colums_to_replace.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/xml_download/utils_cleansing_bulk.py` & `open_mastr-0.13.2/open_mastr/xml_download/utils_cleansing_bulk.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr/xml_download/utils_download_bulk.py` & `open_mastr-0.13.2/open_mastr/xml_download/utils_download_bulk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import requests
-from tqdm import tqdm
-import time
-from bs4 import BeautifulSoup
-import numpy as np
 import os
 import shutil
-from zipfile import ZipFile, BadZipfile
+import time
+from zipfile import BadZipfile, ZipFile
+
+import numpy as np
+import requests
+from bs4 import BeautifulSoup
+from tqdm import tqdm
 
 # setup logger
 from open_mastr.utils.config import setup_logger
 
 log = setup_logger()
 
 
@@ -67,17 +68,17 @@
         "Warning: The servers from MaStR restrict the download speed."
         " You may want to download it another time."
     )
     print(print_message)
     url = get_url_from_Mastr_website()
     time_a = time.perf_counter()
     r = requests.get(url, stream=True)
-    total_length = int(10000 * 1024 * 1024)
+    total_length = int(18000 * 1024 * 1024)
     with open(save_path, "wb") as zfile, tqdm(
-        desc=save_path, total=(total_length / 1024 / 1024), unit="MB"
+        desc=save_path, total=(total_length / 1024 / 1024), unit=""
     ) as bar:
         for chunk in r.iter_content(chunk_size=1024 * 1024):
             # chunk size of 1024 * 1024 needs 9min 11 sek = 551sek
             # chunk size of 1024 needs 9min 11 sek as well
             if chunk:
                 zfile.write(chunk)
                 zfile.flush()
```

### Comparing `open_mastr-0.13.1/open_mastr/xml_download/utils_write_to_database.py` & `open_mastr-0.13.2/open_mastr/xml_download/utils_write_to_database.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/open_mastr.egg-info/PKG-INFO` & `open_mastr-0.13.2/open_mastr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: open-mastr
-Version: 0.13.1
+Version: 0.13.2
 Summary: A package that provides an interface for downloading and processing the data of the Marktstammdatenregister (MaStR)
 Home-page: https://github.com/OpenEnergyPlatform/open-MaStR
-Download-URL: https://github.com/OpenEnergyPlatform/open-MaStR/archive/refs/tags/v0.13.1.tar.gz
+Download-URL: https://github.com/OpenEnergyPlatform/open-MaStR/archive/refs/tags/v0.13.2.tar.gz
 Author: Open Energy Family
 Author-email: datenzentrum@rl-institut.de
 Maintainer: Ludwig Hülk
 Maintainer-email: datenzentrum@rl-institut.de
 Project-URL: Documentation, https://open-mastr.readthedocs.io/
 Project-URL: Changelog, https://open-mastr.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/OpenEnergyPlatform/open-MaStR/issues
```

### Comparing `open_mastr-0.13.1/open_mastr.egg-info/SOURCES.txt` & `open_mastr-0.13.2/open_mastr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.1/setup.py` & `open_mastr-0.13.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,22 @@
         "open_mastr",
         "open_mastr.soap_api",
         "open_mastr.soap_api.metadata",
         "open_mastr.utils",
         "open_mastr.utils.config",
         "open_mastr.xml_download",
     ],
-    version="0.13.1",
+    version="0.13.2",
     description="A package that provides an interface for downloading and"
     " processing the data of the Marktstammdatenregister (MaStR)",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/OpenEnergyPlatform/open-MaStR",
     download_url="https://github.com/OpenEnergyPlatform/open-MaStR/archive"
-    "/refs/tags/v0.13.1.tar.gz",
+    "/refs/tags/v0.13.2.tar.gz",
     author="Open Energy Family",
     author_email="datenzentrum@rl-institut.de",
     maintainer="Ludwig Hülk",
     maintainer_email="datenzentrum@rl-institut.de",
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `open_mastr-0.13.1/tests/test_helpers.py` & `open_mastr-0.13.2/tests/test_helpers.py`

 * *Files identical despite different names*

