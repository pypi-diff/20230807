# Comparing `tmp/tencentcloud-sdk-python-tourism-3.0.950.tar.gz` & `tmp/tencentcloud-sdk-python-tourism-3.0.951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tourism-3.0.950.tar", last modified: Fri Aug  4 00:37:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tourism-3.0.951.tar", last modified: Mon Aug  7 00:37:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tourism-3.0.950.tar` & `tencentcloud-sdk-python-tourism-3.0.951.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud_sdk_python_tourism.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud_sdk_python_tourism.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      539 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud_sdk_python_tourism.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud_sdk_python_tourism.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud_sdk_python_tourism.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud_sdk_python_tourism.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1080 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud/tourism/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud/tourism/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud/tourism/v20230215/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud/tourism/v20230215/__init__.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud/tourism/v20230215/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     8749 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud/tourism/v20230215/models.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud/tourism/v20230215/tourism_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-08-04 00:37:12.000000 tencentcloud-sdk-python-tourism-3.0.950/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud_sdk_python_tourism.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud_sdk_python_tourism.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      539 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud_sdk_python_tourism.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud_sdk_python_tourism.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud_sdk_python_tourism.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud_sdk_python_tourism.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud/tourism/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud/tourism/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud/tourism/v20230215/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud/tourism/v20230215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud/tourism/v20230215/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     8749 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud/tourism/v20230215/models.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud/tourism/v20230215/tourism_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-08-07 00:37:08.000000 tencentcloud-sdk-python-tourism-3.0.951/README.rst
```

### Comparing `tencentcloud-sdk-python-tourism-3.0.950/tencentcloud_sdk_python_tourism.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tourism-3.0.951/tencentcloud_sdk_python_tourism.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tourism-3.0.950/tencentcloud_sdk_python_tourism.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tourism-3.0.951/tencentcloud_sdk_python_tourism.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tourism
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Tourism SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tourism-3.0.950/setup.py` & `tencentcloud-sdk-python-tourism-3.0.951/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-tourism',
-    install_requires=["tencentcloud-sdk-python-common==3.0.950"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.951"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Tourism SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-tourism-3.0.950/tencentcloud/tourism/v20230215/errorcodes.py` & `tencentcloud-sdk-python-tourism-3.0.951/tencentcloud/tourism/v20230215/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tourism-3.0.950/tencentcloud/tourism/v20230215/models.py` & `tencentcloud-sdk-python-tourism-3.0.951/tencentcloud/tourism/v20230215/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tourism-3.0.950/tencentcloud/tourism/v20230215/tourism_client.py` & `tencentcloud-sdk-python-tourism-3.0.951/tencentcloud/tourism/v20230215/tourism_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tourism-3.0.950/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tourism-3.0.951/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tourism-3.0.950/PKG-INFO` & `tencentcloud-sdk-python-tourism-3.0.951/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tourism
-Version: 3.0.950
+Version: 3.0.951
 Summary: Tencent Cloud Tourism SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tourism-3.0.950/README.rst` & `tencentcloud-sdk-python-tourism-3.0.951/README.rst`

 * *Files identical despite different names*

