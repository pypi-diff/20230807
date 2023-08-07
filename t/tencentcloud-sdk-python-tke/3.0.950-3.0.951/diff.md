# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.950.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.950.tar", last modified: Fri Aug  4 00:36:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.951.tar", last modified: Mon Aug  7 00:36:43 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.950.tar` & `tencentcloud-sdk-python-tke-3.0.951.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   191187 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)    19591 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1059143 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud_sdk_python_tke.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:36:51.000000 tencentcloud-sdk-python-tke-3.0.950/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   191187 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)    19591 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1061270 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud_sdk_python_tke.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 00:36:43.000000 tencentcloud-sdk-python-tke-3.0.951/tencentcloud_sdk_python_tke.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tke-3.0.950/setup.py` & `tencentcloud-sdk-python-tke-3.0.951/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-tke',
-    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.951"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Tke SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-tke-3.0.950/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.951/tencentcloud/tke/v20180525/tke_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.950/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.951/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.950/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.951/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3492,14 +3492,48 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ClusterProperty(AbstractModel):
+    """集群属性
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _NodeNameType: 节点hostname命名模式
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NodeNameType: str
+        """
+        self._NodeNameType = None
+
+    @property
+    def NodeNameType(self):
+        return self._NodeNameType
+
+    @NodeNameType.setter
+    def NodeNameType(self, NodeNameType):
+        self._NodeNameType = NodeNameType
+
+
+    def _deserialize(self, params):
+        self._NodeNameType = params.get("NodeNameType")
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
 class ClusterPublicLB(AbstractModel):
     """弹性容器集群公网访问负载均衡信息
 
     """
 
     def __init__(self):
         r"""
@@ -25838,22 +25872,25 @@
         :type ClusterDesc: str
         :param _ClusterLevel: 集群等级
         :type ClusterLevel: str
         :param _AutoUpgradeClusterLevel: 自动变配集群等级
         :type AutoUpgradeClusterLevel: :class:`tencentcloud.tke.v20180525.models.AutoUpgradeClusterLevel`
         :param _QGPUShareEnable: 是否开启QGPU共享
         :type QGPUShareEnable: bool
+        :param _ClusterProperty: 集群属性
+        :type ClusterProperty: :class:`tencentcloud.tke.v20180525.models.ClusterProperty`
         """
         self._ClusterId = None
         self._ProjectId = None
         self._ClusterName = None
         self._ClusterDesc = None
         self._ClusterLevel = None
         self._AutoUpgradeClusterLevel = None
         self._QGPUShareEnable = None
+        self._ClusterProperty = None
 
     @property
     def ClusterId(self):
         return self._ClusterId
 
     @ClusterId.setter
     def ClusterId(self, ClusterId):
@@ -25903,25 +25940,36 @@
     def QGPUShareEnable(self):
         return self._QGPUShareEnable
 
     @QGPUShareEnable.setter
     def QGPUShareEnable(self, QGPUShareEnable):
         self._QGPUShareEnable = QGPUShareEnable
 
+    @property
+    def ClusterProperty(self):
+        return self._ClusterProperty
+
+    @ClusterProperty.setter
+    def ClusterProperty(self, ClusterProperty):
+        self._ClusterProperty = ClusterProperty
+
 
     def _deserialize(self, params):
         self._ClusterId = params.get("ClusterId")
         self._ProjectId = params.get("ProjectId")
         self._ClusterName = params.get("ClusterName")
         self._ClusterDesc = params.get("ClusterDesc")
         self._ClusterLevel = params.get("ClusterLevel")
         if params.get("AutoUpgradeClusterLevel") is not None:
             self._AutoUpgradeClusterLevel = AutoUpgradeClusterLevel()
             self._AutoUpgradeClusterLevel._deserialize(params.get("AutoUpgradeClusterLevel"))
         self._QGPUShareEnable = params.get("QGPUShareEnable")
+        if params.get("ClusterProperty") is not None:
+            self._ClusterProperty = ClusterProperty()
+            self._ClusterProperty._deserialize(params.get("ClusterProperty"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -25949,23 +25997,27 @@
         :type ClusterLevel: str
         :param _AutoUpgradeClusterLevel: 自动变配集群等级
 注意：此字段可能返回 null，表示取不到有效值。
         :type AutoUpgradeClusterLevel: :class:`tencentcloud.tke.v20180525.models.AutoUpgradeClusterLevel`
         :param _QGPUShareEnable: 是否开启QGPU共享
 注意：此字段可能返回 null，表示取不到有效值。
         :type QGPUShareEnable: bool
+        :param _ClusterProperty: 集群属性
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterProperty: :class:`tencentcloud.tke.v20180525.models.ClusterProperty`
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._ProjectId = None
         self._ClusterName = None
         self._ClusterDesc = None
         self._ClusterLevel = None
         self._AutoUpgradeClusterLevel = None
         self._QGPUShareEnable = None
+        self._ClusterProperty = None
         self._RequestId = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
@@ -26009,14 +26061,22 @@
         return self._QGPUShareEnable
 
     @QGPUShareEnable.setter
     def QGPUShareEnable(self, QGPUShareEnable):
         self._QGPUShareEnable = QGPUShareEnable
 
     @property
+    def ClusterProperty(self):
+        return self._ClusterProperty
+
+    @ClusterProperty.setter
+    def ClusterProperty(self, ClusterProperty):
+        self._ClusterProperty = ClusterProperty
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -26026,14 +26086,17 @@
         self._ClusterName = params.get("ClusterName")
         self._ClusterDesc = params.get("ClusterDesc")
         self._ClusterLevel = params.get("ClusterLevel")
         if params.get("AutoUpgradeClusterLevel") is not None:
             self._AutoUpgradeClusterLevel = AutoUpgradeClusterLevel()
             self._AutoUpgradeClusterLevel._deserialize(params.get("AutoUpgradeClusterLevel"))
         self._QGPUShareEnable = params.get("QGPUShareEnable")
+        if params.get("ClusterProperty") is not None:
+            self._ClusterProperty = ClusterProperty()
+            self._ClusterProperty._deserialize(params.get("ClusterProperty"))
         self._RequestId = params.get("RequestId")
 
 
 class ModifyClusterAuthenticationOptionsRequest(AbstractModel):
     """ModifyClusterAuthenticationOptions请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-tke-3.0.950/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.951/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.950/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.951/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.950/README.rst` & `tencentcloud-sdk-python-tke-3.0.951/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.950/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.951/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

