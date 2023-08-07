# Comparing `tmp/pasqal-cloud-0.3.4.tar.gz` & `tmp/pasqal-cloud-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal-cloud-0.3.4.tar", last modified: Thu Aug  3 08:43:43 2023, max compression
+gzip compressed data, was "pasqal-cloud-0.3.5.tar", last modified: Mon Aug  7 13:05:46 2023, max compression
```

## Comparing `pasqal-cloud-0.3.4.tar` & `pasqal-cloud-0.3.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.836665 pasqal-cloud-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-03 08:43:43.836665 pasqal-cloud-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/result_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/utils/strenum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/workload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-03 08:43:43.000000 pasqal-cloud-0.3.4/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-03 08:43:43.000000 pasqal-cloud-0.3.4/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:43:43.000000 pasqal-cloud-0.3.4/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-03 08:43:43.000000 pasqal-cloud-0.3.4/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 08:43:43.000000 pasqal-cloud-0.3.4/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-03 08:43:43.836665 pasqal-cloud-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.836665 pasqal-cloud-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.836665 pasqal-cloud-0.3.4/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_doubles/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_project_renaming_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_workload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:46.372550 pasqal-cloud-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-07 13:05:46.372550 pasqal-cloud-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:46.368550 pasqal-cloud-0.3.5/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:46.368550 pasqal-cloud-0.3.5/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:46.368550 pasqal-cloud-0.3.5/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/device/configuration/result_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:46.368550 pasqal-cloud-0.3.5/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/utils/strenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pasqal_cloud/workload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:46.368550 pasqal-cloud-0.3.5/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-07 13:05:46.000000 pasqal-cloud-0.3.5/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-07 13:05:46.000000 pasqal-cloud-0.3.5/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:05:46.000000 pasqal-cloud-0.3.5/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-07 13:05:46.000000 pasqal-cloud-0.3.5/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 13:05:46.000000 pasqal-cloud-0.3.5/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:46.368550 pasqal-cloud-0.3.5/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:46.368550 pasqal-cloud-0.3.5/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:46.368550 pasqal-cloud-0.3.5/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:46.368550 pasqal-cloud-0.3.5/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-07 13:05:46.372550 pasqal-cloud-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:46.368550 pasqal-cloud-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:46.372550 pasqal-cloud-0.3.5/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/tests/test_doubles/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/tests/test_project_renaming_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-08-07 13:05:35.000000 pasqal-cloud-0.3.5/tests/test_workload.py
```

### Comparing `pasqal-cloud-0.3.4/LICENSE` & `pasqal-cloud-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/PKG-INFO` & `pasqal-cloud-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.3.4
+Version: 0.3.5
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pasqal-cloud-0.3.4/README.md` & `pasqal-cloud-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/pasqal_cloud/__init__.py` & `pasqal-cloud-0.3.5/pasqal_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/pasqal_cloud/_version.py` & `pasqal-cloud-0.3.5/pasqal_cloud/_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.4"
+__version__ = "0.3.5"
```

### Comparing `pasqal-cloud-0.3.4/pasqal_cloud/authentication.py` & `pasqal-cloud-0.3.5/pasqal_cloud/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/pasqal_cloud/batch.py` & `pasqal-cloud-0.3.5/pasqal_cloud/batch.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
-from typing import Any, Dict, Optional, Type, Union
+from typing import Any, Dict, List, Optional, Type, Union
+from warnings import warn
 
 from pydantic import BaseModel, Extra, root_validator, validator
 
 from pasqal_cloud.client import Client
 from pasqal_cloud.device import EmulatorType
 from pasqal_cloud.device.configuration import BaseConfig, EmuFreeConfig, EmuTNConfig
 from pasqal_cloud.job import Job
@@ -31,15 +32,17 @@
             PENDING, RUNNING, DONE, CANCELED, TIMED_OUT, ERROR, PAUSED.
         - webhook: Webhook where the job results are automatically sent to.
         - _client: A Client instance to connect to PCS.
         - sequence_builder: Pulser sequence of the batch.
         - start_datetime: Timestamp of the time the batch was sent to the QPU.
         - end_datetime: Timestamp of when the batch process was finished.
         - device_status: Status of the device where the batch is running.
-        - jobs: Dictionary of all the jobs added to the batch.
+        - jobs (deprecated): Dictionary of all the jobs added to the batch.
+        - ordered_jobs: List of all the jobs added to the batch,
+            ordered by creation time.
         - jobs_count: Number of jobs added to the batch.
         - jobs_count_per_status: Number of jobs per status.
         - configuration: Further configuration for certain emulators.
         - group_id (deprecated): Use project_id instead.
     """
 
     complete: bool
@@ -53,23 +56,51 @@
     status: str
     webhook: Optional[str]
     _client: Client
     sequence_builder: str
     start_datetime: Optional[str]
     end_datetime: Optional[str]
     device_status: Optional[str]
-    jobs: Dict[str, Job] = {}
+    ordered_jobs: List[Job] = []
     jobs_count: int = 0
     jobs_count_per_status: Dict[str, int] = {}
     configuration: Union[BaseConfig, Dict[str, Any], None] = None
 
     class Config:
         extra = Extra.allow
         arbitrary_types_allowed = True
 
+    @root_validator(pre=True)
+    def _build_ordered_jobs(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+        """This root validator will modify the 'jobs' attribute which is a list
+        of jobs dictionaries ordered by creation time before instantiation.
+        It will duplicate the value of 'jobs' in a new attribute 'ordered_jobs'
+        to keep the jobs ordered by creation time.
+        """
+        ordered_jobs_list = []
+        jobs_received = values.get("jobs", [])
+        for job in jobs_received:
+            job_dict = {**job, "_client": values["_client"]}
+            ordered_jobs_list.append(job_dict)
+        values["ordered_jobs"] = ordered_jobs_list
+        return values
+
+    # Ticket (#704), to be removed or updated
+    @property
+    def jobs(self) -> Dict[str, Job]:
+        """Once the 'ordered_jobs' is built, we need to keep the 'jobs' attribute
+        for backward compatibility with the code written by the users of the sdk
+        """
+        warn(
+            "'jobs' attribute is deprecated, use 'ordered_jobs' instead",
+            DeprecationWarning,
+            stacklevel=1,
+        )
+        return {job.id: job for job in self.ordered_jobs}
+
     @validator("configuration", pre=True)
     def _load_configuration(
         cls,
         configuration: Union[Dict[str, Any], BaseConfig, None],
         values: Dict[str, Any],
     ) -> Optional[BaseConfig]:
         if not isinstance(configuration, dict):
@@ -77,27 +108,14 @@
         conf_class: Type[BaseConfig] = BaseConfig
         if values["device_type"] == EmulatorType.EMU_TN.value:
             conf_class = EmuTNConfig
         elif values["device_type"] == EmulatorType.EMU_FREE.value:
             conf_class = EmuFreeConfig
         return conf_class.from_dict(configuration)
 
-    @root_validator(pre=True)
-    def _build_job_dict(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-        """This root validator will modify the 'jobs' attribute (which is a list
-        of jobs dictionaries ordered by creation time before instantiation) and
-        will transform it to a dictionary of jobs dictionaries.
-        """
-        jobs = values.get("jobs", [])
-        job_dict = {}
-        for job in jobs:
-            job_dict[job["id"]] = {**job, "_client": values["_client"]}
-        values["jobs"] = job_dict
-        return values
-
     def add_job(
         self,
         runs: int = 100,
         variables: Optional[Dict[str, Any]] = None,
         wait: bool = False,
     ) -> Job:
         """Add and send a new job for this batch.
@@ -111,15 +129,15 @@
             - Job: the created job.
         """
         job_data: Dict[str, Any] = {"runs": runs, "batch_id": self.id}
         if variables:
             job_data["variables"] = variables
         job_rsp = self._client._send_job(job_data)
         job = Job(**job_rsp, _client=self._client)
-        self.jobs[job.id] = job
+        self.ordered_jobs.append(job)
         if wait:
             while job.status in ["PENDING", "RUNNING"]:
                 time.sleep(RESULT_POLLING_INTERVAL)
                 job_rsp = self._client._get_job(job.id)
                 job = Job(**job_rsp)
         return job
 
@@ -141,16 +159,18 @@
         self.complete = True
         if wait or fetch_results:
             while batch_rsp["status"] in ["PENDING", "RUNNING"]:
                 time.sleep(RESULT_POLLING_INTERVAL)
                 batch_rsp = self._client._get_batch(
                     self.id,
                 )
-            for job_rsp in batch_rsp["jobs"]:
-                self.jobs[job_rsp["id"]] = Job(**job_rsp)
+            self.ordered_jobs = [
+                Job(**job, _client=self._client) for job in batch_rsp["jobs"]
+            ]
+
         return batch_rsp
 
     def cancel(self) -> Dict[str, Any]:
         """Cancel the current batch on the PCS."""
         batch_rsp = self._client._cancel_batch(self.id)
         self.status = batch_rsp.get("status", "CANCELED")
         return batch_rsp
```

### Comparing `pasqal-cloud-0.3.4/pasqal_cloud/client.py` & `pasqal-cloud-0.3.5/pasqal_cloud/client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/base_config.py` & `pasqal-cloud-0.3.5/pasqal_cloud/device/configuration/base_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal-cloud-0.3.5/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/pasqal_cloud/endpoints.py` & `pasqal-cloud-0.3.5/pasqal_cloud/endpoints.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/pasqal_cloud/errors.py` & `pasqal-cloud-0.3.5/pasqal_cloud/errors.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/pasqal_cloud/job.py` & `pasqal-cloud-0.3.5/pasqal_cloud/job.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/pasqal_cloud/utils/jsend.py` & `pasqal-cloud-0.3.5/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/pasqal_cloud/workload.py` & `pasqal-cloud-0.3.5/pasqal_cloud/workload.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/pasqal_cloud.egg-info/PKG-INFO` & `pasqal-cloud-0.3.5/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.3.4
+Version: 0.3.5
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pasqal-cloud-0.3.4/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal-cloud-0.3.5/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/sdk/setup.py` & `pasqal-cloud-0.3.5/sdk/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/setup.py` & `pasqal-cloud-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/tests/conftest.py` & `pasqal-cloud-0.3.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/tests/test_batch.py` & `pasqal-cloud-0.3.5/tests/test_batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,135 +18,96 @@
         self.sdk = SDK(
             username="me@test.com",
             password="password",
             project_id=str(uuid4()),
         )
         self.pulser_sequence = "pulser_test_sequence"
         self.batch_id = "00000000-0000-0000-0000-000000000001"
-        self.job_result = {"1001": 12, "0110": 35, "1111": 1}
-        self.job_full_result = {
-            "counter": {"1001": 12, "0110": 35, "1111": 1},
-            "raw": ["1001", "1001", "0110", "1001", "0110"],
-        }
-        self.n_job_runs = 50
         self.job_id = "00000000-0000-0000-0000-000000022010"
+        self.n_job_runs = 50
         self.job_variables = {
             "Omega_max": 14.4,
             "last_target": "q1",
             "ts": [200, 500],
         }
-
-    @pytest.mark.parametrize("emulator", [None] + [e.value for e in EmulatorType])
-    def test_create_batch(self, emulator):
-        job = {
+        self.simple_job_args = {
             "runs": self.n_job_runs,
             "variables": self.job_variables,
         }
+        self.job_result = {"1001": 12, "0110": 35, "1111": 1}
+        self.job_full_result = {
+            "counter": {"1001": 12, "0110": 35, "1111": 1},
+            "raw": ["1001", "1001", "0110", "1001", "0110"],
+        }
+
+    @pytest.mark.parametrize("emulator", [None] + [e.value for e in EmulatorType])
+    def test_create_batch(self, emulator):
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
-            jobs=[job],
+            jobs=[self.simple_job_args],
             emulator=emulator,
         )
         assert batch.id == self.batch_id
         assert batch.sequence_builder == self.pulser_sequence
         assert batch.complete
-        assert batch.jobs[self.job_id].batch_id == batch.id
+        assert batch.ordered_jobs[0].batch_id == batch.id
 
     @pytest.mark.filterwarnings(
         "ignore:Argument `fetch_results` is deprecated and will be removed "
         "in a future version. Please use argument `wait` instead"
     )
     @pytest.mark.parametrize("wait,fetch_results", [(True, False), (False, True)])
     def test_create_batch_and_wait(self, request_mock, wait, fetch_results):
-        job = {
-            "runs": self.n_job_runs,
-            "variables": self.job_variables,
-        }
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
-            jobs=[job],
+            jobs=[self.simple_job_args],
             wait=wait,
             fetch_results=fetch_results,
         )
         assert (
             batch.id == "00000000-0000-0000-0000-000000000001"
         )  # the batch_id used in the mock data
         assert batch.sequence_builder == self.pulser_sequence
         assert batch.complete
-        assert batch.jobs
-        for job_id, job in batch.jobs.items():
-            assert self.job_id == job_id
-            assert job.result == self.job_result
-            assert job.full_result == self.job_full_result
+        assert batch.ordered_jobs
+        assert batch.ordered_jobs[0].id == self.job_id
+        assert batch.ordered_jobs[0].result == self.job_result
+        assert batch.ordered_jobs[0].full_result == self.job_full_result
+        # Ticket (#704)
+        with pytest.warns(
+            DeprecationWarning,
+            match="'jobs' attribute is deprecated, use 'ordered_jobs' instead",
+        ):
+            for job_id, job in batch.jobs.items():
+                assert self.job_id == job_id
+                assert job.result == self.job_result
+                assert job.full_result == self.job_full_result
+            assert len(batch.jobs) == len(batch.ordered_jobs)
         assert request_mock.last_request.method == "GET"
 
     def test_get_batch(self, batch):
         batch_requested = self.sdk.get_batch(batch.id)
         assert batch_requested.id == self.batch_id
 
-    def test_cancel_batch_self(self, request_mock, batch):
-        batch.cancel()
-        assert batch.status == "CANCELED"
-        assert request_mock.last_request.method == "PUT"
-        assert (
-            request_mock.last_request.url == f"{self.sdk._client.endpoints.core}"
-            f"/api/v1/batches/{self.batch_id}/cancel"
-        )
-
-    def test_cancel_batch_sdk(self, request_mock):
-        client_rsp = self.sdk.cancel_batch(self.batch_id)
-        assert type(client_rsp) == Batch
-        assert client_rsp.status == "CANCELED"
-        assert request_mock.last_request.method == "PUT"
-        assert (
-            request_mock.last_request.url == f"{self.sdk._client.endpoints.core}"
-            f"/api/v1/batches/{self.batch_id}/cancel"
-        )
-
-    def test_get_job(self, job):
-        job_requested = self.sdk.get_job(job.id)
-        print(self.sdk)
-        assert job_requested.id == job.id
-
-    def test_cancel_job_self(self, request_mock, job):
-        job.cancel()
-        assert job.status == "CANCELED"
-        assert request_mock.last_request.method == "PUT"
-        assert (
-            request_mock.last_request.url
-            == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}/cancel"
-        )
-
-    def test_cancel_job_sdk(self, request_mock):
-        client_rsp = self.sdk.cancel_job(self.job_id)
-        assert type(client_rsp) == Job
-        assert client_rsp.status == "CANCELED"
-        assert request_mock.last_request.method == "PUT"
-        assert (
-            request_mock.last_request.url
-            == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}/cancel"
-        )
-
-    @pytest.mark.skip(reason="Not enabled during Iroise MVP")
     def test_batch_add_job(self, request_mock):
         batch = self.sdk.create_batch(
-            serialized_sequence=self.pulser_sequence,
+            serialized_sequence=self.pulser_sequence, jobs=[self.simple_job_args]
         )
         job = batch.add_job(
             runs=self.n_job_runs,
             variables=self.job_variables,
         )
         assert request_mock.last_request.json()["batch_id"] == batch.id
         assert job.batch_id == batch.id
         assert job.runs == self.n_job_runs
+        assert len(batch.ordered_jobs) == 2
 
-    @pytest.mark.skip(reason="Not enabled during Iroise MVP")
     def test_batch_add_job_and_wait_for_results(self, request_mock):
         batch = self.sdk.create_batch(
-            serialized_sequence=self.pulser_sequence,
+            serialized_sequence=self.pulser_sequence, jobs=[self.simple_job_args]
         )
         job = batch.add_job(
             runs=self.n_job_runs,
             variables={
                 "Omega_max": 14.4,
                 "last_target": "q1",
                 "ts": [200, 500],
@@ -159,38 +120,80 @@
         assert (
             request_mock.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}"
         )
         assert job.result == self.job_result
         assert job.full_result == self.job_full_result
 
-    @pytest.mark.skip(reason="Not enabled during Iroise MVP")
     def test_batch_declare_complete(self):
         batch = self.sdk.create_batch(
-            serialized_sequence=self.pulser_sequence,
+            serialized_sequence=self.pulser_sequence, jobs=[self.simple_job_args]
         )
         rsp = batch.declare_complete(wait=False)
         assert rsp["complete"]
-        assert len(batch.jobs) == 0
 
-    @pytest.mark.skip(reason="Not enabled during Iroise MVP")
     def test_batch_declare_complete_and_wait_for_results(self, request_mock):
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
+            jobs=[self.simple_job_args],
         )
         rsp = batch.declare_complete(wait=True)
         assert rsp["complete"]
         assert request_mock.last_request.method == "GET"
         assert (
             request_mock.last_request.url
-            == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}"
+            == f"{self.sdk._client.endpoints.core}/api/v1/batches/{self.batch_id}"
+        )
+        assert batch.ordered_jobs[0].batch_id == batch.id
+        assert batch.ordered_jobs[0].result == self.job_result
+        assert batch.ordered_jobs[0].full_result == self.job_full_result
+        assert len(batch.ordered_jobs) == 1
+
+    def test_cancel_batch_self(self, request_mock, batch):
+        batch.cancel()
+        assert batch.status == "CANCELED"
+        assert request_mock.last_request.method == "PUT"
+        assert (
+            request_mock.last_request.url == f"{self.sdk._client.endpoints.core}"
+            f"/api/v1/batches/{self.batch_id}/cancel"
+        )
+
+    def test_cancel_batch_sdk(self, request_mock):
+        client_rsp = self.sdk.cancel_batch(self.batch_id)
+        assert type(client_rsp) == Batch
+        assert client_rsp.status == "CANCELED"
+        assert request_mock.last_request.method == "PUT"
+        assert (
+            request_mock.last_request.url == f"{self.sdk._client.endpoints.core}"
+            f"/api/v1/batches/{self.batch_id}/cancel"
+        )
+
+    def test_get_job(self, job):
+        job_requested = self.sdk.get_job(job.id)
+        print(self.sdk)
+        assert job_requested.id == job.id
+
+    def test_cancel_job_self(self, request_mock, job):
+        job.cancel()
+        assert job.status == "CANCELED"
+        assert request_mock.last_request.method == "PUT"
+        assert (
+            request_mock.last_request.url
+            == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}/cancel"
+        )
+
+    def test_cancel_job_sdk(self, request_mock):
+        client_rsp = self.sdk.cancel_job(self.job_id)
+        assert type(client_rsp) == Job
+        assert client_rsp.status == "CANCELED"
+        assert request_mock.last_request.method == "PUT"
+        assert (
+            request_mock.last_request.url
+            == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}/cancel"
         )
-        assert batch.jobs[self.job_id].batch_id == batch.id
-        assert batch.jobs[self.job_id].result == self.job_result
-        assert batch.jobs[self.job_id].full_result == self.job_full_result
 
     @pytest.mark.parametrize(
         "emulator, configuration, expected",
         [
             (EmulatorType.EMU_TN, EmuTNConfig(), EmuTNConfig()),
             (None, None, None),
             (
@@ -202,21 +205,17 @@
                 "SomethingElse",
                 BaseConfig(),
                 BaseConfig(extra_config={"dt": 10.0, "precision": "normal"}),
             ),
         ],
     )
     def test_create_batch_configuration(self, emulator, configuration, expected):
-        job = {
-            "runs": self.n_job_runs,
-            "variables": self.job_variables,
-        }
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
-            jobs=[job],
+            jobs=[self.simple_job_args],
             emulator=emulator,
             configuration=configuration,
         )
         assert batch.configuration == expected
 
     def test_batch_instantiation_with_extra_field(self, batch):
         """Instantiating a batch with an extra field should not raise an error.
@@ -233,22 +232,18 @@
         assert (
             new_batch.new_field == "any_value"
         )  # The new value should be stored regardless
 
     def test_create_batch_fetch_results_deprecated(
         self,
     ):
-        job = {
-            "runs": self.n_job_runs,
-            "variables": self.job_variables,
-        }
         with pytest.warns(DeprecationWarning):
             self.sdk.create_batch(
                 serialized_sequence=self.pulser_sequence,
-                jobs=[job],
+                jobs=[self.simple_job_args],
                 fetch_results=True,
             )
 
     def test_get_batch_fetch_results_deprecated(
         self,
     ):
         with pytest.warns(DeprecationWarning):
```

### Comparing `pasqal-cloud-0.3.4/tests/test_client.py` & `pasqal-cloud-0.3.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/tests/test_cloud_sdk_import.py` & `pasqal-cloud-0.3.5/tests/test_cloud_sdk_import.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/tests/test_config.py` & `pasqal-cloud-0.3.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/tests/test_device_specs.py` & `pasqal-cloud-0.3.5/tests/test_device_specs.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/tests/test_doubles/authentication.py` & `pasqal-cloud-0.3.5/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/tests/test_job.py` & `pasqal-cloud-0.3.5/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/tests/test_project_renaming_compatibility.py` & `pasqal-cloud-0.3.5/tests/test_project_renaming_compatibility.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.4/tests/test_workload.py` & `pasqal-cloud-0.3.5/tests/test_workload.py`

 * *Files identical despite different names*

