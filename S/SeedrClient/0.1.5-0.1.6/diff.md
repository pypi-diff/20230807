# Comparing `tmp/SeedrClient-0.1.5.tar.gz` & `tmp/SeedrClient-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeedrClient-0.1.5.tar", last modified: Mon Aug  7 06:30:36 2023, max compression
+gzip compressed data, was "SeedrClient-0.1.6.tar", last modified: Mon Aug  7 06:56:58 2023, max compression
```

## Comparing `SeedrClient-0.1.5.tar` & `SeedrClient-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:30:36.117652 SeedrClient-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-07 06:30:36.121652 SeedrClient-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-07 06:30:24.000000 SeedrClient-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-07 06:30:36.121652 SeedrClient-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-07 06:30:24.000000 SeedrClient-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:30:36.117652 SeedrClient-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:30:36.117652 SeedrClient-0.1.5/src/SeedrClient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-07 06:30:36.000000 SeedrClient-0.1.5/src/SeedrClient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-07 06:30:36.000000 SeedrClient-0.1.5/src/SeedrClient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:30:36.000000 SeedrClient-0.1.5/src/SeedrClient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-07 06:30:36.000000 SeedrClient-0.1.5/src/SeedrClient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 06:30:36.000000 SeedrClient-0.1.5/src/SeedrClient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:30:36.117652 SeedrClient-0.1.5/src/seedr_client/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 06:30:24.000000 SeedrClient-0.1.5/src/seedr_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-07 06:30:24.000000 SeedrClient-0.1.5/src/seedr_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    22197 2023-08-07 06:30:24.000000 SeedrClient-0.1.5/src/seedr_client/seedr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:56:58.281485 SeedrClient-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-07 06:56:58.281485 SeedrClient-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-07 06:56:48.000000 SeedrClient-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-07 06:56:58.281485 SeedrClient-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-07 06:56:48.000000 SeedrClient-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:56:58.281485 SeedrClient-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:56:58.281485 SeedrClient-0.1.6/src/SeedrClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-07 06:56:58.000000 SeedrClient-0.1.6/src/SeedrClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-07 06:56:58.000000 SeedrClient-0.1.6/src/SeedrClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:56:58.000000 SeedrClient-0.1.6/src/SeedrClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-07 06:56:58.000000 SeedrClient-0.1.6/src/SeedrClient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 06:56:58.000000 SeedrClient-0.1.6/src/SeedrClient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:56:58.281485 SeedrClient-0.1.6/src/seedr_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 06:56:48.000000 SeedrClient-0.1.6/src/seedr_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-07 06:56:48.000000 SeedrClient-0.1.6/src/seedr_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22453 2023-08-07 06:56:48.000000 SeedrClient-0.1.6/src/seedr_client/seedr_handler.py
```

### Comparing `SeedrClient-0.1.5/PKG-INFO` & `SeedrClient-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeedrClient
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python library to interface with Seedr
 Home-page: https://github.com/Mr-Developer-X/seedr-client
 Author: Mr Developer X
 Author-email: 139059229+Mr-Developer-X@users.noreply.github.com
 Keywords: seedr,bittorrent,torrent,magnet,seedr api,seedbox
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `SeedrClient-0.1.5/README.md` & `SeedrClient-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `SeedrClient-0.1.5/setup.py` & `SeedrClient-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `SeedrClient-0.1.5/src/SeedrClient.egg-info/PKG-INFO` & `SeedrClient-0.1.6/src/SeedrClient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeedrClient
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python library to interface with Seedr
 Home-page: https://github.com/Mr-Developer-X/seedr-client
 Author: Mr Developer X
 Author-email: 139059229+Mr-Developer-X@users.noreply.github.com
 Keywords: seedr,bittorrent,torrent,magnet,seedr api,seedbox
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `SeedrClient-0.1.5/src/seedr_client/seedr_handler.py` & `SeedrClient-0.1.6/src/seedr_client/seedr_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,23 +350,27 @@
 
         response = requests.post(f"{self.base_oauth_url}/resource.php", data=data)
         response_json = json.loads(response.text)
         sleep(self.rate_limit)
         current_drive_content = self.get_drive()
         torrents_active = current_drive_content["torrents"]
         progress_url = None
-        for torrent in torrents_active:
-            if torrent["torrent_id"] == response_json["user_torrent_id"]:
-                progress_url = torrent["progress_url"]
         if response_json["result"]:
-            return {
-                "torrent_id": response_json["user_torrent_id"],
-                "file_name": response_json["title"],
-                "progress_url": progress_url,
-            }
+            for torrent in torrents_active:
+                if torrent["torrent_id"] == response_json["user_torrent_id"]:
+                    progress_url = torrent["progress_url"]
+            if progress_url is None:
+                for folder in current_drive_content["folders"]:
+                    if folder["folder_name"] == response_json["title"]:
+                        progress_url = "completed"
+                return {
+                    "torrent_id": response_json["user_torrent_id"],
+                    "file_name": response_json["title"],
+                    "progress_url": progress_url,
+                }
         else:
             raise BadLeeching(
                 f"The provided Torrent couldn't be leeched/downloaded to the drive.\n {data=}"
             )
 
     def download_folder(self, folder_id, builtin_downloader=True):
         content = self.get_folder(folder_id=folder_id)
```

