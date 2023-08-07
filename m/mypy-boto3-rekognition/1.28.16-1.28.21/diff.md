# Comparing `tmp/mypy-boto3-rekognition-1.28.16.tar.gz` & `tmp/mypy-boto3-rekognition-1.28.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rekognition-1.28.16.tar", last modified: Tue Aug  1 11:37:39 2023, max compression
+gzip compressed data, was "mypy-boto3-rekognition-1.28.21.tar", last modified: Mon Aug  7 19:32:27 2023, max compression
```

## Comparing `mypy-boto3-rekognition-1.28.16.tar` & `mypy-boto3-rekognition-1.28.21.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:39.060773 mypy-boto3-rekognition-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26703 2023-08-01 11:37:39.060773 mypy-boto3-rekognition-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25203 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:39.040773 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57536 2023-08-01 11:30:14.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57446 2023-08-01 11:30:14.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-08-01 11:30:15.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-08-01 11:30:14.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-08-01 11:30:14.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-08-01 11:30:14.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    98968 2023-08-01 11:30:21.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98847 2023-08-01 11:30:16.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-08-01 11:30:14.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-01 11:30:14.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:39.060773 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26703 2023-08-01 11:37:38.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-01 11:37:38.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:38.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:38.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:38.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 11:37:38.000000 mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:39.060773 mypy-boto3-rekognition-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-01 11:30:13.000000 mypy-boto3-rekognition-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:32:27.514966 mypy-boto3-rekognition-1.28.21/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-07 19:32:12.000000 mypy-boto3-rekognition-1.28.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-08-07 19:32:27.510966 mypy-boto3-rekognition-1.28.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-08-07 19:32:12.000000 mypy-boto3-rekognition-1.28.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:32:27.506966 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-07 19:32:12.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-08-07 19:32:12.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-07 19:32:12.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57491 2023-08-07 19:32:13.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57401 2023-08-07 19:32:12.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-08-07 19:32:13.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-08-07 19:32:13.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-08-07 19:32:13.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-08-07 19:32:13.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:32:12.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    97001 2023-08-07 19:32:16.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96882 2023-08-07 19:32:14.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-07 19:32:12.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-08-07 19:32:13.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-07 19:32:13.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:32:27.510966 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-08-07 19:32:27.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-07 19:32:27.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:32:27.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:32:27.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-07 19:32:27.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 19:32:27.000000 mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:32:27.514966 mypy-boto3-rekognition-1.28.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-07 19:32:12.000000 mypy-boto3-rekognition-1.28.21/setup.py
```

### Comparing `mypy-boto3-rekognition-1.28.16/LICENSE` & `mypy-boto3-rekognition-1.28.21/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/__init__.py` & `mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/__init__.pyi` & `mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/__main__.py` & `mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Rekognition 1.28.16\nVersion:         1.28.16\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for boto3.Rekognition 1.28.21\nVersion:         1.28.21\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.21")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/client.py` & `mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     PutProjectPolicyResponseTypeDef,
     RecognizeCelebritiesResponseTypeDef,
-    RegionOfInterestUnionTypeDef,
+    RegionOfInterestTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     SearchUsersResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
@@ -125,17 +125,17 @@
     StreamProcessingStartSelectorTypeDef,
     StreamProcessingStopSelectorTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorInputTypeDef,
     StreamProcessorNotificationChannelTypeDef,
     StreamProcessorOutputTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
-    StreamProcessorSettingsUnionTypeDef,
-    TestingDataUnionTypeDef,
-    TrainingDataUnionTypeDef,
+    StreamProcessorSettingsTypeDef,
+    TestingDataTypeDef,
+    TrainingDataTypeDef,
     VideoTypeDef,
 )
 from .waiter import ProjectVersionRunningWaiter, ProjectVersionTrainingCompletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -311,16 +311,16 @@
 
     def create_project_version(
         self,
         *,
         ProjectArn: str,
         VersionName: str,
         OutputConfig: OutputConfigTypeDef,
-        TrainingData: TrainingDataUnionTypeDef = ...,
-        TestingData: TestingDataUnionTypeDef = ...,
+        TrainingData: TrainingDataTypeDef = ...,
+        TestingData: TestingDataTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         KmsKeyId: str = ...
     ) -> CreateProjectVersionResponseTypeDef:
         """
         Creates a new version of a model and begins training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project_version)
@@ -329,20 +329,20 @@
 
     def create_stream_processor(
         self,
         *,
         Input: StreamProcessorInputTypeDef,
         Output: StreamProcessorOutputTypeDef,
         Name: str,
-        Settings: StreamProcessorSettingsUnionTypeDef,
+        Settings: StreamProcessorSettingsTypeDef,
         RoleArn: str,
         Tags: Mapping[str, str] = ...,
         NotificationChannel: StreamProcessorNotificationChannelTypeDef = ...,
         KmsKeyId: str = ...,
-        RegionsOfInterest: Sequence[RegionOfInterestUnionTypeDef] = ...,
+        RegionsOfInterest: Sequence[RegionOfInterestTypeDef] = ...,
         DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef = ...
     ) -> CreateStreamProcessorResponseTypeDef:
         """
         Creates an Amazon Rekognition stream processor that you can use to detect and
         recognize faces or to detect labels in a streaming video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_stream_processor)
@@ -1132,15 +1132,15 @@
         """
 
     def update_stream_processor(
         self,
         *,
         Name: str,
         SettingsForUpdate: StreamProcessorSettingsForUpdateTypeDef = ...,
-        RegionsOfInterestForUpdate: Sequence[RegionOfInterestUnionTypeDef] = ...,
+        RegionsOfInterestForUpdate: Sequence[RegionOfInterestTypeDef] = ...,
         DataSharingPreferenceForUpdate: StreamProcessorDataSharingPreferenceTypeDef = ...,
         ParametersToDelete: Sequence[StreamProcessorParameterToDeleteType] = ...
     ) -> Dict[str, Any]:
         """
         Allows you to update a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.update_stream_processor)
```

### Comparing `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/client.pyi` & `mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     PutProjectPolicyResponseTypeDef,
     RecognizeCelebritiesResponseTypeDef,
-    RegionOfInterestUnionTypeDef,
+    RegionOfInterestTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     SearchUsersResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
@@ -125,17 +125,17 @@
     StreamProcessingStartSelectorTypeDef,
     StreamProcessingStopSelectorTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorInputTypeDef,
     StreamProcessorNotificationChannelTypeDef,
     StreamProcessorOutputTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
-    StreamProcessorSettingsUnionTypeDef,
-    TestingDataUnionTypeDef,
-    TrainingDataUnionTypeDef,
+    StreamProcessorSettingsTypeDef,
+    TestingDataTypeDef,
+    TrainingDataTypeDef,
     VideoTypeDef,
 )
 from .waiter import ProjectVersionRunningWaiter, ProjectVersionTrainingCompletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -297,16 +297,16 @@
         """
     def create_project_version(
         self,
         *,
         ProjectArn: str,
         VersionName: str,
         OutputConfig: OutputConfigTypeDef,
-        TrainingData: TrainingDataUnionTypeDef = ...,
-        TestingData: TestingDataUnionTypeDef = ...,
+        TrainingData: TrainingDataTypeDef = ...,
+        TestingData: TestingDataTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         KmsKeyId: str = ...
     ) -> CreateProjectVersionResponseTypeDef:
         """
         Creates a new version of a model and begins training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project_version)
@@ -314,20 +314,20 @@
         """
     def create_stream_processor(
         self,
         *,
         Input: StreamProcessorInputTypeDef,
         Output: StreamProcessorOutputTypeDef,
         Name: str,
-        Settings: StreamProcessorSettingsUnionTypeDef,
+        Settings: StreamProcessorSettingsTypeDef,
         RoleArn: str,
         Tags: Mapping[str, str] = ...,
         NotificationChannel: StreamProcessorNotificationChannelTypeDef = ...,
         KmsKeyId: str = ...,
-        RegionsOfInterest: Sequence[RegionOfInterestUnionTypeDef] = ...,
+        RegionsOfInterest: Sequence[RegionOfInterestTypeDef] = ...,
         DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef = ...
     ) -> CreateStreamProcessorResponseTypeDef:
         """
         Creates an Amazon Rekognition stream processor that you can use to detect and
         recognize faces or to detect labels in a streaming video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_stream_processor)
@@ -1053,15 +1053,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rekognition/client/#update_dataset_entries)
         """
     def update_stream_processor(
         self,
         *,
         Name: str,
         SettingsForUpdate: StreamProcessorSettingsForUpdateTypeDef = ...,
-        RegionsOfInterestForUpdate: Sequence[RegionOfInterestUnionTypeDef] = ...,
+        RegionsOfInterestForUpdate: Sequence[RegionOfInterestTypeDef] = ...,
         DataSharingPreferenceForUpdate: StreamProcessorDataSharingPreferenceTypeDef = ...,
         ParametersToDelete: Sequence[StreamProcessorParameterToDeleteType] = ...
     ) -> Dict[str, Any]:
         """
         Allows you to update a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.update_stream_processor)
```

### Comparing `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/literals.py` & `mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/literals.pyi` & `mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/paginator.py` & `mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/paginator.pyi` & `mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/type_defs.py` & `mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,14 @@
     "KnownGenderTypeDef",
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
-    "ConnectedHomeSettingsOutputTypeDef",
     "ConnectedHomeSettingsTypeDef",
     "ModerationLabelTypeDef",
     "OutputConfigTypeDef",
     "CoversBodyPartTypeDef",
     "CreateCollectionRequestRequestTypeDef",
     "LivenessOutputConfigTypeDef",
     "CreateProjectRequestRequestTypeDef",
@@ -251,18 +250,16 @@
     "InstanceTypeDef",
     "DetectLabelsSettingsTypeDef",
     "LabelDetectionSettingsTypeDef",
     "DetectModerationLabelsResponseTypeDef",
     "DisassociateFacesResponseTypeDef",
     "DistributeDatasetEntriesRequestRequestTypeDef",
     "FaceDetailTypeDef",
-    "StreamProcessorSettingsOutputTypeDef",
     "StreamProcessorSettingsTypeDef",
     "GeometryTypeDef",
-    "RegionOfInterestOutputTypeDef",
     "RegionOfInterestTypeDef",
     "HumanLoopConfigTypeDef",
     "StreamProcessingStartSelectorTypeDef",
     "StreamProcessorInputTypeDef",
     "ListProjectPoliciesResponseTypeDef",
     "ListStreamProcessorsResponseTypeDef",
     "ListUsersResponseTypeDef",
@@ -306,30 +303,28 @@
     "DetectFacesResponseTypeDef",
     "FaceDetectionTypeDef",
     "FaceRecordTypeDef",
     "PersonDetailTypeDef",
     "SearchedFaceDetailsTypeDef",
     "UnindexedFaceTypeDef",
     "UnsearchedFaceTypeDef",
-    "StreamProcessorSettingsUnionTypeDef",
     "CustomLabelTypeDef",
     "TextDetectionTypeDef",
     "DetectTextFiltersTypeDef",
-    "RegionOfInterestUnionTypeDef",
     "StartTextDetectionFiltersTypeDef",
+    "UpdateStreamProcessorRequestRequestTypeDef",
     "DetectModerationLabelsRequestRequestTypeDef",
     "StartStreamProcessorRequestRequestTypeDef",
     "SearchUsersResponseTypeDef",
+    "CreateStreamProcessorRequestRequestTypeDef",
     "DescribeStreamProcessorResponseTypeDef",
     "GetSegmentDetectionResponseTypeDef",
     "SearchFacesByImageResponseTypeDef",
     "SearchFacesResponseTypeDef",
-    "TestingDataOutputTypeDef",
     "TestingDataTypeDef",
-    "TrainingDataOutputTypeDef",
     "TrainingDataTypeDef",
     "ValidationDataTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "StartSegmentDetectionRequestRequestTypeDef",
     "RecognizeCelebritiesResponseTypeDef",
     "CompareFacesResponseTypeDef",
     "ProtectiveEquipmentPersonTypeDef",
@@ -341,20 +336,16 @@
     "PersonMatchTypeDef",
     "IndexFacesResponseTypeDef",
     "SearchUsersByImageResponseTypeDef",
     "DetectCustomLabelsResponseTypeDef",
     "DetectTextResponseTypeDef",
     "TextDetectionResultTypeDef",
     "DetectTextRequestRequestTypeDef",
-    "CreateStreamProcessorRequestRequestTypeDef",
-    "UpdateStreamProcessorRequestRequestTypeDef",
     "StartTextDetectionRequestRequestTypeDef",
-    "TestingDataUnionTypeDef",
     "CreateProjectVersionRequestRequestTypeDef",
-    "TrainingDataUnionTypeDef",
     "TestingDataResultTypeDef",
     "TrainingDataResultTypeDef",
     "DetectProtectiveEquipmentResponseTypeDef",
     "GetLabelDetectionResponseTypeDef",
     "GetCelebrityRecognitionResponseTypeDef",
     "GetPersonTrackingResponseTypeDef",
     "GetFaceSearchResponseTypeDef",
@@ -537,35 +528,14 @@
     {
         "Labels": Sequence[str],
         "MinConfidence": float,
     },
     total=False,
 )
 
-_RequiredConnectedHomeSettingsOutputTypeDef = TypedDict(
-    "_RequiredConnectedHomeSettingsOutputTypeDef",
-    {
-        "Labels": List[str],
-    },
-)
-_OptionalConnectedHomeSettingsOutputTypeDef = TypedDict(
-    "_OptionalConnectedHomeSettingsOutputTypeDef",
-    {
-        "MinConfidence": float,
-    },
-    total=False,
-)
-
-
-class ConnectedHomeSettingsOutputTypeDef(
-    _RequiredConnectedHomeSettingsOutputTypeDef, _OptionalConnectedHomeSettingsOutputTypeDef
-):
-    pass
-
-
 _RequiredConnectedHomeSettingsTypeDef = TypedDict(
     "_RequiredConnectedHomeSettingsTypeDef",
     {
         "Labels": Sequence[str],
     },
 )
 _OptionalConnectedHomeSettingsTypeDef = TypedDict(
@@ -2540,23 +2510,14 @@
         "Confidence": float,
         "FaceOccluded": FaceOccludedTypeDef,
         "EyeDirection": EyeDirectionTypeDef,
     },
     total=False,
 )
 
-StreamProcessorSettingsOutputTypeDef = TypedDict(
-    "StreamProcessorSettingsOutputTypeDef",
-    {
-        "FaceSearch": FaceSearchSettingsTypeDef,
-        "ConnectedHome": ConnectedHomeSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 StreamProcessorSettingsTypeDef = TypedDict(
     "StreamProcessorSettingsTypeDef",
     {
         "FaceSearch": FaceSearchSettingsTypeDef,
         "ConnectedHome": ConnectedHomeSettingsTypeDef,
     },
     total=False,
@@ -2567,23 +2528,14 @@
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
-RegionOfInterestOutputTypeDef = TypedDict(
-    "RegionOfInterestOutputTypeDef",
-    {
-        "BoundingBox": BoundingBoxTypeDef,
-        "Polygon": List[PointTypeDef],
-    },
-    total=False,
-)
-
 RegionOfInterestTypeDef = TypedDict(
     "RegionOfInterestTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": Sequence[PointTypeDef],
     },
     total=False,
@@ -3291,17 +3243,14 @@
     {
         "FaceDetails": FaceDetailTypeDef,
         "Reasons": List[UnsearchedFaceReasonType],
     },
     total=False,
 )
 
-StreamProcessorSettingsUnionTypeDef = Union[
-    StreamProcessorSettingsTypeDef, StreamProcessorSettingsOutputTypeDef
-]
 CustomLabelTypeDef = TypedDict(
     "CustomLabelTypeDef",
     {
         "Name": str,
         "Confidence": float,
         "Geometry": GeometryTypeDef,
     },
@@ -3326,24 +3275,48 @@
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
-RegionOfInterestUnionTypeDef = Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
 StartTextDetectionFiltersTypeDef = TypedDict(
     "StartTextDetectionFiltersTypeDef",
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
+_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
+        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestTypeDef],
+        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
+        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
+    },
+    total=False,
+)
+
+
+class UpdateStreamProcessorRequestRequestTypeDef(
+    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
+    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDetectModerationLabelsRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
@@ -3393,30 +3366,60 @@
         "FaceModelVersion": str,
         "SearchedFace": SearchedFaceTypeDef,
         "SearchedUser": SearchedUserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Input": StreamProcessorInputTypeDef,
+        "Output": StreamProcessorOutputTypeDef,
+        "Name": str,
+        "Settings": StreamProcessorSettingsTypeDef,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
+        "KmsKeyId": str,
+        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
+        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateStreamProcessorRequestRequestTypeDef(
+    _RequiredCreateStreamProcessorRequestRequestTypeDef,
+    _OptionalCreateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeStreamProcessorResponseTypeDef = TypedDict(
     "DescribeStreamProcessorResponseTypeDef",
     {
         "Name": str,
         "StreamProcessorArn": str,
         "Status": StreamProcessorStatusType,
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "Input": StreamProcessorInputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "RoleArn": str,
-        "Settings": StreamProcessorSettingsOutputTypeDef,
+        "Settings": StreamProcessorSettingsTypeDef,
         "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
         "KmsKeyId": str,
-        "RegionsOfInterest": List[RegionOfInterestOutputTypeDef],
+        "RegionsOfInterest": List[RegionOfInterestTypeDef],
         "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentDetectionResponseTypeDef = TypedDict(
     "GetSegmentDetectionResponseTypeDef",
@@ -3452,40 +3455,23 @@
         "SearchedFaceId": str,
         "FaceMatches": List[FaceMatchTypeDef],
         "FaceModelVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TestingDataOutputTypeDef = TypedDict(
-    "TestingDataOutputTypeDef",
-    {
-        "Assets": List[AssetTypeDef],
-        "AutoCreate": bool,
-    },
-    total=False,
-)
-
 TestingDataTypeDef = TypedDict(
     "TestingDataTypeDef",
     {
         "Assets": Sequence[AssetTypeDef],
         "AutoCreate": bool,
     },
     total=False,
 )
 
-TrainingDataOutputTypeDef = TypedDict(
-    "TrainingDataOutputTypeDef",
-    {
-        "Assets": List[AssetTypeDef],
-    },
-    total=False,
-)
-
 TrainingDataTypeDef = TypedDict(
     "TrainingDataTypeDef",
     {
         "Assets": Sequence[AssetTypeDef],
     },
     total=False,
 )
@@ -3710,69 +3696,14 @@
 
 class DetectTextRequestRequestTypeDef(
     _RequiredDetectTextRequestRequestTypeDef, _OptionalDetectTextRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Input": StreamProcessorInputTypeDef,
-        "Output": StreamProcessorOutputTypeDef,
-        "Name": str,
-        "Settings": StreamProcessorSettingsTypeDef,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
-        "KmsKeyId": str,
-        "RegionsOfInterest": Sequence[RegionOfInterestUnionTypeDef],
-        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateStreamProcessorRequestRequestTypeDef(
-    _RequiredCreateStreamProcessorRequestRequestTypeDef,
-    _OptionalCreateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
-        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestUnionTypeDef],
-        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
-        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
-    },
-    total=False,
-)
-
-
-class UpdateStreamProcessorRequestRequestTypeDef(
-    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
-    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredStartTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartTextDetectionRequestRequestTypeDef = TypedDict(
@@ -3790,15 +3721,14 @@
 class StartTextDetectionRequestRequestTypeDef(
     _RequiredStartTextDetectionRequestRequestTypeDef,
     _OptionalStartTextDetectionRequestRequestTypeDef,
 ):
     pass
 
 
-TestingDataUnionTypeDef = Union[TestingDataTypeDef, TestingDataOutputTypeDef]
 _RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectVersionRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "VersionName": str,
         "OutputConfig": OutputConfigTypeDef,
     },
@@ -3818,30 +3748,29 @@
 class CreateProjectVersionRequestRequestTypeDef(
     _RequiredCreateProjectVersionRequestRequestTypeDef,
     _OptionalCreateProjectVersionRequestRequestTypeDef,
 ):
     pass
 
 
-TrainingDataUnionTypeDef = Union[TrainingDataTypeDef, TrainingDataOutputTypeDef]
 TestingDataResultTypeDef = TypedDict(
     "TestingDataResultTypeDef",
     {
-        "Input": TestingDataOutputTypeDef,
-        "Output": TestingDataOutputTypeDef,
+        "Input": TestingDataTypeDef,
+        "Output": TestingDataTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 TrainingDataResultTypeDef = TypedDict(
     "TrainingDataResultTypeDef",
     {
-        "Input": TrainingDataOutputTypeDef,
-        "Output": TrainingDataOutputTypeDef,
+        "Input": TrainingDataTypeDef,
+        "Output": TrainingDataTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 DetectProtectiveEquipmentResponseTypeDef = TypedDict(
     "DetectProtectiveEquipmentResponseTypeDef",
```

### Comparing `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/type_defs.pyi` & `mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,14 @@
     "KnownGenderTypeDef",
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
-    "ConnectedHomeSettingsOutputTypeDef",
     "ConnectedHomeSettingsTypeDef",
     "ModerationLabelTypeDef",
     "OutputConfigTypeDef",
     "CoversBodyPartTypeDef",
     "CreateCollectionRequestRequestTypeDef",
     "LivenessOutputConfigTypeDef",
     "CreateProjectRequestRequestTypeDef",
@@ -250,18 +249,16 @@
     "InstanceTypeDef",
     "DetectLabelsSettingsTypeDef",
     "LabelDetectionSettingsTypeDef",
     "DetectModerationLabelsResponseTypeDef",
     "DisassociateFacesResponseTypeDef",
     "DistributeDatasetEntriesRequestRequestTypeDef",
     "FaceDetailTypeDef",
-    "StreamProcessorSettingsOutputTypeDef",
     "StreamProcessorSettingsTypeDef",
     "GeometryTypeDef",
-    "RegionOfInterestOutputTypeDef",
     "RegionOfInterestTypeDef",
     "HumanLoopConfigTypeDef",
     "StreamProcessingStartSelectorTypeDef",
     "StreamProcessorInputTypeDef",
     "ListProjectPoliciesResponseTypeDef",
     "ListStreamProcessorsResponseTypeDef",
     "ListUsersResponseTypeDef",
@@ -305,30 +302,28 @@
     "DetectFacesResponseTypeDef",
     "FaceDetectionTypeDef",
     "FaceRecordTypeDef",
     "PersonDetailTypeDef",
     "SearchedFaceDetailsTypeDef",
     "UnindexedFaceTypeDef",
     "UnsearchedFaceTypeDef",
-    "StreamProcessorSettingsUnionTypeDef",
     "CustomLabelTypeDef",
     "TextDetectionTypeDef",
     "DetectTextFiltersTypeDef",
-    "RegionOfInterestUnionTypeDef",
     "StartTextDetectionFiltersTypeDef",
+    "UpdateStreamProcessorRequestRequestTypeDef",
     "DetectModerationLabelsRequestRequestTypeDef",
     "StartStreamProcessorRequestRequestTypeDef",
     "SearchUsersResponseTypeDef",
+    "CreateStreamProcessorRequestRequestTypeDef",
     "DescribeStreamProcessorResponseTypeDef",
     "GetSegmentDetectionResponseTypeDef",
     "SearchFacesByImageResponseTypeDef",
     "SearchFacesResponseTypeDef",
-    "TestingDataOutputTypeDef",
     "TestingDataTypeDef",
-    "TrainingDataOutputTypeDef",
     "TrainingDataTypeDef",
     "ValidationDataTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "StartSegmentDetectionRequestRequestTypeDef",
     "RecognizeCelebritiesResponseTypeDef",
     "CompareFacesResponseTypeDef",
     "ProtectiveEquipmentPersonTypeDef",
@@ -340,20 +335,16 @@
     "PersonMatchTypeDef",
     "IndexFacesResponseTypeDef",
     "SearchUsersByImageResponseTypeDef",
     "DetectCustomLabelsResponseTypeDef",
     "DetectTextResponseTypeDef",
     "TextDetectionResultTypeDef",
     "DetectTextRequestRequestTypeDef",
-    "CreateStreamProcessorRequestRequestTypeDef",
-    "UpdateStreamProcessorRequestRequestTypeDef",
     "StartTextDetectionRequestRequestTypeDef",
-    "TestingDataUnionTypeDef",
     "CreateProjectVersionRequestRequestTypeDef",
-    "TrainingDataUnionTypeDef",
     "TestingDataResultTypeDef",
     "TrainingDataResultTypeDef",
     "DetectProtectiveEquipmentResponseTypeDef",
     "GetLabelDetectionResponseTypeDef",
     "GetCelebrityRecognitionResponseTypeDef",
     "GetPersonTrackingResponseTypeDef",
     "GetFaceSearchResponseTypeDef",
@@ -534,33 +525,14 @@
     {
         "Labels": Sequence[str],
         "MinConfidence": float,
     },
     total=False,
 )
 
-_RequiredConnectedHomeSettingsOutputTypeDef = TypedDict(
-    "_RequiredConnectedHomeSettingsOutputTypeDef",
-    {
-        "Labels": List[str],
-    },
-)
-_OptionalConnectedHomeSettingsOutputTypeDef = TypedDict(
-    "_OptionalConnectedHomeSettingsOutputTypeDef",
-    {
-        "MinConfidence": float,
-    },
-    total=False,
-)
-
-class ConnectedHomeSettingsOutputTypeDef(
-    _RequiredConnectedHomeSettingsOutputTypeDef, _OptionalConnectedHomeSettingsOutputTypeDef
-):
-    pass
-
 _RequiredConnectedHomeSettingsTypeDef = TypedDict(
     "_RequiredConnectedHomeSettingsTypeDef",
     {
         "Labels": Sequence[str],
     },
 )
 _OptionalConnectedHomeSettingsTypeDef = TypedDict(
@@ -2467,23 +2439,14 @@
         "Confidence": float,
         "FaceOccluded": FaceOccludedTypeDef,
         "EyeDirection": EyeDirectionTypeDef,
     },
     total=False,
 )
 
-StreamProcessorSettingsOutputTypeDef = TypedDict(
-    "StreamProcessorSettingsOutputTypeDef",
-    {
-        "FaceSearch": FaceSearchSettingsTypeDef,
-        "ConnectedHome": ConnectedHomeSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 StreamProcessorSettingsTypeDef = TypedDict(
     "StreamProcessorSettingsTypeDef",
     {
         "FaceSearch": FaceSearchSettingsTypeDef,
         "ConnectedHome": ConnectedHomeSettingsTypeDef,
     },
     total=False,
@@ -2494,23 +2457,14 @@
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
-RegionOfInterestOutputTypeDef = TypedDict(
-    "RegionOfInterestOutputTypeDef",
-    {
-        "BoundingBox": BoundingBoxTypeDef,
-        "Polygon": List[PointTypeDef],
-    },
-    total=False,
-)
-
 RegionOfInterestTypeDef = TypedDict(
     "RegionOfInterestTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": Sequence[PointTypeDef],
     },
     total=False,
@@ -3188,17 +3142,14 @@
     {
         "FaceDetails": FaceDetailTypeDef,
         "Reasons": List[UnsearchedFaceReasonType],
     },
     total=False,
 )
 
-StreamProcessorSettingsUnionTypeDef = Union[
-    StreamProcessorSettingsTypeDef, StreamProcessorSettingsOutputTypeDef
-]
 CustomLabelTypeDef = TypedDict(
     "CustomLabelTypeDef",
     {
         "Name": str,
         "Confidence": float,
         "Geometry": GeometryTypeDef,
     },
@@ -3223,24 +3174,46 @@
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
-RegionOfInterestUnionTypeDef = Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
 StartTextDetectionFiltersTypeDef = TypedDict(
     "StartTextDetectionFiltersTypeDef",
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
+_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
+        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestTypeDef],
+        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
+        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
+    },
+    total=False,
+)
+
+class UpdateStreamProcessorRequestRequestTypeDef(
+    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
+    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
 _RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDetectModerationLabelsRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
@@ -3286,30 +3259,58 @@
         "FaceModelVersion": str,
         "SearchedFace": SearchedFaceTypeDef,
         "SearchedUser": SearchedUserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Input": StreamProcessorInputTypeDef,
+        "Output": StreamProcessorOutputTypeDef,
+        "Name": str,
+        "Settings": StreamProcessorSettingsTypeDef,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
+        "KmsKeyId": str,
+        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
+        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
+    },
+    total=False,
+)
+
+class CreateStreamProcessorRequestRequestTypeDef(
+    _RequiredCreateStreamProcessorRequestRequestTypeDef,
+    _OptionalCreateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
 DescribeStreamProcessorResponseTypeDef = TypedDict(
     "DescribeStreamProcessorResponseTypeDef",
     {
         "Name": str,
         "StreamProcessorArn": str,
         "Status": StreamProcessorStatusType,
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "Input": StreamProcessorInputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "RoleArn": str,
-        "Settings": StreamProcessorSettingsOutputTypeDef,
+        "Settings": StreamProcessorSettingsTypeDef,
         "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
         "KmsKeyId": str,
-        "RegionsOfInterest": List[RegionOfInterestOutputTypeDef],
+        "RegionsOfInterest": List[RegionOfInterestTypeDef],
         "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentDetectionResponseTypeDef = TypedDict(
     "GetSegmentDetectionResponseTypeDef",
@@ -3345,40 +3346,23 @@
         "SearchedFaceId": str,
         "FaceMatches": List[FaceMatchTypeDef],
         "FaceModelVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TestingDataOutputTypeDef = TypedDict(
-    "TestingDataOutputTypeDef",
-    {
-        "Assets": List[AssetTypeDef],
-        "AutoCreate": bool,
-    },
-    total=False,
-)
-
 TestingDataTypeDef = TypedDict(
     "TestingDataTypeDef",
     {
         "Assets": Sequence[AssetTypeDef],
         "AutoCreate": bool,
     },
     total=False,
 )
 
-TrainingDataOutputTypeDef = TypedDict(
-    "TrainingDataOutputTypeDef",
-    {
-        "Assets": List[AssetTypeDef],
-    },
-    total=False,
-)
-
 TrainingDataTypeDef = TypedDict(
     "TrainingDataTypeDef",
     {
         "Assets": Sequence[AssetTypeDef],
     },
     total=False,
 )
@@ -3597,65 +3581,14 @@
 )
 
 class DetectTextRequestRequestTypeDef(
     _RequiredDetectTextRequestRequestTypeDef, _OptionalDetectTextRequestRequestTypeDef
 ):
     pass
 
-_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Input": StreamProcessorInputTypeDef,
-        "Output": StreamProcessorOutputTypeDef,
-        "Name": str,
-        "Settings": StreamProcessorSettingsTypeDef,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
-        "KmsKeyId": str,
-        "RegionsOfInterest": Sequence[RegionOfInterestUnionTypeDef],
-        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
-    },
-    total=False,
-)
-
-class CreateStreamProcessorRequestRequestTypeDef(
-    _RequiredCreateStreamProcessorRequestRequestTypeDef,
-    _OptionalCreateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
-        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestUnionTypeDef],
-        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
-        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
-    },
-    total=False,
-)
-
-class UpdateStreamProcessorRequestRequestTypeDef(
-    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
-    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
 _RequiredStartTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartTextDetectionRequestRequestTypeDef = TypedDict(
@@ -3671,15 +3604,14 @@
 
 class StartTextDetectionRequestRequestTypeDef(
     _RequiredStartTextDetectionRequestRequestTypeDef,
     _OptionalStartTextDetectionRequestRequestTypeDef,
 ):
     pass
 
-TestingDataUnionTypeDef = Union[TestingDataTypeDef, TestingDataOutputTypeDef]
 _RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectVersionRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "VersionName": str,
         "OutputConfig": OutputConfigTypeDef,
     },
@@ -3697,30 +3629,29 @@
 
 class CreateProjectVersionRequestRequestTypeDef(
     _RequiredCreateProjectVersionRequestRequestTypeDef,
     _OptionalCreateProjectVersionRequestRequestTypeDef,
 ):
     pass
 
-TrainingDataUnionTypeDef = Union[TrainingDataTypeDef, TrainingDataOutputTypeDef]
 TestingDataResultTypeDef = TypedDict(
     "TestingDataResultTypeDef",
     {
-        "Input": TestingDataOutputTypeDef,
-        "Output": TestingDataOutputTypeDef,
+        "Input": TestingDataTypeDef,
+        "Output": TestingDataTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 TrainingDataResultTypeDef = TypedDict(
     "TrainingDataResultTypeDef",
     {
-        "Input": TrainingDataOutputTypeDef,
-        "Output": TrainingDataOutputTypeDef,
+        "Input": TrainingDataTypeDef,
+        "Output": TrainingDataTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 DetectProtectiveEquipmentResponseTypeDef = TypedDict(
     "DetectProtectiveEquipmentResponseTypeDef",
```

### Comparing `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/waiter.py` & `mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition/waiter.pyi` & `mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.16/mypy_boto3_rekognition.egg-info/SOURCES.txt` & `mypy-boto3-rekognition-1.28.21/mypy_boto3_rekognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rekognition-1.28.16/setup.py` & `mypy-boto3-rekognition-1.28.21/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rekognition",
-    version="1.28.16",
+    version="1.28.21",
     packages=["mypy_boto3_rekognition"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Rekognition 1.28.16 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        "Type annotations for boto3.Rekognition 1.28.21 service generated with mypy-boto3-builder"
+        " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

