# Comparing `tmp/mypy-boto3-kinesis-video-archived-media-1.28.16.tar.gz` & `tmp/mypy-boto3-kinesis-video-archived-media-1.28.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesis-video-archived-media-1.28.16.tar", last modified: Tue Aug  1 11:37:06 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesis-video-archived-media-1.28.21.tar", last modified: Mon Aug  7 19:32:27 2023, max compression
```

## Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16.tar` & `mypy-boto3-kinesis-video-archived-media-1.28.21.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.980851 mypy-boto3-kinesis-video-archived-media-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-08-01 11:37:06.980851 mypy-boto3-kinesis-video-archived-media-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.980851 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-08-01 11:21:37.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-08-01 11:21:37.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:06.980851 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 11:37:06.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:06.980851 mypy-boto3-kinesis-video-archived-media-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-01 11:21:36.000000 mypy-boto3-kinesis-video-archived-media-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:32:27.518966 mypy-boto3-kinesis-video-archived-media-1.28.21/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-07 19:32:07.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-08-07 19:32:27.510966 mypy-boto3-kinesis-video-archived-media-1.28.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-08-07 19:32:07.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:32:27.510966 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-07 19:32:07.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-07 19:32:07.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-07 19:32:07.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-08-07 19:32:07.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-08-07 19:32:07.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-08-07 19:32:08.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-08-07 19:32:08.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-07 19:32:07.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-08-07 19:32:07.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:32:07.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-08-07 19:32:09.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-08-07 19:32:08.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-07 19:32:07.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:32:27.510966 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-08-07 19:32:27.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-07 19:32:27.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:32:27.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:32:27.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-07 19:32:27.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-07 19:32:27.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:32:27.518966 mypy-boto3-kinesis-video-archived-media-1.28.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-07 19:32:07.000000 mypy-boto3-kinesis-video-archived-media-1.28.21/setup.py
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/LICENSE` & `mypy-boto3-kinesis-video-archived-media-1.28.21/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/PKG-INFO` & `mypy-boto3-kinesis-video-archived-media-1.28.21/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis-video-archived-media
-Version: 1.28.16
-Summary: Type annotations for boto3.KinesisVideoArchivedMedia 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.21
+Summary: Type annotations for boto3.KinesisVideoArchivedMedia 1.28.21 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-archived-media)](https://pepy.tech/project/mypy-boto3-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoArchivedMedia 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
+[boto3.KinesisVideoArchivedMedia 1.28.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kinesis-video-archived-media docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,83 +300,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_kinesis_video_archived_media.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `KinesisVideoArchivedMedia` Literals can be found in
+[docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/literals/).
+
 ```python
-from mypy_boto3_kinesis_video_archived_media.literals import (
-    ClipFragmentSelectorTypeType,
-    ContainerFormatType,
-    DASHDisplayFragmentNumberType,
-    DASHDisplayFragmentTimestampType,
-    DASHFragmentSelectorTypeType,
-    DASHPlaybackModeType,
-    FormatConfigKeyType,
-    FormatType,
-    FragmentSelectorTypeType,
-    GetImagesPaginatorName,
-    HLSDiscontinuityModeType,
-    HLSDisplayFragmentTimestampType,
-    HLSFragmentSelectorTypeType,
-    HLSPlaybackModeType,
-    ImageErrorType,
-    ImageSelectorTypeType,
-    ListFragmentsPaginatorName,
-    KinesisVideoArchivedMediaServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from mypy_boto3_kinesis_video_archived_media.literals import ClipFragmentSelectorTypeType
 
 
 def check_value(value: ClipFragmentSelectorTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_kinesis_video_archived_media.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `KinesisVideoArchivedMedia` TypeDefs can be found in
+[docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/type_defs/).
+
 ```python
-from mypy_boto3_kinesis_video_archived_media.type_defs import (
-    TimestampTypeDef,
-    FragmentTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    ImageTypeDef,
-    GetMediaForFragmentListInputRequestTypeDef,
-    ClipTimestampRangeTypeDef,
-    DASHTimestampRangeTypeDef,
-    GetImagesInputRequestTypeDef,
-    HLSTimestampRangeTypeDef,
-    TimestampRangeTypeDef,
-    GetClipOutputTypeDef,
-    GetDASHStreamingSessionURLOutputTypeDef,
-    GetHLSStreamingSessionURLOutputTypeDef,
-    GetMediaForFragmentListOutputTypeDef,
-    ListFragmentsOutputTypeDef,
-    GetImagesInputGetImagesPaginateTypeDef,
-    GetImagesOutputTypeDef,
-    ClipFragmentSelectorTypeDef,
-    DASHFragmentSelectorTypeDef,
-    HLSFragmentSelectorTypeDef,
-    FragmentSelectorTypeDef,
-    GetClipInputRequestTypeDef,
-    GetDASHStreamingSessionURLInputRequestTypeDef,
-    GetHLSStreamingSessionURLInputRequestTypeDef,
-    ListFragmentsInputListFragmentsPaginateTypeDef,
-    ListFragmentsInputRequestTypeDef,
-)
+from mypy_boto3_kinesis_video_archived_media.type_defs import TimestampTypeDef
 
 
 def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/README.md` & `mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-kinesis-video-archived-media
+Version: 1.28.21
+Summary: Type annotations for boto3.KinesisVideoArchivedMedia 1.28.21 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 kinesis-video-archived-media type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-kinesis-video-archived-media"></a>
 
 # mypy-boto3-kinesis-video-archived-media
 
 [![PyPI - mypy-boto3-kinesis-video-archived-media](https://img.shields.io/pypi/v/mypy-boto3-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-archived-media)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-archived-media)](https://pepy.tech/project/mypy-boto3-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoArchivedMedia 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
+[boto3.KinesisVideoArchivedMedia 1.28.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kinesis-video-archived-media docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -268,83 +300,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_kinesis_video_archived_media.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `KinesisVideoArchivedMedia` Literals can be found in
+[docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/literals/).
+
 ```python
-from mypy_boto3_kinesis_video_archived_media.literals import (
-    ClipFragmentSelectorTypeType,
-    ContainerFormatType,
-    DASHDisplayFragmentNumberType,
-    DASHDisplayFragmentTimestampType,
-    DASHFragmentSelectorTypeType,
-    DASHPlaybackModeType,
-    FormatConfigKeyType,
-    FormatType,
-    FragmentSelectorTypeType,
-    GetImagesPaginatorName,
-    HLSDiscontinuityModeType,
-    HLSDisplayFragmentTimestampType,
-    HLSFragmentSelectorTypeType,
-    HLSPlaybackModeType,
-    ImageErrorType,
-    ImageSelectorTypeType,
-    ListFragmentsPaginatorName,
-    KinesisVideoArchivedMediaServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from mypy_boto3_kinesis_video_archived_media.literals import ClipFragmentSelectorTypeType
 
 
 def check_value(value: ClipFragmentSelectorTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_kinesis_video_archived_media.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `KinesisVideoArchivedMedia` TypeDefs can be found in
+[docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/type_defs/).
+
 ```python
-from mypy_boto3_kinesis_video_archived_media.type_defs import (
-    TimestampTypeDef,
-    FragmentTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    ImageTypeDef,
-    GetMediaForFragmentListInputRequestTypeDef,
-    ClipTimestampRangeTypeDef,
-    DASHTimestampRangeTypeDef,
-    GetImagesInputRequestTypeDef,
-    HLSTimestampRangeTypeDef,
-    TimestampRangeTypeDef,
-    GetClipOutputTypeDef,
-    GetDASHStreamingSessionURLOutputTypeDef,
-    GetHLSStreamingSessionURLOutputTypeDef,
-    GetMediaForFragmentListOutputTypeDef,
-    ListFragmentsOutputTypeDef,
-    GetImagesInputGetImagesPaginateTypeDef,
-    GetImagesOutputTypeDef,
-    ClipFragmentSelectorTypeDef,
-    DASHFragmentSelectorTypeDef,
-    HLSFragmentSelectorTypeDef,
-    FragmentSelectorTypeDef,
-    GetClipInputRequestTypeDef,
-    GetDASHStreamingSessionURLInputRequestTypeDef,
-    GetHLSStreamingSessionURLInputRequestTypeDef,
-    ListFragmentsInputListFragmentsPaginateTypeDef,
-    ListFragmentsInputRequestTypeDef,
-)
+from mypy_boto3_kinesis_video_archived_media.type_defs import TimestampTypeDef
 
 
 def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/__init__.py` & `mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/__init__.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/__main__.py` & `mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisVideoArchivedMedia 1.28.16\nVersion:        "
-        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
+        "Type annotations for boto3.KinesisVideoArchivedMedia 1.28.21\nVersion:        "
+        " 1.28.21\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia\nOther"
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

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/client.py` & `mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,18 +178,18 @@
 
     def get_images(
         self,
         *,
         ImageSelectorType: ImageSelectorTypeType,
         StartTimestamp: TimestampTypeDef,
         EndTimestamp: TimestampTypeDef,
-        SamplingInterval: int,
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
+        SamplingInterval: int = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> GetImagesOutputTypeDef:
         """
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/client.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -167,18 +167,18 @@
         """
     def get_images(
         self,
         *,
         ImageSelectorType: ImageSelectorTypeType,
         StartTimestamp: TimestampTypeDef,
         EndTimestamp: TimestampTypeDef,
-        SamplingInterval: int,
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
+        SamplingInterval: int = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> GetImagesOutputTypeDef:
         """
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/literals.py` & `mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/literals.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/paginator.py` & `mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -36,55 +36,50 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GetImagesPaginator", "ListFragmentsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class GetImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#getimagespaginator)
     """
 
     def paginate(
         self,
         *,
         ImageSelectorType: ImageSelectorTypeType,
         StartTimestamp: TimestampTypeDef,
         EndTimestamp: TimestampTypeDef,
-        SamplingInterval: int,
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
+        SamplingInterval: int = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetImagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#getimagespaginator)
         """
 
-
 class ListFragmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.ListFragments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#listfragmentspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/paginator.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,50 +36,55 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("GetImagesPaginator", "ListFragmentsPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class GetImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#getimagespaginator)
     """
 
     def paginate(
         self,
         *,
         ImageSelectorType: ImageSelectorTypeType,
         StartTimestamp: TimestampTypeDef,
         EndTimestamp: TimestampTypeDef,
-        SamplingInterval: int,
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
+        SamplingInterval: int = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetImagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#getimagespaginator)
         """
 
+
 class ListFragmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.ListFragments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#listfragmentspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/type_defs.py` & `mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/type_defs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -160,23 +160,23 @@
 
 _RequiredGetImagesInputRequestTypeDef = TypedDict(
     "_RequiredGetImagesInputRequestTypeDef",
     {
         "ImageSelectorType": ImageSelectorTypeType,
         "StartTimestamp": TimestampTypeDef,
         "EndTimestamp": TimestampTypeDef,
-        "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalGetImagesInputRequestTypeDef = TypedDict(
     "_OptionalGetImagesInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
+        "SamplingInterval": int,
         "FormatConfig": Mapping[Literal["JPEGQuality"], str],
         "WidthPixels": int,
         "HeightPixels": int,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -251,23 +251,23 @@
 
 _RequiredGetImagesInputGetImagesPaginateTypeDef = TypedDict(
     "_RequiredGetImagesInputGetImagesPaginateTypeDef",
     {
         "ImageSelectorType": ImageSelectorTypeType,
         "StartTimestamp": TimestampTypeDef,
         "EndTimestamp": TimestampTypeDef,
-        "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalGetImagesInputGetImagesPaginateTypeDef = TypedDict(
     "_OptionalGetImagesInputGetImagesPaginateTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
+        "SamplingInterval": int,
         "FormatConfig": Mapping[Literal["JPEGQuality"], str],
         "WidthPixels": int,
         "HeightPixels": int,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media/type_defs.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media/type_defs.pyi`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -157,23 +157,23 @@
 
 _RequiredGetImagesInputRequestTypeDef = TypedDict(
     "_RequiredGetImagesInputRequestTypeDef",
     {
         "ImageSelectorType": ImageSelectorTypeType,
         "StartTimestamp": TimestampTypeDef,
         "EndTimestamp": TimestampTypeDef,
-        "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalGetImagesInputRequestTypeDef = TypedDict(
     "_OptionalGetImagesInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
+        "SamplingInterval": int,
         "FormatConfig": Mapping[Literal["JPEGQuality"], str],
         "WidthPixels": int,
         "HeightPixels": int,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -246,23 +246,23 @@
 
 _RequiredGetImagesInputGetImagesPaginateTypeDef = TypedDict(
     "_RequiredGetImagesInputGetImagesPaginateTypeDef",
     {
         "ImageSelectorType": ImageSelectorTypeType,
         "StartTimestamp": TimestampTypeDef,
         "EndTimestamp": TimestampTypeDef,
-        "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalGetImagesInputGetImagesPaginateTypeDef = TypedDict(
     "_OptionalGetImagesInputGetImagesPaginateTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
+        "SamplingInterval": int,
         "FormatConfig": Mapping[Literal["JPEGQuality"], str],
         "WidthPixels": int,
         "HeightPixels": int,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/PKG-INFO` & `mypy-boto3-kinesis-video-archived-media-1.28.21/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-kinesis-video-archived-media
-Version: 1.28.16
-Summary: Type annotations for boto3.KinesisVideoArchivedMedia 1.28.16 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kinesis-video-archived-media type-annotations botocore mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-kinesis-video-archived-media"></a>
 
 # mypy-boto3-kinesis-video-archived-media
 
 [![PyPI - mypy-boto3-kinesis-video-archived-media](https://img.shields.io/pypi/v/mypy-boto3-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-archived-media)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-archived-media)](https://pepy.tech/project/mypy-boto3-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoArchivedMedia 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
+[boto3.KinesisVideoArchivedMedia 1.28.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kinesis-video-archived-media docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,83 +268,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_kinesis_video_archived_media.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `KinesisVideoArchivedMedia` Literals can be found in
+[docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/literals/).
+
 ```python
-from mypy_boto3_kinesis_video_archived_media.literals import (
-    ClipFragmentSelectorTypeType,
-    ContainerFormatType,
-    DASHDisplayFragmentNumberType,
-    DASHDisplayFragmentTimestampType,
-    DASHFragmentSelectorTypeType,
-    DASHPlaybackModeType,
-    FormatConfigKeyType,
-    FormatType,
-    FragmentSelectorTypeType,
-    GetImagesPaginatorName,
-    HLSDiscontinuityModeType,
-    HLSDisplayFragmentTimestampType,
-    HLSFragmentSelectorTypeType,
-    HLSPlaybackModeType,
-    ImageErrorType,
-    ImageSelectorTypeType,
-    ListFragmentsPaginatorName,
-    KinesisVideoArchivedMediaServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from mypy_boto3_kinesis_video_archived_media.literals import ClipFragmentSelectorTypeType
 
 
 def check_value(value: ClipFragmentSelectorTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_kinesis_video_archived_media.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `KinesisVideoArchivedMedia` TypeDefs can be found in
+[docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/type_defs/).
+
 ```python
-from mypy_boto3_kinesis_video_archived_media.type_defs import (
-    TimestampTypeDef,
-    FragmentTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    ImageTypeDef,
-    GetMediaForFragmentListInputRequestTypeDef,
-    ClipTimestampRangeTypeDef,
-    DASHTimestampRangeTypeDef,
-    GetImagesInputRequestTypeDef,
-    HLSTimestampRangeTypeDef,
-    TimestampRangeTypeDef,
-    GetClipOutputTypeDef,
-    GetDASHStreamingSessionURLOutputTypeDef,
-    GetHLSStreamingSessionURLOutputTypeDef,
-    GetMediaForFragmentListOutputTypeDef,
-    ListFragmentsOutputTypeDef,
-    GetImagesInputGetImagesPaginateTypeDef,
-    GetImagesOutputTypeDef,
-    ClipFragmentSelectorTypeDef,
-    DASHFragmentSelectorTypeDef,
-    HLSFragmentSelectorTypeDef,
-    FragmentSelectorTypeDef,
-    GetClipInputRequestTypeDef,
-    GetDASHStreamingSessionURLInputRequestTypeDef,
-    GetHLSStreamingSessionURLInputRequestTypeDef,
-    ListFragmentsInputListFragmentsPaginateTypeDef,
-    ListFragmentsInputRequestTypeDef,
-)
+from mypy_boto3_kinesis_video_archived_media.type_defs import TimestampTypeDef
 
 
 def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/mypy_boto3_kinesis_video_archived_media.egg-info/SOURCES.txt` & `mypy-boto3-kinesis-video-archived-media-1.28.21/mypy_boto3_kinesis_video_archived_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.16/setup.py` & `mypy-boto3-kinesis-video-archived-media-1.28.21/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesis-video-archived-media",
-    version="1.28.16",
+    version="1.28.21",
     packages=["mypy_boto3_kinesis_video_archived_media"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisVideoArchivedMedia 1.28.16 service generated with"
-        " mypy-boto3-builder 7.17.1"
+        "Type annotations for boto3.KinesisVideoArchivedMedia 1.28.21 service generated with"
+        " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

