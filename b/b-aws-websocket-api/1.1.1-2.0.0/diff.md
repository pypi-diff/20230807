# Comparing `tmp/b_aws_websocket_api-1.1.1.tar.gz` & `tmp/b_aws_websocket_api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/b_aws_websocket_api-1.1.1.tar", last modified: Thu Feb 11 18:30:36 2021, max compression
+gzip compressed data, was "b_aws_websocket_api-2.0.0.tar", last modified: Mon Aug  7 14:12:31 2023, max compression
```

## Comparing `b_aws_websocket_api-1.1.1.tar` & `b_aws_websocket_api-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-11 18:30:36.149635 b_aws_websocket_api-1.1.1/
--rw-rw-r--   0 root         (0) root         (0)      768 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/HISTORY.md
--rw-rw-r--   0 root         (0) root         (0)    11357 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      113 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7972 2021-02-11 18:30:36.149635 b_aws_websocket_api-1.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4802 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/README.md
--rw-rw-r--   0 root         (0) root         (0)        5 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-11 18:30:36.149635 b_aws_websocket_api-1.1.1/b_aws_websocket_api/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2102 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api/ws_api.py
--rw-rw-r--   0 root         (0) root         (0)     1291 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api/ws_deployment.py
--rw-rw-r--   0 root         (0) root         (0)     6264 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api/ws_function.py
--rw-rw-r--   0 root         (0) root         (0)     4601 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api/ws_integration.py
--rw-rw-r--   0 root         (0) root         (0)     1860 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api/ws_lambda_integration.py
--rw-rw-r--   0 root         (0) root         (0)     3683 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api/ws_route.py
--rw-rw-r--   0 root         (0) root         (0)     5991 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api/ws_stage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-11 18:30:36.149635 b_aws_websocket_api-1.1.1/b_aws_websocket_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7972 2021-02-11 18:30:36.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      710 2021-02-11 18:30:36.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-11 18:30:36.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      315 2021-02-11 18:30:36.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2021-02-11 18:30:36.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-11 18:30:36.145635 b_aws_websocket_api-1.1.1/b_aws_websocket_api_test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-11 18:30:36.149635 b_aws_websocket_api-1.1.1/b_aws_websocket_api_test/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api_test/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      733 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api_test/tests/test_invoke_function.py
--rw-rw-r--   0 root         (0) root         (0)     1502 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/b_aws_websocket_api_test/tests/test_websocket_connection.py
--rw-r--r--   0 root         (0) root         (0)       38 2021-02-11 18:30:36.149635 b_aws_websocket_api-1.1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1578 2021-02-11 18:26:52.000000 b_aws_websocket_api-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:12:31.130461 b_aws_websocket_api-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-08-07 14:12:31.130461 b_aws_websocket_api-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:12:31.130461 b_aws_websocket_api-2.0.0/b_aws_websocket_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api/ws_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api/ws_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api/ws_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api/ws_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api/ws_lambda_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api/ws_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api/ws_stage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:12:31.130461 b_aws_websocket_api-2.0.0/b_aws_websocket_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-08-07 14:12:31.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-07 14:12:31.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:12:31.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-07 14:12:31.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-07 14:12:31.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:12:31.130461 b_aws_websocket_api-2.0.0/b_aws_websocket_api_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:12:31.130461 b_aws_websocket_api-2.0.0/b_aws_websocket_api_test/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api_test/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api_test/tests/test_invoke_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/b_aws_websocket_api_test/tests/test_websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 14:12:31.130461 b_aws_websocket_api-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-07 14:09:15.000000 b_aws_websocket_api-2.0.0/setup.py
```

### Comparing `b_aws_websocket_api-1.1.1/LICENSE` & `b_aws_websocket_api-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b_aws_websocket_api-1.1.1/README.md` & `b_aws_websocket_api-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `b_aws_websocket_api-1.1.1/b_aws_websocket_api/ws_api.py` & `b_aws_websocket_api-2.0.0/b_aws_websocket_api/ws_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Any
 
+from aws_cdk import Stack
 from aws_cdk.aws_apigatewayv2 import CfnApi
-from aws_cdk.core import Stack
 
 
 class WsApi(CfnApi):
     """
     Creates a web socket api.
     """
```

### Comparing `b_aws_websocket_api-1.1.1/b_aws_websocket_api/ws_deployment.py` & `b_aws_websocket_api-2.0.0/b_aws_websocket_api/ws_deployment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Optional
 
-from aws_cdk.core import Stack, Construct
+from aws_cdk import Stack
 from b_stage_deployment.function import StageDeploymentSingletonFunction
 from b_stage_deployment.resource import StageDeploymentResource
+from constructs import Construct
+
 from b_aws_websocket_api.ws_stage import WsStage
 
 
 class WsDeployment(Construct):
     """
     Creates web socket api deployment.
     """
```

### Comparing `b_aws_websocket_api-1.1.1/b_aws_websocket_api/ws_function.py` & `b_aws_websocket_api-2.0.0/b_aws_websocket_api/ws_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import hashlib
 from typing import Optional, Mapping, List
 
+from aws_cdk import Stack, Duration
 from aws_cdk.aws_ec2 import ISecurityGroup, IVpc, SubnetSelection
 from aws_cdk.aws_iam import PolicyStatement, IRole
 from aws_cdk.aws_lambda import *
 from aws_cdk.aws_logs import RetentionDays
 from aws_cdk.aws_sqs import IQueue
-from aws_cdk.core import Stack, Duration
 from jsii import Number
 
 
 class WsFunction(Function):
     """
     Creates a lambda function which is API Gateway friendly.
     """
@@ -130,12 +130,12 @@
             function_name=self.function_name,
             principal='apigateway.amazonaws.com',
         )
 
     @property
     def hash(self):
         hashable = (
-               self.__id +
-               self.__name
+                self.__id +
+                self.__name
         ).encode('utf-8')
 
         return hashlib.sha256(hashable).hexdigest()
```

### Comparing `b_aws_websocket_api-1.1.1/b_aws_websocket_api/ws_integration.py` & `b_aws_websocket_api-2.0.0/b_aws_websocket_api/ws_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Any
 
+from aws_cdk import Stack
 from aws_cdk.aws_apigatewayv2 import CfnIntegration, CfnIntegrationResponse
-from aws_cdk.core import Stack
 from jsii import Number
 
 from b_aws_websocket_api.ws_api import WsApi
 
 
 class WsIntegration(CfnIntegration):
     """
```

### Comparing `b_aws_websocket_api-1.1.1/b_aws_websocket_api/ws_lambda_integration.py` & `b_aws_websocket_api-2.0.0/b_aws_websocket_api/ws_lambda_integration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import hashlib
 from typing import Union
 
+from aws_cdk import Stack
 from aws_cdk.aws_lambda import IFunction
-from aws_cdk.core import Stack
+
 from b_aws_websocket_api.ws_function import WsFunction
 from b_aws_websocket_api.ws_integration import WsIntegration
 
 
 class WsLambdaIntegration(WsIntegration):
     """
     Creates web socket API route lambda integration.
@@ -52,12 +53,12 @@
     @property
     def function(self):
         return self.__function
 
     @property
     def hash(self):
         hashable = (
-               self.__id +
-               self.__integration_name
+                self.__id +
+                self.__integration_name
         ).encode('utf-8')
 
         return hashlib.sha256(hashable).hexdigest()
```

### Comparing `b_aws_websocket_api-1.1.1/b_aws_websocket_api/ws_route.py` & `b_aws_websocket_api-2.0.0/b_aws_websocket_api/ws_route.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import hashlib
 from typing import Optional, List, Any
 
+from aws_cdk import Stack
 from aws_cdk.aws_apigatewayv2 import CfnRoute, CfnRouteResponse
-from aws_cdk.core import Stack
 
 from b_aws_websocket_api.ws_api import WsApi
 
 
 class WsRoute(CfnRoute):
     """
     Creates a route for a web socket API.
@@ -83,12 +83,12 @@
                 route_id=self.ref,
                 route_response_key='$default',
             )
 
     @property
     def hash(self):
         hashable = (
-               self.__id +
-               self.__route_key
+                self.__id +
+                self.__route_key
         ).encode('utf-8')
 
         return hashlib.sha256(hashable).hexdigest()
```

### Comparing `b_aws_websocket_api-1.1.1/b_aws_websocket_api/ws_stage.py` & `b_aws_websocket_api-2.0.0/b_aws_websocket_api/ws_stage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Dict, Any
 
+from aws_cdk import CfnOutput, RemovalPolicy, Stack
 from aws_cdk.aws_apigatewayv2 import CfnStage
 from aws_cdk.aws_logs import RetentionDays, LogGroup
-from aws_cdk.core import CfnOutput, RemovalPolicy, Stack
 
 from b_aws_websocket_api.ws_api import WsApi
 
 
 class WsStage(CfnStage):
     """
     Creates a web socket api stage.
```

### Comparing `b_aws_websocket_api-1.1.1/b_aws_websocket_api.egg-info/SOURCES.txt` & `b_aws_websocket_api-2.0.0/b_aws_websocket_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `b_aws_websocket_api-1.1.1/b_aws_websocket_api_test/tests/test_invoke_function.py` & `b_aws_websocket_api-2.0.0/b_aws_websocket_api_test/tests/test_invoke_function.py`

 * *Files identical despite different names*

### Comparing `b_aws_websocket_api-1.1.1/b_aws_websocket_api_test/tests/test_websocket_connection.py` & `b_aws_websocket_api-2.0.0/b_aws_websocket_api_test/tests/test_websocket_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import json
 import logging
 import time
+
 import websockets
 
 from b_aws_websocket_api_test.infrastructure import Infrastructure
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
@@ -34,15 +35,15 @@
             async with websockets.connect(websocket_url, **timeouts) as websocket:
                 await websocket.send(json.dumps(dict(action='test')))
 
                 data = await websocket.recv()
                 logger.info(f'Received data: {data}.')
 
                 assert json.loads(data)['message'] == 'success'
-        except websockets.exceptions.InvalidStatusCode as ex:
+        except websockets.InvalidStatusCode as ex:
             logger.error(f'Status code from WS API: {ex}. Retrying...')
 
             time.sleep(sleep_seconds)
 
             current_attempt += 1
 
             await hello(current_attempt, max_attempts, sleep_seconds)
```

### Comparing `b_aws_websocket_api-1.1.1/setup.py` & `b_aws_websocket_api-2.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,25 +24,22 @@
         'AWS CDK package that helps creating web socket APIs.'
     ),
     long_description=README + '\n\n' + HISTORY,
     long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=[
         # AWS CDK.
-        'aws-cdk.core>=1.60.0,<2.0.0',
-        'aws_cdk.aws_apigatewayv2>=1.60.0,<2.0.0',
-        'aws-cdk.aws-lambda>=1.60.0,<2.0.0',
-        'aws-cdk.custom_resources>=1.60.0,<2.0.0',
+        'aws-cdk-lib>=2.0.0,<3.0.0',
+        'aws-cdk-constructs>=2.0.0,<3.0.0',
 
         # Our.
-        'b-aws-testing-framework>=0.0.23,<2.0.0',
-        'b-stage-deployment>=0.0.2,<1.0.0',
+        'b-stage-deployment>=1.0.0,<2.0.0',
 
         # Other.
-        'websockets>=8.0.0,<9.0.0',
+        'websockets>=11.0.0,<12.0.0',
         'pytest>=6.0.2,<7.0.0',
         'pytest-cov>=2.10.1,<3.0.0',
         'pytest-timeout>=1.3.4,<1.5.0'
     ],
     author='Laimonas Sutkus',
     author_email='laimonas.sutkus@biomapas.com',
     keywords='AWS CDK API WebSocket',
```

