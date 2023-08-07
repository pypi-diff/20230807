# Comparing `tmp/ayt-api-0.1.3.tar.gz` & `tmp/ayt-api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayt-api-0.1.3.tar", last modified: Tue Jul 18 12:11:49 2023, max compression
+gzip compressed data, was "ayt-api-0.1.4.tar", last modified: Thu Jul 20 12:15:47 2023, max compression
```

## Comparing `ayt-api-0.1.3.tar` & `ayt-api-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:11:49.409800 ayt-api-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-18 12:11:36.000000 ayt-api-0.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-18 12:11:49.409800 ayt-api-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-18 12:11:36.000000 ayt-api-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:11:49.409800 ayt-api-0.1.3/ayt_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-18 12:11:36.000000 ayt-api-0.1.3/ayt_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-18 12:11:36.000000 ayt-api-0.1.3/ayt_api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-18 12:11:36.000000 ayt-api-0.1.3/ayt_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    52925 2023-07-18 12:11:36.000000 ayt-api-0.1.3/ayt_api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-18 12:11:36.000000 ayt-api-0.1.3/ayt_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:11:49.409800 ayt-api-0.1.3/ayt_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-18 12:11:49.000000 ayt-api-0.1.3/ayt_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-18 12:11:49.000000 ayt-api-0.1.3/ayt_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:11:49.000000 ayt-api-0.1.3/ayt_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 12:11:49.000000 ayt-api-0.1.3/ayt_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 12:11:49.000000 ayt-api-0.1.3/ayt_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-18 12:11:36.000000 ayt-api-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 12:11:36.000000 ayt-api-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-18 12:11:49.409800 ayt-api-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-18 12:11:36.000000 ayt-api-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:15:47.065321 ayt-api-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-20 12:15:31.000000 ayt-api-0.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-20 12:15:47.065321 ayt-api-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-20 12:15:31.000000 ayt-api-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:15:47.065321 ayt-api-0.1.4/ayt_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-20 12:15:31.000000 ayt-api-0.1.4/ayt_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-20 12:15:31.000000 ayt-api-0.1.4/ayt_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-20 12:15:31.000000 ayt-api-0.1.4/ayt_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52925 2023-07-20 12:15:31.000000 ayt-api-0.1.4/ayt_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-20 12:15:31.000000 ayt-api-0.1.4/ayt_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:15:47.065321 ayt-api-0.1.4/ayt_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-20 12:15:47.000000 ayt-api-0.1.4/ayt_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 12:15:47.000000 ayt-api-0.1.4/ayt_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:15:47.000000 ayt-api-0.1.4/ayt_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 12:15:47.000000 ayt-api-0.1.4/ayt_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 12:15:47.000000 ayt-api-0.1.4/ayt_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-20 12:15:31.000000 ayt-api-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-20 12:15:31.000000 ayt-api-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-20 12:15:47.065321 ayt-api-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-20 12:15:31.000000 ayt-api-0.1.4/setup.py
```

### Comparing `ayt-api-0.1.3/LICENSE.md` & `ayt-api-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ayt-api-0.1.3/PKG-INFO` & `ayt-api-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayt-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: An Asynchronous, Object oriented python library for the YouTube api
 Home-page: https://github.com/Revnoplex/ayt-api
 Author: Revnoplex
 Author-email: Revnoplex <revnoplex.business@protonmail.com>
 License: # MIT License
         
         Copyright (c) 2022-2023 Revnoplex
```

### Comparing `ayt-api-0.1.3/README.md` & `ayt-api-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ayt-api-0.1.3/ayt_api/__init__.py` & `ayt-api-0.1.4/ayt_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .exceptions import *
 from . import utils
 
 __title__ = "ayt-api"
 __author__ = "Revnoplex"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2022-2023 Revnoplex"
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 
 class VersionInfo(_NamedTuple):
     major: int
     minor: int
     micro: int
     release_level: str
```

### Comparing `ayt-api-0.1.3/ayt_api/api.py` & `ayt-api-0.1.4/ayt_api/api.py`

 * *Files identical despite different names*

### Comparing `ayt-api-0.1.3/ayt_api/exceptions.py` & `ayt-api-0.1.4/ayt_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ayt-api-0.1.3/ayt_api/types.py` & `ayt-api-0.1.4/ayt_api/types.py`

 * *Files identical despite different names*

### Comparing `ayt-api-0.1.3/ayt_api/utils.py` & `ayt-api-0.1.4/ayt_api/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 import pathlib
+from typing import Optional
 from urllib import parse
 
 
-def extract_video_id(url: str) -> str:
+def extract_video_id(url: str) -> Optional[str]:
     """
     This should work for every url listed here:
     https://gist.github.com/rodrigoborgesdeoliveira/987683cfbfcc8d800192da1e73adc486#file-activeyoutubeurlformats-txt
     and more.
     Args:
         url (str): The url to strip the id from
     Returns:
-        str: The video id with the rest of the url removed
+        Optional[str]: The video id with the rest of the url removed
     """
     components = parse.urlparse(url.replace("&", "?", 1) if "?" not in url else url)
     queries = parse.parse_qs(components.query)
     encoded_query_matches = {'u', 'url'}.intersection(set(queries.keys()))
     if 'v' in queries:
         return queries["v"][0]
     elif encoded_query_matches:
         return extract_video_id(parse.unquote(queries[encoded_query_matches.pop()][0]))
     elif components.netloc == "i.ytimg.com":
         return pathlib.Path(components.path).parts[2]
-    else:
+    elif pathlib.Path(components.path).name not in ["playlist"]:
         return pathlib.Path(components.path).name
 
 
-def extract_playlist_id(url: str) -> str:
+def extract_playlist_id(url: str) -> Optional[str]:
     """
     This should work with the following urls
 
     Don't expect this to work on YouTube mixes
     Args:
         url (str): The url to strip the id from
     Returns:
-        str: The playlist id with the rest of the url removed
+        Optional[str]: The playlist id with the rest of the url removed
     """
     components = parse.urlparse(url.replace("&", "?", 1) if "?" not in url else url)
     queries = parse.parse_qs(components.query)
     encoded_query_matches = {'u', 'url'}.intersection(set(queries.keys()))
     if 'list' in queries:
         return queries["list"][0]
     elif encoded_query_matches:
         return extract_playlist_id(parse.unquote(queries[encoded_query_matches.pop()][0]))
-    else:
-        return pathlib.Path(components.path).name
```

### Comparing `ayt-api-0.1.3/ayt_api.egg-info/PKG-INFO` & `ayt-api-0.1.4/ayt_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayt-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: An Asynchronous, Object oriented python library for the YouTube api
 Home-page: https://github.com/Revnoplex/ayt-api
 Author: Revnoplex
 Author-email: Revnoplex <revnoplex.business@protonmail.com>
 License: # MIT License
         
         Copyright (c) 2022-2023 Revnoplex
```

### Comparing `ayt-api-0.1.3/pyproject.toml` & `ayt-api-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ayt-api-0.1.3/setup.py` & `ayt-api-0.1.4/setup.py`

 * *Files identical despite different names*

