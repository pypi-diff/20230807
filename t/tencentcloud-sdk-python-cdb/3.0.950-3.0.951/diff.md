# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.950.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.950.tar", last modified: Fri Aug  4 00:21:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.951.tar", last modified: Mon Aug  7 00:21:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.950.tar` & `tencentcloud-sdk-python-cdb-3.0.951.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud/cdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud/cdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   146951 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19678 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   798528 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud_sdk_python_cdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-04 00:21:34.000000 tencentcloud-sdk-python-cdb-3.0.950/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud/cdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud/cdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   149717 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20088 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   804311 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud_sdk_python_cdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 00:21:27.000000 tencentcloud-sdk-python-cdb-3.0.951/README.rst
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.950/setup.py` & `tencentcloud-sdk-python-cdb-3.0.951/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cdb',
-    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.951"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cdb SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.950/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.951/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdb-3.0.950/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.951/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1264,14 +1264,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeCpuExpandStrategy(self, request):
+        """通过该 API 可以查询实例的 CPU 弹性扩容策略
+
+        :param request: Request instance for DescribeCpuExpandStrategy.
+        :type request: :class:`tencentcloud.cdb.v20170320.models.DescribeCpuExpandStrategyRequest`
+        :rtype: :class:`tencentcloud.cdb.v20170320.models.DescribeCpuExpandStrategyResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeCpuExpandStrategy", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeCpuExpandStrategyResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeDBFeatures(self, request):
         """本接口(DescribeDBFeatures)用于查询云数据库版本属性，包括是否支持数据库加密、数据库审计等功能。
 
         :param request: Request instance for DescribeDBFeatures.
         :type request: :class:`tencentcloud.cdb.v20170320.models.DescribeDBFeaturesRequest`
         :rtype: :class:`tencentcloud.cdb.v20170320.models.DescribeDBFeaturesResponse`
 
@@ -3133,14 +3156,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def StartCpuExpand(self, request):
+        """通过该API，可以开启CPU弹性扩容，包括一次性的手动扩容以及自动弹性扩容。
+
+        :param request: Request instance for StartCpuExpand.
+        :type request: :class:`tencentcloud.cdb.v20170320.models.StartCpuExpandRequest`
+        :rtype: :class:`tencentcloud.cdb.v20170320.models.StartCpuExpandResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("StartCpuExpand", params, headers=headers)
+            response = json.loads(body)
+            model = models.StartCpuExpandResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def StartReplication(self, request):
         """开启 RO 复制，从主实例同步数据。
 
         :param request: Request instance for StartReplication.
         :type request: :class:`tencentcloud.cdb.v20170320.models.StartReplicationRequest`
         :rtype: :class:`tencentcloud.cdb.v20170320.models.StartReplicationResponse`
 
@@ -3154,14 +3200,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def StopCpuExpand(self, request):
+        """通过该API，可以关闭 CPU 弹性扩容。
+
+        :param request: Request instance for StopCpuExpand.
+        :type request: :class:`tencentcloud.cdb.v20170320.models.StopCpuExpandRequest`
+        :rtype: :class:`tencentcloud.cdb.v20170320.models.StopCpuExpandResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("StopCpuExpand", params, headers=headers)
+            response = json.loads(body)
+            model = models.StopCpuExpandResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopDBImportJob(self, request):
         """本接口(StopDBImportJob)用于终止数据导入任务。
 
         :param request: Request instance for StopDBImportJob.
         :type request: :class:`tencentcloud.cdb.v20170320.models.StopDBImportJobRequest`
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.950/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.951/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,17 @@
 
 # json序列化失败。
 FAILEDOPERATION_JSONMARSHALERROR = 'FailedOperation.JsonMarshalError'
 
 # json反序列化失败。
 FAILEDOPERATION_JSONUNMARSHALERROR = 'FailedOperation.JsonUnmarshalError'
 
+# 检查到改动前后策略一致，无改动点。
+FAILEDOPERATION_NOTCHANGESTRATEGY = 'FailedOperation.NotChangeStrategy'
+
 # 不是延迟复制RO。
 FAILEDOPERATION_NOTDELAYRO = 'FailedOperation.NotDelayRo'
 
 # 实例正在执行其他操作，请稍后重试。
 FAILEDOPERATION_OPERATIONINCONFLICTERR = 'FailedOperation.OperationInConflictErr'
 
 # 执行的权限修改操作非法。您可以参照产品文档，了解当前实例支持哪些权限修改操作，如有疑问，请您咨询客服进行处理。
@@ -100,14 +103,17 @@
 
 # 查询审计任务失败。
 FAILEDOPERATION_QUERYAUDITTASKFAILERROR = 'FailedOperation.QueryAuditTaskFailError'
 
 # 查询日志失败。
 FAILEDOPERATION_QUERYLOGERROR = 'FailedOperation.QueryLogError'
 
+# 高可用版服务跨区调用反序列化失败。
+FAILEDOPERATION_REMOTECALLUNMARSHALERROR = 'FailedOperation.RemoteCallUnmarshalError'
+
 # 代理创建中或则已存在，请勿重复创建。
 FAILEDOPERATION_REPEATCREATEPROXYERROR = 'FailedOperation.RepeatCreateProxyError'
 
 # 后台请求服务异常，请您联系客服解决。
 FAILEDOPERATION_RESPONSEVALUEERROR = 'FailedOperation.ResponseValueError'
 
 # 操作发起失败，请稍后重试。如果操作持续不成功，请您联系客服进行处理。
@@ -556,9 +562,12 @@
 
 # 认证失败，没有足够权限。
 UNAUTHORIZEDOPERATION_NOTENOUGHPRIVILEGES = 'UnauthorizedOperation.NotEnoughPrivileges'
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
 
+# 非强隔离实例不支持当前操作。
+UNSUPPORTEDOPERATION_NOTSUPPORTNORMALINSTANCE = 'UnsupportedOperation.NotSupportNormalInstance'
+
 # 权限不支持。
 UNSUPPORTEDOPERATION_PRIVILEGESUNSUPPORTEDERROR = 'UnsupportedOperation.PrivilegesUnsupportedError'
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.950/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.951/tencentcloud/cdb/v20170320/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6071,15 +6071,15 @@
         :type Port: int
         :param _InstanceRole: 实例类型，默认为 master，支持值包括：master - 表示主实例，dr - 表示灾备实例，ro - 表示只读实例。
         :type InstanceRole: str
         :param _MasterInstanceId: 实例 ID，购买只读实例时必填，该字段表示只读实例的主实例ID，请使用 [查询实例列表](https://cloud.tencent.com/document/api/236/15872) 接口查询云数据库实例 ID。
         :type MasterInstanceId: str
         :param _EngineVersion: MySQL 版本，值包括：5.5、5.6 、5.7和8.0，请使用 [获取云数据库可售卖规格](https://cloud.tencent.com/document/api/236/17229) 接口获取可创建的实例版本。
         :type EngineVersion: str
-        :param _Password: 设置 root 帐号密码，密码规则：8 - 64 个字符，至少包含字母、数字、字符（支持的字符：_+-&=!@#$%^*()）中的两种，购买主实例时可指定该参数，购买只读实例或者灾备实例时指定该参数无意义。
+        :param _Password: 设置 root 账号密码，密码规则：8 - 64 个字符，至少包含字母、数字、字符（支持的字符：_+-&=!@#$%^*()）中的两种，购买主实例时可指定该参数，购买只读实例或者灾备实例时指定该参数无意义。
         :type Password: str
         :param _ProtectMode: 数据复制方式，默认为 0，支持值包括：0 - 表示异步复制，1 - 表示半同步复制，2 - 表示强同步复制。
         :type ProtectMode: int
         :param _DeployMode: 多可用区域，默认为 0，支持值包括：0 - 表示单可用区，1 - 表示多可用区。
         :type DeployMode: int
         :param _SlaveZone: 备库 1 的可用区信息，默认为 Zone 的值。
         :type SlaveZone: str
@@ -6103,15 +6103,15 @@
         :type DeployGroupId: str
         :param _ClientToken: 用于保证请求幂等性的字符串。该字符串由客户生成，需保证不同请求之间在48小时内唯一，最大值不超过64个ASCII字符。若不指定该参数，则无法保证请求的幂等性。
         :type ClientToken: str
         :param _DeviceType: 实例隔离类型。支持值包括： "UNIVERSAL" - 通用型实例， "EXCLUSIVE" - 独享型实例， "BASIC" - 基础版实例。 不指定则默认为通用型实例。
         :type DeviceType: str
         :param _ParamTemplateId: 参数模板id。
         :type ParamTemplateId: int
-        :param _AlarmPolicyList: 告警策略id数组。云监控DescribeAlarmPolicy接口返回的OriginId。
+        :param _AlarmPolicyList: 告警策略id数组。腾讯云可观测平台DescribeAlarmPolicy接口返回的OriginId。
         :type AlarmPolicyList: list of int
         :param _InstanceNodes: 实例节点数。对于 RO 和 基础版实例， 该值默认为1。 如果需要购买三节点实例， 请将该值设置为3 或指定 BackupZone 参数。当购买主实例，且未指定该参数和 BackupZone 参数时，该值默认是 2， 即购买两节点实例。
         :type InstanceNodes: int
         :param _Cpu: 实例cpu核数， 如果不传将根据memory指定的内存值自动填充对应的cpu值。
         :type Cpu: int
         :param _AutoSyncFlag: 是否自动发起灾备同步功能。该参数仅对购买灾备实例生效。 可选值为：0 - 不自动发起灾备同步；1 - 自动发起灾备同步。该值默认为0。
         :type AutoSyncFlag: int
@@ -10626,14 +10626,111 @@
             for item in params.get("Items"):
                 obj = CloneItem()
                 obj._deserialize(item)
                 self._Items.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class DescribeCpuExpandStrategyRequest(AbstractModel):
+    """DescribeCpuExpandStrategy请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例 ID 。
+        :type InstanceId: str
+        """
+        self._InstanceId = None
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
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
+class DescribeCpuExpandStrategyResponse(AbstractModel):
+    """DescribeCpuExpandStrategy返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Type: 策略类型。可选值 auto、manual。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Type: str
+        :param _ExpandCpu: 手动扩容的 CPU 。Type为 manual 时有效。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExpandCpu: str
+        :param _AutoStrategy: 自动扩容策略。Type 为 auto 时有效
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AutoStrategy: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Type = None
+        self._ExpandCpu = None
+        self._AutoStrategy = None
+        self._RequestId = None
+
+    @property
+    def Type(self):
+        return self._Type
+
+    @Type.setter
+    def Type(self, Type):
+        self._Type = Type
+
+    @property
+    def ExpandCpu(self):
+        return self._ExpandCpu
+
+    @ExpandCpu.setter
+    def ExpandCpu(self, ExpandCpu):
+        self._ExpandCpu = ExpandCpu
+
+    @property
+    def AutoStrategy(self):
+        return self._AutoStrategy
+
+    @AutoStrategy.setter
+    def AutoStrategy(self, AutoStrategy):
+        self._AutoStrategy = AutoStrategy
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
+        self._Type = params.get("Type")
+        self._ExpandCpu = params.get("ExpandCpu")
+        self._AutoStrategy = params.get("AutoStrategy")
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeDBFeaturesRequest(AbstractModel):
     """DescribeDBFeatures请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -25138,14 +25235,57 @@
 
 
     def _deserialize(self, params):
         self._AsyncRequestId = params.get("AsyncRequestId")
         self._RequestId = params.get("RequestId")
 
 
+class StartCpuExpandRequest(AbstractModel):
+    """StartCpuExpand请求参数结构体
+
+    """
+
+
+class StartCpuExpandResponse(AbstractModel):
+    """StartCpuExpand返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _AsyncRequestId: 异步任务 ID 。可以调用DescribeAsyncRequest 传入该 ID ，进行任务执行进度的查询
+        :type AsyncRequestId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._AsyncRequestId = None
+        self._RequestId = None
+
+    @property
+    def AsyncRequestId(self):
+        return self._AsyncRequestId
+
+    @AsyncRequestId.setter
+    def AsyncRequestId(self, AsyncRequestId):
+        self._AsyncRequestId = AsyncRequestId
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
+        self._AsyncRequestId = params.get("AsyncRequestId")
+        self._RequestId = params.get("RequestId")
+
+
 class StartReplicationRequest(AbstractModel):
     """StartReplication请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -25187,14 +25327,84 @@
         :type AsyncRequestId: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._AsyncRequestId = None
         self._RequestId = None
 
+    @property
+    def AsyncRequestId(self):
+        return self._AsyncRequestId
+
+    @AsyncRequestId.setter
+    def AsyncRequestId(self, AsyncRequestId):
+        self._AsyncRequestId = AsyncRequestId
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
+        self._AsyncRequestId = params.get("AsyncRequestId")
+        self._RequestId = params.get("RequestId")
+
+
+class StopCpuExpandRequest(AbstractModel):
+    """StopCpuExpand请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例 ID 。
+        :type InstanceId: str
+        """
+        self._InstanceId = None
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
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
+class StopCpuExpandResponse(AbstractModel):
+    """StopCpuExpand返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _AsyncRequestId: 异步任务 ID 。可以调用DescribeAsyncRequest 传入该 ID ，进行任务执行进度的查询
+        :type AsyncRequestId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._AsyncRequestId = None
+        self._RequestId = None
+
     @property
     def AsyncRequestId(self):
         return self._AsyncRequestId
 
     @AsyncRequestId.setter
     def AsyncRequestId(self, AsyncRequestId):
         self._AsyncRequestId = AsyncRequestId
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.950/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.951/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.950/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.951/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.950/README.rst` & `tencentcloud-sdk-python-cdb-3.0.951/README.rst`

 * *Files identical despite different names*

