# Comparing `tmp/mikan_card_downloader-1.2.2.tar.gz` & `tmp/mikan_card_downloader-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikan_card_downloader-1.2.2.tar", max compression
+gzip compressed data, was "mikan_card_downloader-1.2.3.tar", max compression
```

## Comparing `mikan_card_downloader-1.2.2.tar` & `mikan_card_downloader-1.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-1.2.2/LICENSE
--rw-r--r--   0        0        0     1041 2023-08-07 16:01:48.568086 mikan_card_downloader-1.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.2.2/src/mikan/__init__.py
--rw-r--r--   0        0        0     1536 2023-05-05 22:20:27.438705 mikan_card_downloader-1.2.2/src/mikan/classes.py
--rw-r--r--   0        0        0     1491 2023-07-26 18:37:20.320555 mikan_card_downloader-1.2.2/src/mikan/config.py
--rw-r--r--   0        0        0     3378 2023-08-07 16:00:58.205929 mikan_card_downloader-1.2.2/src/mikan/downloader.py
--rw-r--r--   0        0        0     5622 2023-08-07 01:40:43.541854 mikan_card_downloader-1.2.2/src/mikan/html_parser.py
--rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-1.2.2/src/mikan/json_utils.py
--rwxr-xr-x   0        0        0     2402 2023-08-06 21:27:00.227335 mikan_card_downloader-1.2.2/src/mikan/main.py
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.2.2/src/mikan/py.typed
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-1.2.3/LICENSE
+-rw-r--r--   0        0        0     1041 2023-08-07 17:06:38.762140 mikan_card_downloader-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.2.3/src/mikan/__init__.py
+-rw-r--r--   0        0        0     1536 2023-05-05 22:20:27.438705 mikan_card_downloader-1.2.3/src/mikan/classes.py
+-rw-r--r--   0        0        0     1491 2023-07-26 18:37:20.320555 mikan_card_downloader-1.2.3/src/mikan/config.py
+-rw-r--r--   0        0        0     3398 2023-08-07 16:51:05.633941 mikan_card_downloader-1.2.3/src/mikan/downloader.py
+-rw-r--r--   0        0        0     5622 2023-08-07 01:40:43.541854 mikan_card_downloader-1.2.3/src/mikan/html_parser.py
+-rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-1.2.3/src/mikan/json_utils.py
+-rwxr-xr-x   0        0        0     2402 2023-08-06 21:27:00.227335 mikan_card_downloader-1.2.3/src/mikan/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.2.3/src/mikan/py.typed
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-1.2.3/PKG-INFO
```

### Comparing `mikan_card_downloader-1.2.2/LICENSE` & `mikan_card_downloader-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.2.2/pyproject.toml` & `mikan_card_downloader-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mikan-card-downloader"
-version = "1.2.2"
+version = "1.2.3"
 description = "Downloads cards and stills from SIFAS and SIF."
 authors = ["DemonicSavage"]
 license = "GPLv3"
 packages = [
     {include = "mikan", from = "src"}
 ]
```

### Comparing `mikan_card_downloader-1.2.2/src/mikan/classes.py` & `mikan_card_downloader-1.2.3/src/mikan/classes.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.2.2/src/mikan/config.py` & `mikan_card_downloader-1.2.3/src/mikan/config.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.2.2/src/mikan/downloader.py` & `mikan_card_downloader-1.2.3/src/mikan/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         self.config_path = config_path
 
         self.img_type = img_type
         self.objs[self.img_type.results_dir] = {}
 
         self.session = aiohttp.ClientSession(
-            connector=aiohttp.TCPConnector(limit=8),
+            connector=aiohttp.TCPConnector(limit=10, limit_per_host=10),
             timeout=aiohttp.ClientTimeout(total=None),
             cookies={"sessionid": cookie},
         )
 
         json_utils.load_cards(self.objs, self.config_path)
 
         self.parser = parser.Parser(self.objs, self.img_type, self.session)
```

### Comparing `mikan_card_downloader-1.2.2/src/mikan/html_parser.py` & `mikan_card_downloader-1.2.3/src/mikan/html_parser.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.2.2/src/mikan/json_utils.py` & `mikan_card_downloader-1.2.3/src/mikan/json_utils.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.2.2/src/mikan/main.py` & `mikan_card_downloader-1.2.3/src/mikan/main.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.2.2/PKG-INFO` & `mikan_card_downloader-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikan-card-downloader
-Version: 1.2.2
+Version: 1.2.3
 Summary: Downloads cards and stills from SIFAS and SIF.
 License: GPLv3
 Author: DemonicSavage
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

