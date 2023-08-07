# Comparing `tmp/dialog-workflow-local-0.0.34.tar.gz` & `tmp/dialog-workflow-local-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-0.0.34.tar", last modified: Fri Jun  9 12:36:59 2023, max compression
+gzip compressed data, was "dialog-workflow-local-0.0.35.tar", last modified: Mon Aug  7 11:37:16 2023, max compression
```

## Comparing `dialog-workflow-local-0.0.34.tar` & `dialog-workflow-local-0.0.35.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:36:59.970797 dialog-workflow-local-0.0.34/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-09 12:36:59.970797 dialog-workflow-local-0.0.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:36:59.966797 dialog-workflow-local-0.0.34/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:36:59.966797 dialog-workflow-local-0.0.34/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-09 12:36:59.000000 dialog-workflow-local-0.0.34/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-09 12:36:59.000000 dialog-workflow-local-0.0.34/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:36:59.000000 dialog-workflow-local-0.0.34/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 12:36:59.000000 dialog-workflow-local-0.0.34/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 12:36:59.970797 dialog-workflow-local-0.0.34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:37:16.028324 dialog-workflow-local-0.0.35/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 11:37:16.024325 dialog-workflow-local-0.0.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-07 11:37:06.000000 dialog-workflow-local-0.0.35/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:37:16.024325 dialog-workflow-local-0.0.35/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-08-07 11:37:06.000000 dialog-workflow-local-0.0.35/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-07 11:37:06.000000 dialog-workflow-local-0.0.35/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-07 11:37:06.000000 dialog-workflow-local-0.0.35/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-08-07 11:37:06.000000 dialog-workflow-local-0.0.35/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 11:37:06.000000 dialog-workflow-local-0.0.35/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-08-07 11:37:06.000000 dialog-workflow-local-0.0.35/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-08-07 11:37:06.000000 dialog-workflow-local-0.0.35/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:37:16.024325 dialog-workflow-local-0.0.35/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 11:37:16.000000 dialog-workflow-local-0.0.35/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-07 11:37:16.000000 dialog-workflow-local-0.0.35/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:37:16.000000 dialog-workflow-local-0.0.35/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 11:37:16.000000 dialog-workflow-local-0.0.35/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-07 11:37:06.000000 dialog-workflow-local-0.0.35/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 11:37:16.028324 dialog-workflow-local-0.0.35/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-07 11:37:06.000000 dialog-workflow-local-0.0.35/setup.py
```

### Comparing `dialog-workflow-local-0.0.34/dialog_workflow/Act.py` & `dialog-workflow-local-0.0.35/dialog_workflow/Act.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.34/dialog_workflow/Constants.py` & `dialog-workflow-local-0.0.35/dialog_workflow/Constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 from dotenv import load_dotenv
 load_dotenv()
-from circles_local_database_python.database import database
+# from circles_local_database_python.database import database
 import mysql.connector
 import os
 
 class action_enum(Enum):
     PRESENT_AND_CHOOSE_SCRIPT = 0
     LABEL_ACTION = 1
     TEXT_MESSAGE_ACTION = 2
@@ -33,10 +33,17 @@
 class communication_type_enum(Enum):
     CONSOLE = 1
     WEBSOCKET = 2
 
 DEFAULT_COMMUNICATION_TYPE = communication_type_enum.WEBSOCKET.value
 COMMUNICATION_TYPE = DEFAULT_COMMUNICATION_TYPE if os.getenv("COMMUNICATION_TYPE") == None else os.getenv("COMMUNICATION_TYPE")
 
-connection = database().connect_to_database()
+
+connection = mysql.connector.connect(
+        host=os.getenv("RDS_HOSTNAME"),
+        user=os.getenv("RDS_USERNAME"),
+        password=os.getenv("RDS_PASSWORD")
+        )
+
+# connection = database().connect_to_database()
 cursor = connection.cursor(dictionary=True, buffered=True)
 cursor.execute("""USE dialog_workflow""")
```

### Comparing `dialog-workflow-local-0.0.34/dialog_workflow/DialogWorkflow.py` & `dialog-workflow-local-0.0.35/dialog_workflow/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.34/dialog_workflow/TablesAsObjects.py` & `dialog-workflow-local-0.0.35/dialog_workflow/TablesAsObjects.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.34/dialog_workflow/test.py` & `dialog-workflow-local-0.0.35/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.34/dialog_workflow/utils.py` & `dialog-workflow-local-0.0.35/dialog_workflow/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # TODO: Let's talk about Constants and the usage in this file
 from dialog_workflow.Constants import *
 import random
 import json
-from circles_local_aws_s3_storage_python.AWSStorage import AwsS3Storage
+# from circles_local_aws_s3_storage_python.AWSStorage import AwsS3Storage
 
 # TOOD: Please include type to all parameters.
 # TODO: Please include return value.
 # TODO: Please add short documentation per PEP8 standard
 
 # TODO:Let's move to Object Oriented Programming
 
@@ -122,25 +122,25 @@
                     VALUES (%s,%s,%s,%s)""", 
                     (profile_id, profile_curr_state, variable_id, variable_value))
     cursor.execute("""USE dialog_workflow""")
     connection.commit()
 
 def store_age_detection_picture(age_range: str, profile_id: int):
     """Stores the picture in Nir's storage schema, gets a storage_id and inserts into the computer_vision_storage_table"""
-    storage = AwsS3Storage(bucket_name="storage.us-east-1.dvlp1.bubblez.life", region="us-east-1")
-    storage_id = storage.upload_file("C:\\Users\\User\\OneDrive\\Circles\\age-detection-backend\\src\\alonPicture.png", "Alon's picture", "", 1)
+    # storage = AwsS3Storage(bucket_name="storage.us-east-1.dvlp1.bubblez.life", region="us-east-1")
+    # storage_id = storage.upload_file("C:\\Users\\User\\OneDrive\\Circles\\age-detection-backend\\src\\alonPicture.png", "Alon's picture", "", 1)
     
     age_range_split = age_range.split('-')
-    min_age = int(age_range_split[0][:len(age_range_split[0])-1])
-    max_age = int((age_range_split[1])[1:])
-    cursor.execute("""USE computer_vision_storage""")
-    cursor.execute("""INSERT INTO computer_vision_storage_table 
-                    (storage_id, profile_id, min_age, max_age) VALUES (%s, %s, %s, %s)""", 
-                   [storage_id, profile_id, min_age, max_age])
-    connection.commit()
+    # min_age = int(age_range_split[0][:len(age_range_split[0])-1])
+    # max_age = int((age_range_split[1])[1:])
+    # cursor.execute("""USE computer_vision_storage""")
+    # cursor.execute("""INSERT INTO computer_vision_storage_table 
+    #                 (storage_id, profile_id, min_age, max_age) VALUES (%s, %s, %s, %s)""", 
+    #                [storage_id, profile_id, min_age, max_age])
+    # connection.commit()
 
 def get_curr_state(profile_id: int):
     """Returns profiles' curernt state number"""
     cursor.execute("""USE profile""")
     cursor.execute("""SELECT last_dialog_workflow_state_id FROM profile_view WHERE user_id = %s ORDER BY id DESC""", [profile_id])
     curr_state = int((cursor.fetchone())["last_dialog_workflow_state_id"])
     cursor.execute("""USE dialog_workflow""")
```

### Comparing `dialog-workflow-local-0.0.34/setup.py` & `dialog-workflow-local-0.0.35/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='dialog-workflow-local',  
-     version='0.0.34',
+     version='0.0.35',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

