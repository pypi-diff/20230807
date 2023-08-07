# Comparing `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731.tar.gz` & `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731.tar", last modified: Thu Jul 27 23:08:23 2023, max compression
+gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156.tar", last modified: Mon Aug  7 19:12:52 2023, max compression
```

## Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731.tar` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:08:23.944400 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-27 23:07:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-27 23:08:23.944400 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2197 2023-07-27 23:07:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 23:08:23.944400 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-07-27 23:08:21.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:08:23.940400 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:08:23.944400 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 23:07:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-07-27 23:07:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    24055 2023-07-27 23:07:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 23:07:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     4701 2023-07-27 23:07:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
--rw-r--r--   0 root         (0) root         (0)     1019 2023-07-27 23:07:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-27 23:07:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
--rw-r--r--   0 root         (0) root         (0)     1288 2023-07-27 23:07:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/test_dynamo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:08:23.944400 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-27 23:08:23.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-27 23:08:23.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 23:08:23.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-27 23:08:23.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-27 23:08:23.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:12:52.021306 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-08-07 19:11:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3248 2023-08-07 19:12:52.021306 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-08-07 19:11:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 19:12:52.021306 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-08-07 19:12:49.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:12:52.017305 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:12:52.021306 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 19:11:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-08-07 19:11:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    20465 2023-08-07 19:11:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-08-07 19:11:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5467 2023-08-07 19:11:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-08-07 19:11:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-08-07 19:11:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:12:52.021306 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3248 2023-08-07 19:12:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      948 2023-08-07 19:12:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 19:12:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2023-08-07 19:12:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-08-07 19:12:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/LICENSE` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230727230731
+Version: 1.0.0.dev20230807191156
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -60,7 +60,19 @@
 ## Maven
 This project can use Apache Maven to easily build this project.  However, this is not required, but recommended.
 Maven can be easily installed by downloading it from the Maven site or using sdkman.
 
 ## Build with Maven
 After setting up your pyenv run:
 ```mvn clean install```
+
+## Functional Testing
+To run a functional test, developer will need to save the associated environment variables in .env for the lambda to
+use. The ACCESS_KEY and SECRET_ACCESS_KEY can be generated in IAM, users, rudy-dev, security credentials,
+access keys, create access key. Copy other values as needed from deployed CloudFormation Template.
+```shell
+export OUTPUT_BUCKET=rudy-dev-echofish-118234403147-echofish-dev-output
+export TABLE_NAME=rudy-dev-echofish-EchoFish-File-Info
+export OUTPUT_BUCKET_ACCESS_KEY="XXX"
+export OUTPUT_BUCKET_SECRET_ACCESS_KEY="YYY"
+export TOPIC_ARN="arn:aws:sns:us-west-2:118234403147:rudy-dev-echofish-processing-finished"
+```
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/README.md` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -50,7 +50,19 @@
 ## Maven
 This project can use Apache Maven to easily build this project.  However, this is not required, but recommended.
 Maven can be easily installed by downloading it from the Maven site or using sdkman.
 
 ## Build with Maven
 After setting up your pyenv run:
 ```mvn clean install```
+
+## Functional Testing
+To run a functional test, developer will need to save the associated environment variables in .env for the lambda to
+use. The ACCESS_KEY and SECRET_ACCESS_KEY can be generated in IAM, users, rudy-dev, security credentials,
+access keys, create access key. Copy other values as needed from deployed CloudFormation Template.
+```shell
+export OUTPUT_BUCKET=rudy-dev-echofish-118234403147-echofish-dev-output
+export TABLE_NAME=rudy-dev-echofish-EchoFish-File-Info
+export OUTPUT_BUCKET_ACCESS_KEY="XXX"
+export OUTPUT_BUCKET_SECRET_ACCESS_KEY="YYY"
+export TOPIC_ARN="arn:aws:sns:us-west-2:118234403147:rudy-dev-echofish-processing-finished"
+```
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/setup.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-resample-and-write-to-zarr-store-lambda",
-  version="1.0.0.dev20230727230731",
+  version="1.0.0.dev20230807191156",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # lambda_executor.py
+
 import json
 import os
-import glob
-import shutil
+import boto3
 import s3fs
 import zarr
 from scipy import interpolate
 import geopandas
-from datetime import datetime
-import boto3
 from botocore.exceptions import ClientError
 import numpy as np
 import xarray as xr
 import pandas as pd
 
 TEMPDIR = "/tmp"
 
 MAX_POOL_CONNECTIONS = 64
 MAX_CONCURRENCY = 100
 TILE_SIZE = 512
 
 SYNCHRONIZER = None  # TODO
 
 class LambdaExecutor:
-
     ############################################################################
     def __init__(
             self,
             s3_operations,
             s3fs_operations,
             dynamo_operations,
             sns_operations,
@@ -191,111 +188,40 @@
                 },
                 ':c': {
                     'L': [{'S': i} for i in channels]
                 }
             }
         )
 
-    ############################################################################
-    ############################################################################
-    # def __write_geojson_to_file(
-    #         self,
-    #         store_name,
-    #         data
-    # ) -> None:
-    #     """Write the GeoJSON file inside the Zarr store folder. Note that the
-    #     file is not a technical part of the store, this is more of a hack
-    #     to help pass the data along to the next processing step.
-    #
-    #     Parameters
-    #     ----------
-    #     path : str
-    #         The path to a local Zarr store where the file will be written.
-    #     data : str
-    #         A GeoJSON Feature Collection to be written to output file.
-    #
-    #     Returns
-    #     -------
-    #     None : None
-    #         No return value.
-    #     """
-    #     with open(os.path.join(store_name, 'geo.json'), "w") as outfile:
-    #         outfile.write(data)
-
-    ############################################################################
-    ############################################################################
-    # def __remove_existing_s3_objects(
-    #         self,
-    #         prefix
-    # ):
-    #     print(f'Removing existing s3 objects from: {self.__output_bucket} with prefix {prefix}')
-    #     keys = self.__s3.list_objects(
-    #         bucket_name=self.__output_bucket,
-    #         prefix=prefix,
-    #         access_key_id=self.__output_bucket_access_key,
-    #         secret_access_key=self.__output_bucket_secret_access_key
-    #     )
-    #     for key in keys:
-    #         self.__s3.delete_object(
-    #             bucket_name=self.__output_bucket,
-    #             key=key,
-    #             access_key_id=self.__output_bucket_access_key,
-    #             secret_access_key=self.__output_bucket_secret_access_key
-    #         )
-    #     print('Removing existing s3 objects done')
-
-    ############################################################################
-    # def __upload_files(
-    #         self,
-    #         local_directory,
-    #         object_prefix
-    # ):
-    #     print('Upload files')
-    #     for subdir, dirs, files in os.walk(local_directory):
-    #         for file in files:
-    #             local_path = os.path.join(subdir, file)
-    #             # print(local_path)
-    #             s3_key = os.path.join(object_prefix, local_path)
-    #             self.__s3.upload_file(
-    #                 file_name=local_path,
-    #                 bucket_name=self.__output_bucket,
-    #                 key=s3_key,
-    #                 access_key_id=self.__output_bucket_access_key,
-    #                 secret_access_key=self.__output_bucket_secret_access_key
-    #             )
-    #     # print('Done uploading files')
 
     ############################################################################
     #####################################################################
 
     def __get_table_as_dataframe(self) -> pd.DataFrame:
         print('get table as dataframe')
-        session = boto3.Session()
+        # session = boto3.Session()
         try:
             print(self.__table_name)
-            #
-            # table = self.__dynamo.Table(self.__table_name)
             table = self.__dynamo.get_table(table_name=self.__table_name)
-            #
-            # Note: table.scan() has 1 MB limit on results so pagination is used.
+            # Note: table.scan() has 1 MB limit on results so pagination is used
             response = table.scan()
             data = response['Items']
             while 'LastEvaluatedKey' in response:
                 response = table.scan(ExclusiveStartKey=response['LastEvaluatedKey'])
                 data.extend(response['Items'])
         except ClientError as err:
             print('Problem finding the dynamodb table')
             raise err
         df = pd.DataFrame(data)
         print(df.shape)
         # assert(  # TODO: need to assure that none are marked as processing still
         #     np.all(df['PIPELINE_STATUS'] == PIPELINE_STATUS.SUCCESS.value) # "POPULATING_CRUISE_ZARR"
         # ), "None of the status fields should still be processing."
-        # df_success = df[df['PIPELINE_STATUS'] == PIPELINE_STATUS.SUCCESS.value]
         df_success = df[df['PIPELINE_STATUS'] == "POPULATING_CRUISE_ZARR"]
+        # df_success = df[df['PIPELINE_STATUS'] == "INITIALIZING_CRUISE_ZARR"]
         if df_success.shape[0] == 0:
             raise
         return df_success.sort_values(by='START_TIME', ignore_index=True)
 
 
     ############################################################################
     # TODO: need to pass in key/secret as optionals
@@ -313,48 +239,46 @@
         # You are already using dask, this is assumed by open_zarr, not the same as open_dataset(engine=“zarr”)
         return xr.open_zarr(store=store, consolidated=None)  # synchronizer=SYNCHRONIZER
 
     ############################################################################
     ############################################################################
     def __interpolate_data(
             self,
-            minimum_resolution: float,  # get from df
-            maximum_cruise_depth_meters: float,  # get from df
+            minimum_resolution,  # get from df, type=np.float32
+            maximum_cruise_depth_meters,  # get from df, type=np.float32
             file_xr: xr.Dataset,  # need to figure out which time values are removed
             cruise_zarr: zarr.Group,
             start_ping_time_index: int,
             end_ping_time_index: int,
             indices: np.ndarray, # the file_xr ping_time and Sv indices that are not np.nan
     ) -> np.ndarray:
         # read remotely once to speed up
-        #
         # Note: file_zarr dimensions are (frequency, time, depth)
-        frequencies = file_xr.channel.shape[0]
+        num_frequencies = file_xr.channel.shape[0]
         file_sv = file_xr.Sv.values  # (4, 9779, 1302)
         all_file_depth_values = file_xr.echo_range.values[:, :, :]  # TODO
         # Note: cruise_zarr dimensions are (depth, time, frequency)
-        cruise_sv_subset = np.empty(shape=cruise_zarr.sv[:, start_ping_time_index:end_ping_time_index, :].shape)
-        cruise_sv_subset[:, :, :] = np.nan # (5208, 9778, 4)
+        cruise_sv_subset = np.empty(shape=cruise_zarr.Sv[:, start_ping_time_index:end_ping_time_index, :].shape)
+        cruise_sv_subset[:, :, :] = np.nan  # (5208, 9778, 4)
         # grid evenly spaced depths over the specified interval
         all_cruise_depth_values = np.linspace(
             start=0,
             stop=maximum_cruise_depth_meters,
             num=int(maximum_cruise_depth_meters / minimum_resolution) + 1,
             endpoint=True
-        )  # 5208
+        )
         #
-        for iii in range(frequencies):
+        for iii in range(num_frequencies):
             for jjj in range(len(indices)):
                 y = file_sv[iii, indices[jjj], :]  # y.shape = (4, 4871, 5208) -> frequency, time, depth
                 # all_Sv is inly 1302 depth measurements
                 f = interpolate.interp1d(  # Interpolate a 1-D function.
                     x=all_file_depth_values[iii, indices[jjj], :],
                     y=y,  # Need to strip off unwanted timestamps
                     kind='nearest',
-                    # axis=0,
                     bounds_error=False,
                     fill_value=np.nan
                 )
                 y_new = f(all_cruise_depth_values)  # y_new.shape = (4, 4871, 5208) --> (frequency, time, depth)
                 # Note: dimensions are (depth, time, frequency)
                 cruise_sv_subset[:, jjj, iii] = y_new #.transpose((2, 1, 0))  # (5208, 89911, 4)
         #
@@ -366,89 +290,75 @@
             self,
             output_zarr_bucket: str,
             ship_name: str,
             cruise_name: str,
             sensor_name: str,
             # zarr_synchronizer: Union[str, None] = None,
     ):
-        # Environment variables are optional parameters
         s3 = s3fs.S3FileSystem(
-            key=os.getenv('ACCESS_KEY_ID'),
-            secret=os.getenv('SECRET_ACCESS_KEY'),
+            key=self.__output_bucket_access_key,
+            secret=self.__output_bucket_secret_access_key
         )
-        root = f's3://{output_zarr_bucket}/level_2/{ship_name}/{cruise_name}/{sensor_name}/{cruise_name}.zarr'
+        root = f'{output_zarr_bucket}/level_2/{ship_name}/{cruise_name}/{sensor_name}/{cruise_name}.zarr'
         # TODO: check if directory exists
-        store = s3fs.S3Map(root=root, s3=s3, check=True)
+        store = s3fs.S3Map(root=root, s3=s3) #, check=True)
         # TODO: properly synchronize with efs mount
         # TODO: zarr.ThreadSynchronizer()
         # Note: 'r+' means read/write (store must already exist)
         cruise_zarr = zarr.open(store=store, mode="r+") #, zarr_synchronizer=zarr_synchronizer)
         return cruise_zarr
 
 
     ############################################################################
     def __get_spatiotemporal_indices(
             self,
-            input_zarr_bucket: str,
             input_zarr_path: str,
     ) -> tuple:
-        """
-        Assumes that there is a GeoJSON file in the file-level Zarr store.
 
-        :param str input_zarr_bucket: Input bucket where file-level Zarr store exists.
-        :param str input_zarr_path: Input bucket path where file-level Zarr store exists.
-        :return: (list, list, list): Returns the latitude, longitude, and epoch seconds
-        needed to properly index the data.
-        """
-        s3 = s3fs.S3FileSystem(
-            key=os.getenv('ACCESS_KEY_ID'),  # optional parameter
-            secret=os.getenv('SECRET_ACCESS_KEY'),
-        )
+        # s3 = s3fs.S3FileSystem(
+        #     key=self.__output_bucket_access_key,
+        #     secret=self.__output_bucket_secret_access_key,
+        # )
         geo_json_s3_path = f's3://{self.__output_bucket}/{input_zarr_path}/geo.json'
-        assert(s3.exists(geo_json_s3_path)), "S3 GeoJSON file does not exist."
+        assert(self.__s3fs.exists(
+            geo_json_s3_path=geo_json_s3_path,
+            access_key_id=self.__output_bucket_access_key,
+            secret_access_key=self.__output_bucket_secret_access_key)
+        ), "S3 GeoJSON file does not exist."
         geo_json = geopandas.read_file(
             filename=geo_json_s3_path,
             storage_options={
-                "key": os.getenv('ACCESS_KEY_ID'),  # Optional values
-                "secret": os.getenv('SECRET_ACCESS_KEY'),
+                "key": self.__output_bucket_access_key,
+                "secret": self.__output_bucket_secret_access_key,
             },
         )
         geo_json.id = pd.to_datetime(geo_json.id)
         geo_json.id.astype('datetime64[ns]')  # TODO: be careful with conversions for pandas >=2.0.0
         epoch_seconds = (
-                                pd.to_datetime(geo_json.dropna().id, unit='s', origin='unix') - pd.Timestamp('1970-01-01')
-                        ) / pd.Timedelta('1s')
+            pd.to_datetime(geo_json.dropna().id, unit='s', origin='unix') - pd.Timestamp('1970-01-01')
+        ) / pd.Timedelta('1s')
         epoch_seconds = epoch_seconds.tolist()
         longitude = geo_json.dropna().longitude.tolist()
         latitude = geo_json.dropna().latitude.tolist()
         #
         return latitude, longitude, epoch_seconds
 
 
     ############################################################################
     def __read_s3_geo_json(
             self,
             input_zarr_path: str,
-            access_key_id: str = None,
-            secret_access_key: str = None,
     ) -> str:
-        # reads geojson file from s3 bucket w boto3
-        # session = boto3.Session()
-        # s3 = boto3.resource(
-        #     service_name='s3',
-        #     aws_access_key_id=access_key_id,
-        #     aws_secret_access_key=secret_access_key,
-        # )
-        content_object = self.__s3.get_object(
-            self.__output_bucket,
-            input_zarr_path,
-            access_key_id=access_key_id,
-            secret_access_key=secret_access_key
+        s3 = boto3.resource(
+            service_name='s3',
+            aws_access_key_id=self.__output_bucket_access_key,
+            aws_secret_access_key=self.__output_bucket_secret_access_key,
         )
-        # content_object = s3.Object(self.__output_bucket, f'{input_zarr_path}/geo.json')
+        content_object = s3.Object(bucket_name=self.__output_bucket, key=f"{input_zarr_path}/geo.json")
+        print(content_object.get())
         file_content = content_object.get()['Body'].read().decode('utf-8')
         json_content = json.loads(file_content)
         return json_content
 
 
     ############################################################################
     def __publish_done_message(self, message):
@@ -462,14 +372,15 @@
         ship_name = message['shipName']  # 'Henry_B._Bigelow'
         cruise_name = message['cruiseName']  # 'HB0707'
         sensor_name = message['sensorName']  # 'EK60'
         input_file_name = message['fileName']  # 'D20070711-T210709.raw'
         #
         file_stem = os.path.splitext(input_file_name)[0]
         input_zarr_path = f"level_1/{ship_name}/{cruise_name}/{sensor_name}/{file_stem}.zarr"
+        print(input_zarr_path)
         #
         os.chdir(TEMPDIR)
         #
         ### COPY N PASTED IN BELOW #######################################################
         # [0] get dynamoDB table info
         df = self.__get_table_as_dataframe()
         # Zarr path is derived from DynamoDB
@@ -479,38 +390,42 @@
         index = df.index[df['ZARR_PATH'] == input_zarr_path][0]  # index among all cruise files
         print(index)
         #
         file_info = df.iloc[index].to_dict()
         input_zarr_bucket = file_info['ZARR_BUCKET']
         input_zarr_path = file_info['ZARR_PATH']
         output_zarr_bucket = file_info['ZARR_BUCKET']
+        print(file_info)
+        print(input_zarr_bucket)
+        print(input_zarr_path)
+        print(output_zarr_bucket)
         #
         #################################################################
         # [1] read file-level Zarr store using xarray
         file_xr = self.__get_s3_zarr_as_xr(zarr_path=input_zarr_path)
         geo_json = self.__read_s3_geo_json(
             input_zarr_path=input_zarr_path,
-            access_key_id=os.getenv('ACCESS_KEY_ID'),
-            secret_access_key=os.getenv('SECRET_ACCESS_KEY')
         )
-        #geo_json['features'][0]
         # {'id': '2007-07-12T15:24:16.032000000', 'type': 'Feature', 'properties': {'latitude': None, 'longitude': None}, 'geometry': None}
         # reads GeoJSON with the id as the index
         geospatial = geopandas.GeoDataFrame.from_features(geo_json['features']).set_index(pd.json_normalize(geo_json["features"])["id"].values)
         geospatial_index = geospatial.dropna().index.values.astype('datetime64[ns]')
         # find the indices where 'v' can be inserted into 'a'
-        indices = np.searchsorted(a=file_xr.ping_time.values, v=geospatial_index)
-        #
-        # TODO: only need to read the geojson file once instead of twice here...
-        #
+        aa = file_xr.ping_time.values.tolist()
+        vv = geospatial_index.tolist()
+        indices = np.searchsorted(a=aa, v=vv)
         #########################################################################
         #########################################################################
         # [2] open cruise level zarr store for writing
         # output_zarr_path: str = f'',
         print('opening cruise zarr')
+        print(output_zarr_bucket)
+        print(ship_name)
+        print(cruise_name)
+        print(sensor_name)
         cruise_zarr = self.__s3_zarr(
             output_zarr_bucket,
             ship_name,
             cruise_name,
             sensor_name,
             # zarr_synchronizer  # TODO:
         )
@@ -526,43 +441,44 @@
         start_ping_time_index = ping_time_cumsum[index]
         end_ping_time_index = ping_time_cumsum[index + 1]
         #
         #########################################################################
         # [4] extract gps and time coordinate from file-level Zarr store,
         # write subset of ping_time to the larger zarr store
         # reference: https://osoceanacoustics.github.io/echopype-examples/echopype_tour.html
-        latitude, longitude, epoch_seconds = self.__get_spatiotemporal_indices(input_zarr_bucket, input_zarr_path)
+        latitude, longitude, epoch_seconds = self.__get_spatiotemporal_indices(
+            input_zarr_path=input_zarr_path
+        )
         assert(
                 len(epoch_seconds) == len(cruise_zarr.time[start_ping_time_index:end_ping_time_index])
         ), "Number of the timestamps is not equivalent to indices given."
         cruise_zarr.time[start_ping_time_index:end_ping_time_index] = epoch_seconds
         #########################################################################
         # [5] write subset of latitude/longitude
         cruise_zarr.latitude[start_ping_time_index:end_ping_time_index] = latitude
         cruise_zarr.longitude[start_ping_time_index:end_ping_time_index] = longitude
         #########################################################################
         # [6] get interpolated Sv data
-        filename = os.path.basename(input_zarr_path)
+        # filename = os.path.basename(input_zarr_path)
         print('interpolate_data')
         print(type(df['MIN_ECHO_RANGE']))
         print(df['MIN_ECHO_RANGE'])
         print(np.float32(df['MIN_ECHO_RANGE']))
         all_Sv_prototype = self.__interpolate_data(
             minimum_resolution = np.nanmin(np.float32(df['MIN_ECHO_RANGE'])),
             maximum_cruise_depth_meters = np.nanmax(np.float32(df['MAX_ECHO_RANGE'])),
-            # num_ping_time_dropna = int(df.iloc[index]['NUM_PING_TIME_DROPNA']),
             file_xr=file_xr,
             cruise_zarr=cruise_zarr,
             start_ping_time_index=start_ping_time_index,
             end_ping_time_index=end_ping_time_index,
             indices=indices,
         )  # TODO:
-        cruise_zarr.sv[:, start_ping_time_index:end_ping_time_index, :] = all_Sv_prototype
+        cruise_zarr.Sv[:, start_ping_time_index:end_ping_time_index, :] = all_Sv_prototype
         #
-        #np.nanmean(cruise_zarr.sv[:, start_ping_time_index:end_ping_time_index, :])
+        #np.nanmean(cruise_zarr.Sv[:, start_ping_time_index:end_ping_time_index, :])
         #
-        print(cruise_zarr.sv.info)
-        print('done')
+        print(cruise_zarr.Sv.info)
         # logger.info("Finishing lambda.")
         # TODO: Work on synchronizing the data as written
         self.__publish_done_message(message)
         print(f'Done processing {input_file_name}')
+        # TODO: update status in the dynamodb
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # s3_operations.py
+import os
 import boto3
 from collections.abc import Generator
 
 class S3Operations:
     #####################################################################
     def __get_client(
             self,
@@ -23,24 +24,24 @@
 
     #####################################################################
     def __get_resource(
             self,
             access_key_id=None,
             secret_access_key=None
     ):
-        session = boto3.Session()
+        # session = boto3.Session()
         if access_key_id:
-            s3_resource = session.resource(
+            s3_resource = boto3.resource(
                 service_name='s3',
                 aws_access_key_id=access_key_id,
                 aws_secret_access_key=secret_access_key
             )
             print('NODD Authenticated')
         else:
-            s3_resource = session.resource(service_name='s3')
+            s3_resource = boto3.resource(service_name='s3')
         return s3_resource
 
     #####################################################################
     def __chunked(
             self,
             ll: list,
             n: int
@@ -122,14 +123,30 @@
     def get_object(
             self,
             bucket_name,
             input_zarr_path,
             access_key_id=None,
             secret_access_key=None
     ):
-        s3_resource = self.__get_resource(access_key_id=access_key_id, secret_access_key=secret_access_key)
+        import os
+        # s3 = boto3.resource(
+        #     service_name='s3',
+        #     aws_access_key_id=os.getenv('ACCESS_KEY_ID'),
+        #     aws_secret_access_key=os.getenv('SECRET_ACCESS_KEY'),
+        # )
+        # content_object = s3.Object(input_zarr_bucket, f'{input_zarr_path}/geo.json')
+        # file_content = content_object.get()['Body'].read().decode('utf-8')
+        #
+        s3_resource = self.__get_resource(
+            # access_key_id=access_key_id,
+            # secret_access_key=secret_access_key
+            access_key_id=os.getenv('ACCESS_KEY_ID'),
+            secret_access_key=os.getenv('SECRET_ACCESS_KEY')
+        )
+        s3_resource.Object(bucket_name, f'{input_zarr_path}/geo.json').get()
         # content_object = s3.Object(input_zarr_bucket, f'{input_zarr_path}/geo.json')
+        # 'rudy-dev-echofish-118234403147-echofish-dev-output/level_1/Henry_B._Bigelow/HB0707/EK60/D20070712-T004447.zarr/geo.json'
         return s3_resource.Object(bucket_name, f'{input_zarr_path}/geo.json')
 
 
     #####################################################################
     #####################################################################
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py`

 * *Files 23% similar despite different names*

```diff
@@ -29,7 +29,21 @@
         s3_fs = self.__get_s3_fs(
             access_key_id=access_key_id,
             secret_access_key=secret_access_key
         )
         return s3fs.S3Map(root=s3_zarr_store_path, s3=s3_fs, check=True)
 
     #####################################################################
+    def exists(
+            self,
+            geo_json_s3_path,
+            access_key_id=None,
+            secret_access_key=None,
+    ):
+        s3_fs = self.__get_s3_fs(
+            access_key_id=access_key_id,
+            secret_access_key=secret_access_key
+        )
+        return s3_fs.exists(path=geo_json_s3_path)
+
+    #####################################################################
+    #####################################################################
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230727230731
+Version: 1.0.0.dev20230807191156
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -60,7 +60,19 @@
 ## Maven
 This project can use Apache Maven to easily build this project.  However, this is not required, but recommended.
 Maven can be easily installed by downloading it from the Maven site or using sdkman.
 
 ## Build with Maven
 After setting up your pyenv run:
 ```mvn clean install```
+
+## Functional Testing
+To run a functional test, developer will need to save the associated environment variables in .env for the lambda to
+use. The ACCESS_KEY and SECRET_ACCESS_KEY can be generated in IAM, users, rudy-dev, security credentials,
+access keys, create access key. Copy other values as needed from deployed CloudFormation Template.
+```shell
+export OUTPUT_BUCKET=rudy-dev-echofish-118234403147-echofish-dev-output
+export TABLE_NAME=rudy-dev-echofish-EchoFish-File-Info
+export OUTPUT_BUCKET_ACCESS_KEY="XXX"
+export OUTPUT_BUCKET_SECRET_ACCESS_KEY="YYY"
+export TOPIC_ARN="arn:aws:sns:us-west-2:118234403147:rudy-dev-echofish-processing-finished"
+```
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727230731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230807191156/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,13 +4,12 @@
 src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
 src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
 src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
 src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
 src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
 src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
 src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
-src/echofish_aws_resample_and_write_to_zarr_store_lambda/test_dynamo.py
 src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
 src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
 src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
 src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
 src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
```

