# Comparing `tmp/locker-secrets-0.0.6b1.tar.gz` & `tmp/locker-secrets-0.0.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locker-secrets-0.0.6b1.tar", last modified: Mon Aug  7 09:35:02 2023, max compression
+gzip compressed data, was "locker-secrets-0.0.7b1.tar", last modified: Mon Aug  7 09:41:21 2023, max compression
```

## Comparing `locker-secrets-0.0.6b1.tar` & `locker-secrets-0.0.7b1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 09:35:02.366679 locker-secrets-0.0.6b1/
--rw-rw-rw-   0        0        0      267 2023-06-17 10:25:18.000000 locker-secrets-0.0.6b1/MANIFEST.in
--rw-rw-rw-   0        0        0     5502 2023-08-07 09:35:02.366679 locker-secrets-0.0.6b1/PKG-INFO
--rw-rw-rw-   0        0        0     4487 2023-08-01 07:36:40.000000 locker-secrets-0.0.6b1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 09:35:02.288679 locker-secrets-0.0.6b1/docs/
--rw-rw-rw-   0        0        0     1676 2023-06-17 02:37:40.000000 locker-secrets-0.0.6b1/docs/standard.md
-drwxrwxrwx   0        0        0        0 2023-08-07 09:35:02.293678 locker-secrets-0.0.6b1/examples/
--rw-rw-rw-   0        0        0        0 2023-06-14 02:59:05.000000 locker-secrets-0.0.6b1/examples/__init__.py
--rw-rw-rw-   0        0        0      435 2023-06-17 10:29:22.000000 locker-secrets-0.0.6b1/examples/binary_adapter_example.py
--rw-rw-rw-   0        0        0      772 2023-07-11 09:07:28.000000 locker-secrets-0.0.6b1/examples/environment_example.py
--rw-rw-rw-   0        0        0     1019 2023-08-07 06:58:55.000000 locker-secrets-0.0.6b1/examples/environment_quick_usage_example.py
--rw-rw-rw-   0        0        0      127 2023-07-11 10:19:35.000000 locker-secrets-0.0.6b1/examples/logger_test.py
--rw-rw-rw-   0        0        0      783 2023-07-20 06:59:21.000000 locker-secrets-0.0.6b1/examples/secret_example.py
--rw-rw-rw-   0        0        0     2032 2023-08-07 09:25:46.000000 locker-secrets-0.0.6b1/examples/secret_quick_usage_example.py
-drwxrwxrwx   0        0        0        0 2023-08-07 09:35:02.303680 locker-secrets-0.0.6b1/locker/
--rw-rw-rw-   0        0        0      242 2023-08-07 09:32:12.000000 locker-secrets-0.0.6b1/locker/__about__.py
--rw-rw-rw-   0        0        0      739 2023-08-01 10:11:52.000000 locker-secrets-0.0.6b1/locker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 09:35:02.322679 locker-secrets-0.0.6b1/locker/bin/
--rwxrwxrwx   0        0        0  8527360 2023-08-07 07:49:25.000000 locker-secrets-0.0.6b1/locker/bin/locker_secret.exe
--rw-rw-rw-   0        0        0  8261632 2023-08-07 07:49:23.000000 locker-secrets-0.0.6b1/locker/bin/locker_secret_linux
--rw-rw-rw-   0        0        0  8877312 2023-08-07 07:49:20.000000 locker-secrets-0.0.6b1/locker/bin/locker_secret_mac
--rw-rw-rw-   0        0        0     7510 2023-08-07 09:26:12.000000 locker-secrets-0.0.6b1/locker/binary_adapter.py
--rw-rw-rw-   0        0        0     1040 2023-07-12 10:04:10.000000 locker-secrets-0.0.6b1/locker/config.py
--rw-rw-rw-   0        0        0      770 2023-07-05 07:00:13.000000 locker-secrets-0.0.6b1/locker/environment_quick_usage.py
--rw-rw-rw-   0        0        0     3705 2023-08-07 09:14:58.000000 locker-secrets-0.0.6b1/locker/error.py
--rw-rw-rw-   0        0        0     1945 2023-07-11 10:19:24.000000 locker-secrets-0.0.6b1/locker/logger.py
--rw-rw-rw-   0        0        0    12236 2023-07-05 04:42:40.000000 locker-secrets-0.0.6b1/locker/ls_object.py
-drwxrwxrwx   0        0        0        0 2023-08-07 09:35:02.334679 locker-secrets-0.0.6b1/locker/ls_resources/
--rw-rw-rw-   0        0        0      259 2023-08-07 08:26:08.000000 locker-secrets-0.0.6b1/locker/ls_resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 09:35:02.341678 locker-secrets-0.0.6b1/locker/ls_resources/abstract/
--rw-rw-rw-   0        0        0      723 2023-06-15 03:39:37.000000 locker-secrets-0.0.6b1/locker/ls_resources/abstract/__init__.py
--rw-rw-rw-   0        0        0     4334 2023-07-05 10:01:33.000000 locker-secrets-0.0.6b1/locker/ls_resources/abstract/api_resource.py
--rw-rw-rw-   0        0        0      492 2023-06-29 02:08:47.000000 locker-secrets-0.0.6b1/locker/ls_resources/abstract/createable_api_resource.py
--rw-rw-rw-   0        0        0      663 2023-06-13 08:52:10.000000 locker-secrets-0.0.6b1/locker/ls_resources/abstract/deletable_api_resource.py
--rw-rw-rw-   0        0        0      314 2023-06-15 03:38:42.000000 locker-secrets-0.0.6b1/locker/ls_resources/abstract/detailable_api_resource.py
--rw-rw-rw-   0        0        0      627 2023-06-17 09:08:36.000000 locker-secrets-0.0.6b1/locker/ls_resources/abstract/listable_api_resource.py
--rw-rw-rw-   0        0        0      849 2023-06-13 08:57:15.000000 locker-secrets-0.0.6b1/locker/ls_resources/abstract/singleton_api_resource.py
--rw-rw-rw-   0        0        0      465 2023-07-05 10:07:21.000000 locker-secrets-0.0.6b1/locker/ls_resources/abstract/updateable_api_resource.py
--rw-rw-rw-   0        0        0     1519 2023-08-07 09:30:08.000000 locker-secrets-0.0.6b1/locker/ls_resources/environment.py
--rw-rw-rw-   0        0        0     1228 2023-08-07 09:29:35.000000 locker-secrets-0.0.6b1/locker/ls_resources/error_object.py
--rw-rw-rw-   0        0        0     2241 2023-08-07 06:43:33.000000 locker-secrets-0.0.6b1/locker/ls_resources/secret.py
--rw-rw-rw-   0        0        0      946 2023-06-13 02:58:30.000000 locker-secrets-0.0.6b1/locker/ls_response.py
--rw-rw-rw-   0        0        0      436 2023-06-14 10:08:05.000000 locker-secrets-0.0.6b1/locker/object_classes.py
--rw-rw-rw-   0        0        0     1578 2023-08-01 10:32:35.000000 locker-secrets-0.0.6b1/locker/secret_quick_usage.py
--rw-rw-rw-   0        0        0     4064 2023-08-07 08:35:39.000000 locker-secrets-0.0.6b1/locker/util.py
-drwxrwxrwx   0        0        0        0 2023-08-07 09:35:02.362678 locker-secrets-0.0.6b1/locker_secrets.egg-info/
--rw-rw-rw-   0        0        0     5502 2023-08-07 09:35:02.000000 locker-secrets-0.0.6b1/locker_secrets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1525 2023-08-07 09:35:02.000000 locker-secrets-0.0.6b1/locker_secrets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 09:35:02.000000 locker-secrets-0.0.6b1/locker_secrets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-08-07 09:35:02.000000 locker-secrets-0.0.6b1/locker_secrets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-07 09:35:02.000000 locker-secrets-0.0.6b1/locker_secrets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2023-06-12 10:54:59.000000 locker-secrets-0.0.6b1/pyproject.toml
--rw-rw-rw-   0        0        0       46 2023-06-16 07:30:15.000000 locker-secrets-0.0.6b1/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-17 02:17:22.000000 locker-secrets-0.0.6b1/requirements-test.txt
--rw-rw-rw-   0        0        0       29 2023-06-12 10:54:59.000000 locker-secrets-0.0.6b1/requirements.txt
--rw-rw-rw-   0        0        0       68 2023-08-07 09:35:02.370678 locker-secrets-0.0.6b1/setup.cfg
--rw-rw-rw-   0        0        0     2618 2023-07-11 09:03:48.000000 locker-secrets-0.0.6b1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-07 09:35:02.365679 locker-secrets-0.0.6b1/tests/
--rw-rw-rw-   0        0        0        0 2023-06-12 10:54:59.000000 locker-secrets-0.0.6b1/tests/__init__.py
--rw-rw-rw-   0        0        0     1963 2023-07-05 11:01:04.000000 locker-secrets-0.0.6b1/tests/test_environment_quick_usage.py
--rw-rw-rw-   0        0        0     1461 2023-07-20 06:59:21.000000 locker-secrets-0.0.6b1/tests/test_util.py
--rw-rw-rw-   0        0        0     1313 2023-06-17 02:26:10.000000 locker-secrets-0.0.6b1/tox.ini
+drwxrwxrwx   0        0        0        0 2023-08-07 09:41:21.066895 locker-secrets-0.0.7b1/
+-rw-rw-rw-   0        0        0      267 2023-06-17 10:25:18.000000 locker-secrets-0.0.7b1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5502 2023-08-07 09:41:21.066895 locker-secrets-0.0.7b1/PKG-INFO
+-rw-rw-rw-   0        0        0     4487 2023-08-01 07:36:40.000000 locker-secrets-0.0.7b1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 09:41:20.988904 locker-secrets-0.0.7b1/docs/
+-rw-rw-rw-   0        0        0     1676 2023-06-17 02:37:40.000000 locker-secrets-0.0.7b1/docs/standard.md
+drwxrwxrwx   0        0        0        0 2023-08-07 09:41:20.994895 locker-secrets-0.0.7b1/examples/
+-rw-rw-rw-   0        0        0        0 2023-06-14 02:59:05.000000 locker-secrets-0.0.7b1/examples/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-06-17 10:29:22.000000 locker-secrets-0.0.7b1/examples/binary_adapter_example.py
+-rw-rw-rw-   0        0        0      772 2023-07-11 09:07:28.000000 locker-secrets-0.0.7b1/examples/environment_example.py
+-rw-rw-rw-   0        0        0     1019 2023-08-07 06:58:55.000000 locker-secrets-0.0.7b1/examples/environment_quick_usage_example.py
+-rw-rw-rw-   0        0        0      127 2023-07-11 10:19:35.000000 locker-secrets-0.0.7b1/examples/logger_test.py
+-rw-rw-rw-   0        0        0      783 2023-07-20 06:59:21.000000 locker-secrets-0.0.7b1/examples/secret_example.py
+-rw-rw-rw-   0        0        0     2032 2023-08-07 09:25:46.000000 locker-secrets-0.0.7b1/examples/secret_quick_usage_example.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:41:21.006898 locker-secrets-0.0.7b1/locker/
+-rw-rw-rw-   0        0        0      242 2023-08-07 09:40:59.000000 locker-secrets-0.0.7b1/locker/__about__.py
+-rw-rw-rw-   0        0        0      739 2023-08-01 10:11:52.000000 locker-secrets-0.0.7b1/locker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:41:21.028937 locker-secrets-0.0.7b1/locker/bin/
+-rwxrwxrwx   0        0        0  8527360 2023-08-07 07:49:25.000000 locker-secrets-0.0.7b1/locker/bin/locker_secret.exe
+-rw-rw-rw-   0        0        0  8261632 2023-08-07 07:49:23.000000 locker-secrets-0.0.7b1/locker/bin/locker_secret_linux
+-rw-rw-rw-   0        0        0  8877312 2023-08-07 07:49:20.000000 locker-secrets-0.0.7b1/locker/bin/locker_secret_mac
+-rw-rw-rw-   0        0        0     7514 2023-08-07 09:40:19.000000 locker-secrets-0.0.7b1/locker/binary_adapter.py
+-rw-rw-rw-   0        0        0     1040 2023-07-12 10:04:10.000000 locker-secrets-0.0.7b1/locker/config.py
+-rw-rw-rw-   0        0        0      770 2023-07-05 07:00:13.000000 locker-secrets-0.0.7b1/locker/environment_quick_usage.py
+-rw-rw-rw-   0        0        0     3705 2023-08-07 09:14:58.000000 locker-secrets-0.0.7b1/locker/error.py
+-rw-rw-rw-   0        0        0     1945 2023-07-11 10:19:24.000000 locker-secrets-0.0.7b1/locker/logger.py
+-rw-rw-rw-   0        0        0    12236 2023-07-05 04:42:40.000000 locker-secrets-0.0.7b1/locker/ls_object.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:41:21.043904 locker-secrets-0.0.7b1/locker/ls_resources/
+-rw-rw-rw-   0        0        0      259 2023-08-07 08:26:08.000000 locker-secrets-0.0.7b1/locker/ls_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:41:21.049902 locker-secrets-0.0.7b1/locker/ls_resources/abstract/
+-rw-rw-rw-   0        0        0      723 2023-06-15 03:39:37.000000 locker-secrets-0.0.7b1/locker/ls_resources/abstract/__init__.py
+-rw-rw-rw-   0        0        0     4334 2023-07-05 10:01:33.000000 locker-secrets-0.0.7b1/locker/ls_resources/abstract/api_resource.py
+-rw-rw-rw-   0        0        0      492 2023-06-29 02:08:47.000000 locker-secrets-0.0.7b1/locker/ls_resources/abstract/createable_api_resource.py
+-rw-rw-rw-   0        0        0      663 2023-06-13 08:52:10.000000 locker-secrets-0.0.7b1/locker/ls_resources/abstract/deletable_api_resource.py
+-rw-rw-rw-   0        0        0      314 2023-06-15 03:38:42.000000 locker-secrets-0.0.7b1/locker/ls_resources/abstract/detailable_api_resource.py
+-rw-rw-rw-   0        0        0      627 2023-06-17 09:08:36.000000 locker-secrets-0.0.7b1/locker/ls_resources/abstract/listable_api_resource.py
+-rw-rw-rw-   0        0        0      849 2023-06-13 08:57:15.000000 locker-secrets-0.0.7b1/locker/ls_resources/abstract/singleton_api_resource.py
+-rw-rw-rw-   0        0        0      465 2023-07-05 10:07:21.000000 locker-secrets-0.0.7b1/locker/ls_resources/abstract/updateable_api_resource.py
+-rw-rw-rw-   0        0        0     1519 2023-08-07 09:30:08.000000 locker-secrets-0.0.7b1/locker/ls_resources/environment.py
+-rw-rw-rw-   0        0        0     1228 2023-08-07 09:29:35.000000 locker-secrets-0.0.7b1/locker/ls_resources/error_object.py
+-rw-rw-rw-   0        0        0     2241 2023-08-07 06:43:33.000000 locker-secrets-0.0.7b1/locker/ls_resources/secret.py
+-rw-rw-rw-   0        0        0      946 2023-06-13 02:58:30.000000 locker-secrets-0.0.7b1/locker/ls_response.py
+-rw-rw-rw-   0        0        0      436 2023-06-14 10:08:05.000000 locker-secrets-0.0.7b1/locker/object_classes.py
+-rw-rw-rw-   0        0        0     1578 2023-08-01 10:32:35.000000 locker-secrets-0.0.7b1/locker/secret_quick_usage.py
+-rw-rw-rw-   0        0        0     4064 2023-08-07 08:35:39.000000 locker-secrets-0.0.7b1/locker/util.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:41:21.063894 locker-secrets-0.0.7b1/locker_secrets.egg-info/
+-rw-rw-rw-   0        0        0     5502 2023-08-07 09:41:20.000000 locker-secrets-0.0.7b1/locker_secrets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1525 2023-08-07 09:41:20.000000 locker-secrets-0.0.7b1/locker_secrets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 09:41:20.000000 locker-secrets-0.0.7b1/locker_secrets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-08-07 09:41:20.000000 locker-secrets-0.0.7b1/locker_secrets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-07 09:41:20.000000 locker-secrets-0.0.7b1/locker_secrets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2023-06-12 10:54:59.000000 locker-secrets-0.0.7b1/pyproject.toml
+-rw-rw-rw-   0        0        0       46 2023-06-16 07:30:15.000000 locker-secrets-0.0.7b1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-17 02:17:22.000000 locker-secrets-0.0.7b1/requirements-test.txt
+-rw-rw-rw-   0        0        0       29 2023-06-12 10:54:59.000000 locker-secrets-0.0.7b1/requirements.txt
+-rw-rw-rw-   0        0        0       68 2023-08-07 09:41:21.067895 locker-secrets-0.0.7b1/setup.cfg
+-rw-rw-rw-   0        0        0     2618 2023-07-11 09:03:48.000000 locker-secrets-0.0.7b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:41:21.065901 locker-secrets-0.0.7b1/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-12 10:54:59.000000 locker-secrets-0.0.7b1/tests/__init__.py
+-rw-rw-rw-   0        0        0     1963 2023-07-05 11:01:04.000000 locker-secrets-0.0.7b1/tests/test_environment_quick_usage.py
+-rw-rw-rw-   0        0        0     1461 2023-07-20 06:59:21.000000 locker-secrets-0.0.7b1/tests/test_util.py
+-rw-rw-rw-   0        0        0     1313 2023-06-17 02:26:10.000000 locker-secrets-0.0.7b1/tox.ini
```

### Comparing `locker-secrets-0.0.6b1/PKG-INFO` & `locker-secrets-0.0.7b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locker-secrets
-Version: 0.0.6b1
+Version: 0.0.7b1
 Summary: Locker Secret Python SDK
 Home-page: https://locker.io
 Download-URL: 
 Author: CyStack
 Author-email: contact@locker.io
 Keywords: django,vault management,security
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `locker-secrets-0.0.6b1/README.md` & `locker-secrets-0.0.7b1/README.md`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/docs/standard.md` & `locker-secrets-0.0.7b1/docs/standard.md`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/examples/environment_example.py` & `locker-secrets-0.0.7b1/examples/environment_example.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/examples/environment_quick_usage_example.py` & `locker-secrets-0.0.7b1/examples/environment_quick_usage_example.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/examples/secret_example.py` & `locker-secrets-0.0.7b1/examples/secret_example.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/examples/secret_quick_usage_example.py` & `locker-secrets-0.0.7b1/examples/secret_quick_usage_example.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/__init__.py` & `locker-secrets-0.0.7b1/locker/__init__.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/bin/locker_secret.exe` & `locker-secrets-0.0.7b1/locker/bin/locker_secret.exe`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/bin/locker_secret_linux` & `locker-secrets-0.0.7b1/locker/bin/locker_secret_linux`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/bin/locker_secret_mac` & `locker-secrets-0.0.7b1/locker/bin/locker_secret_mac`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/binary_adapter.py` & `locker-secrets-0.0.7b1/locker/binary_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,16 +150,16 @@
             logger.error(f"[!] CLI result json decode error:::{res_body}")
             exc = error.CliRunError(
                 f"CLI JSONDecodeError:::{res_body}",
                 res_body
             )
             exc.process = res_body
             raise exc
-        res_body.update({"object": "error"})
         if self._should_handle_as_error(res_body):
+            res_body.update({"object": "error"})
             self.handle_error_response(res_body)
         return res_body
 
     @staticmethod
     def _should_handle_as_error(res_body):
         try:
             return res_body.get("object") == "error" or res_body.get("is_success") is False or \
```

### Comparing `locker-secrets-0.0.6b1/locker/config.py` & `locker-secrets-0.0.7b1/locker/config.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/environment_quick_usage.py` & `locker-secrets-0.0.7b1/locker/environment_quick_usage.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/error.py` & `locker-secrets-0.0.7b1/locker/error.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/logger.py` & `locker-secrets-0.0.7b1/locker/logger.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/ls_object.py` & `locker-secrets-0.0.7b1/locker/ls_object.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/ls_resources/abstract/__init__.py` & `locker-secrets-0.0.7b1/locker/ls_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/ls_resources/abstract/api_resource.py` & `locker-secrets-0.0.7b1/locker/ls_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/ls_resources/abstract/deletable_api_resource.py` & `locker-secrets-0.0.7b1/locker/ls_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/ls_resources/abstract/listable_api_resource.py` & `locker-secrets-0.0.7b1/locker/ls_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/ls_resources/abstract/singleton_api_resource.py` & `locker-secrets-0.0.7b1/locker/ls_resources/abstract/singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/ls_resources/environment.py` & `locker-secrets-0.0.7b1/locker/ls_resources/environment.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/ls_resources/error_object.py` & `locker-secrets-0.0.7b1/locker/ls_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/ls_resources/secret.py` & `locker-secrets-0.0.7b1/locker/ls_resources/secret.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/ls_response.py` & `locker-secrets-0.0.7b1/locker/ls_response.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/secret_quick_usage.py` & `locker-secrets-0.0.7b1/locker/secret_quick_usage.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker/util.py` & `locker-secrets-0.0.7b1/locker/util.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/locker_secrets.egg-info/PKG-INFO` & `locker-secrets-0.0.7b1/locker_secrets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locker-secrets
-Version: 0.0.6b1
+Version: 0.0.7b1
 Summary: Locker Secret Python SDK
 Home-page: https://locker.io
 Download-URL: 
 Author: CyStack
 Author-email: contact@locker.io
 Keywords: django,vault management,security
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `locker-secrets-0.0.6b1/locker_secrets.egg-info/SOURCES.txt` & `locker-secrets-0.0.7b1/locker_secrets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/setup.py` & `locker-secrets-0.0.7b1/setup.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/tests/test_environment_quick_usage.py` & `locker-secrets-0.0.7b1/tests/test_environment_quick_usage.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/tests/test_util.py` & `locker-secrets-0.0.7b1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `locker-secrets-0.0.6b1/tox.ini` & `locker-secrets-0.0.7b1/tox.ini`

 * *Files identical despite different names*

