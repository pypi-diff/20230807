# Comparing `tmp/tencentcloud-sdk-python-chdfs-3.0.950.tar.gz` & `tmp/tencentcloud-sdk-python-chdfs-3.0.951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-chdfs-3.0.950.tar", last modified: Fri Aug  4 00:22:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-chdfs-3.0.951.tar", last modified: Mon Aug  7 00:22:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-chdfs-3.0.950.tar` & `tencentcloud-sdk-python-chdfs-3.0.951.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud_sdk_python_chdfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud_sdk_python_chdfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      685 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud_sdk_python_chdfs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud_sdk_python_chdfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1076 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20201112/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20201112/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3600 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20201112/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    27402 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20201112/chdfs_client.py
--rw-r--r--   0 root         (0) root         (0)    92834 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20201112/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20190718/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20190718/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3280 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20190718/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28126 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20190718/chdfs_client.py
--rw-r--r--   0 root         (0) root         (0)    78138 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20190718/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-08-04 00:22:34.000000 tencentcloud-sdk-python-chdfs-3.0.950/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud_sdk_python_chdfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud_sdk_python_chdfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      685 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud_sdk_python_chdfs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud_sdk_python_chdfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20201112/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20201112/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3600 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20201112/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    27402 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20201112/chdfs_client.py
+-rw-r--r--   0 root         (0) root         (0)    92834 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20201112/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20190718/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20190718/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3280 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20190718/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28126 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20190718/chdfs_client.py
+-rw-r--r--   0 root         (0) root         (0)    78138 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20190718/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-08-07 00:22:13.000000 tencentcloud-sdk-python-chdfs-3.0.951/README.rst
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-chdfs
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Chdfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.950/setup.py` & `tencentcloud-sdk-python-chdfs-3.0.951/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-chdfs',
-    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.951"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Chdfs SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20201112/errorcodes.py` & `tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20201112/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20201112/chdfs_client.py` & `tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20201112/chdfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20201112/models.py` & `tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20201112/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20190718/errorcodes.py` & `tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20190718/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20190718/chdfs_client.py` & `tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20190718/chdfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/chdfs/v20190718/models.py` & `tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/chdfs/v20190718/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.950/tencentcloud/__init__.py` & `tencentcloud-sdk-python-chdfs-3.0.951/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-chdfs-3.0.950/PKG-INFO` & `tencentcloud-sdk-python-chdfs-3.0.951/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-chdfs
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Chdfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.950/README.rst` & `tencentcloud-sdk-python-chdfs-3.0.951/README.rst`

 * *Files identical despite different names*

