# Comparing `tmp/seven2one-4.2.0.tar.gz` & `tmp/seven2one-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seven2one-4.2.0.tar", last modified: Mon May 22 08:35:18 2023, max compression
+gzip compressed data, was "seven2one-4.3.0.tar", last modified: Mon Aug  7 11:33:04 2023, max compression
```

## Comparing `seven2one-4.2.0.tar` & `seven2one-4.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-05-22 08:35:18.712959 seven2one-4.2.0/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1105 2023-04-14 08:32:42.000000 seven2one-4.2.0/LICENSE
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-14 08:32:42.000000 seven2one-4.2.0/MANIFEST.in
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3179 2023-05-22 08:35:18.712959 seven2one-4.2.0/PKG-INFO
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2726 2023-05-22 07:46:14.000000 seven2one-4.2.0/README.md
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       38 2023-05-22 08:35:18.712959 seven2one-4.2.0/setup.cfg
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1388 2023-04-25 08:08:15.000000 seven2one-4.2.0/setup.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-05-22 08:35:18.708959 seven2one-4.2.0/seven2one/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       51 2023-05-22 08:35:13.000000 seven2one-4.2.0/seven2one/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15405 2023-04-25 08:08:15.000000 seven2one-4.2.0/seven2one/authorization.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    10848 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/automation.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    64496 2023-05-22 07:46:14.000000 seven2one-4.2.0/seven2one/core.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3769 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/email.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1549 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/fileImportService.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    53999 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/fileimport.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-05-22 08:35:18.712959 seven2one-4.2.0/seven2one/logging_loki/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      189 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/logging_loki/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      756 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/logging_loki/const.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5177 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/logging_loki/emitter.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2929 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/logging_loki/handlers.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15392 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/programming.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     9486 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/schedule.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    61479 2023-04-25 08:08:15.000000 seven2one-4.2.0/seven2one/timeseries.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-05-22 08:35:18.712959 seven2one-4.2.0/seven2one/utils/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       21 2023-05-22 08:35:13.000000 seven2one-4.2.0/seven2one/utils/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    35567 2023-04-25 08:08:15.000000 seven2one-4.2.0/seven2one/utils/ut.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1832 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/utils/ut_autprog.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    26023 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/utils/ut_fileimport.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5856 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/utils/ut_init.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      989 2023-04-25 08:08:15.000000 seven2one-4.2.0/seven2one/utils/ut_log.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     4229 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/utils/ut_meta.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3435 2023-04-14 08:32:42.000000 seven2one-4.2.0/seven2one/utils/ut_time.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     6567 2023-04-25 08:08:15.000000 seven2one-4.2.0/seven2one/utils/ut_timeseries.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-05-22 08:35:18.712959 seven2one-4.2.0/seven2one.egg-info/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3179 2023-05-22 08:35:18.000000 seven2one-4.2.0/seven2one.egg-info/PKG-INFO
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      859 2023-05-22 08:35:18.000000 seven2one-4.2.0/seven2one.egg-info/SOURCES.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-05-22 08:35:18.000000 seven2one-4.2.0/seven2one.egg-info/dependency_links.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-05-22 08:35:18.000000 seven2one-4.2.0/seven2one.egg-info/not-zip-safe
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       97 2023-05-22 08:35:18.000000 seven2one-4.2.0/seven2one.egg-info/requires.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       10 2023-05-22 08:35:18.000000 seven2one-4.2.0/seven2one.egg-info/top_level.txt
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-07 11:33:04.803949 seven2one-4.3.0/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1105 2023-08-07 11:26:59.000000 seven2one-4.3.0/LICENSE
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-07 11:26:59.000000 seven2one-4.3.0/MANIFEST.in
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3179 2023-08-07 11:33:04.803949 seven2one-4.3.0/PKG-INFO
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2726 2023-08-07 11:26:59.000000 seven2one-4.3.0/README.md
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       38 2023-08-07 11:33:04.803949 seven2one-4.3.0/setup.cfg
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1388 2023-08-07 11:26:59.000000 seven2one-4.3.0/setup.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-07 11:33:04.799949 seven2one-4.3.0/seven2one/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       51 2023-08-07 11:32:59.000000 seven2one-4.3.0/seven2one/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15405 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/authorization.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    11073 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/automation.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    64496 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/core.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3769 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/email.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1549 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/fileImportService.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    53999 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/fileimport.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-07 11:33:04.803949 seven2one-4.3.0/seven2one/logging_loki/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      189 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/logging_loki/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      756 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/logging_loki/const.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5177 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/logging_loki/emitter.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2929 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/logging_loki/handlers.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15392 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/programming.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     9486 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/schedule.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    61479 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/timeseries.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-07 11:33:04.803949 seven2one-4.3.0/seven2one/utils/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       21 2023-08-07 11:32:59.000000 seven2one-4.3.0/seven2one/utils/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    35567 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1832 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut_autprog.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    26023 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut_fileimport.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5856 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut_init.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      989 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut_log.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     4229 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut_meta.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3435 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut_time.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     6567 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut_timeseries.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-07 11:33:04.799949 seven2one-4.3.0/seven2one.egg-info/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3179 2023-08-07 11:33:04.000000 seven2one-4.3.0/seven2one.egg-info/PKG-INFO
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      859 2023-08-07 11:33:04.000000 seven2one-4.3.0/seven2one.egg-info/SOURCES.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-08-07 11:33:04.000000 seven2one-4.3.0/seven2one.egg-info/dependency_links.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-08-07 11:33:04.000000 seven2one-4.3.0/seven2one.egg-info/not-zip-safe
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       97 2023-08-07 11:33:04.000000 seven2one-4.3.0/seven2one.egg-info/requires.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       10 2023-08-07 11:33:04.000000 seven2one-4.3.0/seven2one.egg-info/top_level.txt
```

### Comparing `seven2one-4.2.0/LICENSE` & `seven2one-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/PKG-INFO` & `seven2one-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven2one
-Version: 4.2.0
+Version: 4.3.0
 Summary: Functions to interact with the Seven2one TechStack
 Home-page: http://www.seven2one.de
 Author: Seven2one Informationssysteme GmbH
 Author-email: info@seven2one.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `seven2one-4.2.0/README.md` & `seven2one-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/setup.py` & `seven2one-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/authorization.py` & `seven2one-4.3.0/seven2one/authorization.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/automation.py` & `seven2one-4.3.0/seven2one/automation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from uuid import uuid4
 import pandas as pd
 from loguru import logger
 
 from .utils.ut import Utils
 from .utils.ut_autprog import AutProgUtils
 
+
 class Automation():
     accessToken = ''
 
-    def __init__(self, accessToken:str, endpoint:str, client:object) -> None:
-        
+    def __init__(self, accessToken: str, endpoint: str, client: object) -> None:
+
         self.raiseException = client.raiseException
         self.defaults = client.defaults
 
         self.accessToken = accessToken
         self.endpoint = endpoint
         self.proxies = client.proxies
 
@@ -33,63 +34,67 @@
                 name
                 description
                 }}
             }}
             '''
 
         result = Utils._executeGraphQL(self, graphQLString)
-        if result == None: return
+        if result == None:
+            return
 
         df = pd.json_normalize(result['workflows'])
         return df
 
-    def workflowInstances(self, workflowId:str=None, fromTimepoint:str=None, toTimepoint:str=None, 
-        fields:list=None, where:str=None, showTasks=False) -> pd.DataFrame:
+    def workflowInstances(self, workflowId: str = None, fromTimepoint: str = None, toTimepoint: str = None,
+                          fields: list = None, where: str = None, showTasks=False, skip=0, take=50) -> pd.DataFrame:
         """Shows Instances of a workflow. If workflowId=None, all Instances of all 
         workflows will be returned."""
 
-        meta = ['id', 'name', 'businessKey', 'version', 'startTime', 'endTime', 'state']
+        meta = ['id', 'name', 'businessKey',
+                'version', 'startTime', 'endTime', 'state']
         key = 'workflowInstances'
 
         if workflowId != None:
             _workflowId = f'workflowId: "{workflowId}"'
         else:
             _workflowId = ''
 
         if fromTimepoint != None:
             _fromTimepoint = f'from: "{fromTimepoint}"'
-        else: 
+        else:
             _fromTimepoint = ''
 
         if toTimepoint != None:
             _toTimepoint = f'from: "{toTimepoint}"'
-        else: 
+        else:
             _toTimepoint = ''
 
         if fields != None:
             if type(fields) != list:
                 fields = [fields]
-            _fields = Utils._queryFields(fields, recursive=True)   
+            _fields = Utils._queryFields(fields, recursive=True)
         else:
-            _fields =f'''
+            _fields = f'''
                 id
+                workflowId
                 name
                 businessKey
                 version
                 startTime
                 endTime
+                duration
                 state
                 variables {{
                     name
                     value
                     time
-                }}''' 
+                }}'''
 
         resolvedFilter = ''
-        if where != None: 
+        if where != None:
             resolvedFilter = Utils._resolveWhereString(where)
 
         if showTasks != False:
             _tasks = f'''tasks {{
                             id
                             topic
                             workerId
@@ -98,38 +103,42 @@
                             retries
                             errorMessage
                         }}'''
         else:
             _tasks = ''
 
         graphQLString = f'''query Instances {{
-            {key}({_workflowId}, {_fromTimepoint}, {_toTimepoint}, {resolvedFilter}, all:true) {{
+            {key}(skip: {skip} take: {take} {_workflowId} {_fromTimepoint} {_toTimepoint} {resolvedFilter}) {{
+            items {{
                 {_fields}
                 {_tasks}
                 }}
             }}
-            '''
-     
+        }}
+        '''
+
         result = Utils._executeGraphQL(self, graphQLString)
-        if result == None: return
+        if result == None:
+            return
 
         if showTasks != False:
-            df = pd.json_normalize(result[key], meta=meta, record_path=['tasks'], record_prefix='task.', errors='ignore')
+            df = pd.json_normalize(result[key]['items'], meta=meta, record_path=[
+                                   'tasks'], record_prefix='task.', errors='ignore')
             if 'startTime' in df.columns:
                 df = df.sort_values(by='startTime', ascending=False)
         else:
-            df = pd.json_normalize(result[key])
+            df = pd.json_normalize(result[key]['items'])
             if 'startTime' in df.columns:
                 df = df.sort_values(by='startTime', ascending=False)
         return df
-    
-    def createWorkflow(self, id, name, description:str=None):
+
+    def createWorkflow(self, id, name, description: str = None):
 
         correlationId = str(uuid4())
-        context_logger = logger.bind(correlation_id = correlationId)
+        context_logger = logger.bind(correlation_id=correlationId)
 
         graphQLString = f'''mutation createWorkflow {{
             createWorkflow(
                 input: {{
                     id: "{id}"
                     name: "{name}"
                     description: "{description}"
@@ -142,27 +151,28 @@
                         workflow {{
                             id
                         }}
                     }}
                 }}
             }}
         '''
-        
+
         result = Utils._executeGraphQL(self, graphQLString)
-        if result == None: return
+        if result == None:
+            return
 
         context_logger.info(f"New workflow {id} created.")
 
         return result
-                        
-    def deployWorkflow(self, workflowId:str, filePath:str) -> None:
+
+    def deployWorkflow(self, workflowId: str, filePath: str) -> None:
         """Deploys a Camunda XML to an existing workflow"""
 
         correlationId = str(uuid4())
-        context_logger = logger.bind(correlation_id = correlationId)
+        context_logger = logger.bind(correlation_id=correlationId)
 
         fileContent = Utils._encodeBase64(filePath)
         context_logger.debug(f"fileContent: {fileContent[:10]}")
 
         graphQLString = f'''mutation deployWorkflow {{
             deployWorkflow(
                 input: {{
@@ -182,24 +192,25 @@
                     version
                 }}
             }}
         }}
         '''
 
         result = Utils._executeGraphQL(self, graphQLString)
-        if result == None: return
+        if result == None:
+            return
 
         context_logger.info(f"Workflow '{workflowId}' deployed.")
         return result
 
-    def startWorkflow(self, workflowId:str, businessKey:str, inputVariables:dict=None):
+    def startWorkflow(self, workflowId: str, businessKey: str, inputVariables: dict = None):
         """Starts a workflow"""
 
         correlationId = str(uuid4())
-        context_logger = logger.bind(correlation_id = correlationId)
+        context_logger = logger.bind(correlation_id=correlationId)
 
         if inputVariables == None:
             _vars = ''
         else:
             _vars = AutProgUtils._varsToString(inputVariables, 'input')
 
         graphQLString = f'''
@@ -221,25 +232,26 @@
                         workflowInstanceId
                         }}
                     }}
                 }}
             '''
 
         result = Utils._executeGraphQL(self, graphQLString)
-        if result == None: return
+        if result == None:
+            return
 
         context_logger.info(f"Workflow {workflowId} started.")
 
         return result
 
-    def deleteWorkflow(self, workflowId:str):
+    def deleteWorkflow(self, workflowId: str):
         """Deletes a workflow"""
 
         correlationId = str(uuid4())
-        context_logger = logger.bind(correlation_id = correlationId)
+        context_logger = logger.bind(correlation_id=correlationId)
 
         graphQLString = f'''mutation deleteWorkflow {{
             deleteWorkflow (id: "{workflowId}")
             {{
                 ... on DeleteWorkflowError {{
                     message
                     }}
@@ -259,15 +271,15 @@
         context_logger.info(f"Workflow {workflowId} deleted.")
         return result
 
     def terminateWorkflowInstance(self, workflowInstanceId):
         """Terminates a workflow instance"""
 
         correlationId = str(uuid4())
-        context_logger = logger.bind(correlation_id = correlationId)
+        context_logger = logger.bind(correlation_id=correlationId)
 
         graphQLString = f'''mutation terminateWorkflowInstance {{
             terminateWorkflowInstance(
                 workflowInstanceId:"{workflowInstanceId}") {{
                 ...on TerminateWorkflowInstanceError {{
                     message
                     }}
@@ -282,19 +294,19 @@
             }}
         '''
 
         result = Utils._executeGraphQL(self, graphQLString)
         context_logger.info(f"Workflow instance {workflowInstanceId} started.")
         return result
 
-    def updateWorkflow(self, workflowId:str, name:str=None, description:str=None):
+    def updateWorkflow(self, workflowId: str, name: str = None, description: str = None):
         """Updates a workflow (name and description can be changed)"""
 
         correlationId = str(uuid4())
-        context_logger = logger.bind(correlation_id = correlationId)
+        context_logger = logger.bind(correlation_id=correlationId)
 
         name = Utils._argNone('name', name)
         description = Utils._argNone('description', description)
 
         key = 'updateWorkflow'
         graphQLString = f'''mutation updateWorkflow {{
             {key}(workflowId: "{workflowId}", properties: {{
@@ -323,15 +335,15 @@
         context_logger.info(f"Workflow {workflowId} updated.")
         return result
 
     def retryTask(self, externalTaskId):
         key = 'retryTask'
 
         correlationId = str(uuid4())
-        context_logger = logger.bind(correlation_id = correlationId)
+        context_logger = logger.bind(correlation_id=correlationId)
 
         graphQLString = f'''mutation retryTask {{
             {key}(externalTaskId: "{externalTaskId}") {{
                 ... on RetryTaskError {{
                 message
                 }}
                 ...on TaskNotFound {{
```

### Comparing `seven2one-4.2.0/seven2one/core.py` & `seven2one-4.3.0/seven2one/core.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/email.py` & `seven2one-4.3.0/seven2one/email.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/fileImportService.py` & `seven2one-4.3.0/seven2one/fileImportService.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/fileimport.py` & `seven2one-4.3.0/seven2one/fileimport.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/logging_loki/const.py` & `seven2one-4.3.0/seven2one/logging_loki/const.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/logging_loki/emitter.py` & `seven2one-4.3.0/seven2one/logging_loki/emitter.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/logging_loki/handlers.py` & `seven2one-4.3.0/seven2one/logging_loki/handlers.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/programming.py` & `seven2one-4.3.0/seven2one/programming.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/schedule.py` & `seven2one-4.3.0/seven2one/schedule.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/timeseries.py` & `seven2one-4.3.0/seven2one/timeseries.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/utils/ut.py` & `seven2one-4.3.0/seven2one/utils/ut.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/utils/ut_autprog.py` & `seven2one-4.3.0/seven2one/utils/ut_autprog.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/utils/ut_fileimport.py` & `seven2one-4.3.0/seven2one/utils/ut_fileimport.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/utils/ut_init.py` & `seven2one-4.3.0/seven2one/utils/ut_init.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/utils/ut_log.py` & `seven2one-4.3.0/seven2one/utils/ut_log.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/utils/ut_meta.py` & `seven2one-4.3.0/seven2one/utils/ut_meta.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/utils/ut_time.py` & `seven2one-4.3.0/seven2one/utils/ut_time.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one/utils/ut_timeseries.py` & `seven2one-4.3.0/seven2one/utils/ut_timeseries.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.2.0/seven2one.egg-info/PKG-INFO` & `seven2one-4.3.0/seven2one.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven2one
-Version: 4.2.0
+Version: 4.3.0
 Summary: Functions to interact with the Seven2one TechStack
 Home-page: http://www.seven2one.de
 Author: Seven2one Informationssysteme GmbH
 Author-email: info@seven2one.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `seven2one-4.2.0/seven2one.egg-info/SOURCES.txt` & `seven2one-4.3.0/seven2one.egg-info/SOURCES.txt`

 * *Files identical despite different names*

