# Comparing `tmp/cdk-cloudformation-fastly-services-domain-1.2.0a7.tar.gz` & `tmp/cdk-cloudformation-fastly-services-domain-1.4.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/fastly-services-domain/dist/python/cdk-cloudformation-f", last modified: Mon Mar 27 06:14:06 2023, max compression
+gzip compressed data, was "cdk-cloudformation-fastly-services-domain-1.4.0a7.tar", last modified: Mon Aug  7 06:17:31 2023, max compression
```

## Comparing `cdk-cloudformation-fastly-services-domain-1.2.0a7.tar` & `cdk-cloudformation-fastly-services-domain-1.4.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-03-27 06:13:59.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-03-27 06:13:59.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2971 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2050 2023-03-27 06:13:59.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-03-27 06:13:59.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1892 2023-03-27 06:13:59.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    12186 2023-03-27 06:13:59.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      460 2023-03-27 06:13:59.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    17418 2023-03-27 06:13:59.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain/_jsii/fastly-services-domain@1.2.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-03-27 06:13:59.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2971 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      672 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       42 2023-03-27 06:14:06.000000 cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:31.213300 cdk-cloudformation-fastly-services-domain-1.4.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-08-07 06:17:16.000000 cdk-cloudformation-fastly-services-domain-1.4.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-08-07 06:17:16.000000 cdk-cloudformation-fastly-services-domain-1.4.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2971 2023-08-07 06:17:31.213300 cdk-cloudformation-fastly-services-domain-1.4.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2050 2023-08-07 06:17:16.000000 cdk-cloudformation-fastly-services-domain-1.4.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-08-07 06:17:16.000000 cdk-cloudformation-fastly-services-domain-1.4.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-08-07 06:17:31.213300 cdk-cloudformation-fastly-services-domain-1.4.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1891 2023-08-07 06:17:16.000000 cdk-cloudformation-fastly-services-domain-1.4.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:31.205300 cdk-cloudformation-fastly-services-domain-1.4.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:31.209300 cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    12931 2023-08-07 06:17:16.000000 cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:31.209300 cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      460 2023-08-07 06:17:16.000000 cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    17773 2023-08-07 06:17:16.000000 cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain/_jsii/fastly-services-domain@1.4.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-08-07 06:17:16.000000 cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-08-07 06:17:31.209300 cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2971 2023-08-07 06:17:31.000000 cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      672 2023-08-07 06:17:31.000000 cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-08-07 06:17:31.000000 cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-08-07 06:17:31.000000 cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       42 2023-08-07 06:17:31.000000 cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cdk-cloudformation-fastly-services-domain-1.2.0a7/LICENSE` & `cdk-cloudformation-fastly-services-domain-1.4.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-fastly-services-domain-1.2.0a7/PKG-INFO` & `cdk-cloudformation-fastly-services-domain-1.4.0a7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-fastly-services-domain
-Version: 1.2.0a7
+Version: 1.4.0a7
 Summary: Manage a Fastly service domain.
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
 
 # fastly-services-domain
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Domain` v1.2.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Domain` v1.4.0.
 
 ## Description
 
 Manage a Fastly service domain.
 
 ## References
 
@@ -56,13 +56,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Fastly::Services::Domain`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-domain+v1.2.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-domain+v1.4.0).
 * Issues related to `Fastly::Services::Domain` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-fastly-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-fastly-services-domain-1.2.0a7/README.md` & `cdk-cloudformation-fastly-services-domain-1.4.0a7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # fastly-services-domain
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Domain` v1.2.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Domain` v1.4.0.
 
 ## Description
 
 Manage a Fastly service domain.
 
 ## References
 
@@ -33,13 +33,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Fastly::Services::Domain`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-domain+v1.2.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-domain+v1.4.0).
 * Issues related to `Fastly::Services::Domain` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-fastly-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-fastly-services-domain-1.2.0a7/setup.py` & `cdk-cloudformation-fastly-services-domain-1.4.0a7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-fastly-services-domain",
-    "version": "1.2.0.a7",
+    "version": "1.4.0.a7",
     "description": "Manage a Fastly service domain.",
     "license": "Apache-2.0",
     "url": "https://github.com/aws-ia/cloudformation-fastly-resource-providers",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_cloudformation_fastly_services_domain",
         "cdk_cloudformation_fastly_services_domain._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_fastly_services_domain._jsii": [
-            "fastly-services-domain@1.2.0-alpha.7.jsii.tgz"
+            "fastly-services-domain@1.4.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_fastly_services_domain": [
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

### Comparing `cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain/__init__.py` & `cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # fastly-services-domain
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Domain` v1.2.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Domain` v1.4.0.
 
 ## Description
 
 Manage a Fastly service domain.
 
 ## References
 
@@ -34,15 +34,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Fastly::Services::Domain`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-domain+v1.2.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-domain+v1.4.0).
 * Issues related to `Fastly::Services::Domain` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-fastly-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
@@ -77,33 +77,35 @@
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
         service_id: builtins.str,
-        version_id: builtins.str,
+        version_id: jsii.Number,
         comment: typing.Optional[builtins.str] = None,
         created_at: typing.Optional[datetime.datetime] = None,
         deleted_at: typing.Optional[datetime.datetime] = None,
         domain_name: typing.Optional[builtins.str] = None,
+        service: typing.Optional[builtins.str] = None,
         updated_at: typing.Optional[datetime.datetime] = None,
-        version: typing.Optional[builtins.str] = None,
+        version: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''Create a new ``Fastly::Services::Domain``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param name: 
         :param service_id: 
         :param version_id: 
         :param comment: 
         :param created_at: 
         :param deleted_at: 
         :param domain_name: 
+        :param service: 
         :param updated_at: 
         :param version: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b2ecc58ed5375cf1aa8ab5f97d04b3d35cb931520d8e4b9478c69206bf527c77)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
@@ -111,14 +113,15 @@
             name=name,
             service_id=service_id,
             version_id=version_id,
             comment=comment,
             created_at=created_at,
             deleted_at=deleted_at,
             domain_name=domain_name,
+            service=service,
             updated_at=updated_at,
             version=version,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.python.classproperty
@@ -141,55 +144,59 @@
         "name": "name",
         "service_id": "serviceId",
         "version_id": "versionId",
         "comment": "comment",
         "created_at": "createdAt",
         "deleted_at": "deletedAt",
         "domain_name": "domainName",
+        "service": "service",
         "updated_at": "updatedAt",
         "version": "version",
     },
 )
 class CfnDomainProps:
     def __init__(
         self,
         *,
         name: builtins.str,
         service_id: builtins.str,
-        version_id: builtins.str,
+        version_id: jsii.Number,
         comment: typing.Optional[builtins.str] = None,
         created_at: typing.Optional[datetime.datetime] = None,
         deleted_at: typing.Optional[datetime.datetime] = None,
         domain_name: typing.Optional[builtins.str] = None,
+        service: typing.Optional[builtins.str] = None,
         updated_at: typing.Optional[datetime.datetime] = None,
-        version: typing.Optional[builtins.str] = None,
+        version: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''Manage a Fastly service domain.
 
         :param name: 
         :param service_id: 
         :param version_id: 
         :param comment: 
         :param created_at: 
         :param deleted_at: 
         :param domain_name: 
+        :param service: 
         :param updated_at: 
         :param version: 
 
         :schema: CfnDomainProps
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4c7f119958b7fecc973cb67c19ae3538ad24f98bf83d16fb01994370e9789b23)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument service_id", value=service_id, expected_type=type_hints["service_id"])
             check_type(argname="argument version_id", value=version_id, expected_type=type_hints["version_id"])
             check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
             check_type(argname="argument created_at", value=created_at, expected_type=type_hints["created_at"])
             check_type(argname="argument deleted_at", value=deleted_at, expected_type=type_hints["deleted_at"])
             check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
+            check_type(argname="argument service", value=service, expected_type=type_hints["service"])
             check_type(argname="argument updated_at", value=updated_at, expected_type=type_hints["updated_at"])
             check_type(argname="argument version", value=version, expected_type=type_hints["version"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "name": name,
             "service_id": service_id,
             "version_id": version_id,
         }
@@ -197,14 +204,16 @@
             self._values["comment"] = comment
         if created_at is not None:
             self._values["created_at"] = created_at
         if deleted_at is not None:
             self._values["deleted_at"] = deleted_at
         if domain_name is not None:
             self._values["domain_name"] = domain_name
+        if service is not None:
+            self._values["service"] = service
         if updated_at is not None:
             self._values["updated_at"] = updated_at
         if version is not None:
             self._values["version"] = version
 
     @builtins.property
     def name(self) -> builtins.str:
@@ -221,21 +230,21 @@
         :schema: CfnDomainProps#ServiceId
         '''
         result = self._values.get("service_id")
         assert result is not None, "Required property 'service_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def version_id(self) -> builtins.str:
+    def version_id(self) -> jsii.Number:
         '''
         :schema: CfnDomainProps#VersionId
         '''
         result = self._values.get("version_id")
         assert result is not None, "Required property 'version_id' is missing"
-        return typing.cast(builtins.str, result)
+        return typing.cast(jsii.Number, result)
 
     @builtins.property
     def comment(self) -> typing.Optional[builtins.str]:
         '''
         :schema: CfnDomainProps#Comment
         '''
         result = self._values.get("comment")
@@ -262,28 +271,36 @@
         '''
         :schema: CfnDomainProps#DomainName
         '''
         result = self._values.get("domain_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def service(self) -> typing.Optional[builtins.str]:
+        '''
+        :schema: CfnDomainProps#Service
+        '''
+        result = self._values.get("service")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def updated_at(self) -> typing.Optional[datetime.datetime]:
         '''
         :schema: CfnDomainProps#UpdatedAt
         '''
         result = self._values.get("updated_at")
         return typing.cast(typing.Optional[datetime.datetime], result)
 
     @builtins.property
-    def version(self) -> typing.Optional[builtins.str]:
+    def version(self) -> typing.Optional[jsii.Number]:
         '''
         :schema: CfnDomainProps#Version
         '''
         result = self._values.get("version")
-        return typing.cast(typing.Optional[builtins.str], result)
+        return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -302,32 +319,34 @@
 
 def _typecheckingstub__b2ecc58ed5375cf1aa8ab5f97d04b3d35cb931520d8e4b9478c69206bf527c77(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     name: builtins.str,
     service_id: builtins.str,
-    version_id: builtins.str,
+    version_id: jsii.Number,
     comment: typing.Optional[builtins.str] = None,
     created_at: typing.Optional[datetime.datetime] = None,
     deleted_at: typing.Optional[datetime.datetime] = None,
     domain_name: typing.Optional[builtins.str] = None,
+    service: typing.Optional[builtins.str] = None,
     updated_at: typing.Optional[datetime.datetime] = None,
-    version: typing.Optional[builtins.str] = None,
+    version: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__4c7f119958b7fecc973cb67c19ae3538ad24f98bf83d16fb01994370e9789b23(
     *,
     name: builtins.str,
     service_id: builtins.str,
-    version_id: builtins.str,
+    version_id: jsii.Number,
     comment: typing.Optional[builtins.str] = None,
     created_at: typing.Optional[datetime.datetime] = None,
     deleted_at: typing.Optional[datetime.datetime] = None,
     domain_name: typing.Optional[builtins.str] = None,
+    service: typing.Optional[builtins.str] = None,
     updated_at: typing.Optional[datetime.datetime] = None,
-    version: typing.Optional[builtins.str] = None,
+    version: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/PKG-INFO` & `cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-fastly-services-domain
-Version: 1.2.0a7
+Version: 1.4.0a7
 Summary: Manage a Fastly service domain.
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
 
 # fastly-services-domain
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Domain` v1.2.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Fastly::Services::Domain` v1.4.0.
 
 ## Description
 
 Manage a Fastly service domain.
 
 ## References
 
@@ -56,13 +56,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Fastly::Services::Domain`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-domain+v1.2.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Ffastly-services-domain+v1.4.0).
 * Issues related to `Fastly::Services::Domain` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-fastly-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-fastly-services-domain-1.2.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/SOURCES.txt` & `cdk-cloudformation-fastly-services-domain-1.4.0a7/src/cdk_cloudformation_fastly_services_domain.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_fastly_services_domain/py.typed
 src/cdk_cloudformation_fastly_services_domain.egg-info/PKG-INFO
 src/cdk_cloudformation_fastly_services_domain.egg-info/SOURCES.txt
 src/cdk_cloudformation_fastly_services_domain.egg-info/dependency_links.txt
 src/cdk_cloudformation_fastly_services_domain.egg-info/requires.txt
 src/cdk_cloudformation_fastly_services_domain.egg-info/top_level.txt
 src/cdk_cloudformation_fastly_services_domain/_jsii/__init__.py
-src/cdk_cloudformation_fastly_services_domain/_jsii/fastly-services-domain@1.2.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_fastly_services_domain/_jsii/fastly-services-domain@1.4.0-alpha.7.jsii.tgz
```

