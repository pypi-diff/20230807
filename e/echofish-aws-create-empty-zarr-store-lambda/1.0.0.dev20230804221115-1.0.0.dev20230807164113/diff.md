# Comparing `tmp/echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115.tar.gz` & `tmp/echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115.tar", last modified: Fri Aug  4 22:12:01 2023, max compression
+gzip compressed data, was "echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113.tar", last modified: Mon Aug  7 16:41:59 2023, max compression
```

## Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115.tar` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 22:12:01.952032 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-08-04 22:12:01.952032 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2868 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 22:12:01.952032 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      734 2023-08-04 22:11:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 22:12:01.948032 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 22:12:01.952032 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15401 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1230 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     6392 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/s3_operations.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/sns_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 22:12:01.952032 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-08-04 22:12:01.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      773 2023-08-04 22:12:01.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 22:12:01.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-08-04 22:12:01.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-08-04 22:12:01.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:41:59.559629 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-08-07 16:41:59.559629 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 16:41:59.559629 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      734 2023-08-07 16:41:57.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:41:59.555629 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:41:59.559629 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    16097 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     6392 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/s3_operations.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/sns_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:41:59.559629 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-08-07 16:41:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      773 2023-08-07 16:41:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 16:41:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-08-07 16:41:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-08-07 16:41:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/LICENSE` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/PKG-INFO` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-create-empty-zarr-store-lambda
-Version: 1.0.0.dev20230804221115
+Version: 1.0.0.dev20230807164113
 Home-page: https://github.com/ci-cmg/echofish-aws-create-empty-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/README.md` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/setup.py` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-create-empty-zarr-store-lambda",
-  version="1.0.0.dev20230804221115",
+  version="1.0.0.dev20230807164113",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-create-empty-zarr-store-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/dynamo_operations.py` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # lambda_executor.py
 
 import os
+import json
 import glob
 import shutil
 # import logging
 from boto3.s3.transfer import TransferConfig
 from botocore.exceptions import ClientError
 from botocore.config import Config
 import numpy as np
@@ -302,14 +303,17 @@
                         raw_files.append(i['Key'])
                 return raw_files
         except ClientError as err:
             print(f"Some problem was encountered: {err}")
             raise
         return raw_files
 
+    def __publish_done_message(self, message):
+        print("Sending done message")
+        self.__sns_operations.publish(self.__done_topic_arn, json.dumps(message))
 
     ############################################################################
     def execute(self, message):
         #################################################################
         ship_name = message['shipName']  # 'Henry_B._Bigelow'
         cruise_name = message['cruiseName']  # 'HB0707'
         sensor_name = message['sensorName']  # 'EK60'
@@ -374,11 +378,24 @@
             raise
         else:
             print("Counts match.")
         ###########
         if os.path.exists(store_name):
             print(f'Removing local zarr directory: {store_name}')
             shutil.rmtree(store_name)
-        print('done')
         #################################################################
+        #
+        #
+        for file_name in list(df["FILE_NAME"]):
+            outputMessage = {
+                'cruiseName': cruise_name,
+                'shipName': ship_name,
+                'sensorName': sensor_name,
+                'fileName': file_name,
+            }
+            json.dumps(outputMessage)
+            self.__publish_done_message(outputMessage)
+            print(outputMessage)
+        # TODO: iterate through all success files and prompt  resample_and_write_to_zarr_store_lambda
+        print(f'Done processing.')
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/lambda_handler.py` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/s3_operations.py` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/s3_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-create-empty-zarr-store-lambda
-Version: 1.0.0.dev20230804221115
+Version: 1.0.0.dev20230807164113
 Home-page: https://github.com/ci-cmg/echofish-aws-create-empty-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

