# Comparing `tmp/blob_mounting_helper_utility-1.0.9.tar.gz` & `tmp/blob_mounting_helper_utility-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blob_mounting_helper_utility-1.0.9.tar", last modified: Wed Aug  2 08:39:13 2023, max compression
+gzip compressed data, was "blob_mounting_helper_utility-1.1.0.tar", last modified: Mon Aug  7 09:38:37 2023, max compression
```

## Comparing `blob_mounting_helper_utility-1.0.9.tar` & `blob_mounting_helper_utility-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-02 08:39:13.560468 blob_mounting_helper_utility-1.0.9/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2559 2023-08-02 08:39:13.560468 blob_mounting_helper_utility-1.0.9/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2029 2023-06-15 13:30:00.000000 blob_mounting_helper_utility-1.0.9/README.md
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-02 08:39:13.560468 blob_mounting_helper_utility-1.0.9/blob_mounting_helper_utility/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       37 2023-06-15 11:11:15.000000 blob_mounting_helper_utility-1.0.9/blob_mounting_helper_utility/__init__.py
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     6766 2023-08-02 08:38:25.000000 blob_mounting_helper_utility-1.0.9/blob_mounting_helper_utility/utils.py
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-02 08:39:13.560468 blob_mounting_helper_utility-1.0.9/blob_mounting_helper_utility.egg-info/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     2559 2023-08-02 08:39:13.000000 blob_mounting_helper_utility-1.0.9/blob_mounting_helper_utility.egg-info/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      356 2023-08-02 08:39:13.000000 blob_mounting_helper_utility-1.0.9/blob_mounting_helper_utility.egg-info/SOURCES.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-08-02 08:39:13.000000 blob_mounting_helper_utility-1.0.9/blob_mounting_helper_utility.egg-info/dependency_links.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       28 2023-08-02 08:39:13.000000 blob_mounting_helper_utility-1.0.9/blob_mounting_helper_utility.egg-info/requires.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       29 2023-08-02 08:39:13.000000 blob_mounting_helper_utility-1.0.9/blob_mounting_helper_utility.egg-info/top_level.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-08-02 08:39:13.560468 blob_mounting_helper_utility-1.0.9/setup.cfg
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1055 2023-08-02 08:38:40.000000 blob_mounting_helper_utility-1.0.9/setup.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-07 09:38:37.093593 blob_mounting_helper_utility-1.1.0/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     3018 2023-08-07 09:38:37.093593 blob_mounting_helper_utility-1.1.0/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     2029 2023-06-15 13:30:00.000000 blob_mounting_helper_utility-1.1.0/README.md
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-07 09:38:37.089593 blob_mounting_helper_utility-1.1.0/blob_mounting_helper_utility/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       37 2023-06-15 11:11:15.000000 blob_mounting_helper_utility-1.1.0/blob_mounting_helper_utility/__init__.py
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     7828 2023-08-07 09:36:42.000000 blob_mounting_helper_utility-1.1.0/blob_mounting_helper_utility/utils.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-07 09:38:37.093593 blob_mounting_helper_utility-1.1.0/blob_mounting_helper_utility.egg-info/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     3018 2023-08-07 09:38:37.000000 blob_mounting_helper_utility-1.1.0/blob_mounting_helper_utility.egg-info/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      356 2023-08-07 09:38:37.000000 blob_mounting_helper_utility-1.1.0/blob_mounting_helper_utility.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-08-07 09:38:37.000000 blob_mounting_helper_utility-1.1.0/blob_mounting_helper_utility.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       28 2023-08-07 09:38:37.000000 blob_mounting_helper_utility-1.1.0/blob_mounting_helper_utility.egg-info/requires.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       29 2023-08-07 09:38:37.000000 blob_mounting_helper_utility-1.1.0/blob_mounting_helper_utility.egg-info/top_level.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-08-07 09:38:37.093593 blob_mounting_helper_utility-1.1.0/setup.cfg
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1055 2023-08-07 09:37:17.000000 blob_mounting_helper_utility-1.1.0/setup.py
```

### Comparing `blob_mounting_helper_utility-1.0.9/PKG-INFO` & `blob_mounting_helper_utility-1.1.0/blob_mounting_helper_utility.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 Metadata-Version: 2.1
-Name: blob_mounting_helper_utility
-Version: 1.0.9
+Name: blob-mounting-helper-utility
+Version: 1.1.0
 Summary: Blob mapping utility for easy translation between azure urls and local paths
 Home-page: UNKNOWN
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
 License: UNKNOWN
+Description: 
+        # Blob mapping utility
+        
+        When your code needs to access many mapped blobs as a mounted folder, the utility to make translation between blob urls and filepaths easier was made.
+        It can be configured using the configuration json file.
+        
+        Configuration file example:
+        
+        ``` json
+        {
+          "blob_mounting_configurations": [
+            {
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "heightstore-example1-raw",
+              "mount_point": "/mnt/heightstore-example1-raw"
+            },
+            {
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "heightstore-example2-raw",
+              "mount_point": "/mnt/heightstore-example2-raw"
+            },
+            {
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "heightstore-example3-raw",
+              "mount_point": "/mnt/heightstore-example3-raw"
+            },
+            {
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "example-container-raw",
+              "mount_point": "/mnt/example-container-raw"
+            }
+          ]
+        }
+        ```
+        
+        ## How to use
+        
+        ```python
+        from blob_mounting_helper_utility import BlobMappingUtility
+        json_config_file = "blob_mapping_config.json"
+        
+        # read the file into a dictionary
+        with open(json_config_file) as json_file:
+            config = json.load(json_file)["blob_mounting_configurations"]
+        
+        # create the utility object
+        blob_mapping_utility = BlobMappingUtility(config)
+        
+        filepath1 = "/mnt/example-container-raw/cool_picture.png
+        blob_url = blob_mapping_utility.get_url_from_mounted_filepath(filepath1) # -> https://examplestagingstrgacc.blob.core.windows.net/example-container-raw/cool_picture.png
+        
+        filepath2 = get_mounted_filepath_from_url(blob_url) # -> /mnt/example-container-raw/cool_picture.png
+        ```
 Keywords: python,azure,blob,mount
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
-
-
-# Blob mapping utility
-
-When your code needs to access many mapped blobs as a mounted folder, the utility to make translation between blob urls and filepaths easier was made.
-It can be configured using the configuration json file.
-
-Configuration file example:
-
-``` json
-{
-  "blob_mounting_configurations": [
-    {
-      "storage_account_name": "examplestagingstrgacc",
-      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-      "container_name": "heightstore-example1-raw",
-      "mount_point": "/mnt/heightstore-example1-raw"
-    },
-    {
-      "storage_account_name": "examplestagingstrgacc",
-      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-      "container_name": "heightstore-example2-raw",
-      "mount_point": "/mnt/heightstore-example2-raw"
-    },
-    {
-      "storage_account_name": "examplestagingstrgacc",
-      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-      "container_name": "heightstore-example3-raw",
-      "mount_point": "/mnt/heightstore-example3-raw"
-    },
-    {
-      "storage_account_name": "examplestagingstrgacc",
-      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-      "container_name": "example-container-raw",
-      "mount_point": "/mnt/example-container-raw"
-    }
-  ]
-}
-```
-
-## How to use
-
-```python
-from blob_mounting_helper_utility import BlobMappingUtility
-json_config_file = "blob_mapping_config.json"
-
-# read the file into a dictionary
-with open(json_config_file) as json_file:
-    config = json.load(json_file)["blob_mounting_configurations"]
-
-# create the utility object
-blob_mapping_utility = BlobMappingUtility(config)
-
-filepath1 = "/mnt/example-container-raw/cool_picture.png
-blob_url = blob_mapping_utility.get_url_from_mounted_filepath(filepath1) # -> https://examplestagingstrgacc.blob.core.windows.net/example-container-raw/cool_picture.png
-
-filepath2 = get_mounted_filepath_from_url(blob_url) # -> /mnt/example-container-raw/cool_picture.png
-```
-
```

### Comparing `blob_mounting_helper_utility-1.0.9/README.md` & `blob_mounting_helper_utility-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `blob_mounting_helper_utility-1.0.9/blob_mounting_helper_utility/utils.py` & `blob_mounting_helper_utility-1.1.0/blob_mounting_helper_utility/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os.path
 import logging
 logger = logging.getLogger(__name__)
 from typing import Tuple, List
 from urllib.parse import urlparse, urljoin
 from azure.storage.blob import BlobClient
-logging.getLogger('azure').setLevel(logging.WARNING)
+from azure.core.exceptions import ResourceModifiedError
+from time import sleep
+# logging.getLogger('azure').setLevel(logging.WARNING)
 
 
 class BlobMappingUtility:
     downloaded_paths = []
     uploaded_paths = []
 
     def __init__(self, blob_mounting_configurations_list: List, azure_storage_account_key: str = None):
@@ -90,51 +92,77 @@
                 url = urljoin(url + '/', subdirectory_path)
                 url = urljoin(url + '/', filename)
                 return url
 
         raise ValueError(f"Folder path {folder_path} is not a mounted folder")
 
     def download_blob(self, url: str) -> None:
+        if not self.azure_storage_account_key:
+            raise ValueError("azure_storage_account_key is required for downloading blobs")
+        
         logger.debug(f"Downloading blob from {url}")
         blob_client = BlobClient.from_blob_url(url, credential=self.azure_storage_account_key)
         download_file_path = self.get_mounted_filepath_from_url(url)
-        if not os.path.exists(download_file_path):
-            os.makedirs(os.path.dirname(download_file_path), exist_ok=True)
-            with open(download_file_path, "wb") as download_file:
-                download_file.write(blob_client.download_blob().readall())
-            logger.debug(f"Downloaded blob to {download_file_path}")
-            self.downloaded_paths.append(download_file_path)
-        else:
+        
+        if os.path.exists(download_file_path):
             logger.debug(f"Blob already downloaded to {download_file_path}")
+            return
+
+        # Attempt to fetch blob's properties multiple times.
+        for attempt in range(10):
+            try:
+                blob_client.get_blob_properties()
+                break  # If successful, break out of the loop
+            except ResourceModifiedError:
+                if attempt == 9:  # If it's the last attempt
+                    raise ResourceModifiedError
+                logger.warning(f"Failed to fetch blob properties for {url} on attempt {attempt + 1}. Retrying in 1 second.")
+                sleep(1)  # Wait for 1 second
+
+        os.makedirs(os.path.dirname(download_file_path), exist_ok=True)
+        
+        with open(download_file_path, "wb") as download_file:
+            download_file.write(blob_client.download_blob().readall())
+        
+        logger.debug(f"Downloaded blob to {download_file_path}")
+        self.downloaded_paths.append(download_file_path)
 
     def upload_blob(self, file_path: str) -> None:
+        if not self.azure_storage_account_key:
+            raise ValueError("azure_storage_account_key is required for uploading blobs")
         logger.debug(f"Uploading blob from {file_path}")
         blob_client = BlobClient.from_blob_url(self.get_url_from_mounted_filepath(file_path),
                                                credential=self.azure_storage_account_key)
         with open(file_path, "rb") as data:
             blob_client.upload_blob(data, overwrite=True)
         if file_path not in self.uploaded_paths:
             self.uploaded_paths.append(file_path)
         logger.debug(f"Uploaded blob from {file_path}")
 
     def cleanup_files(self) -> None:
         logger.debug("Cleaning up files")
         for file_path in self.downloaded_paths:
             logger.debug(f"Removing downloaded file {file_path}")
-            os.remove(file_path)
+            try:
+                os.remove(file_path)
+            except OSError:
+                pass
             # remove the directory if it is empty
             try:
                 os.rmdir(os.path.dirname(file_path))
                 if file_path in self.uploaded_paths:
                     self.uploaded_paths.remove(file_path)
             except OSError:
                 pass
         for file_path in self.uploaded_paths:
             logger.debug(f"Removing uploaded file {file_path}")
-            os.remove(file_path)
+            try:
+                os.remove(file_path)
+            except OSError:
+                pass
             # remove the directory if it is empty
             try:
                 os.rmdir(os.path.dirname(file_path))
             except OSError:
                 pass
         self.downloaded_paths = []
         self.uploaded_paths = []
```

### Comparing `blob_mounting_helper_utility-1.0.9/blob_mounting_helper_utility.egg-info/PKG-INFO` & `blob_mounting_helper_utility-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 Metadata-Version: 2.1
-Name: blob-mounting-helper-utility
-Version: 1.0.9
+Name: blob_mounting_helper_utility
+Version: 1.1.0
 Summary: Blob mapping utility for easy translation between azure urls and local paths
 Home-page: UNKNOWN
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
 License: UNKNOWN
+Description: 
+        # Blob mapping utility
+        
+        When your code needs to access many mapped blobs as a mounted folder, the utility to make translation between blob urls and filepaths easier was made.
+        It can be configured using the configuration json file.
+        
+        Configuration file example:
+        
+        ``` json
+        {
+          "blob_mounting_configurations": [
+            {
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "heightstore-example1-raw",
+              "mount_point": "/mnt/heightstore-example1-raw"
+            },
+            {
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "heightstore-example2-raw",
+              "mount_point": "/mnt/heightstore-example2-raw"
+            },
+            {
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "heightstore-example3-raw",
+              "mount_point": "/mnt/heightstore-example3-raw"
+            },
+            {
+              "storage_account_name": "examplestagingstrgacc",
+              "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
+              "container_name": "example-container-raw",
+              "mount_point": "/mnt/example-container-raw"
+            }
+          ]
+        }
+        ```
+        
+        ## How to use
+        
+        ```python
+        from blob_mounting_helper_utility import BlobMappingUtility
+        json_config_file = "blob_mapping_config.json"
+        
+        # read the file into a dictionary
+        with open(json_config_file) as json_file:
+            config = json.load(json_file)["blob_mounting_configurations"]
+        
+        # create the utility object
+        blob_mapping_utility = BlobMappingUtility(config)
+        
+        filepath1 = "/mnt/example-container-raw/cool_picture.png
+        blob_url = blob_mapping_utility.get_url_from_mounted_filepath(filepath1) # -> https://examplestagingstrgacc.blob.core.windows.net/example-container-raw/cool_picture.png
+        
+        filepath2 = get_mounted_filepath_from_url(blob_url) # -> /mnt/example-container-raw/cool_picture.png
+        ```
 Keywords: python,azure,blob,mount
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
-
-
-# Blob mapping utility
-
-When your code needs to access many mapped blobs as a mounted folder, the utility to make translation between blob urls and filepaths easier was made.
-It can be configured using the configuration json file.
-
-Configuration file example:
-
-``` json
-{
-  "blob_mounting_configurations": [
-    {
-      "storage_account_name": "examplestagingstrgacc",
-      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-      "container_name": "heightstore-example1-raw",
-      "mount_point": "/mnt/heightstore-example1-raw"
-    },
-    {
-      "storage_account_name": "examplestagingstrgacc",
-      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-      "container_name": "heightstore-example2-raw",
-      "mount_point": "/mnt/heightstore-example2-raw"
-    },
-    {
-      "storage_account_name": "examplestagingstrgacc",
-      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-      "container_name": "heightstore-example3-raw",
-      "mount_point": "/mnt/heightstore-example3-raw"
-    },
-    {
-      "storage_account_name": "examplestagingstrgacc",
-      "storage_account_url": "https://examplestagingstrgacc.blob.core.windows.net/",
-      "container_name": "example-container-raw",
-      "mount_point": "/mnt/example-container-raw"
-    }
-  ]
-}
-```
-
-## How to use
-
-```python
-from blob_mounting_helper_utility import BlobMappingUtility
-json_config_file = "blob_mapping_config.json"
-
-# read the file into a dictionary
-with open(json_config_file) as json_file:
-    config = json.load(json_file)["blob_mounting_configurations"]
-
-# create the utility object
-blob_mapping_utility = BlobMappingUtility(config)
-
-filepath1 = "/mnt/example-container-raw/cool_picture.png
-blob_url = blob_mapping_utility.get_url_from_mounted_filepath(filepath1) # -> https://examplestagingstrgacc.blob.core.windows.net/example-container-raw/cool_picture.png
-
-filepath2 = get_mounted_filepath_from_url(blob_url) # -> /mnt/example-container-raw/cool_picture.png
-```
-
```

### Comparing `blob_mounting_helper_utility-1.0.9/setup.py` & `blob_mounting_helper_utility-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.9'
+VERSION = '1.1.0'
 DESCRIPTION = 'Blob mapping utility for easy translation between azure urls and local paths'
 LONG_DESCRIPTION = 'Blob mapping utility for easy translation between azure urls and local paths'
 
 # Setting up
 setup(
     name="blob_mounting_helper_utility",
     version=VERSION,
```

