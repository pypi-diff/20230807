# Comparing `tmp/tencentcloud-sdk-python-cdwch-3.0.950.tar.gz` & `tmp/tencentcloud-sdk-python-cdwch-3.0.951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdwch-3.0.950.tar", last modified: Fri Aug  4 00:22:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdwch-3.0.951.tar", last modified: Mon Aug  7 00:21:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdwch-3.0.950.tar` & `tencentcloud-sdk-python-cdwch-3.0.951.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/
--rw-r--r--   0 root         (0) root         (0)     1076 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud/cdwch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud/cdwch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud/cdwch/v20200915/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud/cdwch/v20200915/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud/cdwch/v20200915/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    20110 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud/cdwch/v20200915/cdwch_client.py
--rw-r--r--   0 root         (0) root         (0)   135557 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud/cdwch/v20200915/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud_sdk_python_cdwch.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud_sdk_python_cdwch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      517 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud_sdk_python_cdwch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud_sdk_python_cdwch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud_sdk_python_cdwch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:22:15.000000 tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud_sdk_python_cdwch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud/cdwch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud/cdwch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud/cdwch/v20200915/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud/cdwch/v20200915/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud/cdwch/v20200915/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    20110 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud/cdwch/v20200915/cdwch_client.py
+-rw-r--r--   0 root         (0) root         (0)   135557 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud/cdwch/v20200915/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud_sdk_python_cdwch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud_sdk_python_cdwch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      517 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud_sdk_python_cdwch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud_sdk_python_cdwch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud_sdk_python_cdwch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 00:21:51.000000 tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud_sdk_python_cdwch.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cdwch-3.0.950/setup.py` & `tencentcloud-sdk-python-cdwch-3.0.951/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cdwch',
-    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.951"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cdwch SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud/cdwch/v20200915/errorcodes.py` & `tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud/cdwch/v20200915/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud/cdwch/v20200915/cdwch_client.py` & `tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud/cdwch/v20200915/cdwch_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud/cdwch/v20200915/models.py` & `tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud/cdwch/v20200915/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwch-3.0.950/PKG-INFO` & `tencentcloud-sdk-python-cdwch-3.0.951/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwch
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Cdwch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdwch-3.0.950/README.rst` & `tencentcloud-sdk-python-cdwch-3.0.951/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud_sdk_python_cdwch.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud_sdk_python_cdwch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwch-3.0.950/tencentcloud_sdk_python_cdwch.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdwch-3.0.951/tencentcloud_sdk_python_cdwch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwch
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Cdwch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

