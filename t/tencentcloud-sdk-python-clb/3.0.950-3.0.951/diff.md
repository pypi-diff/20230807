# Comparing `tmp/tencentcloud-sdk-python-clb-3.0.950.tar.gz` & `tmp/tencentcloud-sdk-python-clb-3.0.951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.950.tar", last modified: Fri Aug  4 00:23:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.951.tar", last modified: Mon Aug  7 00:22:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-clb-3.0.950.tar` & `tencentcloud-sdk-python-clb-3.0.951.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    90730 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/clb_client.py
--rw-r--r--   0 root         (0) root         (0)   508027 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud_sdk_python_clb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud_sdk_python_clb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:23:04.000000 tencentcloud-sdk-python-clb-3.0.950/tencentcloud_sdk_python_clb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud/clb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud/clb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud/clb/v20180317/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud/clb/v20180317/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud/clb/v20180317/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    90730 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud/clb/v20180317/clb_client.py
+-rw-r--r--   0 root         (0) root         (0)   508030 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud/clb/v20180317/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud_sdk_python_clb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud_sdk_python_clb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 00:22:44.000000 tencentcloud-sdk-python-clb-3.0.951/tencentcloud_sdk_python_clb.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-clb-3.0.950/setup.py` & `tencentcloud-sdk-python-clb-3.0.951/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-clb',
-    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.951"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Clb SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/errorcodes.py` & `tencentcloud-sdk-python-clb-3.0.951/tencentcloud/clb/v20180317/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/clb_client.py` & `tencentcloud-sdk-python-clb-3.0.951/tencentcloud/clb/v20180317/clb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.950/tencentcloud/clb/v20180317/models.py` & `tencentcloud-sdk-python-clb-3.0.951/tencentcloud/clb/v20180317/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3184,15 +3184,15 @@
         :param _MasterZoneId: 仅适用于公网负载均衡。设置跨可用区容灾时的主可用区ID，例如 100001 或 ap-guangzhou-1
 注：主可用区是需要承载流量的可用区，备可用区默认不承载流量，主可用区不可用时才使用备可用区。目前仅广州、上海、南京、北京、中国香港、首尔地域的 IPv4 版本的 CLB 支持主备可用区。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213) 接口查询一个地域的主可用区的列表。
         :type MasterZoneId: str
         :param _ZoneId: 仅适用于公网负载均衡。可用区ID，指定可用区以创建负载均衡实例。如：ap-guangzhou-1。
         :type ZoneId: str
         :param _InternetAccessible: 仅对内网属性的性能容量型实例和公网属性的所有实例生效。
         :type InternetAccessible: :class:`tencentcloud.clb.v20180317.models.InternetAccessible`
-        :param _VipIsp: 仅适用于公网负载均衡。CMCC | CTCC | CUCC，分别对应 移动 | 电信 | 联通，如果不指定本参数，则默认使用BGP。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213)  接口查询一个地域所支持的Isp。如果指定运营商，则网络计费式只能使用按带宽包计费(BANDWIDTH_PACKAGE)。
+        :param _VipIsp: 仅适用于公网负载均衡。CMCC | CTCC | CUCC，分别对应 移动 | 电信 | 联通，如果不指定本参数，则默认使用BGP。可通过 [DescribeResources](https://cloud.tencent.com/document/api/214/70213)  接口查询一个地域所支持的Isp。如果指定运营商，则网络计费模式只能使用按带宽包计费(BANDWIDTH_PACKAGE)。
         :type VipIsp: str
         :param _Tags: 购买负载均衡的同时，给负载均衡打上标签，最大支持20个标签键值对。
         :type Tags: list of TagInfo
         :param _Vip: 指定VIP申请负载均衡。此参数选填，不填写此参数时自动分配VIP。IPv4和IPv6类型支持此参数，IPv6 NAT64类型不支持。
 注意：当指定VIP创建内网实例、或公网IPv6 BGP实例时，若VIP不属于指定VPC子网的网段内时，会创建失败；若VIP已被占用，也会创建失败。
         :type Vip: str
         :param _BandwidthPackageId: 带宽包ID，指定此参数时，网络计费方式（InternetAccessible.InternetChargeType）只支持按带宽包计费（BANDWIDTH_PACKAGE）。
```

### Comparing `tencentcloud-sdk-python-clb-3.0.950/tencentcloud/__init__.py` & `tencentcloud-sdk-python-clb-3.0.951/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-clb-3.0.950/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.951/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.950/README.rst` & `tencentcloud-sdk-python-clb-3.0.951/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.950/tencentcloud_sdk_python_clb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.951/tencentcloud_sdk_python_clb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

