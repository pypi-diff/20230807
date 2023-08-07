# Comparing `tmp/tencentcloud-sdk-python-scf-3.0.950.tar.gz` & `tmp/tencentcloud-sdk-python-scf-3.0.951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.950.tar", last modified: Fri Aug  4 00:33:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.951.tar", last modified: Mon Aug  7 00:32:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-scf-3.0.950.tar` & `tencentcloud-sdk-python-scf-3.0.951.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud/scf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud/scf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud/scf/v20180416/
--rw-r--r--   0 root         (0) root         (0)    42891 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud/scf/v20180416/scf_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud/scf/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32507 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud/scf/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   318099 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud/scf/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud_sdk_python_scf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud_sdk_python_scf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:33:02.000000 tencentcloud-sdk-python-scf-3.0.950/tencentcloud_sdk_python_scf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud/scf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud/scf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud/scf/v20180416/
+-rw-r--r--   0 root         (0) root         (0)    42891 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud/scf/v20180416/scf_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud/scf/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32507 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud/scf/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   318099 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud/scf/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud_sdk_python_scf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud_sdk_python_scf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 00:32:42.000000 tencentcloud-sdk-python-scf-3.0.951/tencentcloud_sdk_python_scf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-scf-3.0.950/setup.py` & `tencentcloud-sdk-python-scf-3.0.951/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-scf',
-    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.951"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Scf SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-scf-3.0.950/tencentcloud/scf/v20180416/scf_client.py` & `tencentcloud-sdk-python-scf-3.0.951/tencentcloud/scf/v20180416/scf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.950/tencentcloud/scf/v20180416/errorcodes.py` & `tencentcloud-sdk-python-scf-3.0.951/tencentcloud/scf/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.950/tencentcloud/scf/v20180416/models.py` & `tencentcloud-sdk-python-scf-3.0.951/tencentcloud/scf/v20180416/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.950/tencentcloud/__init__.py` & `tencentcloud-sdk-python-scf-3.0.951/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-scf-3.0.950/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.951/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-scf-3.0.950/README.rst` & `tencentcloud-sdk-python-scf-3.0.951/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.950/tencentcloud_sdk_python_scf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.951/tencentcloud_sdk_python_scf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

