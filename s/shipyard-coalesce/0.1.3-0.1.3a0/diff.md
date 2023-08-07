# Comparing `tmp/shipyard_coalesce-0.1.3.tar.gz` & `tmp/shipyard_coalesce-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_coalesce-0.1.3.tar", max compression
+gzip compressed data, was "shipyard_coalesce-0.1.3a0.tar", max compression
```

## Comparing `shipyard_coalesce-0.1.3.tar` & `shipyard_coalesce-0.1.3a0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1098 2023-05-12 18:48:21.826104 shipyard_coalesce-0.1.3/README.md
--rw-r--r--   0        0        0      556 2023-08-04 01:05:23.964944 shipyard_coalesce-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       36 2023-05-12 18:48:21.826398 shipyard_coalesce-0.1.3/shipyard_coalesce/__init__.py
--rw-r--r--   0        0        0      292 2023-07-28 00:25:41.245643 shipyard_coalesce-0.1.3/shipyard_coalesce/cli/authtest.py
--rw-r--r--   0        0        0     1212 2023-05-12 18:48:21.826571 shipyard_coalesce-0.1.3/shipyard_coalesce/cli/determine_status.py
--rw-r--r--   0        0        0     3824 2023-08-04 01:04:12.592273 shipyard_coalesce-0.1.3/shipyard_coalesce/cli/trigger_sync.py
--rw-r--r--   0        0        0     6422 2023-08-04 01:04:28.661613 shipyard_coalesce-0.1.3/shipyard_coalesce/coalesce.py
--rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 shipyard_coalesce-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-12 18:48:21.826104 shipyard_coalesce-0.1.3a0/README.md
+-rw-r--r--   0        0        0      559 2023-08-03 19:23:49.387830 shipyard_coalesce-0.1.3a0/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-05-12 18:48:21.826398 shipyard_coalesce-0.1.3a0/shipyard_coalesce/__init__.py
+-rw-r--r--   0        0        0      292 2023-07-28 00:25:41.245643 shipyard_coalesce-0.1.3a0/shipyard_coalesce/cli/authtest.py
+-rw-r--r--   0        0        0     1212 2023-05-12 18:48:21.826571 shipyard_coalesce-0.1.3a0/shipyard_coalesce/cli/determine_status.py
+-rw-r--r--   0        0        0     3761 2023-08-03 19:22:47.195084 shipyard_coalesce-0.1.3a0/shipyard_coalesce/cli/trigger_sync.py
+-rw-r--r--   0        0        0     6424 2023-08-03 19:24:04.784231 shipyard_coalesce-0.1.3a0/shipyard_coalesce/coalesce.py
+-rw-r--r--   0        0        0     1588 1970-01-01 00:00:00.000000 shipyard_coalesce-0.1.3a0/PKG-INFO
```

### Comparing `shipyard_coalesce-0.1.3/README.md` & `shipyard_coalesce-0.1.3a0/README.md`

 * *Files identical despite different names*

### Comparing `shipyard_coalesce-0.1.3/pyproject.toml` & `shipyard_coalesce-0.1.3a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-coalesce"
-version = "0.1.3"
+version = "0.1.3a0"
 description = "A local client for connecting and working with Coalesce"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shipyard_coalesce"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -14,8 +14,8 @@
 [tool.poetry.group.dev.dependencies]
 shipyard-templates = {path = "../../shipyard-templates"}
 shipyard-bp-utils = {path = "../shipyard-bp-utils"}
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `shipyard_coalesce-0.1.3/shipyard_coalesce/cli/determine_status.py` & `shipyard_coalesce-0.1.3a0/shipyard_coalesce/cli/determine_status.py`

 * *Files identical despite different names*

### Comparing `shipyard_coalesce-0.1.3/shipyard_coalesce/cli/trigger_sync.py` & `shipyard_coalesce-0.1.3a0/shipyard_coalesce/cli/trigger_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import sys
 import time
 import argparse
 import shipyard_bp_utils as shipyard
 from shipyard_coalesce import CoalesceClient
 
-
 def create_pickle_file(response):
     # create artifacts folder to save response
     base_folder_name = shipyard.logs.determine_base_artifact_folder("coalesce")
     artifact_subfolder_paths = shipyard.logs.determine_artifact_subfolders(
         base_folder_name
     )
     shipyard.logs.create_artifacts_folders(artifact_subfolder_paths)
     # save sync response as variable
     shipyard.logs.create_pickle_file(
         artifact_subfolder_paths, "coalesce_response", response
     )
 
-
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--access-token", dest="access_token", required=True)
     parser.add_argument("--environment-id", dest="environment_id", required=True)
     parser.add_argument("--job-id", dest="job_id", required=False, default=None)
     parser.add_argument(
         "--snowflake-username", dest="snowflake_username", required=True
@@ -36,16 +34,16 @@
     parser.add_argument("--parallelism", dest="parallelism", required=False, default=16)
     parser.add_argument(
         "--include-nodes-selector", dest="include_nodes", required=False, default=None
     )
     parser.add_argument(
         "--exclude-nodes-selector", dest="exclude_nodes", required=False, default=None
     )
-    parser.add_argument("--wait-for-completion", dest="wait_for_completion")
-    parser.add_argument("--poke-interval", dest="poke_interval")
+    parser.add_argument("--wait-for-completion",dest="wait_for_completion")
+    parser.add_argument("--poke-interval",dest="poke_interval")
 
     return parser.parse_args()
 
 
 def main():
     args = get_args()
     access_token = args.access_token
@@ -71,25 +69,25 @@
     if args.wait_for_completion == 'TRUE' and (0 < int(args.poke_interval) <= 60):
         run_id = response["runCounter"]
         status = client.determine_sync_status(run_id)
 
         while status not in (client.EXIT_CODE_FINAL_STATUS_COMPLETED,
                              client.EXIT_CODE_FINAL_STATUS_INCOMPLETE,
                              client.EXIT_CODE_FINAL_STATUS_CANCELLED,
-                             client.EXIT_CODE_FINAL_STATUS_ERRORED,
+            client.E
                              ):
             client.logger.info(f"Waiting {args.poke_interval} minute(s)...")
             time.sleep(int(args.poke_interval) * 60)
             status = client.determine_sync_status(run_id)
 
         sys.exit(status)
     elif args.wait_for_completion == 'TRUE':
         client.logger.error(
             "Poke interval must be between 1 and 60 minutes")
         sys.exit(client.EXIT_CODE_SYNC_INVALID_POKE_INTERVAL)
     else:
-        create_pickle_file(
-            response)  # Backwards Compatibility: Ensures this code works with older versions of Check Sync Blueprint.
+        create_pickle_file(response) # Backwards Compatibility: Ensures this code works with older versions of Check Sync Blueprint.
+
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `shipyard_coalesce-0.1.3/shipyard_coalesce/coalesce.py` & `shipyard_coalesce-0.1.3a0/shipyard_coalesce/coalesce.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         response = self.get_run_status(run_counter)
         json = response.json()
         if response.status_code == 200:
             status = json.get("runStatus")
             # go through the statuses and return the appropriate exit code
             # documentation does not provide options for status aside from completed
             if status == "completed":
-                self.logger.info("Status: completed")
+                self.logger.info(f"Status: completed")
                 return self.EXIT_CODE_FINAL_STATUS_COMPLETED
             elif status == "pending":
                 self.logger.info("Status: pending")
                 return self.EXIT_CODE_FINAL_STATUS_PENDING
             elif status == "running":
                 self.logger.info("Status: running")
                 return self.EXIT_CODE_SYNC_ALREADY_RUNNING
@@ -137,15 +137,15 @@
         elif response.status_code == 401:
             self.logger.error(
                 "Error occurred when attempting to authenticate, please ensure that the token provided is valid"
             )
             return self.EXIT_CODE_INVALID_CREDENTIALS
 
     def connect(self):
-        """
+        """ 
         Connects to the Coalesce API and returns the response
         """
         url = "https://app.coalescesoftware.io/scheduler/runStatus?runCounter=1"
         headers = {
             "accept": "application/json",
             "Authorization": f"Bearer {self.access_token}",
         }
```

### Comparing `shipyard_coalesce-0.1.3/PKG-INFO` & `shipyard_coalesce-0.1.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-coalesce
-Version: 0.1.3
+Version: 0.1.3a0
 Summary: A local client for connecting and working with Coalesce
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

