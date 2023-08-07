# Comparing `tmp/mypy-boto3-kinesisvideo-1.28.16.tar.gz` & `tmp/mypy-boto3-kinesisvideo-1.28.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesisvideo-1.28.16.tar", last modified: Tue Aug  1 11:37:09 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesisvideo-1.28.21.tar", last modified: Mon Aug  7 19:32:27 2023, max compression
```

## Comparing `mypy-boto3-kinesisvideo-1.28.16.tar` & `mypy-boto3-kinesisvideo-1.28.21.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:09.864845 mypy-boto3-kinesisvideo-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-08-01 11:37:09.864845 mypy-boto3-kinesisvideo-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:09.864845 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24988 2023-08-01 11:21:47.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24947 2023-08-01 11:21:47.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-08-01 11:21:47.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-08-01 11:21:47.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-08-01 11:21:47.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-08-01 11:21:47.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-08-01 11:21:50.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29617 2023-08-01 11:21:47.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:09.864845 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-08-01 11:37:09.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:37:09.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:09.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:09.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:09.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:37:09.000000 mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:09.864845 mypy-boto3-kinesisvideo-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:21:46.000000 mypy-boto3-kinesisvideo-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:32:27.482966 mypy-boto3-kinesisvideo-1.28.21/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-07 19:32:09.000000 mypy-boto3-kinesisvideo-1.28.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-08-07 19:32:27.474965 mypy-boto3-kinesisvideo-1.28.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-08-07 19:32:09.000000 mypy-boto3-kinesisvideo-1.28.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:32:27.474965 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-07 19:32:09.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-07 19:32:09.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-07 19:32:09.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-08-07 19:32:09.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-08-07 19:32:09.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-08-07 19:32:10.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-08-07 19:32:10.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-08-07 19:32:10.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-08-07 19:32:09.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:32:09.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28598 2023-08-07 19:32:10.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28559 2023-08-07 19:32:10.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-07 19:32:09.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:32:27.474965 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-08-07 19:32:27.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-07 19:32:27.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:32:27.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:32:27.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-07 19:32:27.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-07 19:32:27.000000 mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:32:27.482966 mypy-boto3-kinesisvideo-1.28.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-07 19:32:09.000000 mypy-boto3-kinesisvideo-1.28.21/setup.py
```

### Comparing `mypy-boto3-kinesisvideo-1.28.16/LICENSE` & `mypy-boto3-kinesisvideo-1.28.21/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/__init__.py` & `mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/__init__.pyi` & `mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/__main__.py` & `mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisVideo 1.28.16\nVersion:         1.28.16\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for boto3.KinesisVideo 1.28.21\nVersion:         1.28.21\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo\nOther"
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

### Comparing `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/client.py` & `mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     DescribeMediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     DescribeStreamOutputTypeDef,
     EdgeConfigTypeDef,
     GetDataEndpointOutputTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
-    ImageGenerationConfigurationUnionTypeDef,
+    ImageGenerationConfigurationTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     MediaStorageConfigurationTypeDef,
     NotificationConfigurationTypeDef,
@@ -422,15 +422,15 @@
         """
 
     def update_image_generation_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        ImageGenerationConfiguration: ImageGenerationConfigurationUnionTypeDef = ...
+        ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_image_generation_configuration)
         """
```

### Comparing `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/client.pyi` & `mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     DescribeMediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     DescribeStreamOutputTypeDef,
     EdgeConfigTypeDef,
     GetDataEndpointOutputTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
-    ImageGenerationConfigurationUnionTypeDef,
+    ImageGenerationConfigurationTypeDef,
     ListEdgeAgentConfigurationsOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     MediaStorageConfigurationTypeDef,
     NotificationConfigurationTypeDef,
@@ -389,15 +389,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_data_retention)
         """
     def update_image_generation_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        ImageGenerationConfiguration: ImageGenerationConfigurationUnionTypeDef = ...
+        ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisvideo/client/#update_image_generation_configuration)
         """
```

### Comparing `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/literals.py` & `mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/literals.pyi` & `mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/paginator.py` & `mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/paginator.pyi` & `mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/type_defs.py` & `mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef
 
     data: SingleMasterConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     APINameType,
     ChannelProtocolType,
     ChannelRoleType,
     ChannelTypeType,
     ConfigurationStatusType,
@@ -38,15 +38,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "SingleMasterConfigurationTypeDef",
     "ChannelNameConditionTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "CreateStreamInputRequestTypeDef",
     "DeleteEdgeConfigurationInputRequestTypeDef",
@@ -100,25 +99,23 @@
     "DescribeMediaStorageConfigurationOutputTypeDef",
     "UpdateMediaStorageConfigurationInputRequestTypeDef",
     "DescribeStreamOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "EdgeAgentStatusTypeDef",
     "GetSignalingChannelEndpointInputRequestTypeDef",
     "GetSignalingChannelEndpointOutputTypeDef",
-    "ImageGenerationConfigurationOutputTypeDef",
     "ImageGenerationConfigurationTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "RecorderConfigTypeDef",
     "UploaderConfigTypeDef",
     "DescribeSignalingChannelOutputTypeDef",
     "ListSignalingChannelsOutputTypeDef",
     "DescribeImageGenerationConfigurationOutputTypeDef",
-    "ImageGenerationConfigurationUnionTypeDef",
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     "DescribeNotificationConfigurationOutputTypeDef",
     "UpdateNotificationConfigurationInputRequestTypeDef",
     "EdgeConfigTypeDef",
     "DescribeEdgeConfigurationOutputTypeDef",
     "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
     "StartEdgeConfigurationUpdateInputRequestTypeDef",
@@ -176,21 +173,19 @@
         "KmsKeyId": str,
         "DataRetentionInHours": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateStreamInputRequestTypeDef(
     _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
 ):
     pass
 
-
 DeleteEdgeConfigurationInputRequestTypeDef = TypedDict(
     "DeleteEdgeConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
@@ -206,43 +201,39 @@
     "_OptionalDeleteSignalingChannelInputRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
-
 class DeleteSignalingChannelInputRequestTypeDef(
     _RequiredDeleteSignalingChannelInputRequestTypeDef,
     _OptionalDeleteSignalingChannelInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStreamInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamInputRequestTypeDef",
     {
         "StreamARN": str,
     },
 )
 _OptionalDeleteStreamInputRequestTypeDef = TypedDict(
     "_OptionalDeleteStreamInputRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
-
 class DeleteStreamInputRequestTypeDef(
     _RequiredDeleteStreamInputRequestTypeDef, _OptionalDeleteStreamInputRequestTypeDef
 ):
     pass
 
-
 LocalSizeConfigTypeDef = TypedDict(
     "LocalSizeConfigTypeDef",
     {
         "MaxLocalMediaSizeInMB": int,
         "StrategyOnFullSize": StrategyOnFullSizeType,
     },
     total=False,
@@ -315,21 +306,19 @@
     "_OptionalMediaStorageConfigurationTypeDef",
     {
         "StreamARN": str,
     },
     total=False,
 )
 
-
 class MediaStorageConfigurationTypeDef(
     _RequiredMediaStorageConfigurationTypeDef, _OptionalMediaStorageConfigurationTypeDef
 ):
     pass
 
-
 DescribeNotificationConfigurationInputRequestTypeDef = TypedDict(
     "DescribeNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
@@ -402,21 +391,19 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
-
 class GetDataEndpointInputRequestTypeDef(
     _RequiredGetDataEndpointInputRequestTypeDef, _OptionalGetDataEndpointInputRequestTypeDef
 ):
     pass
 
-
 SingleMasterChannelEndpointConfigurationTypeDef = TypedDict(
     "SingleMasterChannelEndpointConfigurationTypeDef",
     {
         "Protocols": Sequence[ChannelProtocolType],
         "Role": ChannelRoleType,
     },
     total=False,
@@ -450,22 +437,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListEdgeAgentConfigurationsInputRequestTypeDef(
     _RequiredListEdgeAgentConfigurationsInputRequestTypeDef,
     _OptionalListEdgeAgentConfigurationsInputRequestTypeDef,
 ):
     pass
 
-
 StreamNameConditionTypeDef = TypedDict(
     "StreamNameConditionTypeDef",
     {
         "ComparisonOperator": Literal["BEGINS_WITH"],
         "ComparisonValue": str,
     },
     total=False,
@@ -481,21 +466,19 @@
     "_OptionalListTagsForResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-
 ListTagsForStreamInputRequestTypeDef = TypedDict(
     "ListTagsForStreamInputRequestTypeDef",
     {
         "NextToken": str,
         "StreamARN": str,
         "StreamName": str,
     },
@@ -536,21 +519,19 @@
     {
         "StreamARN": str,
         "StreamName": str,
     },
     total=False,
 )
 
-
 class TagStreamInputRequestTypeDef(
     _RequiredTagStreamInputRequestTypeDef, _OptionalTagStreamInputRequestTypeDef
 ):
     pass
 
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeyList": Sequence[str],
     },
 )
@@ -566,21 +547,19 @@
     {
         "StreamARN": str,
         "StreamName": str,
     },
     total=False,
 )
 
-
 class UntagStreamInputRequestTypeDef(
     _RequiredUntagStreamInputRequestTypeDef, _OptionalUntagStreamInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateDataRetentionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDataRetentionInputRequestTypeDef",
     {
         "CurrentVersion": str,
         "Operation": UpdateDataRetentionOperationType,
         "DataRetentionChangeInHours": int,
     },
@@ -590,21 +569,19 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
-
 class UpdateDataRetentionInputRequestTypeDef(
     _RequiredUpdateDataRetentionInputRequestTypeDef, _OptionalUpdateDataRetentionInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateStreamInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamInputRequestTypeDef",
     {
         "CurrentVersion": str,
     },
 )
 _OptionalUpdateStreamInputRequestTypeDef = TypedDict(
@@ -614,21 +591,19 @@
         "StreamARN": str,
         "DeviceName": str,
         "MediaType": str,
     },
     total=False,
 )
 
-
 class UpdateStreamInputRequestTypeDef(
     _RequiredUpdateStreamInputRequestTypeDef, _OptionalUpdateStreamInputRequestTypeDef
 ):
     pass
 
-
 ChannelInfoTypeDef = TypedDict(
     "ChannelInfoTypeDef",
     {
         "ChannelName": str,
         "ChannelARN": str,
         "ChannelType": ChannelTypeType,
         "ChannelStatus": StatusType,
@@ -650,22 +625,20 @@
     "_OptionalUpdateSignalingChannelInputRequestTypeDef",
     {
         "SingleMasterConfiguration": SingleMasterConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateSignalingChannelInputRequestTypeDef(
     _RequiredUpdateSignalingChannelInputRequestTypeDef,
     _OptionalUpdateSignalingChannelInputRequestTypeDef,
 ):
     pass
 
-
 ListSignalingChannelsInputRequestTypeDef = TypedDict(
     "ListSignalingChannelsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "ChannelNameCondition": ChannelNameConditionTypeDef,
     },
@@ -684,22 +657,20 @@
         "ChannelType": ChannelTypeType,
         "SingleMasterConfiguration": SingleMasterConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSignalingChannelInputRequestTypeDef(
     _RequiredCreateSignalingChannelInputRequestTypeDef,
     _OptionalCreateSignalingChannelInputRequestTypeDef,
 ):
     pass
 
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -776,22 +747,20 @@
     "_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef(
     _RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
     _OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
 ):
     pass
 
-
 ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
     "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     {
         "ChannelNameCondition": ChannelNameConditionTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -858,85 +827,53 @@
     "_OptionalGetSignalingChannelEndpointInputRequestTypeDef",
     {
         "SingleMasterChannelEndpointConfiguration": SingleMasterChannelEndpointConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class GetSignalingChannelEndpointInputRequestTypeDef(
     _RequiredGetSignalingChannelEndpointInputRequestTypeDef,
     _OptionalGetSignalingChannelEndpointInputRequestTypeDef,
 ):
     pass
 
-
 GetSignalingChannelEndpointOutputTypeDef = TypedDict(
     "GetSignalingChannelEndpointOutputTypeDef",
     {
         "ResourceEndpointList": List[ResourceEndpointListItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredImageGenerationConfigurationOutputTypeDef = TypedDict(
-    "_RequiredImageGenerationConfigurationOutputTypeDef",
-    {
-        "Status": ConfigurationStatusType,
-        "ImageSelectorType": ImageSelectorTypeType,
-        "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
-        "SamplingInterval": int,
-        "Format": FormatType,
-    },
-)
-_OptionalImageGenerationConfigurationOutputTypeDef = TypedDict(
-    "_OptionalImageGenerationConfigurationOutputTypeDef",
-    {
-        "FormatConfig": Dict[Literal["JPEGQuality"], str],
-        "WidthPixels": int,
-        "HeightPixels": int,
-    },
-    total=False,
-)
-
-
-class ImageGenerationConfigurationOutputTypeDef(
-    _RequiredImageGenerationConfigurationOutputTypeDef,
-    _OptionalImageGenerationConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredImageGenerationConfigurationTypeDef = TypedDict(
     "_RequiredImageGenerationConfigurationTypeDef",
     {
         "Status": ConfigurationStatusType,
         "ImageSelectorType": ImageSelectorTypeType,
         "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
         "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalImageGenerationConfigurationTypeDef = TypedDict(
     "_OptionalImageGenerationConfigurationTypeDef",
     {
-        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
+        "FormatConfig": Dict[Literal["JPEGQuality"], str],
         "WidthPixels": int,
         "HeightPixels": int,
     },
     total=False,
 )
 
-
 class ImageGenerationConfigurationTypeDef(
     _RequiredImageGenerationConfigurationTypeDef, _OptionalImageGenerationConfigurationTypeDef
 ):
     pass
 
-
 ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsInputListStreamsPaginateTypeDef",
     {
         "StreamNameCondition": StreamNameConditionTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -970,19 +907,17 @@
     "_OptionalRecorderConfigTypeDef",
     {
         "ScheduleConfig": ScheduleConfigTypeDef,
     },
     total=False,
 )
 
-
 class RecorderConfigTypeDef(_RequiredRecorderConfigTypeDef, _OptionalRecorderConfigTypeDef):
     pass
 
-
 UploaderConfigTypeDef = TypedDict(
     "UploaderConfigTypeDef",
     {
         "ScheduleConfig": ScheduleConfigTypeDef,
     },
 )
 
@@ -1002,22 +937,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImageGenerationConfigurationOutputTypeDef = TypedDict(
     "DescribeImageGenerationConfigurationOutputTypeDef",
     {
-        "ImageGenerationConfiguration": ImageGenerationConfigurationOutputTypeDef,
+        "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImageGenerationConfigurationUnionTypeDef = Union[
-    ImageGenerationConfigurationTypeDef, ImageGenerationConfigurationOutputTypeDef
-]
 UpdateImageGenerationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
     },
@@ -1054,19 +986,17 @@
     {
         "UploaderConfig": UploaderConfigTypeDef,
         "DeletionConfig": DeletionConfigTypeDef,
     },
     total=False,
 )
 
-
 class EdgeConfigTypeDef(_RequiredEdgeConfigTypeDef, _OptionalEdgeConfigTypeDef):
     pass
 
-
 DescribeEdgeConfigurationOutputTypeDef = TypedDict(
     "DescribeEdgeConfigurationOutputTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
@@ -1103,22 +1033,20 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
-
 class StartEdgeConfigurationUpdateInputRequestTypeDef(
     _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef,
     _OptionalStartEdgeConfigurationUpdateInputRequestTypeDef,
 ):
     pass
 
-
 StartEdgeConfigurationUpdateOutputTypeDef = TypedDict(
     "StartEdgeConfigurationUpdateOutputTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
```

### Comparing `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo/type_defs.pyi` & `mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef
 
     data: SingleMasterConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     APINameType,
     ChannelProtocolType,
     ChannelRoleType,
     ChannelTypeType,
     ConfigurationStatusType,
@@ -38,14 +38,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "SingleMasterConfigurationTypeDef",
     "ChannelNameConditionTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "CreateStreamInputRequestTypeDef",
     "DeleteEdgeConfigurationInputRequestTypeDef",
@@ -99,25 +100,23 @@
     "DescribeMediaStorageConfigurationOutputTypeDef",
     "UpdateMediaStorageConfigurationInputRequestTypeDef",
     "DescribeStreamOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "EdgeAgentStatusTypeDef",
     "GetSignalingChannelEndpointInputRequestTypeDef",
     "GetSignalingChannelEndpointOutputTypeDef",
-    "ImageGenerationConfigurationOutputTypeDef",
     "ImageGenerationConfigurationTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "RecorderConfigTypeDef",
     "UploaderConfigTypeDef",
     "DescribeSignalingChannelOutputTypeDef",
     "ListSignalingChannelsOutputTypeDef",
     "DescribeImageGenerationConfigurationOutputTypeDef",
-    "ImageGenerationConfigurationUnionTypeDef",
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     "DescribeNotificationConfigurationOutputTypeDef",
     "UpdateNotificationConfigurationInputRequestTypeDef",
     "EdgeConfigTypeDef",
     "DescribeEdgeConfigurationOutputTypeDef",
     "ListEdgeAgentConfigurationsEdgeConfigTypeDef",
     "StartEdgeConfigurationUpdateInputRequestTypeDef",
@@ -175,19 +174,21 @@
         "KmsKeyId": str,
         "DataRetentionInHours": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateStreamInputRequestTypeDef(
     _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
 ):
     pass
 
+
 DeleteEdgeConfigurationInputRequestTypeDef = TypedDict(
     "DeleteEdgeConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
@@ -203,39 +204,43 @@
     "_OptionalDeleteSignalingChannelInputRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
+
 class DeleteSignalingChannelInputRequestTypeDef(
     _RequiredDeleteSignalingChannelInputRequestTypeDef,
     _OptionalDeleteSignalingChannelInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStreamInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamInputRequestTypeDef",
     {
         "StreamARN": str,
     },
 )
 _OptionalDeleteStreamInputRequestTypeDef = TypedDict(
     "_OptionalDeleteStreamInputRequestTypeDef",
     {
         "CurrentVersion": str,
     },
     total=False,
 )
 
+
 class DeleteStreamInputRequestTypeDef(
     _RequiredDeleteStreamInputRequestTypeDef, _OptionalDeleteStreamInputRequestTypeDef
 ):
     pass
 
+
 LocalSizeConfigTypeDef = TypedDict(
     "LocalSizeConfigTypeDef",
     {
         "MaxLocalMediaSizeInMB": int,
         "StrategyOnFullSize": StrategyOnFullSizeType,
     },
     total=False,
@@ -308,19 +313,21 @@
     "_OptionalMediaStorageConfigurationTypeDef",
     {
         "StreamARN": str,
     },
     total=False,
 )
 
+
 class MediaStorageConfigurationTypeDef(
     _RequiredMediaStorageConfigurationTypeDef, _OptionalMediaStorageConfigurationTypeDef
 ):
     pass
 
+
 DescribeNotificationConfigurationInputRequestTypeDef = TypedDict(
     "DescribeNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
@@ -393,19 +400,21 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
+
 class GetDataEndpointInputRequestTypeDef(
     _RequiredGetDataEndpointInputRequestTypeDef, _OptionalGetDataEndpointInputRequestTypeDef
 ):
     pass
 
+
 SingleMasterChannelEndpointConfigurationTypeDef = TypedDict(
     "SingleMasterChannelEndpointConfigurationTypeDef",
     {
         "Protocols": Sequence[ChannelProtocolType],
         "Role": ChannelRoleType,
     },
     total=False,
@@ -439,20 +448,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListEdgeAgentConfigurationsInputRequestTypeDef(
     _RequiredListEdgeAgentConfigurationsInputRequestTypeDef,
     _OptionalListEdgeAgentConfigurationsInputRequestTypeDef,
 ):
     pass
 
+
 StreamNameConditionTypeDef = TypedDict(
     "StreamNameConditionTypeDef",
     {
         "ComparisonOperator": Literal["BEGINS_WITH"],
         "ComparisonValue": str,
     },
     total=False,
@@ -468,19 +479,21 @@
     "_OptionalListTagsForResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
+
 ListTagsForStreamInputRequestTypeDef = TypedDict(
     "ListTagsForStreamInputRequestTypeDef",
     {
         "NextToken": str,
         "StreamARN": str,
         "StreamName": str,
     },
@@ -521,19 +534,21 @@
     {
         "StreamARN": str,
         "StreamName": str,
     },
     total=False,
 )
 
+
 class TagStreamInputRequestTypeDef(
     _RequiredTagStreamInputRequestTypeDef, _OptionalTagStreamInputRequestTypeDef
 ):
     pass
 
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeyList": Sequence[str],
     },
 )
@@ -549,19 +564,21 @@
     {
         "StreamARN": str,
         "StreamName": str,
     },
     total=False,
 )
 
+
 class UntagStreamInputRequestTypeDef(
     _RequiredUntagStreamInputRequestTypeDef, _OptionalUntagStreamInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateDataRetentionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDataRetentionInputRequestTypeDef",
     {
         "CurrentVersion": str,
         "Operation": UpdateDataRetentionOperationType,
         "DataRetentionChangeInHours": int,
     },
@@ -571,19 +588,21 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
+
 class UpdateDataRetentionInputRequestTypeDef(
     _RequiredUpdateDataRetentionInputRequestTypeDef, _OptionalUpdateDataRetentionInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateStreamInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamInputRequestTypeDef",
     {
         "CurrentVersion": str,
     },
 )
 _OptionalUpdateStreamInputRequestTypeDef = TypedDict(
@@ -593,19 +612,21 @@
         "StreamARN": str,
         "DeviceName": str,
         "MediaType": str,
     },
     total=False,
 )
 
+
 class UpdateStreamInputRequestTypeDef(
     _RequiredUpdateStreamInputRequestTypeDef, _OptionalUpdateStreamInputRequestTypeDef
 ):
     pass
 
+
 ChannelInfoTypeDef = TypedDict(
     "ChannelInfoTypeDef",
     {
         "ChannelName": str,
         "ChannelARN": str,
         "ChannelType": ChannelTypeType,
         "ChannelStatus": StatusType,
@@ -627,20 +648,22 @@
     "_OptionalUpdateSignalingChannelInputRequestTypeDef",
     {
         "SingleMasterConfiguration": SingleMasterConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateSignalingChannelInputRequestTypeDef(
     _RequiredUpdateSignalingChannelInputRequestTypeDef,
     _OptionalUpdateSignalingChannelInputRequestTypeDef,
 ):
     pass
 
+
 ListSignalingChannelsInputRequestTypeDef = TypedDict(
     "ListSignalingChannelsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "ChannelNameCondition": ChannelNameConditionTypeDef,
     },
@@ -659,20 +682,22 @@
         "ChannelType": ChannelTypeType,
         "SingleMasterConfiguration": SingleMasterConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSignalingChannelInputRequestTypeDef(
     _RequiredCreateSignalingChannelInputRequestTypeDef,
     _OptionalCreateSignalingChannelInputRequestTypeDef,
 ):
     pass
 
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -749,20 +774,22 @@
     "_OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef(
     _RequiredListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
     _OptionalListEdgeAgentConfigurationsInputListEdgeAgentConfigurationsPaginateTypeDef,
 ):
     pass
 
+
 ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
     "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     {
         "ChannelNameCondition": ChannelNameConditionTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -829,79 +856,57 @@
     "_OptionalGetSignalingChannelEndpointInputRequestTypeDef",
     {
         "SingleMasterChannelEndpointConfiguration": SingleMasterChannelEndpointConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class GetSignalingChannelEndpointInputRequestTypeDef(
     _RequiredGetSignalingChannelEndpointInputRequestTypeDef,
     _OptionalGetSignalingChannelEndpointInputRequestTypeDef,
 ):
     pass
 
+
 GetSignalingChannelEndpointOutputTypeDef = TypedDict(
     "GetSignalingChannelEndpointOutputTypeDef",
     {
         "ResourceEndpointList": List[ResourceEndpointListItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredImageGenerationConfigurationOutputTypeDef = TypedDict(
-    "_RequiredImageGenerationConfigurationOutputTypeDef",
-    {
-        "Status": ConfigurationStatusType,
-        "ImageSelectorType": ImageSelectorTypeType,
-        "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
-        "SamplingInterval": int,
-        "Format": FormatType,
-    },
-)
-_OptionalImageGenerationConfigurationOutputTypeDef = TypedDict(
-    "_OptionalImageGenerationConfigurationOutputTypeDef",
-    {
-        "FormatConfig": Dict[Literal["JPEGQuality"], str],
-        "WidthPixels": int,
-        "HeightPixels": int,
-    },
-    total=False,
-)
-
-class ImageGenerationConfigurationOutputTypeDef(
-    _RequiredImageGenerationConfigurationOutputTypeDef,
-    _OptionalImageGenerationConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredImageGenerationConfigurationTypeDef = TypedDict(
     "_RequiredImageGenerationConfigurationTypeDef",
     {
         "Status": ConfigurationStatusType,
         "ImageSelectorType": ImageSelectorTypeType,
         "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
         "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalImageGenerationConfigurationTypeDef = TypedDict(
     "_OptionalImageGenerationConfigurationTypeDef",
     {
-        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
+        "FormatConfig": Dict[Literal["JPEGQuality"], str],
         "WidthPixels": int,
         "HeightPixels": int,
     },
     total=False,
 )
 
+
 class ImageGenerationConfigurationTypeDef(
     _RequiredImageGenerationConfigurationTypeDef, _OptionalImageGenerationConfigurationTypeDef
 ):
     pass
 
+
 ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsInputListStreamsPaginateTypeDef",
     {
         "StreamNameCondition": StreamNameConditionTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -935,17 +940,19 @@
     "_OptionalRecorderConfigTypeDef",
     {
         "ScheduleConfig": ScheduleConfigTypeDef,
     },
     total=False,
 )
 
+
 class RecorderConfigTypeDef(_RequiredRecorderConfigTypeDef, _OptionalRecorderConfigTypeDef):
     pass
 
+
 UploaderConfigTypeDef = TypedDict(
     "UploaderConfigTypeDef",
     {
         "ScheduleConfig": ScheduleConfigTypeDef,
     },
 )
 
@@ -965,22 +972,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImageGenerationConfigurationOutputTypeDef = TypedDict(
     "DescribeImageGenerationConfigurationOutputTypeDef",
     {
-        "ImageGenerationConfiguration": ImageGenerationConfigurationOutputTypeDef,
+        "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImageGenerationConfigurationUnionTypeDef = Union[
-    ImageGenerationConfigurationTypeDef, ImageGenerationConfigurationOutputTypeDef
-]
 UpdateImageGenerationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
     },
@@ -1017,17 +1021,19 @@
     {
         "UploaderConfig": UploaderConfigTypeDef,
         "DeletionConfig": DeletionConfigTypeDef,
     },
     total=False,
 )
 
+
 class EdgeConfigTypeDef(_RequiredEdgeConfigTypeDef, _OptionalEdgeConfigTypeDef):
     pass
 
+
 DescribeEdgeConfigurationOutputTypeDef = TypedDict(
     "DescribeEdgeConfigurationOutputTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
@@ -1064,20 +1070,22 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
+
 class StartEdgeConfigurationUpdateInputRequestTypeDef(
     _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef,
     _OptionalStartEdgeConfigurationUpdateInputRequestTypeDef,
 ):
     pass
 
+
 StartEdgeConfigurationUpdateOutputTypeDef = TypedDict(
     "StartEdgeConfigurationUpdateOutputTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
```

### Comparing `mypy-boto3-kinesisvideo-1.28.16/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt` & `mypy-boto3-kinesisvideo-1.28.21/mypy_boto3_kinesisvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisvideo-1.28.16/setup.py` & `mypy-boto3-kinesisvideo-1.28.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesisvideo",
-    version="1.28.16",
+    version="1.28.21",
     packages=["mypy_boto3_kinesisvideo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisVideo 1.28.16 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        "Type annotations for boto3.KinesisVideo 1.28.21 service generated with mypy-boto3-builder"
+        " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

