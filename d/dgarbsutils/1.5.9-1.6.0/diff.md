# Comparing `tmp/dgarbsutils-1.5.9.tar.gz` & `tmp/dgarbsutils-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgarbsutils-1.5.9.tar", last modified: Tue Feb 21 14:54:33 2023, max compression
+gzip compressed data, was "dgarbsutils-1.6.0.tar", last modified: Mon Aug  7 12:30:46 2023, max compression
```

## Comparing `dgarbsutils-1.5.9.tar` & `dgarbsutils-1.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-21 14:54:33.810099 dgarbsutils-1.5.9/
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1072 2022-06-10 11:14:25.000000 dgarbsutils-1.5.9/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      913 2023-02-21 14:54:33.810099 dgarbsutils-1.5.9/PKG-INFO
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      419 2022-06-14 21:50:35.000000 dgarbsutils-1.5.9/README.md
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)       84 2022-06-13 13:28:13.000000 dgarbsutils-1.5.9/pyproject.toml
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      693 2023-02-21 14:54:33.814099 dgarbsutils-1.5.9/setup.cfg
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-21 14:54:33.806100 dgarbsutils-1.5.9/src/
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-21 14:54:33.810099 dgarbsutils-1.5.9/src/dgarbsutils/
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     2312 2022-08-10 12:24:46.000000 dgarbsutils-1.5.9/src/dgarbsutils/Cloudwatch.py
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5610 2023-02-21 14:53:27.000000 dgarbsutils-1.5.9/src/dgarbsutils/DynamoDB.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2069 2022-12-05 15:01:17.000000 dgarbsutils-1.5.9/src/dgarbsutils/EventBridge.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5153 2023-02-07 14:19:45.000000 dgarbsutils-1.5.9/src/dgarbsutils/GraphMail.py
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-06-13 13:28:13.000000 dgarbsutils-1.5.9/src/dgarbsutils/__init__.py
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5991 2023-01-17 18:38:11.000000 dgarbsutils-1.5.9/src/dgarbsutils/awsUtils.py
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5839 2023-01-20 20:04:01.000000 dgarbsutils-1.5.9/src/dgarbsutils/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-21 14:54:33.810099 dgarbsutils-1.5.9/src/dgarbsutils.egg-info/
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      913 2023-02-21 14:54:33.000000 dgarbsutils-1.5.9/src/dgarbsutils.egg-info/PKG-INFO
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      455 2023-02-21 14:54:33.000000 dgarbsutils-1.5.9/src/dgarbsutils.egg-info/SOURCES.txt
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        1 2023-02-21 14:54:33.000000 dgarbsutils-1.5.9/src/dgarbsutils.egg-info/dependency_links.txt
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)       31 2023-02-21 14:54:33.000000 dgarbsutils-1.5.9/src/dgarbsutils.egg-info/requires.txt
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)       12 2023-02-21 14:54:33.000000 dgarbsutils-1.5.9/src/dgarbsutils.egg-info/top_level.txt
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-02-21 14:54:33.810099 dgarbsutils-1.5.9/tests/
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1782 2022-07-16 22:59:17.000000 dgarbsutils-1.5.9/tests/test_utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:30:46.684533 dgarbsutils-1.6.0/
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1072 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      913 2023-08-07 12:30:46.688533 dgarbsutils-1.6.0/PKG-INFO
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      419 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/README.md
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)       84 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/pyproject.toml
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      693 2023-08-07 12:30:46.688533 dgarbsutils-1.6.0/setup.cfg
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:30:46.684533 dgarbsutils-1.6.0/src/
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:30:46.684533 dgarbsutils-1.6.0/src/dgarbsutils/
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     2311 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/src/dgarbsutils/Cloudwatch.py
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5604 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/src/dgarbsutils/DynamoDB.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2069 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/src/dgarbsutils/EventBridge.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6879 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/src/dgarbsutils/GraphMail.py
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/src/dgarbsutils/__init__.py
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     7118 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/src/dgarbsutils/awsUtils.py
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5839 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/src/dgarbsutils/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:30:46.684533 dgarbsutils-1.6.0/src/dgarbsutils.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      913 2023-08-07 12:30:46.000000 dgarbsutils-1.6.0/src/dgarbsutils.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      455 2023-08-07 12:30:46.000000 dgarbsutils-1.6.0/src/dgarbsutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-08-07 12:30:46.000000 dgarbsutils-1.6.0/src/dgarbsutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       31 2023-08-07 12:30:46.000000 dgarbsutils-1.6.0/src/dgarbsutils.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       12 2023-08-07 12:30:46.000000 dgarbsutils-1.6.0/src/dgarbsutils.egg-info/top_level.txt
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:30:46.684533 dgarbsutils-1.6.0/tests/
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1782 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/tests/test_utils.py
```

### Comparing `dgarbsutils-1.5.9/LICENSE` & `dgarbsutils-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.5.9/PKG-INFO` & `dgarbsutils-1.6.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: dgarbsutils
-Version: 1.5.9
+Version: 1.6.0
 Summary: A set of curated utils
 Home-page: https://github.com/dgarbalo/py-utils
 Author: Devon Garbalosa
 Author-email: dgarbalo@gmail.com
 Project-URL: Bug Tracker, https://github.com/dgarbalo/py-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Utils
 
 ## Description
```

### Comparing `dgarbsutils-1.5.9/setup.cfg` & `dgarbsutils-1.6.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dgarbsutils
-version = 1.5.9
+version = 1.6.0
 author = Devon Garbalosa
 author_email = dgarbalo@gmail.com
 description = A set of curated utils
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/dgarbalo/py-utils
 project_urls = 
@@ -16,15 +16,15 @@
 testpaths = 
 	tests
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.7
 install_requires = 
 	boto3
 	botocore
 	psycopg2-binary
 
 [options.packages.find]
 where = src
```

### Comparing `dgarbsutils-1.5.9/src/dgarbsutils/Cloudwatch.py` & `dgarbsutils-1.6.0/src/dgarbsutils/Cloudwatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # declare the logging object
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 
 
 class Cloudwatch:
     def __init__(self, log_group, profile=None, region="us-east-1"):
-
         self._region = region
         if profile:
             self._session = boto3.session.Session(profile_name=profile, region_name=self._region)
         else:
             self._session = boto3.session.Session(region_name=self._region)
         self._client = self._session.client("logs")
         self._log_group = log_group
```

### Comparing `dgarbsutils-1.5.9/src/dgarbsutils/DynamoDB.py` & `dgarbsutils-1.6.0/src/dgarbsutils/DynamoDB.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         if data_type in ["<class 'int'>", "<class 'float'>", "<class 'complex'>"]:
             return {"N": str(data)}
         if data_type == "<class 'list'>":
             return {"L": [self.dynamodb_translate_data_type(item) for item in data]}
         if data_type == "<class 'dict'>":
             return {"M": {key: self.dynamodb_translate_data_type(value) for key, value in data.items()}}
         if data_type == "<class 'bool'>":
-            return {"BOOL": str(data)}
+            return {"BOOL": data}
         if data_type == "<class 'NoneType'>":
             return {"NULL": True}
         return None
 
     def dynamodb_convert_to_json(self, data):
         """converts the dynamodb json to a python json"""
         output = {}
@@ -121,15 +121,14 @@
         for row in data:
             if row[pk_name]["S"] == pk_value:
                 output.append({"M": row})
 
         return output
 
     def dynamodb_update_item(self, key_fields, update_fields, start_key=None):
-
         Key = self.dynamodb_format_json(key_fields)
         Names = {}
         if start_key:
             rand_start = utils.randStr()
             Names[f"#{rand_start}"] = start_key
         Values = {}
         Expression = "SET "
```

### Comparing `dgarbsutils-1.5.9/src/dgarbsutils/EventBridge.py` & `dgarbsutils-1.6.0/src/dgarbsutils/EventBridge.py`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.5.9/src/dgarbsutils/GraphMail.py` & `dgarbsutils-1.6.0/src/dgarbsutils/GraphMail.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import urllib3
 
 urllib3.disable_warnings()
 
 
 class GraphMail:
     def __init__(self, tenant=None, client_id=None, secret=None, base_url=None, **kwargs):
-
         self.tenantID = tenant if tenant else os.getenv("AZURE_TENANT_ID")
         self.clientID = client_id if client_id else os.getenv("AZURE_EMAIL_CLIENT_ID")
         self.clientSecret = secret if secret else os.getenv("AZURE_EMAIL_CLIENT_SECRET")
         self._baseUrl = base_url if base_url else os.getenv("AZURE_BASE_URL")
 
         oAuth = self.oAuth()
         if "error" not in oAuth.keys():
@@ -60,22 +59,25 @@
             url = f"{self._baseUrl}/v1.0/users/{_emailBox}/mailFolders/{_folderId}/messages/{_email_id}/attachments"
 
         request = requests.request("get", url, headers=headers, params=params, verify=False)
         response = request.json()
 
         return response
 
-    def getMailBySearch(self, _search, _emailBox, _folder=None, _select=None):
+    def getMailBySearch(self, _search, _emailBox, _folder=None, _select=None, _filter=None):
         url = f"{self._baseUrl}/v1.0/users/{_emailBox}/messages"
         headers = {"Authorization": f"Bearer {self.accessToken}"}
         params = {}
         _folderId = None
         if _search:
             params["$search"] = _search
 
+        if _filter:
+            params["$filter"] = _filter
+
         if _select:
             params["$select"] = _select
 
         if _folder:
             data = self.getMailFolders(_emailBox)
 
             for folders in data["value"]:
@@ -89,14 +91,22 @@
             url = f"{self._baseUrl}/v1.0/users/{_emailBox}/mailFolders/{_folderId}/messages"
 
         request = requests.request("get", url, headers=headers, params=params, verify=False)
         response = request.json()
 
         return response
 
+    def getMailBySearchNext(self, nextLink):
+        headers = {"Authorization": f"Bearer {self.accessToken}"}
+        params = {}
+        request = requests.request("get", nextLink, headers=headers, params=params, verify=False)
+        response = request.json()
+
+        return response
+
     def getMailBySearchRaw(self, _emailBox, _id=""):
         url = f"{self._baseUrl}/v1.0/users/{_emailBox}/messages/{_id}/$value"
         headers = {"Authorization": f"Bearer {self.accessToken}"}
         params = {}
         request = requests.request("get", url, headers=headers, params=params, verify=False)
         response = request.content
         return response
@@ -112,23 +122,50 @@
         url = f"{self._baseUrl}/v1.0/users/{_emailBox}/mailFolders"
         headers = {"Authorization": f"Bearer {self.accessToken}"}
         params = {"includeHiddenFolders": True}
         request = requests.request("get", url, headers=headers, params=params, verify=False)
         response = request.json()
         return response
 
+    def getMailChildFolders(self, _emailBox, _folderId):
+        url = f"{self._baseUrl}/v1.0/users/{_emailBox}/mailFolders/{_folderId}/childFolders"
+        headers = {"Authorization": f"Bearer {self.accessToken}"}
+        params = {"includeHiddenFolders": True}
+        request = requests.request("get", url, headers=headers, params=params, verify=False)
+        response = request.json()
+        return response
+
     def postMoveEmails(self, _emailBox, _id, _destFolder):
         _folderId = None
         data = self.getMailFolders(_emailBox)
 
+        _destFolderArray = _destFolder.split("/")
         for folders in data["value"]:
-            if folders["displayName"] == _destFolder:
+            if folders["displayName"] == _destFolderArray[0]:
                 _folderId = folders["id"]
-                break
 
+        if len(_destFolderArray) > 1:
+            for i in range(1, len(_destFolderArray)):
+                # Get a list of emails that match the search criteria
+                folders = []
+                done = False
+                response = self.getMailChildFolders(_emailBox, _folderId)
+                while not done:
+                    for folder in response["value"]:
+                        folders.append(folder)
+                    if "@odata.nextLink" in response.keys():
+                        response = self.getMailBySearchNext(response["@odata.nextLink"])
+                    else:
+                        done = True
+                        break
+                    done = False
+                for folder in folders:
+                    if folder["displayName"] == _destFolderArray[i]:
+                        print(folder["displayName"])
+                        _folderId = folder["id"]
         if not _folderId:
             return {"statusCode": 404, "message": "Folder not found"}
 
         url = f"{self._baseUrl}/v1.0/users/{_emailBox}/messages/{_id}/move"
         headers = {"Content-Type": "application/json", "Authorization": f"Bearer {self.accessToken}"}
         payload = json.dumps({"destinationId": _folderId})
         request = requests.request("post", url, headers=headers, data=payload, verify=False)
```

### Comparing `dgarbsutils-1.5.9/src/dgarbsutils/awsUtils.py` & `dgarbsutils-1.6.0/src/dgarbsutils/awsUtils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
 import tempfile
+from datetime import datetime, timedelta
 from urllib.parse import unquote_plus
 
 import boto3
 import botocore
 
 from . import utils
 
@@ -37,15 +38,15 @@
         logger.info(f"sqs message {receipt_handle} deleted")
 
 
 def sqs_send_message(body, queue_url, attributes=None, profile=None):
     """sends a message to the SQS queue"""
     logger.debug('send_sqs_message("body") called')
 
-    # establich a boto3 client for SQS
+    # establish a boto3 client for SQS
     s = boto3.session.Session()
     if profile:
         s = boto3.session.Session(profile_name=profile)
     c = s.client("sqs")
     logger.info("boto3 sqs client created")
 
     try:
@@ -172,7 +173,41 @@
     if profile:
         s = boto3.session.Session(profile_name=profile)
     c = s.resource("s3")
     logger.info("boto3 s3 client created")
     bucket = c.Bucket(bucket)
     objects = bucket.objects.filter(Prefix=prefix)
     return objects
+
+
+def textract_get_in_flight_count():
+    values: list[str] = [
+        "StartDocumentAnalysis",
+        "StartDocumentTextDetection",
+        # "StartExpenseAnalysis",
+        # "StartLendingAnalysis",
+        "GetDocumentAnalysis",
+        "GetDocumentTextDetection",
+        # "GetExpenseAnalysis",
+        # "GetLendingAnalysis",
+        # "GetLendingAnalysisSummary",
+    ]
+    now: datetime = datetime.now()
+
+    c = boto3.client("cloudwatch")
+    current_count: int = 0
+    for value in values:
+        response = c.get_metric_statistics(
+            Namespace="AWS/Textract",
+            MetricName="ResponseTime",
+            Dimensions=[{"Name": "Operation", "Value": value}],
+            StartTime=now - timedelta(minutes=5),
+            EndTime=now,
+            Period=60,
+            Statistics=["SampleCount"],
+        )
+        for datapoint in response["Datapoints"]:
+            if datapoint["Timestamp"] == max([x["Timestamp"] for x in response["Datapoints"]]):
+                current_count += datapoint["SampleCount"]
+                break
+
+    return current_count
```

### Comparing `dgarbsutils-1.5.9/src/dgarbsutils/utils.py` & `dgarbsutils-1.6.0/src/dgarbsutils/utils.py`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.5.9/src/dgarbsutils.egg-info/PKG-INFO` & `dgarbsutils-1.6.0/src/dgarbsutils.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: dgarbsutils
-Version: 1.5.9
+Version: 1.6.0
 Summary: A set of curated utils
 Home-page: https://github.com/dgarbalo/py-utils
 Author: Devon Garbalosa
 Author-email: dgarbalo@gmail.com
 Project-URL: Bug Tracker, https://github.com/dgarbalo/py-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Utils
 
 ## Description
```

### Comparing `dgarbsutils-1.5.9/tests/test_utils.py` & `dgarbsutils-1.6.0/tests/test_utils.py`

 * *Files identical despite different names*

