# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.950.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.950.tar", last modified: Fri Aug  4 00:38:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.951.tar", last modified: Mon Aug  7 00:38:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.950.tar` & `tencentcloud-sdk-python-vpc-3.0.951.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud/vpc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud/vpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   334726 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43302 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1325019 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud_sdk_python_vpc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-04 00:38:18.000000 tencentcloud-sdk-python-vpc-3.0.950/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud/vpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud/vpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   340601 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44508 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1332591 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud_sdk_python_vpc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 00:38:21.000000 tencentcloud-sdk-python-vpc-3.0.951/README.rst
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.950/setup.py` & `tencentcloud-sdk-python-vpc-3.0.951/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-vpc',
-    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.951"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Vpc SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.950/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.951/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def AcceptVpcPeeringConnection(self, request):
+        """本接口（AcceptVpcPeeringConnection）用于接受对等连接请求。
+
+        :param request: Request instance for AcceptVpcPeeringConnection.
+        :type request: :class:`tencentcloud.vpc.v20170312.models.AcceptVpcPeeringConnectionRequest`
+        :rtype: :class:`tencentcloud.vpc.v20170312.models.AcceptVpcPeeringConnectionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("AcceptVpcPeeringConnection", params, headers=headers)
+            response = json.loads(body)
+            model = models.AcceptVpcPeeringConnectionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def AddBandwidthPackageResources(self, request):
         """接口用于添加带宽包资源，包括[弹性公网IP](https://cloud.tencent.com/document/product/213/1941)和[负载均衡](https://cloud.tencent.com/document/product/214/517)等
 
         :param request: Request instance for AddBandwidthPackageResources.
         :type request: :class:`tencentcloud.vpc.v20170312.models.AddBandwidthPackageResourcesRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.AddBandwidthPackageResourcesResponse`
 
@@ -1618,14 +1641,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def CreateVpcPeeringConnection(self, request):
+        """本接口（CreateVpcPeeringConnection）用于创建私有网络对等连接。
+
+        :param request: Request instance for CreateVpcPeeringConnection.
+        :type request: :class:`tencentcloud.vpc.v20170312.models.CreateVpcPeeringConnectionRequest`
+        :rtype: :class:`tencentcloud.vpc.v20170312.models.CreateVpcPeeringConnectionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateVpcPeeringConnection", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateVpcPeeringConnectionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def CreateVpnConnection(self, request):
         """本接口（CreateVpnConnection）用于创建VPN通道。
         >?本接口为异步接口，可调用 [DescribeVpcTaskResult](https://cloud.tencent.com/document/api/215/59037) 接口查询任务执行结果，待任务执行成功后再进行其他操作。
         >
 
         :param request: Request instance for CreateVpnConnection.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateVpnConnectionRequest`
@@ -2538,14 +2584,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DeleteVpcPeeringConnection(self, request):
+        """本接口（DeleteVpcPeeringConnection）用于删除私有网络对等连接。
+
+        :param request: Request instance for DeleteVpcPeeringConnection.
+        :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteVpcPeeringConnectionRequest`
+        :rtype: :class:`tencentcloud.vpc.v20170312.models.DeleteVpcPeeringConnectionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteVpcPeeringConnection", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteVpcPeeringConnectionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DeleteVpnConnection(self, request):
         """本接口（DeleteVpnConnection）用于删除VPN通道。
 
         :param request: Request instance for DeleteVpnConnection.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteVpnConnectionRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.DeleteVpnConnectionResponse`
 
@@ -4376,14 +4445,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeVpcPeeringConnections(self, request):
+        """查询私有网络对等连接。
+
+        :param request: Request instance for DescribeVpcPeeringConnections.
+        :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpcPeeringConnectionsRequest`
+        :rtype: :class:`tencentcloud.vpc.v20170312.models.DescribeVpcPeeringConnectionsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeVpcPeeringConnections", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeVpcPeeringConnectionsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeVpcPrivateIpAddresses(self, request):
         """本接口（DescribeVpcPrivateIpAddresses）用于查询VPC内网IP信息。<br />
         只能查询已使用的IP信息，当查询未使用的IP时，本接口不会报错，但不会出现在返回结果里。
 
         :param request: Request instance for DescribeVpcPrivateIpAddresses.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpcPrivateIpAddressesRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.DescribeVpcPrivateIpAddressesResponse`
@@ -6516,14 +6608,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def ModifyVpcPeeringConnection(self, request):
+        """本接口（ModifyVpcPeeringConnection）用于修改私有网络对等连接属性。
+
+        :param request: Request instance for ModifyVpcPeeringConnection.
+        :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyVpcPeeringConnectionRequest`
+        :rtype: :class:`tencentcloud.vpc.v20170312.models.ModifyVpcPeeringConnectionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyVpcPeeringConnection", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyVpcPeeringConnectionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def ModifyVpnConnectionAttribute(self, request):
         """本接口（ModifyVpnConnectionAttribute）用于修改VPN通道。
 
         :param request: Request instance for ModifyVpnConnectionAttribute.
         :type request: :class:`tencentcloud.vpc.v20170312.models.ModifyVpnConnectionAttributeRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.ModifyVpnConnectionAttributeResponse`
 
@@ -6675,14 +6790,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def RejectVpcPeeringConnection(self, request):
+        """本接口（RejectVpcPeeringConnection）用于驳回对等连接请求。
+
+        :param request: Request instance for RejectVpcPeeringConnection.
+        :type request: :class:`tencentcloud.vpc.v20170312.models.RejectVpcPeeringConnectionRequest`
+        :rtype: :class:`tencentcloud.vpc.v20170312.models.RejectVpcPeeringConnectionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RejectVpcPeeringConnection", params, headers=headers)
+            response = json.loads(body)
+            model = models.RejectVpcPeeringConnectionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ReleaseAddresses(self, request):
         """本接口 (ReleaseAddresses) 用于释放一个或多个[弹性公网IP](https://cloud.tencent.com/document/product/213/1941)（简称 EIP）。
         * 该操作不可逆，释放后 EIP 关联的 IP 地址将不再属于您的名下。
         * 只有状态为 UNBIND 的 EIP 才能进行释放操作。
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.950/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.951/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,17 @@
 
 # 入参重复。
 INVALIDPARAMETERVALUE_DUPLICATE = 'InvalidParameterValue.Duplicate'
 
 # 参数值存在重复。
 INVALIDPARAMETERVALUE_DUPLICATEPARA = 'InvalidParameterValue.DuplicatePara'
 
+# 本端地域和端地域重复。
+INVALIDPARAMETERVALUE_DUPLICATEREGION = 'InvalidParameterValue.DuplicateRegion'
+
 # 值超过上限。
 INVALIDPARAMETERVALUE_EIPBRANDWIDTHOUTINVALID = 'InvalidParameterValue.EIPBrandWidthOutInvalid'
 
 # 缺少参数。
 INVALIDPARAMETERVALUE_EMPTY = 'InvalidParameterValue.Empty'
 
 # IPv6转换实例ID已经存在。
@@ -553,14 +556,20 @@
 
 # 标签键的数目已达到上限。
 LIMITEXCEEDED_TAGTAGSEXCEEDED = 'LimitExceeded.TagTagsExceeded'
 
 # 流量包配额超过限制。
 LIMITEXCEEDED_TRAFFICPACKAGEQUOTA = 'LimitExceeded.TrafficPackageQuota'
 
+# 有效的对等个数超过配额上限。
+LIMITEXCEEDED_VPCPEERAVALIMITEXCEEDED = 'LimitExceeded.VpcPeerAvaLimitExceeded'
+
+# 可创建的对等连接个数超过总上限。
+LIMITEXCEEDED_VPCPEERTOTALLIMITEXCEEDED = 'LimitExceeded.VpcPeerTotalLimitExceeded'
+
 # 缺少参数错误。
 MISSINGPARAMETER = 'MissingParameter'
 
 # 指定公网IP处于隔离状态。
 OPERATIONDENIED_ADDRESSINARREARS = 'OperationDenied.AddressInArrears'
 
 # 互斥的任务正在执行。
@@ -607,14 +616,17 @@
 
 # 账号未实名。
 UNAUTHORIZEDOPERATION_NOREALNAMEAUTHENTICATION = 'UnauthorizedOperation.NoRealNameAuthentication'
 
 # 主IP不支持指定操作。
 UNAUTHORIZEDOPERATION_PRIMARYIP = 'UnauthorizedOperation.PrimaryIp'
 
+# 对等连接本端VPC与对端VPC存在CIDR冲突,或一端与已建立的对等连接某一端冲突。
+UNAUTHORIZEDOPERATION_VPCPEERCIDRCONFLICT = 'UnauthorizedOperation.VpcPeerCidrConflict'
+
 # 未知参数错误。
 UNKNOWNPARAMETER = 'UnknownParameter'
 
 # 参数无法识别，可以尝试相似参数代替。
 UNKNOWNPARAMETER_WITHGUESS = 'UnknownParameter.WithGuess'
 
 # 操作不支持。
@@ -865,14 +877,17 @@
 
 # 当前云联网不支持同时关联EDGE实例和跨境实例
 UNSUPPORTEDOPERATION_NOTSUPPORTATTACHEDGEANDCROSSBORDERINSTANCE = 'UnsupportedOperation.NotSupportAttachEdgeAndCrossBorderInstance'
 
 # 不支持删除默认路由表。
 UNSUPPORTEDOPERATION_NOTSUPPORTDELETEDEFAULTROUTETABLE = 'UnsupportedOperation.NotSupportDeleteDefaultRouteTable'
 
+# 公有云到黑石的对等连接不支持删除。
+UNSUPPORTEDOPERATION_NOTSUPPORTDELETEVPCBMPEER = 'UnsupportedOperation.NotSupportDeleteVpcBmPeer'
+
 # 该地址类型不支持释放操作。
 UNSUPPORTEDOPERATION_NOTSUPPORTEDADDRESSIPSCHARGETYPE = 'UnsupportedOperation.NotSupportedAddressIpsChargeType'
 
 # 此地域没有上线出口二资源，请到北京/广州/南京购买。
 UNSUPPORTEDOPERATION_NOTSUPPORTEDPURCHASECENTEREGRESSRESOURCE = 'UnsupportedOperation.NotSupportedPurchaseCenterEgressResource'
 
 # 当前云联网不支持更新路由发布。
@@ -1012,14 +1027,26 @@
 
 # 指定安全组规则版本号和当前最新版本不一致。
 UNSUPPORTEDOPERATION_VERSIONMISMATCH = 'UnsupportedOperation.VersionMismatch'
 
 # 资源不属于同一个VPC。
 UNSUPPORTEDOPERATION_VPCMISMATCH = 'UnsupportedOperation.VpcMismatch'
 
+# 对等连接已存在。
+UNSUPPORTEDOPERATION_VPCPEERALREADYEXIST = 'UnsupportedOperation.VpcPeerAlreadyExist'
+
+# VPC网段存在CIDR冲突。
+UNSUPPORTEDOPERATION_VPCPEERCIDRCONFLICT = 'UnsupportedOperation.VpcPeerCidrConflict'
+
+# 对等连接状态错误。
+UNSUPPORTEDOPERATION_VPCPEERINVALIDSTATECHANGE = 'UnsupportedOperation.VpcPeerInvalidStateChange'
+
+# 该账不能发起操作。
+UNSUPPORTEDOPERATION_VPCPEERPURVIEWERROR = 'UnsupportedOperation.VpcPeerPurviewError'
+
 # 当前通道为非可用状态，不支持该操作。
 UNSUPPORTEDOPERATION_VPNCONNINVALIDSTATE = 'UnsupportedOperation.VpnConnInvalidState'
 
 # VPC类型VPN网关必须携带VpcId。
 UNSUPPORTEDOPERATION_VPNGWVPCIDMUSTHAVE = 'UnsupportedOperation.VpnGwVpcIdMustHave'
 
 # 指定资源在不同的可用区。
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.950/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.951/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,45 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class AcceptVpcPeeringConnectionRequest(AbstractModel):
+    """AcceptVpcPeeringConnection请求参数结构体
+
+    """
+
+
+class AcceptVpcPeeringConnectionResponse(AbstractModel):
+    """AcceptVpcPeeringConnection返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._RequestId = params.get("RequestId")
+
+
 class AccessPolicy(AbstractModel):
     """策略信息
 
     """
 
     def __init__(self):
         r"""
@@ -9477,14 +9508,45 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class CreateVpcPeeringConnectionRequest(AbstractModel):
+    """CreateVpcPeeringConnection请求参数结构体
+
+    """
+
+
+class CreateVpcPeeringConnectionResponse(AbstractModel):
+    """CreateVpcPeeringConnection返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._RequestId = params.get("RequestId")
+
+
 class CreateVpcRequest(AbstractModel):
     """CreateVpc请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -13312,14 +13374,45 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class DeleteVpcPeeringConnectionRequest(AbstractModel):
+    """DeleteVpcPeeringConnection请求参数结构体
+
+    """
+
+
+class DeleteVpcPeeringConnectionResponse(AbstractModel):
+    """DeleteVpcPeeringConnection返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._RequestId = params.get("RequestId")
+
+
 class DeleteVpcRequest(AbstractModel):
     """DeleteVpc请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -22524,14 +22617,140 @@
             for item in params.get("VpcLimitSet"):
                 obj = VpcLimit()
                 obj._deserialize(item)
                 self._VpcLimitSet.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class DescribeVpcPeeringConnectionsRequest(AbstractModel):
+    """DescribeVpcPeeringConnections请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PeeringConnectionIds: 对等连接唯一ID数组。
+        :type PeeringConnectionIds: list of str
+        :param _Filters: 过滤条件，参数不支持同时指定PeeringConnectionIds和Filters。
+<li>vpc-id - String - （过滤条件）VPC实例ID，形如：vpc-f49l6u0z。</li>
+<li>state String - （过滤条件）对等连接状态，可选值有：PENDING，投放中；ACTIVE，使用中；EXPIRED，已过期；REJECTED，拒绝。</li>
+<li>peering-connection-name - String - （过滤条件）对等连接名称。</li>
+        :type Filters: list of Filter
+        :param _Offset: 偏移量。
+        :type Offset: int
+        :param _Limit: 请求对象个数。
+        :type Limit: int
+        :param _OrderField: 排序字段，可选值有：CreatedTime，PeeringConnectionName。
+        :type OrderField: str
+        :param _OrderDirection: 排序方式：DESC，降序；ASC，升序。
+        :type OrderDirection: str
+        """
+        self._PeeringConnectionIds = None
+        self._Filters = None
+        self._Offset = None
+        self._Limit = None
+        self._OrderField = None
+        self._OrderDirection = None
+
+    @property
+    def PeeringConnectionIds(self):
+        return self._PeeringConnectionIds
+
+    @PeeringConnectionIds.setter
+    def PeeringConnectionIds(self, PeeringConnectionIds):
+        self._PeeringConnectionIds = PeeringConnectionIds
+
+    @property
+    def Filters(self):
+        return self._Filters
+
+    @Filters.setter
+    def Filters(self, Filters):
+        self._Filters = Filters
+
+    @property
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
+
+    @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
+    @property
+    def OrderField(self):
+        return self._OrderField
+
+    @OrderField.setter
+    def OrderField(self, OrderField):
+        self._OrderField = OrderField
+
+    @property
+    def OrderDirection(self):
+        return self._OrderDirection
+
+    @OrderDirection.setter
+    def OrderDirection(self, OrderDirection):
+        self._OrderDirection = OrderDirection
+
+
+    def _deserialize(self, params):
+        self._PeeringConnectionIds = params.get("PeeringConnectionIds")
+        if params.get("Filters") is not None:
+            self._Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self._Filters.append(obj)
+        self._Offset = params.get("Offset")
+        self._Limit = params.get("Limit")
+        self._OrderField = params.get("OrderField")
+        self._OrderDirection = params.get("OrderDirection")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeVpcPeeringConnectionsResponse(AbstractModel):
+    """DescribeVpcPeeringConnections返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeVpcPrivateIpAddressesRequest(AbstractModel):
     """DescribeVpcPrivateIpAddresses请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -33378,14 +33597,45 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class ModifyVpcPeeringConnectionRequest(AbstractModel):
+    """ModifyVpcPeeringConnection请求参数结构体
+
+    """
+
+
+class ModifyVpcPeeringConnectionResponse(AbstractModel):
+    """ModifyVpcPeeringConnection返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._RequestId = params.get("RequestId")
+
+
 class ModifyVpnConnectionAttributeRequest(AbstractModel):
     """ModifyVpnConnectionAttribute请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -36203,14 +36453,45 @@
 
     """
 
     def __init__(self):
         r"""
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
+        """
+        self._RequestId = None
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._RequestId = params.get("RequestId")
+
+
+class RejectVpcPeeringConnectionRequest(AbstractModel):
+    """RejectVpcPeeringConnection请求参数结构体
+
+    """
+
+
+class RejectVpcPeeringConnectionResponse(AbstractModel):
+    """RejectVpcPeeringConnection返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
         self._RequestId = None
 
     @property
     def RequestId(self):
         return self._RequestId
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.950/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.951/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.950'
+__version__ = '3.0.951'
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.950/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.951/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.950/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.951/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.950/README.rst` & `tencentcloud-sdk-python-vpc-3.0.951/README.rst`

 * *Files identical despite different names*

