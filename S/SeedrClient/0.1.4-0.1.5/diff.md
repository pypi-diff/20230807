# Comparing `tmp/SeedrClient-0.1.4.tar.gz` & `tmp/SeedrClient-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeedrClient-0.1.4.tar", last modified: Tue Aug  1 06:35:18 2023, max compression
+gzip compressed data, was "SeedrClient-0.1.5.tar", last modified: Mon Aug  7 06:30:36 2023, max compression
```

## Comparing `SeedrClient-0.1.4.tar` & `SeedrClient-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:35:18.635229 SeedrClient-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-01 06:35:18.635229 SeedrClient-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-01 06:35:06.000000 SeedrClient-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-01 06:35:18.635229 SeedrClient-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-01 06:35:06.000000 SeedrClient-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:35:18.635229 SeedrClient-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:35:18.635229 SeedrClient-0.1.4/src/SeedrClient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-01 06:35:18.000000 SeedrClient-0.1.4/src/SeedrClient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-01 06:35:18.000000 SeedrClient-0.1.4/src/SeedrClient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:35:18.000000 SeedrClient-0.1.4/src/SeedrClient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 06:35:18.000000 SeedrClient-0.1.4/src/SeedrClient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 06:35:18.000000 SeedrClient-0.1.4/src/SeedrClient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:35:18.635229 SeedrClient-0.1.4/src/seedr_client/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-01 06:35:06.000000 SeedrClient-0.1.4/src/seedr_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-01 06:35:06.000000 SeedrClient-0.1.4/src/seedr_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-08-01 06:35:06.000000 SeedrClient-0.1.4/src/seedr_client/seedr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:30:36.117652 SeedrClient-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-07 06:30:36.121652 SeedrClient-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-07 06:30:24.000000 SeedrClient-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-07 06:30:36.121652 SeedrClient-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-07 06:30:24.000000 SeedrClient-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:30:36.117652 SeedrClient-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:30:36.117652 SeedrClient-0.1.5/src/SeedrClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-07 06:30:36.000000 SeedrClient-0.1.5/src/SeedrClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-07 06:30:36.000000 SeedrClient-0.1.5/src/SeedrClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:30:36.000000 SeedrClient-0.1.5/src/SeedrClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-07 06:30:36.000000 SeedrClient-0.1.5/src/SeedrClient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 06:30:36.000000 SeedrClient-0.1.5/src/SeedrClient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:30:36.117652 SeedrClient-0.1.5/src/seedr_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 06:30:24.000000 SeedrClient-0.1.5/src/seedr_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-07 06:30:24.000000 SeedrClient-0.1.5/src/seedr_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22197 2023-08-07 06:30:24.000000 SeedrClient-0.1.5/src/seedr_client/seedr_handler.py
```

### Comparing `SeedrClient-0.1.4/PKG-INFO` & `SeedrClient-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeedrClient
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python library to interface with Seedr
 Home-page: https://github.com/Mr-Developer-X/seedr-client
 Author: Mr Developer X
 Author-email: 139059229+Mr-Developer-X@users.noreply.github.com
 Keywords: seedr,bittorrent,torrent,magnet,seedr api,seedbox
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `SeedrClient-0.1.4/README.md` & `SeedrClient-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `SeedrClient-0.1.4/setup.py` & `SeedrClient-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `SeedrClient-0.1.4/src/SeedrClient.egg-info/PKG-INFO` & `SeedrClient-0.1.5/src/SeedrClient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeedrClient
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python library to interface with Seedr
 Home-page: https://github.com/Mr-Developer-X/seedr-client
 Author: Mr Developer X
 Author-email: 139059229+Mr-Developer-X@users.noreply.github.com
 Keywords: seedr,bittorrent,torrent,magnet,seedr api,seedbox
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `SeedrClient-0.1.4/src/seedr_client/seedr_handler.py` & `SeedrClient-0.1.5/src/seedr_client/seedr_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         :type wishlist_id: int
         :param folder_id: The folder you want the torrent to be downloaded to. Defaults to parent.
         :type folder_id: int
         :param check_size: Used to inform function if checking of Seedr drive space with torrent size is
             required or not. By default, it checks the torrent size with drive size and raise error if torrent
             size is larger than drive size.
         :type check_size: bool
-        :return: If successful returns the name and ID of the torrent.
+        :return: If successful returns the name, ID and progress url of  the torrent.
         :rtype: dict
         """
         if torrent:
             if check_size:
                 if self.torrent_regex.match(torrent):
                     pass
                 elif self.magnet_regex.match(torrent):
@@ -346,18 +346,26 @@
             "torrent_magnet": torrent_magnet_uri,
             "wishlist_id": wishlist_id,
             "folder_id": folder_id,
         }
 
         response = requests.post(f"{self.base_oauth_url}/resource.php", data=data)
         response_json = json.loads(response.text)
+        sleep(self.rate_limit)
+        current_drive_content = self.get_drive()
+        torrents_active = current_drive_content["torrents"]
+        progress_url = None
+        for torrent in torrents_active:
+            if torrent["torrent_id"] == response_json["user_torrent_id"]:
+                progress_url = torrent["progress_url"]
         if response_json["result"]:
             return {
                 "torrent_id": response_json["user_torrent_id"],
                 "file_name": response_json["title"],
+                "progress_url": progress_url,
             }
         else:
             raise BadLeeching(
                 f"The provided Torrent couldn't be leeched/downloaded to the drive.\n {data=}"
             )
 
     def download_folder(self, folder_id, builtin_downloader=True):
```

