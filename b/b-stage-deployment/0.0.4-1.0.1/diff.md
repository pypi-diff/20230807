# Comparing `tmp/b_stage_deployment-0.0.4.tar.gz` & `tmp/b_stage_deployment-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/b_stage_deployment-0.0.4.tar", last modified: Mon Feb  1 11:11:01 2021, max compression
+gzip compressed data, was "b_stage_deployment-1.0.1.tar", last modified: Mon Aug  7 13:33:57 2023, max compression
```

## Comparing `b_stage_deployment-0.0.4.tar` & `b_stage_deployment-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 11:11:01.321834 b_stage_deployment-0.0.4/
--rw-rw-r--   0 root         (0) root         (0)      163 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/HISTORY.md
--rw-rw-r--   0 root         (0) root         (0)    11357 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      112 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      810 2021-02-01 11:11:01.321834 b_stage_deployment-0.0.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)        6 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/README.md
--rw-rw-r--   0 root         (0) root         (0)        5 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 11:11:01.321834 b_stage_deployment-0.0.4/b_stage_deployment/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/b_stage_deployment/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1741 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/b_stage_deployment/function.py
--rw-rw-r--   0 root         (0) root         (0)     1388 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/b_stage_deployment/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 11:11:01.321834 b_stage_deployment-0.0.4/b_stage_deployment/source/
--rw-rw-r--   0 root         (0) root         (0)       61 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/b_stage_deployment/source/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2564 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/b_stage_deployment/source/action.py
--rw-rw-r--   0 root         (0) root         (0)     3112 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/b_stage_deployment/source/cfnresponse.py
--rw-rw-r--   0 root         (0) root         (0)     2175 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/b_stage_deployment/source/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 11:11:01.321834 b_stage_deployment-0.0.4/b_stage_deployment.egg-info/
--rw-r--r--   0 root         (0) root         (0)      810 2021-02-01 11:11:01.000000 b_stage_deployment-0.0.4/b_stage_deployment.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      598 2021-02-01 11:11:01.000000 b_stage_deployment-0.0.4/b_stage_deployment.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-01 11:11:01.000000 b_stage_deployment-0.0.4/b_stage_deployment.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      183 2021-02-01 11:11:01.000000 b_stage_deployment-0.0.4/b_stage_deployment.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       43 2021-02-01 11:11:01.000000 b_stage_deployment-0.0.4/b_stage_deployment.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 11:11:01.317834 b_stage_deployment-0.0.4/b_stage_deployment_test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 11:11:01.321834 b_stage_deployment-0.0.4/b_stage_deployment_test/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/b_stage_deployment_test/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      746 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/b_stage_deployment_test/tests/test_deployed.py
--rw-r--r--   0 root         (0) root         (0)       38 2021-02-01 11:11:01.321834 b_stage_deployment-0.0.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1419 2021-02-01 11:07:45.000000 b_stage_deployment-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:33:57.219616 b_stage_deployment-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-07 13:33:57.219616 b_stage_deployment-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:33:57.215616 b_stage_deployment-1.0.1/b_stage_deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/b_stage_deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/b_stage_deployment/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/b_stage_deployment/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:33:57.215616 b_stage_deployment-1.0.1/b_stage_deployment/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/b_stage_deployment/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/b_stage_deployment/source/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/b_stage_deployment/source/cfnresponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/b_stage_deployment/source/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:33:57.215616 b_stage_deployment-1.0.1/b_stage_deployment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-07 13:33:57.000000 b_stage_deployment-1.0.1/b_stage_deployment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-07 13:33:57.000000 b_stage_deployment-1.0.1/b_stage_deployment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:33:57.000000 b_stage_deployment-1.0.1/b_stage_deployment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-07 13:33:57.000000 b_stage_deployment-1.0.1/b_stage_deployment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 13:33:57.000000 b_stage_deployment-1.0.1/b_stage_deployment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:33:57.215616 b_stage_deployment-1.0.1/b_stage_deployment_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:33:57.219616 b_stage_deployment-1.0.1/b_stage_deployment_test/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/b_stage_deployment_test/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/b_stage_deployment_test/tests/test_deployed.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:33:57.219616 b_stage_deployment-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-08-07 13:30:13.000000 b_stage_deployment-1.0.1/setup.py
```

### Comparing `b_stage_deployment-0.0.4/LICENSE` & `b_stage_deployment-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `b_stage_deployment-0.0.4/b_stage_deployment/function.py` & `b_stage_deployment-1.0.1/b_stage_deployment/function.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import lru_cache
 
+from aws_cdk import Stack, Duration
 from aws_cdk.aws_iam import PolicyStatement
 from aws_cdk.aws_lambda import Code, SingletonFunction, Runtime
-from aws_cdk.core import Stack, Duration
 
 
 class StageDeploymentSingletonFunction(SingletonFunction):
     """
     Custom api gateway stage deployment resource singleton lambda function.
     """
```

### Comparing `b_stage_deployment-0.0.4/b_stage_deployment/resource.py` & `b_stage_deployment-1.0.1/b_stage_deployment/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from aws_cdk.core import Stack, CustomResource, RemovalPolicy
+from aws_cdk import Stack, CustomResource, RemovalPolicy
 
 from b_stage_deployment.function import StageDeploymentSingletonFunction
 
 
 class StageDeploymentResource(CustomResource):
     """
     Custom resource used for create a custom stage deployment.
```

### Comparing `b_stage_deployment-0.0.4/b_stage_deployment/source/action.py` & `b_stage_deployment-1.0.1/b_stage_deployment/source/action.py`

 * *Files identical despite different names*

### Comparing `b_stage_deployment-0.0.4/b_stage_deployment/source/cfnresponse.py` & `b_stage_deployment-1.0.1/b_stage_deployment/source/cfnresponse.py`

 * *Files identical despite different names*

### Comparing `b_stage_deployment-0.0.4/b_stage_deployment/source/index.py` & `b_stage_deployment-1.0.1/b_stage_deployment/source/index.py`

 * *Files identical despite different names*

### Comparing `b_stage_deployment-0.0.4/b_stage_deployment.egg-info/SOURCES.txt` & `b_stage_deployment-1.0.1/b_stage_deployment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `b_stage_deployment-0.0.4/b_stage_deployment_test/tests/test_deployed.py` & `b_stage_deployment-1.0.1/b_stage_deployment_test/tests/test_deployed.py`

 * *Files identical despite different names*

### Comparing `b_stage_deployment-0.0.4/setup.py` & `b_stage_deployment-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,21 +25,18 @@
         'has too many bugs.'
     ),
     long_description=README + '\n\n' + HISTORY,
     long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=[
         'boto3>=1.16.0,<2.0.0',
-        'pytest>=6.0.2,<7.0.0',
-        'b-aws-testing-framework>=0.0.24,<1.0.0',
 
         # AWS CDK.
-        'aws-cdk.core>=1.75.0,<2.0.0',
-        'aws-cdk.aws-apigatewayv2>=1.75.0,<2.0.0',
-        'aws-cdk.aws-lambda>=1.75.0,<2.0.0',
+        'aws-cdk-lib>=2.0.0,<3.0.0',
+        'aws-cdk-constructs>=2.0.0,<3.0.0',
     ],
     author='Laimonas Sutkus',
     author_email='laimonas.sutkus@biomapas.com',
     keywords='AWS API Gateway Stage Deployment',
     url='https://github.com/biomapas/B.StageDeployment.git',
     classifiers=[
         'Programming Language :: Python :: 3',
```

