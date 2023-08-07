# Comparing `tmp/echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113.tar.gz` & `tmp/echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113.tar", last modified: Mon Aug  7 16:41:59 2023, max compression
+gzip compressed data, was "echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104.tar", last modified: Mon Aug  7 17:21:51 2023, max compression
```

## Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113.tar` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:41:59.559629 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-08-07 16:41:59.559629 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2868 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 16:41:59.559629 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      734 2023-08-07 16:41:57.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:41:59.555629 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:41:59.559629 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    16097 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1230 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     6392 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/s3_operations.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-08-07 16:41:08.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/sns_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 16:41:59.559629 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-08-07 16:41:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      773 2023-08-07 16:41:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 16:41:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-08-07 16:41:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-08-07 16:41:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 17:21:51.336054 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-08-07 17:20:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-08-07 17:21:51.336054 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-08-07 17:20:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 17:21:51.336054 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      734 2023-08-07 17:21:49.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 17:21:51.336054 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 17:21:51.336054 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 17:20:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-08-07 17:20:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    17315 2023-08-07 17:20:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-08-07 17:20:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     6392 2023-08-07 17:20:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda/s3_operations.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-08-07 17:20:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda/sns_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 17:21:51.336054 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-08-07 17:21:51.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      773 2023-08-07 17:21:51.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 17:21:51.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-08-07 17:21:51.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-08-07 17:21:51.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/LICENSE` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/PKG-INFO` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-create-empty-zarr-store-lambda
-Version: 1.0.0.dev20230807164113
+Version: 1.0.0.dev20230807172104
 Home-page: https://github.com/ci-cmg/echofish-aws-create-empty-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/README.md` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/setup.py` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-create-empty-zarr-store-lambda",
-  version="1.0.0.dev20230807164113",
+  version="1.0.0.dev20230807172104",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-create-empty-zarr-store-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/dynamo_operations.py` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         self.__done_topic_arn = done_topic_arn
 
 
     ############################################################################
     def __get_table_as_dataframe(
             self,
     ):
+        print('getting table as dataframe')
         try:
             table = self.__dynamo.get_table(self.__table_name)
             # Note: table.scan() has 1 MB limit on results so pagination is used.
             response = table.scan()
             data = response['Items']
             while 'LastEvaluatedKey' in response:
                 response = table.scan(ExclusiveStartKey=response['LastEvaluatedKey'])
@@ -93,14 +94,15 @@
             self,
             store_name: str,
             width: int,
             height: int,
             min_echo_range: float,
             frequency: list,
     ) -> None:
+        print('creating zarr store')
         compressor = Blosc(cname="zstd", clevel=5, shuffle=Blosc.BITSHUFFLE)
         # Note: normalize_keys sets keys to lower case characters
         store = zarr.DirectoryStore(path=store_name, normalize_keys=False)  # TODO: write directly to s3?
         root = zarr.group(store=store, overwrite=True, cache_attrs=True) # path="/",
         #####################################################################
         # Coordinate: Time -- no missing values will be included
         # https://zarr.readthedocs.io/en/stable/spec/v2.html#data-type-encoding
@@ -228,14 +230,15 @@
 
     ############################################################################
     def __upload_zarr_store_to_s3(
             self,
             local_directory: str,
             object_prefix: str,
     ) -> None:
+        print('uploading zarr store to s3')
         for subdir, dirs, files in os.walk(local_directory):
             for file in files:
                 local_path = os.path.join(subdir, file)
                 # print(local_path)
                 s3_key = os.path.join(object_prefix, local_path)
                 try:
                     self.__s3.upload_file(
@@ -303,14 +306,38 @@
                         raw_files.append(i['Key'])
                 return raw_files
         except ClientError as err:
             print(f"Some problem was encountered: {err}")
             raise
         return raw_files
 
+    ############################################################################
+    def __update_processing_status(
+            self,
+            cruise_name,
+            file_name,
+            new_status
+    ):
+        self.__dynamo.update_item(
+            table_name=self.__table_name,
+            key={
+                'FILE_NAME': {'S': file_name},  # Partition Key
+                'CRUISE_NAME': {'S': cruise_name},  # Sort Key
+            },
+            expression='SET #PS = :ps',
+            attribute_names={
+                '#PS': 'PIPELINE_STATUS'
+            },
+            attribute_values={
+                ':ps': {
+                    'S': new_status
+                }
+            }
+        )
+
     def __publish_done_message(self, message):
         print("Sending done message")
         self.__sns_operations.publish(self.__done_topic_arn, json.dumps(message))
 
     ############################################################################
     def execute(self, message):
         #################################################################
@@ -380,22 +407,30 @@
             print("Counts match.")
         ###########
         if os.path.exists(store_name):
             print(f'Removing local zarr directory: {store_name}')
             shutil.rmtree(store_name)
         #################################################################
         #
+        # TODO: update the status in dynamo db
+        # from zarr-cruise-accumulator-lambda: "INITIALIZING_CRUISE_ZARR"
+        # from create-empty-zarr-store-lambda: "POPULATING_CRUISE_ZARR"
         #
         for file_name in list(df["FILE_NAME"]):
             outputMessage = {
                 'cruiseName': cruise_name,
                 'shipName': ship_name,
                 'sensorName': sensor_name,
                 'fileName': file_name,
             }
             json.dumps(outputMessage)
             self.__publish_done_message(outputMessage)
+            self.__update_processing_status(
+                cruise_name=cruise_name,
+                file_name=file_name,
+                new_status='POPULATING_CRUISE_ZARR'
+            )
             print(outputMessage)
         # TODO: iterate through all success files and prompt  resample_and_write_to_zarr_store_lambda
         print(f'Done processing.')
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/lambda_handler.py` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda/s3_operations.py` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda/s3_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-create-empty-zarr-store-lambda
-Version: 1.0.0.dev20230807164113
+Version: 1.0.0.dev20230807172104
 Home-page: https://github.com/ci-cmg/echofish-aws-create-empty-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807164113/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230807172104/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

