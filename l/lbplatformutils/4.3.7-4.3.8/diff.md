# Comparing `tmp/LbPlatformUtils-4.3.7.tar.gz` & `tmp/LbPlatformUtils-4.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbPlatformUtils-4.3.7.tar", max compression
+gzip compressed data, was "LbPlatformUtils-4.3.8.tar", max compression
```

## Comparing `LbPlatformUtils-4.3.7.tar` & `LbPlatformUtils-4.3.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35097 2021-07-03 10:07:09.368000 LbPlatformUtils-4.3.7/LICENSE
--rw-r--r--   0        0        0    13567 2021-07-03 10:07:09.368000 LbPlatformUtils-4.3.7/LbPlatformUtils/__init__.py
--rw-r--r--   0        0        0     8345 2021-07-03 10:07:09.368000 LbPlatformUtils-4.3.7/LbPlatformUtils/architectures.py
--rw-r--r--   0        0        0       65 2021-07-03 10:07:09.368000 LbPlatformUtils-4.3.7/LbPlatformUtils/bash-completion/README.txt
--rw-r--r--   0        0        0     1221 2021-07-03 10:07:09.368000 LbPlatformUtils-4.3.7/LbPlatformUtils/bash-completion/_lb-describe-platform
--rw-r--r--   0        0        0     1020 2021-07-03 10:07:09.368000 LbPlatformUtils-4.3.7/LbPlatformUtils/bash-completion/_lb-host-binary-tag
--rw-r--r--   0        0        0     6989 2021-07-03 10:07:09.368000 LbPlatformUtils-4.3.7/LbPlatformUtils/debug.py
--rw-r--r--   0        0        0     8558 2021-07-03 10:07:09.368000 LbPlatformUtils-4.3.7/LbPlatformUtils/describe.py
--rw-r--r--   0        0        0     9159 2021-07-03 10:07:09.368000 LbPlatformUtils-4.3.7/LbPlatformUtils/inspect.py
--rw-r--r--   0        0        0     3563 2021-07-03 10:07:09.368000 LbPlatformUtils-4.3.7/LbPlatformUtils/platforms-list.json
--rw-r--r--   0        0        0     1132 2021-07-03 10:07:09.368000 LbPlatformUtils-4.3.7/pyproject.toml
--rw-r--r--   0        0        0     1004 2021-07-03 10:07:19.202472 LbPlatformUtils-4.3.7/setup.py
--rw-r--r--   0        0        0      844 2021-07-03 10:07:19.202868 LbPlatformUtils-4.3.7/PKG-INFO
+-rw-r--r--   0        0        0    35097 2021-08-25 08:03:50.368000 LbPlatformUtils-4.3.8/LICENSE
+-rw-r--r--   0        0        0    13567 2021-08-25 08:03:50.368000 LbPlatformUtils-4.3.8/LbPlatformUtils/__init__.py
+-rw-r--r--   0        0        0     8345 2021-08-25 08:03:50.368000 LbPlatformUtils-4.3.8/LbPlatformUtils/architectures.py
+-rw-r--r--   0        0        0       65 2021-08-25 08:03:50.368000 LbPlatformUtils-4.3.8/LbPlatformUtils/bash-completion/README.txt
+-rw-r--r--   0        0        0     1221 2021-08-25 08:03:50.368000 LbPlatformUtils-4.3.8/LbPlatformUtils/bash-completion/_lb-describe-platform
+-rw-r--r--   0        0        0     1020 2021-08-25 08:03:50.368000 LbPlatformUtils-4.3.8/LbPlatformUtils/bash-completion/_lb-host-binary-tag
+-rw-r--r--   0        0        0     6989 2021-08-25 08:03:50.368000 LbPlatformUtils-4.3.8/LbPlatformUtils/debug.py
+-rw-r--r--   0        0        0     8558 2021-08-25 08:03:50.368000 LbPlatformUtils-4.3.8/LbPlatformUtils/describe.py
+-rw-r--r--   0        0        0     9229 2021-08-25 08:03:50.368000 LbPlatformUtils-4.3.8/LbPlatformUtils/inspect.py
+-rw-r--r--   0        0        0     3563 2021-08-25 08:03:50.368000 LbPlatformUtils-4.3.8/LbPlatformUtils/platforms-list.json
+-rw-r--r--   0        0        0     1132 2021-08-25 08:03:50.372000 LbPlatformUtils-4.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1004 2021-08-25 08:04:00.185879 LbPlatformUtils-4.3.8/setup.py
+-rw-r--r--   0        0        0      844 2021-08-25 08:04:00.186314 LbPlatformUtils-4.3.8/PKG-INFO
```

### Comparing `LbPlatformUtils-4.3.7/LICENSE` & `LbPlatformUtils-4.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `LbPlatformUtils-4.3.7/LbPlatformUtils/__init__.py` & `LbPlatformUtils-4.3.8/LbPlatformUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `LbPlatformUtils-4.3.7/LbPlatformUtils/architectures.py` & `LbPlatformUtils-4.3.8/LbPlatformUtils/architectures.py`

 * *Files identical despite different names*

### Comparing `LbPlatformUtils-4.3.7/LbPlatformUtils/bash-completion/_lb-describe-platform` & `LbPlatformUtils-4.3.8/LbPlatformUtils/bash-completion/_lb-describe-platform`

 * *Files identical despite different names*

### Comparing `LbPlatformUtils-4.3.7/LbPlatformUtils/bash-completion/_lb-host-binary-tag` & `LbPlatformUtils-4.3.8/LbPlatformUtils/bash-completion/_lb-host-binary-tag`

 * *Files identical despite different names*

### Comparing `LbPlatformUtils-4.3.7/LbPlatformUtils/debug.py` & `LbPlatformUtils-4.3.8/LbPlatformUtils/debug.py`

 * *Files identical despite different names*

### Comparing `LbPlatformUtils-4.3.7/LbPlatformUtils/describe.py` & `LbPlatformUtils-4.3.8/LbPlatformUtils/describe.py`

 * *Files identical despite different names*

### Comparing `LbPlatformUtils-4.3.7/LbPlatformUtils/inspect.py` & `LbPlatformUtils-4.3.8/LbPlatformUtils/inspect.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,11 +279,12 @@
         container_dir = check_output(test_cmd, stderr=STDOUT).decode()
     except (CalledProcessError, OSError, IndexError):
         return []
 
     # If singularity fails to set up the bind mounts it will quietly change the
     # current working directory to be $HOME so fail if the current working
     # directory is not what we expect
-    if os.getcwd() == os.path.normpath(container_dir.strip()):
+    container_dir = os.path.normpath(container_dir.strip())
+    if os.path.realpath(os.getcwd()) == os.path.realpath(container_dir):
         return available_roots
     else:
         return []
```

### Comparing `LbPlatformUtils-4.3.7/LbPlatformUtils/platforms-list.json` & `LbPlatformUtils-4.3.8/LbPlatformUtils/platforms-list.json`

 * *Files identical despite different names*

### Comparing `LbPlatformUtils-4.3.7/pyproject.toml` & `LbPlatformUtils-4.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LbPlatformUtils"
-version = "4.3.7"
+version = "4.3.8"
 description = "utilities for platform detection"
 authors = ["CERN - LHCb Core Software <lhcb-core-soft@cern.ch>"]
 license = "GPL-3.0+"
 homepage = "https://gitlab.cern.ch/lhcb-core/LbPlatformUtils"
 classifiers = [
     "Development Status :: 4 - Beta",
 ]
```

### Comparing `LbPlatformUtils-4.3.7/setup.py` & `LbPlatformUtils-4.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'console_scripts': ['lb-debug-platform = LbPlatformUtils.debug:main',
                      'lb-describe-platform = LbPlatformUtils.describe:main',
                      'lb-host-binary-tag = '
                      'LbPlatformUtils.describe:host_binary_tag_script']}
 
 setup_kwargs = {
     'name': 'lbplatformutils',
-    'version': '4.3.7',
+    'version': '4.3.8',
     'description': 'utilities for platform detection',
     'long_description': None,
     'author': 'CERN - LHCb Core Software',
     'author_email': 'lhcb-core-soft@cern.ch',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.cern.ch/lhcb-core/LbPlatformUtils',
```

### Comparing `LbPlatformUtils-4.3.7/PKG-INFO` & `LbPlatformUtils-4.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbplatformutils
-Version: 4.3.7
+Version: 4.3.8
 Summary: utilities for platform detection
 Home-page: https://gitlab.cern.ch/lhcb-core/LbPlatformUtils
 License: GPL-3.0+
 Author: CERN - LHCb Core Software
 Author-email: lhcb-core-soft@cern.ch
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 Classifier: Development Status :: 4 - Beta
```

