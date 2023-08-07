# Comparing `tmp/tencentcloud-sdk-python-dlc-3.0.950.tar.gz` & `tmp/tencentcloud-sdk-python-dlc-3.0.951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.950.tar", last modified: Fri Aug  4 00:25:26 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.951.tar", last modified: Mon Aug  7 00:25:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dlc-3.0.950.tar` & `tencentcloud-sdk-python-dlc-3.0.951.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud_sdk_python_dlc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud_sdk_python_dlc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82705 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/dlc_client.py
--rw-r--r--   0 root         (0) root         (0)    11538 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   562911 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-04 00:25:26.000000 tencentcloud-sdk-python-dlc-3.0.950/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud_sdk_python_dlc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud_sdk_python_dlc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud/dlc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud/dlc/v20210125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud/dlc/v20210125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    83580 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud/dlc/v20210125/dlc_client.py
+-rw-r--r--   0 root         (0) root         (0)    11538 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud/dlc/v20210125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   571600 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud/dlc/v20210125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud/dlc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 00:25:15.000000 tencentcloud-sdk-python-dlc-3.0.951/README.rst
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.950/setup.py` & `tencentcloud-sdk-python-dlc-3.0.951/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-dlc',
-    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.951"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Dlc SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.950/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.951/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/dlc_client.py` & `tencentcloud-sdk-python-dlc-3.0.951/tencentcloud/dlc/v20210125/dlc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1586,14 +1586,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeUserRoles(self, request):
+        """列举用户角色信息
+
+        :param request: Request instance for DescribeUserRoles.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeUserRolesRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeUserRolesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeUserRoles", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeUserRolesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeUsers(self, request):
         """获取用户列表信息
 
         :param request: Request instance for DescribeUsers.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeUsersRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeUsersResponse`
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/errorcodes.py` & `tencentcloud-sdk-python-dlc-3.0.951/tencentcloud/dlc/v20210125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/dlc/v20210125/models.py` & `tencentcloud-sdk-python-dlc-3.0.951/tencentcloud/dlc/v20210125/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1873,14 +1873,61 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class CosPermission(AbstractModel):
+    """cos权限描述
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _CosPath: cos路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CosPath: str
+        :param _Permissions: 权限【"read","write"】
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Permissions: list of str
+        """
+        self._CosPath = None
+        self._Permissions = None
+
+    @property
+    def CosPath(self):
+        return self._CosPath
+
+    @CosPath.setter
+    def CosPath(self, CosPath):
+        self._CosPath = CosPath
+
+    @property
+    def Permissions(self):
+        return self._Permissions
+
+    @Permissions.setter
+    def Permissions(self, Permissions):
+        self._Permissions = Permissions
+
+
+    def _deserialize(self, params):
+        self._CosPath = params.get("CosPath")
+        self._Permissions = params.get("Permissions")
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
 class CreateDMSDatabaseRequest(AbstractModel):
     """CreateDMSDatabase请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -11145,14 +11192,149 @@
         self._TotalCount = params.get("TotalCount")
         if params.get("TasksOverview") is not None:
             self._TasksOverview = TasksOverview()
             self._TasksOverview._deserialize(params.get("TasksOverview"))
         self._RequestId = params.get("RequestId")
 
 
+class DescribeUserRolesRequest(AbstractModel):
+    """DescribeUserRoles请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Limit: 列举的数量限制
+        :type Limit: int
+        :param _Offset: 列举的偏移位置
+        :type Offset: int
+        :param _Fuzzy: 按照arn模糊列举
+        :type Fuzzy: str
+        :param _SortBy: 返回结果按照该字段排序
+        :type SortBy: str
+        :param _Sorting: 正序或者倒序，例如：desc
+        :type Sorting: str
+        """
+        self._Limit = None
+        self._Offset = None
+        self._Fuzzy = None
+        self._SortBy = None
+        self._Sorting = None
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
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
+
+    @property
+    def Fuzzy(self):
+        return self._Fuzzy
+
+    @Fuzzy.setter
+    def Fuzzy(self, Fuzzy):
+        self._Fuzzy = Fuzzy
+
+    @property
+    def SortBy(self):
+        return self._SortBy
+
+    @SortBy.setter
+    def SortBy(self, SortBy):
+        self._SortBy = SortBy
+
+    @property
+    def Sorting(self):
+        return self._Sorting
+
+    @Sorting.setter
+    def Sorting(self, Sorting):
+        self._Sorting = Sorting
+
+
+    def _deserialize(self, params):
+        self._Limit = params.get("Limit")
+        self._Offset = params.get("Offset")
+        self._Fuzzy = params.get("Fuzzy")
+        self._SortBy = params.get("SortBy")
+        self._Sorting = params.get("Sorting")
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
+class DescribeUserRolesResponse(AbstractModel):
+    """DescribeUserRoles返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Total: 符合列举条件的总数量
+        :type Total: int
+        :param _UserRoles: 用户角色信息
+        :type UserRoles: list of UserRole
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Total = None
+        self._UserRoles = None
+        self._RequestId = None
+
+    @property
+    def Total(self):
+        return self._Total
+
+    @Total.setter
+    def Total(self, Total):
+        self._Total = Total
+
+    @property
+    def UserRoles(self):
+        return self._UserRoles
+
+    @UserRoles.setter
+    def UserRoles(self, UserRoles):
+        self._UserRoles = UserRoles
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
+        self._Total = params.get("Total")
+        if params.get("UserRoles") is not None:
+            self._UserRoles = []
+            for item in params.get("UserRoles"):
+                obj = UserRole()
+                obj._deserialize(item)
+                self._UserRoles.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeUsersRequest(AbstractModel):
     """DescribeUsers请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -18614,14 +18796,164 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UserRole(AbstractModel):
+    """用户角色
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RoleId: 角色ID
+        :type RoleId: int
+        :param _AppId: 用户app ID
+        :type AppId: str
+        :param _Uin: 用户ID
+        :type Uin: str
+        :param _Arn: 角色权限
+        :type Arn: str
+        :param _ModifyTime: 最近修改时间戳
+        :type ModifyTime: int
+        :param _Desc: 角色描述信息
+        :type Desc: str
+        :param _RoleName: 角色名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RoleName: str
+        :param _Creator: 创建者UIN
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Creator: str
+        :param _CosPermissionList: cos授权路径列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CosPermissionList: list of CosPermission
+        :param _PermissionJson: cam策略json
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PermissionJson: str
+        """
+        self._RoleId = None
+        self._AppId = None
+        self._Uin = None
+        self._Arn = None
+        self._ModifyTime = None
+        self._Desc = None
+        self._RoleName = None
+        self._Creator = None
+        self._CosPermissionList = None
+        self._PermissionJson = None
+
+    @property
+    def RoleId(self):
+        return self._RoleId
+
+    @RoleId.setter
+    def RoleId(self, RoleId):
+        self._RoleId = RoleId
+
+    @property
+    def AppId(self):
+        return self._AppId
+
+    @AppId.setter
+    def AppId(self, AppId):
+        self._AppId = AppId
+
+    @property
+    def Uin(self):
+        return self._Uin
+
+    @Uin.setter
+    def Uin(self, Uin):
+        self._Uin = Uin
+
+    @property
+    def Arn(self):
+        return self._Arn
+
+    @Arn.setter
+    def Arn(self, Arn):
+        self._Arn = Arn
+
+    @property
+    def ModifyTime(self):
+        return self._ModifyTime
+
+    @ModifyTime.setter
+    def ModifyTime(self, ModifyTime):
+        self._ModifyTime = ModifyTime
+
+    @property
+    def Desc(self):
+        return self._Desc
+
+    @Desc.setter
+    def Desc(self, Desc):
+        self._Desc = Desc
+
+    @property
+    def RoleName(self):
+        return self._RoleName
+
+    @RoleName.setter
+    def RoleName(self, RoleName):
+        self._RoleName = RoleName
+
+    @property
+    def Creator(self):
+        return self._Creator
+
+    @Creator.setter
+    def Creator(self, Creator):
+        self._Creator = Creator
+
+    @property
+    def CosPermissionList(self):
+        return self._CosPermissionList
+
+    @CosPermissionList.setter
+    def CosPermissionList(self, CosPermissionList):
+        self._CosPermissionList = CosPermissionList
+
+    @property
+    def PermissionJson(self):
+        return self._PermissionJson
+
+    @PermissionJson.setter
+    def PermissionJson(self, PermissionJson):
+        self._PermissionJson = PermissionJson
+
+
+    def _deserialize(self, params):
+        self._RoleId = params.get("RoleId")
+        self._AppId = params.get("AppId")
+        self._Uin = params.get("Uin")
+        self._Arn = params.get("Arn")
+        self._ModifyTime = params.get("ModifyTime")
+        self._Desc = params.get("Desc")
+        self._RoleName = params.get("RoleName")
+        self._Creator = params.get("Creator")
+        if params.get("CosPermissionList") is not None:
+            self._CosPermissionList = []
+            for item in params.get("CosPermissionList"):
+                obj = CosPermission()
+                obj._deserialize(item)
+                self._CosPermissionList.append(obj)
+        self._PermissionJson = params.get("PermissionJson")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ViewBaseInfo(AbstractModel):
     """视图基本配置信息
 
     """
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.950/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dlc-3.0.951/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dlc-3.0.950/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.951/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.950/README.rst` & `tencentcloud-sdk-python-dlc-3.0.951/README.rst`

 * *Files identical despite different names*

