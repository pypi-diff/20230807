# Comparing `tmp/tencentcloud-sdk-python-gme-3.0.950.tar.gz` & `tmp/tencentcloud-sdk-python-gme-3.0.951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-gme-3.0.950.tar", last modified: Fri Aug  4 00:27:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-gme-3.0.951.tar", last modified: Mon Aug  7 00:27:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-gme-3.0.950.tar` & `tencentcloud-sdk-python-gme-3.0.951.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud/gme/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud/gme/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud/gme/v20180711/
--rw-r--r--   0 root         (0) root         (0)    33362 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud/gme/v20180711/gme_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud/gme/v20180711/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3906 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud/gme/v20180711/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   157807 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud/gme/v20180711/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud_sdk_python_gme.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud_sdk_python_gme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud_sdk_python_gme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud_sdk_python_gme.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud_sdk_python_gme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:27:30.000000 tencentcloud-sdk-python-gme-3.0.950/tencentcloud_sdk_python_gme.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud/gme/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud/gme/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud/gme/v20180711/
+-rw-r--r--   0 root         (0) root         (0)    34890 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud/gme/v20180711/gme_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud/gme/v20180711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3906 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud/gme/v20180711/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   157807 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud/gme/v20180711/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud_sdk_python_gme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud_sdk_python_gme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud_sdk_python_gme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud_sdk_python_gme.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud_sdk_python_gme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 00:27:14.000000 tencentcloud-sdk-python-gme-3.0.951/tencentcloud_sdk_python_gme.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-gme-3.0.950/setup.py` & `tencentcloud-sdk-python-gme-3.0.951/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-gme',
-    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.951"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Gme SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-gme-3.0.950/tencentcloud/__init__.py` & `tencentcloud-sdk-python-gme-3.0.951/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-gme-3.0.950/tencentcloud/gme/v20180711/gme_client.py` & `tencentcloud-sdk-python-gme-3.0.951/tencentcloud/gme/v20180711/gme_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateScanUser(self, request):
-        """新增自定义送检用户
+        """新增自定义送检用户。**接口使用前提**：目前 CreateScanUser 接口通过白名单开放，如需使用，需要 [提交工单申请](https://console.cloud.tencent.com/workorder/category?level1_id=438&level2_id=445&source=0&data_title=%E6%B8%B8%E6%88%8F%E5%A4%9A%E5%AA%92%E4%BD%93%E5%BC%95%E6%93%8EGME&step=1)。
 
         :param request: Request instance for CreateScanUser.
         :type request: :class:`tencentcloud.gme.v20180711.models.CreateScanUserRequest`
         :rtype: :class:`tencentcloud.gme.v20180711.models.CreateScanUserResponse`
 
         """
         try:
@@ -171,15 +171,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteScanUser(self, request):
-        """删除自定义送检用户
+        """删除自定义送检用户。**接口使用前提**：目前 DeleteScanUser 接口通过白名单开放，如需使用，需要 [提交工单申请](https://console.cloud.tencent.com/workorder/category?level1_id=438&level2_id=445&source=0&data_title=%E6%B8%B8%E6%88%8F%E5%A4%9A%E5%AA%92%E4%BD%93%E5%BC%95%E6%93%8EGME&step=1)。
 
         :param request: Request instance for DeleteScanUser.
         :type request: :class:`tencentcloud.gme.v20180711.models.DeleteScanUserRequest`
         :rtype: :class:`tencentcloud.gme.v20180711.models.DeleteScanUserResponse`
 
         """
         try:
@@ -286,15 +286,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeRealtimeScanConfig(self, request):
-        """获取用户自定义送检信息
+        """获取用户自定义送检信息。**接口使用前提**：目前 DescribeRealtimeScanConfig 接口通过白名单开放，如需使用，需要 [提交工单申请](https://console.cloud.tencent.com/workorder/category?level1_id=438&level2_id=445&source=0&data_title=%E6%B8%B8%E6%88%8F%E5%A4%9A%E5%AA%92%E4%BD%93%E5%BC%95%E6%93%8EGME&step=1)。
 
         :param request: Request instance for DescribeRealtimeScanConfig.
         :type request: :class:`tencentcloud.gme.v20180711.models.DescribeRealtimeScanConfigRequest`
         :rtype: :class:`tencentcloud.gme.v20180711.models.DescribeRealtimeScanConfigResponse`
 
         """
         try:
@@ -769,15 +769,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateScanRooms(self, request):
-        """更新自定义送检房间号
+        """更新自定义送检房间号。**接口使用前提**：目前 UpdateScanRooms 接口通过白名单开放，如需使用，需要 [提交工单申请](https://console.cloud.tencent.com/workorder/category?level1_id=438&level2_id=445&source=0&data_title=%E6%B8%B8%E6%88%8F%E5%A4%9A%E5%AA%92%E4%BD%93%E5%BC%95%E6%93%8EGME&step=1)。
 
         :param request: Request instance for UpdateScanRooms.
         :type request: :class:`tencentcloud.gme.v20180711.models.UpdateScanRoomsRequest`
         :rtype: :class:`tencentcloud.gme.v20180711.models.UpdateScanRoomsResponse`
 
         """
         try:
@@ -792,15 +792,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def UpdateScanUsers(self, request):
-        """更新自定义送检用户号
+        """更新自定义送检用户号。
+        **接口使用前提**：目前 UpdateScanUsers 接口通过白名单开放，如需使用，需要 [提交工单申请](https://console.cloud.tencent.com/workorder/category?level1_id=438&level2_id=445&source=0&data_title=%E6%B8%B8%E6%88%8F%E5%A4%9A%E5%AA%92%E4%BD%93%E5%BC%95%E6%93%8EGME&step=1)。
 
         :param request: Request instance for UpdateScanUsers.
         :type request: :class:`tencentcloud.gme.v20180711.models.UpdateScanUsersRequest`
         :rtype: :class:`tencentcloud.gme.v20180711.models.UpdateScanUsersResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-gme-3.0.950/tencentcloud/gme/v20180711/errorcodes.py` & `tencentcloud-sdk-python-gme-3.0.951/tencentcloud/gme/v20180711/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.950/tencentcloud/gme/v20180711/models.py` & `tencentcloud-sdk-python-gme-3.0.951/tencentcloud/gme/v20180711/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.950/PKG-INFO` & `tencentcloud-sdk-python-gme-3.0.951/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gme
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Gme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gme-3.0.950/README.rst` & `tencentcloud-sdk-python-gme-3.0.951/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.950/tencentcloud_sdk_python_gme.egg-info/PKG-INFO` & `tencentcloud-sdk-python-gme-3.0.951/tencentcloud_sdk_python_gme.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gme
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Gme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

