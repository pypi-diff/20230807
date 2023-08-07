# Comparing `tmp/qwak_inference-0.1.7.tar.gz` & `tmp/qwak_inference-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_inference-0.1.7.tar", max compression
+gzip compressed data, was "qwak_inference-0.1.8.tar", max compression
```

## Comparing `qwak_inference-0.1.7.tar` & `qwak_inference-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    10480 2023-07-26 10:34:32.413627 qwak_inference-0.1.7/LICENSE
--rw-r--r--   0        0        0      267 2023-07-26 10:34:32.413627 qwak_inference-0.1.7/README.md
--rw-r--r--   0        0        0     2192 2023-07-26 10:35:34.786138 qwak_inference-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      804 2023-07-26 10:35:34.786138 qwak_inference-0.1.7/qwak_inference/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 10:34:32.413627 qwak_inference-0.1.7/qwak_inference/batch_client/__init__.py
--rw-r--r--   0        0        0    20136 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/batch_client/batch_client.py
--rw-r--r--   0        0        0     2172 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/batch_client/file_serialization.py
--rw-r--r--   0        0        0     1497 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/batch_client/instance_validation.py
--rw-r--r--   0        0        0      739 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/batch_client/s3.py
--rw-r--r--   0        0        0       95 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/configuration/__init__.py
--rw-r--r--   0        0        0     3127 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/configuration/account.py
--rw-r--r--   0        0        0     2676 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/configuration/auth.py
--rw-r--r--   0        0        0      929 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/configuration/session.py
--rw-r--r--   0        0        0      688 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/constants.py
--rw-r--r--   0        0        0     1592 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/exceptions.py
--rw-r--r--   0        0        0     1999 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/feedback_client.py
--rw-r--r--   0        0        0       65 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/realtime_client/__init__.py
--rw-r--r--   0        0        0     4811 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/realtime_client/client.py
--rw-r--r--   0        0        0     2346 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/realtime_client/rest_helpers.py
--rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 qwak_inference-0.1.7/setup.py
--rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 qwak_inference-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    10480 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/LICENSE
+-rw-r--r--   0        0        0      267 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/README.md
+-rw-r--r--   0        0        0     2192 2023-08-07 12:40:43.624905 qwak_inference-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      804 2023-08-07 12:40:43.624905 qwak_inference-0.1.8/qwak_inference/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/batch_client/__init__.py
+-rw-r--r--   0        0        0    26621 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/batch_client/batch_client.py
+-rw-r--r--   0        0        0     2172 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/batch_client/file_serialization.py
+-rw-r--r--   0        0        0     1497 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/batch_client/instance_validation.py
+-rw-r--r--   0        0        0     1300 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/batch_client/s3.py
+-rw-r--r--   0        0        0       95 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/configuration/__init__.py
+-rw-r--r--   0        0        0     3127 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/configuration/account.py
+-rw-r--r--   0        0        0     2676 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/configuration/auth.py
+-rw-r--r--   0        0        0      929 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/configuration/session.py
+-rw-r--r--   0        0        0      688 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/constants.py
+-rw-r--r--   0        0        0     1592 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/exceptions.py
+-rw-r--r--   0        0        0     1999 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/feedback_client.py
+-rw-r--r--   0        0        0       65 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/realtime_client/__init__.py
+-rw-r--r--   0        0        0     4811 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/realtime_client/client.py
+-rw-r--r--   0        0        0     2346 2023-08-07 12:39:54.673456 qwak_inference-0.1.8/qwak_inference/realtime_client/rest_helpers.py
+-rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 qwak_inference-0.1.8/setup.py
+-rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 qwak_inference-0.1.8/PKG-INFO
```

### Comparing `qwak_inference-0.1.7/LICENSE` & `qwak_inference-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.7/pyproject.toml` & `qwak_inference-0.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-inference"
-version = "0.1.7"
+version = "0.1.8"
 description = "Qwak Inference is a Python library for running predictions again Qwak Models."
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
```

### Comparing `qwak_inference-0.1.7/qwak_inference/__init__.py` & `qwak_inference-0.1.8/qwak_inference/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     print(
         "Notice that BatchInferenceClient and FeedbackClient are not available in the skinny package. "
         'In order to use them, please install them as extras: pip install "qwak-inference[batch,feedback]".'
     )
 
 __all__ = clients
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
```

### Comparing `qwak_inference-0.1.7/qwak_inference/batch_client/batch_client.py` & `qwak_inference-0.1.8/qwak_inference/batch_client/batch_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 import string
 import time
 from io import BytesIO
 from typing import List, Optional, Union
 
 import pandas as pd
 import requests
+from _qwak_proto.qwak.batch_job.v1.batch_job_service_pb2 import (
+    GetBatchJobUploadDetailsResponse,
+)
 from joblib import Parallel, delayed
 from qwak.clients.batch_job_management import BatchJobManagerClient
 from qwak.clients.batch_job_management.executions_config import ExecutionConfig
 from qwak.clients.batch_job_management.results import (
     GetBatchJobPreSignedUploadUrlResult,
     StartExecutionResult,
     StartWarmupJobResult,
@@ -94,21 +97,21 @@
                 f"{Color.RED}Passing `bucket`  will be deprecated. To stop passing it please "
                 f"re-build your model with a qwak-sdk version >= 0.8.156.{Color.END}"
             )
         self.model_id = model_id
         self.bucket = bucket
         self.access_key_secret = access_key_secret
         self.secret_access_key_secret = secret_access_key_secret
-        self.s3_client = self.get_s3_client()
+        self.s3_client = self._get_s3_client()
         self.batch_job_manager_client = BatchJobManagerClient()
         self.instance_template_client = InstanceTemplateManagementClient()
 
         logging.basicConfig(level=log_level)
 
-    def get_s3_client(self):
+    def _get_s3_client(self):
         if self.access_key_secret:
             secret_service_client = SecretServiceClient()
             aws_access_key_id = secret_service_client.get_secret(self.access_key_secret)
             aws_secret_access_key = secret_service_client.get_secret(
                 self.secret_access_key_secret
             )
             return S3Utils.get_client(aws_access_key_id, aws_secret_access_key)
@@ -288,14 +291,168 @@
         except KeyboardInterrupt:
             interrupted_msg = "Keyboard interrupted - canceling execution job"
             logging.warning(interrupted_msg)
             self.batch_job_manager_client.cancel_execution(execution_id)
 
             raise QwakException(interrupted_msg)
 
+    def local_file_run(
+        self,
+        model_id: str,
+        source_folder: str,
+        destination_folder: str,
+        input_file_type: str,
+        output_file_type: str = None,
+        job_timeout: int = 0,
+        task_timeout: int = 0,
+        executors: int = None,
+        cpus: float = None,
+        memory: int = None,
+        gpus: int = 0,
+        gpu_type: str = None,
+        iam_role_arn: str = None,
+        build_id: str = None,
+        parameters: dict = None,
+        instance: str = "",
+    ) -> None:
+        """Perform batch inference on given input directory (or a single input file), and store the result in the destination folder.
+
+        Args:
+            model_id: Model ID to perform batch inference on.
+            source_folder: Input directory (or a single input file) to perform batch inference on.
+            destination_folder: Output directory to store the result in. (will be created if it doesn't exist)
+            job_timeout: The entire execution job timeout.
+            task_timeout: Timeout for processing a single file.
+            executors: Number of executors to use in parallel.
+            cpus: Requested amount of CPUs for each executor.
+            memory: Requested amount of Memory for each executor.
+            gpus: Requested amount of GPUs for each executor.
+            gpu_type: Requested GPU type.
+            iam_role_arn: IAM role arn to be used in executors.
+            build_id: Build ID which will be used for performing the batch request.
+            parameters:
+            instance: The instance size to use in batch inference. E.g.: 'small', 'medium', etc.
+
+        Returns:
+            None.
+        """
+        file_extension = input_file_type.lower() if input_file_type else "csv"
+        destination_folder = destination_folder.removeprefix("file://")
+        source_folder = source_folder.removeprefix("file://")
+        if os.path.isdir(source_folder):
+            files = [
+                os.path.join(source_folder, f)
+                for f in os.listdir(source_folder)
+                if f.endswith(file_extension)
+            ]
+        else:
+            files = [source_folder] if source_folder.endswith(file_extension) else []
+        if files:
+            upload_details = self._upload_input_files(model_id, files)
+
+            execution_spec = ExecutionConfig.Execution(
+                model_id=model_id,
+                bucket=upload_details.bucket,
+                source_folder=upload_details.input_path,
+                destination_folder=upload_details.output_path.replace("//", "/"),
+            )
+            execution_spec.build_id = build_id
+            if parameters is not None:
+                execution_spec.parameters = parameters
+
+            execution_spec.input_file_type = input_file_type
+            execution_spec.output_file_type = (
+                output_file_type if output_file_type else input_file_type
+            )
+            execution_spec.job_timeout = job_timeout
+            execution_spec.file_timeout = task_timeout
+
+            advanced_options_config = ExecutionConfig.AdvancedOptions(
+                custom_iam_role_arn=iam_role_arn
+            )
+
+            resources_config = ExecutionConfig.Resources(
+                pods=executors,
+                cpus=cpus,
+                memory=memory,
+                gpu_type=gpu_type,
+                gpu_amount=gpus,
+                instance_size=instance,
+            )
+            execution_config = ExecutionConfig(
+                execution=execution_spec,
+                resources=resources_config,
+                advanced_options=advanced_options_config,
+            )
+
+            execution_result: StartExecutionResult = (
+                self.batch_job_manager_client.start_execution(execution_config)
+            )
+            if not execution_result.success:
+                error_message = (
+                    f"{Color.RED}An error occurred while starting execution: "
+                    f"{execution_result.failure_message} {execution_result.execution_id}{Color.END}"
+                )
+                logging.error(error_message)
+                raise QwakException(error_message)
+
+            execution_id = execution_result.execution_id
+
+            try:
+                logging.info(
+                    f"{Color.GREEN}Started execution {execution_id}{Color.END}"
+                )
+                job_status = self.get_job_status(execution_id)
+
+                if job_status == "Successful":
+                    self._download_batch_job_results_as_files(
+                        execution_id, destination_folder
+                    )
+                else:
+                    error_message = f"{Color.RED}Execution failed!{Color.END}"
+                    logging.error(error_message)
+                    raise QwakException(error_message)
+            except KeyboardInterrupt:
+                interrupted_msg = "Keyboard interrupted - canceling execution job"
+                logging.warning(interrupted_msg)
+                self.batch_job_manager_client.cancel_execution(execution_id)
+
+                raise QwakException(interrupted_msg)
+        else:
+            raise ValueError(
+                f"No files found in {source_folder} with extension {file_extension}"
+            )
+
+    def _upload_input_files(self, model_id, files):
+        upload_details: GetBatchJobUploadDetailsResponse = (
+            self.batch_job_manager_client.get_upload_details(model_id)
+        )
+        s3_client = S3Utils.get_client_with_temp_creds(upload_details.credentials)
+
+        for file in files:
+            file_name = os.path.basename(file)
+            s3_client.upload_file(
+                file, upload_details.bucket, f"{upload_details.input_path}/{file_name}"
+            )
+
+        return upload_details
+
+    def _download_batch_job_results_as_files(self, execution_id, destination_folder):
+        download_details = self.batch_job_manager_client.get_download_details(
+            execution_id
+        )
+        s3_client = S3Utils.get_client_with_temp_creds(download_details.credentials)
+
+        os.makedirs(destination_folder, exist_ok=True)
+        for key in download_details.keys:
+            file_name = os.path.basename(key)
+            s3_client.download_file(
+                download_details.bucket, key, f"{destination_folder}/{file_name}"
+            )
+
     def __default_auth_execute(
         self, df: pd.DataFrame, batch_size: int, serde_handler: SerializationFormat
     ):
         num_of_batches = math.ceil(len(df.index) / batch_size)
         if num_of_batches > self.MAX_PRE_SIGNED_BATCHES:
             raise QwakException(
                 f"Number of batches is larger than {self.MAX_PRE_SIGNED_BATCHES} ({num_of_batches}). "
@@ -317,15 +474,15 @@
             )
 
         source_folder = pre_signed_results.input_path
         destination_folder = pre_signed_results.output_path
         self.bucket = pre_signed_results.bucket
 
         # Upload files to S3
-        self.upload_df(
+        self._upload_df(
             df=df,
             batch_size=batch_size,
             pre_signed_urls=pre_signed_results.urls,
             serde_handler=serde_handler,
         )
 
         # Create qwak execution
@@ -340,15 +497,15 @@
         self, df: pd.DataFrame, batch_size: int, serde_handler: SerializationFormat
     ):
         job_id = "".join(
             random.choices(string.ascii_letters + string.digits, k=16)  # nosec
         )
 
         # Upload files to S3
-        source_folder = self.upload_df(
+        source_folder = self._upload_df(
             df=df,
             batch_size=batch_size,
             pre_signed_urls=None,
             job_id=job_id,
             serde_handler=serde_handler,
         )
 
@@ -430,15 +587,15 @@
                 )
                 if execution_report.success:
                     report = "\n".join(execution_report.records)
                     logs = "\n".join(execution_report.model_logs)
                     logging.error(f"{Color.WHITE}{report}\n{logs}{Color.END}")
                 return "Failed"
 
-    def upload_df(
+    def _upload_df(
         self,
         df: pd.DataFrame,
         batch_size: int,
         serde_handler: SerializationFormat,
         pre_signed_urls: Union[List[str], None],
         job_id: str = None,
     ):
```

### Comparing `qwak_inference-0.1.7/qwak_inference/batch_client/file_serialization.py` & `qwak_inference-0.1.8/qwak_inference/batch_client/file_serialization.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.7/qwak_inference/batch_client/instance_validation.py` & `qwak_inference-0.1.8/qwak_inference/batch_client/instance_validation.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.7/qwak_inference/configuration/account.py` & `qwak_inference-0.1.8/qwak_inference/configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.7/qwak_inference/configuration/auth.py` & `qwak_inference-0.1.8/qwak_inference/configuration/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.7/qwak_inference/configuration/session.py` & `qwak_inference-0.1.8/qwak_inference/configuration/session.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.7/qwak_inference/constants.py` & `qwak_inference-0.1.8/qwak_inference/constants.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.7/qwak_inference/exceptions.py` & `qwak_inference-0.1.8/qwak_inference/exceptions.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.7/qwak_inference/feedback_client.py` & `qwak_inference-0.1.8/qwak_inference/feedback_client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.7/qwak_inference/realtime_client/client.py` & `qwak_inference-0.1.8/qwak_inference/realtime_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.7/qwak_inference/realtime_client/rest_helpers.py` & `qwak_inference-0.1.8/qwak_inference/realtime_client/rest_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.7/setup.py` & `qwak_inference-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'feedback:python_version >= "3.10"': ['qwak-core>=0.0.147',
                                        'qwak-core>=0.0.147'],
  'feedback:python_version >= "3.8" and python_version < "3.12"': ['pandas>=1.4.0',
                                                                   'pandas>=1.4.0']}
 
 setup_kwargs = {
     'name': 'qwak-inference',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Qwak Inference is a Python library for running predictions again Qwak Models.',
     'long_description': '# Qwak Inference\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Inference contains tools that allow predicting against the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_inference-0.1.7/PKG-INFO` & `qwak_inference-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-inference
-Version: 0.1.7
+Version: 0.1.8
 Summary: Qwak Inference is a Python library for running predictions again Qwak Models.
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

