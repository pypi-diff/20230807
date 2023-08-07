# Comparing `tmp/cdk-cloudformation-fastly-tls-domain-1.1.0a7.tar.gz` & `tmp/cdk-cloudformation-fastly-tls-domain-1.3.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/fastly-tls-domain/dist/python/cdk-cloudformation-fastly", last modified: Mon Mar 27 06:13:52 2023, max compression
+gzip compressed data, was "cdk-cloudformation-fastly-tls-domain-1.3.0a7.tar", last modified: Mon Aug  7 06:17:43 2023, max compression
```

## Comparing `cdk-cloudformation-fastly-tls-domain-1.1.0a7.tar` & `cdk-cloudformation-fastly-tls-domain-1.3.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:13:52.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-03-27 06:13:46.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-03-27 06:13:46.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2853 2023-03-27 06:13:52.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1931 2023-03-27 06:13:46.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-03-27 06:13:46.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-03-27 06:13:52.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1868 2023-03-27 06:13:46.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:13:52.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:13:52.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    21708 2023-03-27 06:13:46.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:13:52.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      450 2023-03-27 06:13:46.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    20162 2023-03-27 06:13:46.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain/_jsii/fastly-tls-domain@1.1.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-03-27 06:13:46.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:13:52.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2853 2023-03-27 06:13:52.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      622 2023-03-27 06:13:52.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-03-27 06:13:52.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-03-27 06:13:52.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       37 2023-03-27 06:13:52.000000 cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:43.767209 cdk-cloudformation-fastly-tls-domain-1.3.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-08-07 06:17:28.000000 cdk-cloudformation-fastly-tls-domain-1.3.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-08-07 06:17:28.000000 cdk-cloudformation-fastly-tls-domain-1.3.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2853 2023-08-07 06:17:43.763209 cdk-cloudformation-fastly-tls-domain-1.3.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1931 2023-08-07 06:17:28.000000 cdk-cloudformation-fastly-tls-domain-1.3.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-08-07 06:17:28.000000 cdk-cloudformation-fastly-tls-domain-1.3.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-08-07 06:17:43.767209 cdk-cloudformation-fastly-tls-domain-1.3.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1867 2023-08-07 06:17:28.000000 cdk-cloudformation-fastly-tls-domain-1.3.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:43.751208 cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:43.759209 cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    21708 2023-08-07 06:17:28.000000 cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:43.763209 cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      450 2023-08-07 06:17:28.000000 cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    20314 2023-08-07 06:17:28.000000 cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain/_jsii/fastly-tls-domain@1.3.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-08-07 06:17:28.000000 cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:43.763209 cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2853 2023-08-07 06:17:43.000000 cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      622 2023-08-07 06:17:43.000000 cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-08-07 06:17:43.000000 cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-08-07 06:17:43.000000 cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       37 2023-08-07 06:17:43.000000 cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cdk-cloudformation-fastly-tls-domain-1.1.0a7/LICENSE` & `cdk-cloudformation-fastly-tls-domain-1.3.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-fastly-tls-domain-1.1.0a7/PKG-INFO` & `cdk-cloudformation-fastly-tls-domain-1.3.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-fastly-tls-domain
-Version: 1.1.0a7
+Version: 1.3.0a7
 Summary: Manage the activation of a Tls Domain
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
 
 # fastly-tls-domain
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Tls::Domain` v1.1.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Tls::Domain` v1.3.0.
 
 ## Description
 
 Manage the activation of a Tls Domain
 
 ## References
 
@@ -55,13 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Fastly::Tls::Domain`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-tls-domain+v1.1.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-tls-domain+v1.3.0).
 * Issues related to `Fastly::Tls::Domain` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-fastly-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-fastly-tls-domain-1.1.0a7/README.md` & `cdk-cloudformation-fastly-tls-domain-1.3.0a7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # fastly-tls-domain
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Tls::Domain` v1.1.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Tls::Domain` v1.3.0.
 
 ## Description
 
 Manage the activation of a Tls Domain
 
 ## References
 
@@ -32,13 +32,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Fastly::Tls::Domain`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-tls-domain+v1.1.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-tls-domain+v1.3.0).
 * Issues related to `Fastly::Tls::Domain` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-fastly-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-fastly-tls-domain-1.1.0a7/setup.py` & `cdk-cloudformation-fastly-tls-domain-1.3.0a7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-fastly-tls-domain",
-    "version": "1.1.0.a7",
+    "version": "1.3.0.a7",
     "description": "Manage the activation of a Tls Domain",
     "license": "Apache-2.0",
     "url": "https://github.com/aws-ia/cloudformation-fastly-resource-providers",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_cloudformation_fastly_tls_domain",
         "cdk_cloudformation_fastly_tls_domain._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_fastly_tls_domain._jsii": [
-            "fastly-tls-domain@1.1.0-alpha.7.jsii.tgz"
+            "fastly-tls-domain@1.3.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_fastly_tls_domain": [
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

### Comparing `cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain/__init__.py` & `cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # fastly-tls-domain
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Tls::Domain` v1.1.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Tls::Domain` v1.3.0.
 
 ## Description
 
 Manage the activation of a Tls Domain
 
 ## References
 
@@ -33,15 +33,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Fastly::Tls::Domain`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-tls-domain+v1.1.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-tls-domain+v1.3.0).
 * Issues related to `Fastly::Tls::Domain` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-fastly-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
```

### Comparing `cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/PKG-INFO` & `cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-fastly-tls-domain
-Version: 1.1.0a7
+Version: 1.3.0a7
 Summary: Manage the activation of a Tls Domain
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
 
 # fastly-tls-domain
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Tls::Domain` v1.1.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Tls::Domain` v1.3.0.
 
 ## Description
 
 Manage the activation of a Tls Domain
 
 ## References
 
@@ -55,13 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Fastly::Tls::Domain`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-tls-domain+v1.1.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-tls-domain+v1.3.0).
 * Issues related to `Fastly::Tls::Domain` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-fastly-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-fastly-tls-domain-1.1.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/SOURCES.txt` & `cdk-cloudformation-fastly-tls-domain-1.3.0a7/src/cdk_cloudformation_fastly_tls_domain.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_fastly_tls_domain/py.typed
 src/cdk_cloudformation_fastly_tls_domain.egg-info/PKG-INFO
 src/cdk_cloudformation_fastly_tls_domain.egg-info/SOURCES.txt
 src/cdk_cloudformation_fastly_tls_domain.egg-info/dependency_links.txt
 src/cdk_cloudformation_fastly_tls_domain.egg-info/requires.txt
 src/cdk_cloudformation_fastly_tls_domain.egg-info/top_level.txt
 src/cdk_cloudformation_fastly_tls_domain/_jsii/__init__.py
-src/cdk_cloudformation_fastly_tls_domain/_jsii/fastly-tls-domain@1.1.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_fastly_tls_domain/_jsii/fastly-tls-domain@1.3.0-alpha.7.jsii.tgz
```

