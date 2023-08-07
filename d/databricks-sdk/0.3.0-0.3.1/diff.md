# Comparing `tmp/databricks-sdk-0.3.0.tar.gz` & `tmp/databricks-sdk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-sdk-0.3.0.tar", last modified: Thu Jul 27 12:07:31 2023, max compression
+gzip compressed data, was "databricks-sdk-0.3.1.tar", last modified: Wed Aug  2 13:31:37 2023, max compression
```

## Comparing `databricks-sdk-0.3.0.tar` & `databricks-sdk-0.3.1.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:07:31.211931 databricks-sdk-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-07-27 12:07:31.211931 databricks-sdk-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33991 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:07:31.203931 databricks-sdk-0.3.0/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:07:31.203931 databricks-sdk-0.3.0/databricks/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14684 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:07:31.203931 databricks-sdk-0.3.0/databricks/sdk/_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/_widgets/default_widgets_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/_widgets/ipywidgets_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    43138 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/dbutils.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:07:31.207931 databricks-sdk-0.3.0/databricks/sdk/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/mixins/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/mixins/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/mixins/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:07:31.207931 databricks-sdk-0.3.0/databricks/sdk/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/runtime/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:07:31.207931 databricks-sdk-0.3.0/databricks/sdk/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/_internal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34413 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/billing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   226833 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/catalog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   246857 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/compute.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17825 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   105549 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/iam.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   159216 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/jobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   152495 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/ml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29244 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/oauth2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    65654 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/pipelines.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   107875 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/provisioning.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28772 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/serving.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54013 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    76715 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/sharing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   172090 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/sql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55433 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/service/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/databricks/sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:07:31.211931 databricks-sdk-0.3.0/databricks_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-07-27 12:07:31.000000 databricks-sdk-0.3.0/databricks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-27 12:07:31.000000 databricks-sdk-0.3.0/databricks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:07:31.000000 databricks-sdk-0.3.0/databricks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-27 12:07:31.000000 databricks-sdk-0.3.0/databricks_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 12:07:31.000000 databricks-sdk-0.3.0/databricks_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-27 12:07:31.211931 databricks-sdk-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-27 12:07:13.000000 databricks-sdk-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:31:37.196375 databricks-sdk-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-08-02 13:31:37.196375 databricks-sdk-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33991 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:31:37.188374 databricks-sdk-0.3.1/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:31:37.188374 databricks-sdk-0.3.1/databricks/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14686 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:31:37.188374 databricks-sdk-0.3.1/databricks/sdk/_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/_widgets/default_widgets_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/_widgets/ipywidgets_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43138 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/dbutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:31:37.192375 databricks-sdk-0.3.1/databricks/sdk/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/mixins/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/mixins/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/mixins/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:31:37.192375 databricks-sdk-0.3.1/databricks/sdk/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/runtime/dbutils_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/runtime/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:31:37.196375 databricks-sdk-0.3.1/databricks/sdk/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/_internal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34413 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/billing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   226833 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/catalog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   246857 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/compute.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17825 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   105549 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/iam.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   159216 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/jobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   152495 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/ml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29244 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/oauth2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    65654 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/pipelines.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   107875 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/provisioning.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28772 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/serving.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54013 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    76715 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/sharing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   172120 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/sql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55433 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/service/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/databricks/sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:31:37.196375 databricks-sdk-0.3.1/databricks_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-08-02 13:31:37.000000 databricks-sdk-0.3.1/databricks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-02 13:31:37.000000 databricks-sdk-0.3.1/databricks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:31:37.000000 databricks-sdk-0.3.1/databricks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-02 13:31:37.000000 databricks-sdk-0.3.1/databricks_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 13:31:37.000000 databricks-sdk-0.3.1/databricks_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-08-02 13:31:37.200375 databricks-sdk-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-02 13:31:16.000000 databricks-sdk-0.3.1/setup.py
```

### Comparing `databricks-sdk-0.3.0/LICENSE` & `databricks-sdk-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/NOTICE` & `databricks-sdk-0.3.1/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/PKG-INFO` & `databricks-sdk-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sdk
-Version: 0.3.0
+Version: 0.3.1
 Summary: Databricks SDK for Python (Beta)
 Home-page: https://databricks-sdk-py.readthedocs.io
 Author: Serge Smertin
 Author-email: serge.smertin@databricks.com
 License: UNKNOWN
 Keywords: databricks sdk
 Platform: UNKNOWN
```

### Comparing `databricks-sdk-0.3.0/README.md` & `databricks-sdk-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/__init__.py` & `databricks-sdk-0.3.1/databricks/sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                  azure_client_secret: str = None,
                  azure_client_id: str = None,
                  azure_tenant_id: str = None,
                  azure_environment: str = None,
                  auth_type: str = None,
                  cluster_id: str = None,
                  debug_truncate_bytes: int = None,
-                 debug_headers: int = None,
+                 debug_headers: bool = None,
                  product="unknown",
                  product_version="0.0.0",
                  credentials_provider: client.CredentialsProvider = None,
                  config: client.Config = None):
         if not config:
             config = client.Config(host=host,
                                    account_id=account_id,
@@ -201,15 +201,15 @@
                  azure_client_secret: str = None,
                  azure_client_id: str = None,
                  azure_tenant_id: str = None,
                  azure_environment: str = None,
                  auth_type: str = None,
                  cluster_id: str = None,
                  debug_truncate_bytes: int = None,
-                 debug_headers: int = None,
+                 debug_headers: bool = None,
                  product="unknown",
                  product_version="0.0.0",
                  credentials_provider: client.CredentialsProvider = None,
                  config: client.Config = None):
         if not config:
             config = client.Config(host=host,
                                    account_id=account_id,
```

### Comparing `databricks-sdk-0.3.0/databricks/sdk/_widgets/__init__.py` & `databricks-sdk-0.3.1/databricks/sdk/_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/_widgets/default_widgets_utils.py` & `databricks-sdk-0.3.1/databricks/sdk/_widgets/default_widgets_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/_widgets/ipywidgets_utils.py` & `databricks-sdk-0.3.1/databricks/sdk/_widgets/ipywidgets_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/azure.py` & `databricks-sdk-0.3.1/databricks/sdk/azure.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/core.py` & `databricks-sdk-0.3.1/databricks/sdk/core.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/dbutils.py` & `databricks-sdk-0.3.1/databricks/sdk/dbutils.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/mixins/compute.py` & `databricks-sdk-0.3.1/databricks/sdk/mixins/compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+import datetime
+import logging
 import re
+import time
 from dataclasses import dataclass
 from typing import Optional
 
+from databricks.sdk.errors import OperationFailed
 from databricks.sdk.service import compute
 
+_LOG = logging.getLogger('databricks.sdk')
+
 
 @dataclass
 class SemVer:
     major: int
     minor: int
     patch: int
     pre_release: Optional[str] = None
@@ -199,20 +205,32 @@
             if photon_worker_capable and not nt.photon_worker_capable:
                 continue
             if graviton and nt.is_graviton != graviton:
                 continue
             return nt.node_type_id
         raise ValueError("cannot determine smallest node type")
 
-    def ensure_cluster_is_running(self, cluster_id: str):
+    def ensure_cluster_is_running(self, cluster_id: str) -> None:
         """Ensures that given cluster is running, regardless of the current state"""
-        state = compute.State
-        info = self.get(cluster_id)
-        if info.state == state.TERMINATED:
-            self.start(cluster_id).result()
-        elif info.state == state.TERMINATING:
-            self.wait_get_cluster_terminated(cluster_id)
-            self.start(cluster_id).result()
-        elif info.state in (state.PENDING, state.RESIZING, state.RESTARTING):
-            self.wait_get_cluster_running(cluster_id)
-        elif info.state in (state.ERROR, state.UNKNOWN):
-            raise RuntimeError(f'Cluster {info.cluster_name} is {info.state}: {info.state_message}')
+        timeout = datetime.timedelta(minutes=20)
+        deadline = time.time() + timeout.total_seconds()
+        while time.time() < deadline:
+            try:
+                state = compute.State
+                info = self.get(cluster_id)
+                if info.state == state.RUNNING:
+                    return
+                elif info.state == state.TERMINATED:
+                    self.start(cluster_id).result()
+                    return
+                elif info.state == state.TERMINATING:
+                    self.wait_get_cluster_terminated(cluster_id)
+                    self.start(cluster_id).result()
+                    return
+                elif info.state in (state.PENDING, state.RESIZING, state.RESTARTING):
+                    self.wait_get_cluster_running(cluster_id)
+                    return
+                elif info.state in (state.ERROR, state.UNKNOWN):
+                    raise RuntimeError(f'Cluster {info.cluster_name} is {info.state}: {info.state_message}')
+            except OperationFailed as e:
+                _LOG.debug('Operation failed, retrying', exc_info=e)
+        raise TimeoutError(f'timed out after {timeout}')
```

### Comparing `databricks-sdk-0.3.0/databricks/sdk/mixins/files.py` & `databricks-sdk-0.3.1/databricks/sdk/mixins/files.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/mixins/workspace.py` & `databricks-sdk-0.3.1/databricks/sdk/mixins/workspace.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/oauth.py` & `databricks-sdk-0.3.1/databricks/sdk/oauth.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/runtime/__init__.py` & `databricks-sdk-0.3.1/databricks/sdk/runtime/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from typing import Union
+
 is_local_implementation = True
 
 # All objects that are injected into the Notebook's user namespace should also be made
 # available to be imported from databricks.sdk.runtime.globals. This import can be used
 # in Python modules so users can access these objects from Files more easily.
 dbruntime_objects = [
     "display", "displayHTML", "dbutils", "table", "sql", "udf", "getArgument", "sc", "sqlContext", "spark"
@@ -29,26 +31,27 @@
     _globals = globals()
     for var in dbruntime_objects:
         if var not in userNamespaceGlobals:
             continue
         _globals[var] = userNamespaceGlobals[var]
     is_local_implementation = False
 except ImportError:
-    from typing import Type, cast
+    from typing import cast
 
     # OSS implementation
     is_local_implementation = True
 
+    from databricks.sdk.dbutils import RemoteDbUtils
+
+    from . import dbutils_stub
+
+    dbutils_type = Union[dbutils_stub.dbutils, RemoteDbUtils]
+
     try:
-        from . import stub
         from .stub import *
-        dbutils_type = Type[stub.dbutils]
     except (ImportError, NameError):
-        from databricks.sdk.dbutils import RemoteDbUtils
-
         # this assumes that all environment variables are set
         dbutils = RemoteDbUtils()
-        dbutils_type = RemoteDbUtils
 
     dbutils = cast(dbutils_type, dbutils)
 
 __all__ = ['dbutils'] if is_local_implementation else dbruntime_objects
```

### Comparing `databricks-sdk-0.3.0/databricks/sdk/runtime/stub.py` & `databricks-sdk-0.3.1/databricks/sdk/runtime/dbutils_stub.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,10 @@
 import typing
 from collections import namedtuple
 
-from pyspark.sql.context import SQLContext
-from pyspark.sql.functions import udf as U
-from pyspark.sql.session import SparkSession
-
-udf = U
-spark: SparkSession
-sc = spark.sparkContext
-sqlContext: SQLContext
-sql = sqlContext.sql
-table = sqlContext.table
-
 
 class FileInfo(namedtuple('FileInfo', ['path', 'name', 'size', "modificationTime"])):
     pass
 
 
 class MountInfo(namedtuple('MountInfo', ['mountPoint', 'source', 'encryptionType'])):
     pass
@@ -27,52 +16,14 @@
         return self.name
 
 
 class SecretMetadata(namedtuple('SecretMetadata', ['key'])):
     pass
 
 
-def displayHTML(html):
-    """
-    Display HTML data.
-    Parameters
-    ----------
-    data : URL or HTML string
-                    If data is a URL, display the resource at that URL, the resource is loaded dynamically by the browser.
-                    Otherwise data should be the HTML to be displayed.
-    See also:
-    IPython.display.HTML
-    IPython.display.display_html
-    """
-    ...
-
-
-def display(input=None, *args, **kwargs):
-    """
-    Display plots or data.
-    Display plot:
-                    - display() # no-op
-                    - display(matplotlib.figure.Figure)
-    Display dataset:
-                    - display(spark.DataFrame)
-                    - display(list) # if list can be converted to DataFrame, e.g., list of named tuples
-                    - display(pandas.DataFrame)
-                    - display(koalas.DataFrame)
-                    - display(pyspark.pandas.DataFrame)
-    Display any other value that has a _repr_html_() method
-    For Spark 2.0 and 2.1:
-                    - display(DataFrame, streamName='optional', trigger=optional pyspark.sql.streaming.Trigger,
-                                                    checkpointLocation='optional')
-    For Spark 2.2+:
-                    - display(DataFrame, streamName='optional', trigger=optional interval like '1 second',
-                                                    checkpointLocation='optional')
-    """
-    ...
-
-
 class dbutils:
 
     class credentials:
         """
         Utilities for interacting with credentials within notebooks
         """
 
@@ -206,15 +157,15 @@
             ...
 
         @staticmethod
         def updateMount(source: str,
                         mount_point: str,
                         encryption_type: str = "",
                         owner: typing.Optional[str] = None,
-                        extra_configs: typing.Map[str, str] = {},
+                        extra_configs: typing.Mapping[str, str] = {},
                         ) -> bool:
             """
             Similar to mount(), but updates an existing mount point (if present) instead of creating a new one
             """
             ...
 
         @staticmethod
@@ -283,15 +234,15 @@
         def exit(value: str) -> None:
             """
             This method lets you exit a notebook with a value
             """
             ...
 
         @staticmethod
-        def run(path: str, timeout_seconds: int, arguments: typing.Map[str, str]) -> str:
+        def run(path: str, timeout_seconds: int, arguments: typing.Mapping[str, str]) -> str:
             """
             This method runs a notebook and returns its exit value
             """
             ...
 
     class secrets:
         """
```

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/_internal.py` & `databricks-sdk-0.3.1/databricks/sdk/service/_internal.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/billing.py` & `databricks-sdk-0.3.1/databricks/sdk/service/billing.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/catalog.py` & `databricks-sdk-0.3.1/databricks/sdk/service/catalog.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/compute.py` & `databricks-sdk-0.3.1/databricks/sdk/service/compute.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/files.py` & `databricks-sdk-0.3.1/databricks/sdk/service/files.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/iam.py` & `databricks-sdk-0.3.1/databricks/sdk/service/iam.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/jobs.py` & `databricks-sdk-0.3.1/databricks/sdk/service/jobs.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/ml.py` & `databricks-sdk-0.3.1/databricks/sdk/service/ml.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/oauth2.py` & `databricks-sdk-0.3.1/databricks/sdk/service/oauth2.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/pipelines.py` & `databricks-sdk-0.3.1/databricks/sdk/service/pipelines.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/provisioning.py` & `databricks-sdk-0.3.1/databricks/sdk/service/provisioning.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/serving.py` & `databricks-sdk-0.3.1/databricks/sdk/service/serving.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/settings.py` & `databricks-sdk-0.3.1/databricks/sdk/service/settings.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/sharing.py` & `databricks-sdk-0.3.1/databricks/sdk/service/sharing.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/sql.py` & `databricks-sdk-0.3.1/databricks/sdk/service/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,14 +208,15 @@
 
     @classmethod
     def from_dict(cls, d: Dict[str, any]) -> 'ChannelInfo':
         return cls(dbsql_version=d.get('dbsql_version', None), name=_enum(d, 'name', ChannelName))
 
 
 class ChannelName(Enum):
+    """Name of the channel"""
 
     CHANNEL_NAME_CURRENT = 'CHANNEL_NAME_CURRENT'
     CHANNEL_NAME_CUSTOM = 'CHANNEL_NAME_CUSTOM'
     CHANNEL_NAME_PREVIEW = 'CHANNEL_NAME_PREVIEW'
     CHANNEL_NAME_PREVIOUS = 'CHANNEL_NAME_PREVIOUS'
     CHANNEL_NAME_UNSPECIFIED = 'CHANNEL_NAME_UNSPECIFIED'
```

### Comparing `databricks-sdk-0.3.0/databricks/sdk/service/workspace.py` & `databricks-sdk-0.3.1/databricks/sdk/service/workspace.py`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/databricks_sdk.egg-info/PKG-INFO` & `databricks-sdk-0.3.1/databricks_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sdk
-Version: 0.3.0
+Version: 0.3.1
 Summary: Databricks SDK for Python (Beta)
 Home-page: https://databricks-sdk-py.readthedocs.io
 Author: Serge Smertin
 Author-email: serge.smertin@databricks.com
 License: UNKNOWN
 Keywords: databricks sdk
 Platform: UNKNOWN
```

### Comparing `databricks-sdk-0.3.0/databricks_sdk.egg-info/SOURCES.txt` & `databricks-sdk-0.3.1/databricks_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 databricks/sdk/_widgets/default_widgets_utils.py
 databricks/sdk/_widgets/ipywidgets_utils.py
 databricks/sdk/mixins/__init__.py
 databricks/sdk/mixins/compute.py
 databricks/sdk/mixins/files.py
 databricks/sdk/mixins/workspace.py
 databricks/sdk/runtime/__init__.py
+databricks/sdk/runtime/dbutils_stub.py
 databricks/sdk/runtime/stub.py
 databricks/sdk/service/__init__.py
 databricks/sdk/service/_internal.py
 databricks/sdk/service/billing.py
 databricks/sdk/service/catalog.py
 databricks/sdk/service/compute.py
 databricks/sdk/service/files.py
```

### Comparing `databricks-sdk-0.3.0/setup.cfg` & `databricks-sdk-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `databricks-sdk-0.3.0/setup.py` & `databricks-sdk-0.3.1/setup.py`

 * *Files identical despite different names*

