# Comparing `tmp/cdk-cloudformation-fastly-services-backend-1.2.0a7.tar.gz` & `tmp/cdk-cloudformation-fastly-services-backend-1.4.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/fastly-services-backend/dist/python/cdk-cloudformation-", last modified: Mon Mar 27 06:14:06 2023, max compression
+gzip compressed data, was "cdk-cloudformation-fastly-services-backend-1.4.0a7.tar", last modified: Mon Aug  7 06:17:40 2023, max compression
```

## Comparing `cdk-cloudformation-fastly-services-backend-1.2.0a7.tar` & `cdk-cloudformation-fastly-services-backend-1.4.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-03-27 06:14:00.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-03-27 06:14:00.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2981 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2058 2023-03-27 06:14:00.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-03-27 06:14:00.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1899 2023-03-27 06:14:00.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    34632 2023-03-27 06:14:00.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      462 2023-03-27 06:14:00.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    21064 2023-03-27 06:14:00.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend/_jsii/fastly-services-backend@1.2.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-03-27 06:14:00.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2981 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      682 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       43 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:40.270885 cdk-cloudformation-fastly-services-backend-1.4.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-08-07 06:17:26.000000 cdk-cloudformation-fastly-services-backend-1.4.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-08-07 06:17:26.000000 cdk-cloudformation-fastly-services-backend-1.4.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2981 2023-08-07 06:17:40.270885 cdk-cloudformation-fastly-services-backend-1.4.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2058 2023-08-07 06:17:26.000000 cdk-cloudformation-fastly-services-backend-1.4.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-08-07 06:17:26.000000 cdk-cloudformation-fastly-services-backend-1.4.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-08-07 06:17:40.270885 cdk-cloudformation-fastly-services-backend-1.4.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1898 2023-08-07 06:17:26.000000 cdk-cloudformation-fastly-services-backend-1.4.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:40.266884 cdk-cloudformation-fastly-services-backend-1.4.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:40.266884 cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    34632 2023-08-07 06:17:26.000000 cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:40.270885 cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      462 2023-08-07 06:17:26.000000 cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    21215 2023-08-07 06:17:26.000000 cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend/_jsii/fastly-services-backend@1.4.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-08-07 06:17:26.000000 cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:40.270885 cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2981 2023-08-07 06:17:40.000000 cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      682 2023-08-07 06:17:40.000000 cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-08-07 06:17:40.000000 cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-08-07 06:17:40.000000 cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       43 2023-08-07 06:17:40.000000 cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cdk-cloudformation-fastly-services-backend-1.2.0a7/LICENSE` & `cdk-cloudformation-fastly-services-backend-1.4.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-fastly-services-backend-1.2.0a7/PKG-INFO` & `cdk-cloudformation-fastly-services-backend-1.4.0a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-fastly-services-backend
-Version: 1.2.0a7
+Version: 1.4.0a7
 Summary: Manage a Fastly service backend.
 Home-page: https://github.com/aws-ia/cloudformation-fastly-resource-providers
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fastly-services-backend
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Backend` v1.2.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Backend` v1.4.0.
 
 ## Description
 
 Manage a Fastly service backend.
 
 ## References
 
@@ -56,13 +56,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Fastly::Services::Backend`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-backend+v1.2.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-backend+v1.4.0).
 * Issues related to `Fastly::Services::Backend` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-fastly-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-fastly-services-backend-1.2.0a7/README.md` & `cdk-cloudformation-fastly-services-backend-1.4.0a7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # fastly-services-backend
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Backend` v1.2.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Backend` v1.4.0.
 
 ## Description
 
 Manage a Fastly service backend.
 
 ## References
 
@@ -33,13 +33,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Fastly::Services::Backend`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-backend+v1.2.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-backend+v1.4.0).
 * Issues related to `Fastly::Services::Backend` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-fastly-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-fastly-services-backend-1.2.0a7/setup.py` & `cdk-cloudformation-fastly-services-backend-1.4.0a7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-fastly-services-backend",
-    "version": "1.2.0.a7",
+    "version": "1.4.0.a7",
     "description": "Manage a Fastly service backend.",
     "license": "Apache-2.0",
     "url": "https://github.com/aws-ia/cloudformation-fastly-resource-providers",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_cloudformation_fastly_services_backend",
         "cdk_cloudformation_fastly_services_backend._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_fastly_services_backend._jsii": [
-            "fastly-services-backend@1.2.0-alpha.7.jsii.tgz"
+            "fastly-services-backend@1.4.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_fastly_services_backend": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.70.0, <3.0.0",
-        "constructs>=10.1.292, <11.0.0",
-        "jsii>=1.79.0, <2.0.0",
+        "aws-cdk-lib>=2.89.0, <3.0.0",
+        "constructs>=10.2.69, <11.0.0",
+        "jsii>=1.86.1, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend/__init__.py` & `cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # fastly-services-backend
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Backend` v1.2.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Backend` v1.4.0.
 
 ## Description
 
 Manage a Fastly service backend.
 
 ## References
 
@@ -34,15 +34,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Fastly::Services::Backend`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-backend+v1.2.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-backend+v1.4.0).
 * Issues related to `Fastly::Services::Backend` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-fastly-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
```

### Comparing `cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/PKG-INFO` & `cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-fastly-services-backend
-Version: 1.2.0a7
+Version: 1.4.0a7
 Summary: Manage a Fastly service backend.
 Home-page: https://github.com/aws-ia/cloudformation-fastly-resource-providers
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fastly-services-backend
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Backend` v1.2.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Backend` v1.4.0.
 
 ## Description
 
 Manage a Fastly service backend.
 
 ## References
 
@@ -56,13 +56,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Fastly::Services::Backend`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-backend+v1.2.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-backend+v1.4.0).
 * Issues related to `Fastly::Services::Backend` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-fastly-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-fastly-services-backend-1.2.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/SOURCES.txt` & `cdk-cloudformation-fastly-services-backend-1.4.0a7/src/cdk_cloudformation_fastly_services_backend.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_fastly_services_backend/py.typed
 src/cdk_cloudformation_fastly_services_backend.egg-info/PKG-INFO
 src/cdk_cloudformation_fastly_services_backend.egg-info/SOURCES.txt
 src/cdk_cloudformation_fastly_services_backend.egg-info/dependency_links.txt
 src/cdk_cloudformation_fastly_services_backend.egg-info/requires.txt
 src/cdk_cloudformation_fastly_services_backend.egg-info/top_level.txt
 src/cdk_cloudformation_fastly_services_backend/_jsii/__init__.py
-src/cdk_cloudformation_fastly_services_backend/_jsii/fastly-services-backend@1.2.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_fastly_services_backend/_jsii/fastly-services-backend@1.4.0-alpha.7.jsii.tgz
```

