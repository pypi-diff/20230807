# Comparing `tmp/baram-0.3.1.tar.gz` & `tmp/baram-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baram-0.3.1.tar", max compression
+gzip compressed data, was "baram-0.3.2.tar", max compression
```

## Comparing `baram-0.3.1.tar` & `baram-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      660 2022-05-04 05:03:24.350145 baram-0.3.1/baram/airflow_manager.py
--rw-r--r--   0        0        0     1161 2022-05-31 00:21:03.987264 baram-0.3.1/baram/async_crawler.py
--rw-r--r--   0        0        0      644 2023-02-13 00:11:32.025035 baram-0.3.1/baram/conf_manager.py
--rw-r--r--   0        0        0    14117 2023-03-25 00:33:32.824139 baram-0.3.1/baram/ec2_manager.py
--rw-r--r--   0        0        0      773 2022-05-24 00:56:46.354660 baram-0.3.1/baram/ecr_manager.py
--rw-r--r--   0        0        0     2385 2023-03-15 07:55:06.640970 baram-0.3.1/baram/efs_manager.py
--rw-r--r--   0        0        0     7405 2022-05-24 00:56:46.354824 baram-0.3.1/baram/glue_manager.py
--rw-r--r--   0        0        0     3101 2023-03-25 00:11:36.843156 baram-0.3.1/baram/iam_manager.py
--rw-r--r--   0        0        0     1098 2022-05-04 05:35:56.208476 baram-0.3.1/baram/kms_manager.py
--rw-r--r--   0        0        0     2064 2022-05-06 01:06:54.382347 baram-0.3.1/baram/lambda_manager.py
--rw-r--r--   0        0        0      477 2022-05-06 01:06:54.382534 baram-0.3.1/baram/log_manager.py
--rw-r--r--   0        0        0      605 2022-05-04 05:35:56.213543 baram-0.3.1/baram/poetry_manager.py
--rw-r--r--   0        0        0      560 2022-05-04 05:23:44.845922 baram-0.3.1/baram/process_manager.py
--rw-r--r--   0        0        0      679 2023-02-13 00:11:32.025599 baram-0.3.1/baram/requests_manager.py
--rw-r--r--   0        0        0     9281 2022-06-28 04:05:40.812460 baram-0.3.1/baram/s3_manager.py
--rw-r--r--   0        0        0     7231 2023-03-15 07:55:06.641394 baram-0.3.1/baram/sagemaker_manager.py
--rw-r--r--   0        0        0      498 2023-03-25 00:34:46.444098 baram-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      224 2022-05-03 23:39:58.553478 baram-0.3.1/readme.md
--rw-r--r--   0        0        0     1020 2023-03-25 00:37:00.511358 baram-0.3.1/setup.py
--rw-r--r--   0        0        0      950 2023-03-25 00:37:00.511508 baram-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      660 2022-05-04 05:03:24.350145 baram-0.3.2/baram/airflow_manager.py
+-rw-r--r--   0        0        0     1161 2022-05-31 00:21:03.987264 baram-0.3.2/baram/async_crawler.py
+-rw-r--r--   0        0        0      644 2023-02-13 00:11:32.025035 baram-0.3.2/baram/conf_manager.py
+-rw-r--r--   0        0        0    14117 2023-08-07 01:33:48.528999 baram-0.3.2/baram/ec2_manager.py
+-rw-r--r--   0        0        0      773 2022-05-24 00:56:46.354660 baram-0.3.2/baram/ecr_manager.py
+-rw-r--r--   0        0        0     2385 2023-03-15 07:55:06.640970 baram-0.3.2/baram/efs_manager.py
+-rw-r--r--   0        0        0    15031 2023-08-05 15:07:15.520000 baram-0.3.2/baram/ge_manager.py
+-rw-r--r--   0        0        0     7405 2022-05-24 00:56:46.354824 baram-0.3.2/baram/glue_manager.py
+-rw-r--r--   0        0        0     3101 2023-03-25 00:11:36.843156 baram-0.3.2/baram/iam_manager.py
+-rw-r--r--   0        0        0     1098 2022-05-04 05:35:56.208476 baram-0.3.2/baram/kms_manager.py
+-rw-r--r--   0        0        0     2064 2022-05-06 01:06:54.382347 baram-0.3.2/baram/lambda_manager.py
+-rw-r--r--   0        0        0      477 2022-05-06 01:06:54.382534 baram-0.3.2/baram/log_manager.py
+-rw-r--r--   0        0        0      605 2022-05-04 05:35:56.213543 baram-0.3.2/baram/poetry_manager.py
+-rw-r--r--   0        0        0      560 2022-05-04 05:23:44.845922 baram-0.3.2/baram/process_manager.py
+-rw-r--r--   0        0        0      679 2023-02-13 00:11:32.025599 baram-0.3.2/baram/requests_manager.py
+-rw-r--r--   0        0        0     9281 2022-06-28 04:05:40.812460 baram-0.3.2/baram/s3_manager.py
+-rw-r--r--   0        0        0     7231 2023-03-15 07:55:06.641394 baram-0.3.2/baram/sagemaker_manager.py
+-rw-r--r--   0        0        0      566 2023-08-07 01:40:55.932601 baram-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      224 2022-05-03 23:39:58.553478 baram-0.3.2/readme.md
+-rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 baram-0.3.2/PKG-INFO
```

### Comparing `baram-0.3.1/baram/airflow_manager.py` & `baram-0.3.2/baram/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/baram/async_crawler.py` & `baram-0.3.2/baram/async_crawler.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/baram/conf_manager.py` & `baram-0.3.2/baram/conf_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/baram/ec2_manager.py` & `baram-0.3.2/baram/ec2_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/baram/ecr_manager.py` & `baram-0.3.2/baram/ecr_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/baram/efs_manager.py` & `baram-0.3.2/baram/efs_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/baram/glue_manager.py` & `baram-0.3.2/baram/glue_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/baram/iam_manager.py` & `baram-0.3.2/baram/iam_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/baram/kms_manager.py` & `baram-0.3.2/baram/kms_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/baram/lambda_manager.py` & `baram-0.3.2/baram/lambda_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/baram/poetry_manager.py` & `baram-0.3.2/baram/poetry_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/baram/process_manager.py` & `baram-0.3.2/baram/process_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/baram/requests_manager.py` & `baram-0.3.2/baram/requests_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/baram/s3_manager.py` & `baram-0.3.2/baram/s3_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/baram/sagemaker_manager.py` & `baram-0.3.2/baram/sagemaker_manager.py`

 * *Files identical despite different names*

### Comparing `baram-0.3.1/PKG-INFO` & `baram-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: baram
-Version: 0.3.1
+Version: 0.3.2
 Summary: AWS Framework for python
 Author: Kwangsik Lee
 Author-email: lks21c@gmail.com
-Requires-Python: >=3.7.10,<4.0.0
+Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: boto3 (==1.26.74)
 Requires-Dist: fire (>=0.4.0,<0.5.0)
+Requires-Dist: great-expectations (==0.17.8)
 Requires-Dist: nest-asyncio (>=1.5.5,<2.0.0)
+Requires-Dist: pyathena (==3.0.6)
 Requires-Dist: pytest-cov (>=3.0.0,<4.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: sqlalchemy (==1.4.49)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: ujson (>=5.5.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 ## Baram
 
 Cloud Framework for AWS Framework.
```

