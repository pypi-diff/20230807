# Comparing `tmp/google-cloud-automlops-1.1.4.tar.gz` & `tmp/google-cloud-automlops-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-automlops-1.1.4.tar", last modified: Fri Jul 28 18:40:58 2023, max compression
+gzip compressed data, was "google-cloud-automlops-1.1.5.tar", last modified: Mon Aug  7 17:58:24 2023, max compression
```

## Comparing `google-cloud-automlops-1.1.4.tar` & `google-cloud-automlops-1.1.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.580439 google-cloud-automlops-1.1.4/
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.571569 google-cloud-automlops-1.1.4/AutoMLOps/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    15964 2023-07-28 15:38:11.000000 google-cloud-automlops-1.1.4/AutoMLOps/AutoMLOps.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1199 2023-07-25 21:27:56.000000 google-cloud-automlops-1.1.4/AutoMLOps/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.571734 google-cloud-automlops-1.1.4/AutoMLOps/deployments/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/deployments/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.572271 google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2258 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/builder.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.572606 google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/constructs/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)        0 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/constructs/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9302 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/constructs/scripts.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.573140 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2271 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/base.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.573652 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11384 2023-07-28 15:31:24.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/builder.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.574841 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    20732 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/cloudrun.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3711 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/component.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9207 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/pipeline.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    29657 2023-07-28 15:37:31.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/scripts.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8714 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/scaffold.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.575471 google-cloud-automlops-1.1.4/AutoMLOps/utils/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/utils/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3229 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/AutoMLOps/utils/constants.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    10106 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/AutoMLOps/utils/utils.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11357 2023-01-13 20:01:02.000000 google-cloud-automlops-1.1.4/LICENSE
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14825 2023-07-28 18:40:58.580250 google-cloud-automlops-1.1.4/PKG-INFO
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13957 2023-07-28 15:52:25.000000 google-cloud-automlops-1.1.4/README.md
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.576433 google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14825 2023-07-28 18:40:58.000000 google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/PKG-INFO
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1621 2023-07-28 18:40:58.000000 google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/SOURCES.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)        1 2023-07-28 18:40:58.000000 google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/dependency_links.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       79 2023-07-28 18:40:58.000000 google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/requires.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       16 2023-07-28 18:40:58.000000 google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/top_level.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       38 2023-07-28 18:40:58.580486 google-cloud-automlops-1.1.4/setup.cfg
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1949 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/setup.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.576676 google-cloud-automlops-1.1.4/tests/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/tests/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.576835 google-cloud-automlops-1.1.4/tests/unit/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/tests/unit/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.577162 google-cloud-automlops-1.1.4/tests/unit/deployments/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/tests/unit/deployments/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.577504 google-cloud-automlops-1.1.4/tests/unit/frameworks/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     4438 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/base_test.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.578240 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    12725 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/builder_test.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.579456 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:59.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    21114 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/cloudrun_test.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     5358 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/component_test.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9119 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/pipeline_test.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    24644 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/scripts_test.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9008 2023-07-25 21:49:15.000000 google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/scaffold_test.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-07-28 18:40:58.579989 google-cloud-automlops-1.1.4/tests/unit/utils/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.4/tests/unit/utils/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    18039 2023-07-28 16:03:01.000000 google-cloud-automlops-1.1.4/tests/unit/utils/utils_test.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.875860 google-cloud-automlops-1.1.5/
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.868923 google-cloud-automlops-1.1.5/AutoMLOps/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    15972 2023-08-07 17:52:26.000000 google-cloud-automlops-1.1.5/AutoMLOps/AutoMLOps.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1199 2023-08-07 17:54:47.000000 google-cloud-automlops-1.1.5/AutoMLOps/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.869088 google-cloud-automlops-1.1.5/AutoMLOps/deployments/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.5/AutoMLOps/deployments/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.869459 google-cloud-automlops-1.1.5/AutoMLOps/deployments/cloudbuild/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.5/AutoMLOps/deployments/cloudbuild/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2259 2023-08-07 17:52:26.000000 google-cloud-automlops-1.1.5/AutoMLOps/deployments/cloudbuild/builder.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.869819 google-cloud-automlops-1.1.5/AutoMLOps/deployments/cloudbuild/constructs/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)        0 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.5/AutoMLOps/deployments/cloudbuild/constructs/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9303 2023-08-07 17:52:26.000000 google-cloud-automlops-1.1.5/AutoMLOps/deployments/cloudbuild/constructs/scripts.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.870161 google-cloud-automlops-1.1.5/AutoMLOps/frameworks/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.5/AutoMLOps/frameworks/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2274 2023-08-04 17:14:51.000000 google-cloud-automlops-1.1.5/AutoMLOps/frameworks/base.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.870654 google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11388 2023-08-07 17:52:26.000000 google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/builder.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.871523 google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/constructs/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/constructs/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    20733 2023-08-04 17:14:51.000000 google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/constructs/cloudrun.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3712 2023-08-04 17:14:51.000000 google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/constructs/component.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9206 2023-08-04 17:14:51.000000 google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/constructs/pipeline.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    29658 2023-08-07 17:52:26.000000 google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/constructs/scripts.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8721 2023-08-04 17:14:51.000000 google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/scaffold.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.872029 google-cloud-automlops-1.1.5/AutoMLOps/utils/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.5/AutoMLOps/utils/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3229 2023-08-07 17:52:26.000000 google-cloud-automlops-1.1.5/AutoMLOps/utils/constants.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    10121 2023-08-07 17:52:26.000000 google-cloud-automlops-1.1.5/AutoMLOps/utils/utils.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11357 2023-01-13 20:01:02.000000 google-cloud-automlops-1.1.5/LICENSE
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14825 2023-08-07 17:58:24.875630 google-cloud-automlops-1.1.5/PKG-INFO
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13957 2023-08-07 17:52:26.000000 google-cloud-automlops-1.1.5/README.md
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.872839 google-cloud-automlops-1.1.5/google_cloud_automlops.egg-info/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14825 2023-08-07 17:58:24.000000 google-cloud-automlops-1.1.5/google_cloud_automlops.egg-info/PKG-INFO
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1621 2023-08-07 17:58:24.000000 google-cloud-automlops-1.1.5/google_cloud_automlops.egg-info/SOURCES.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)        1 2023-08-07 17:58:24.000000 google-cloud-automlops-1.1.5/google_cloud_automlops.egg-info/dependency_links.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       79 2023-08-07 17:58:24.000000 google-cloud-automlops-1.1.5/google_cloud_automlops.egg-info/requires.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       16 2023-08-07 17:58:24.000000 google-cloud-automlops-1.1.5/google_cloud_automlops.egg-info/top_level.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       38 2023-08-07 17:58:24.875906 google-cloud-automlops-1.1.5/setup.cfg
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1949 2023-08-07 17:54:04.000000 google-cloud-automlops-1.1.5/setup.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.872997 google-cloud-automlops-1.1.5/tests/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.5/tests/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.873182 google-cloud-automlops-1.1.5/tests/unit/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.5/tests/unit/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.873381 google-cloud-automlops-1.1.5/tests/unit/deployments/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.5/tests/unit/deployments/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.873704 google-cloud-automlops-1.1.5/tests/unit/frameworks/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.5/tests/unit/frameworks/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     4441 2023-08-04 17:14:51.000000 google-cloud-automlops-1.1.5/tests/unit/frameworks/base_test.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.874186 google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    12730 2023-08-04 17:14:51.000000 google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/builder_test.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.875060 google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/constructs/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:59.000000 google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/constructs/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    21116 2023-08-04 17:14:51.000000 google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/constructs/cloudrun_test.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     5360 2023-08-04 17:14:51.000000 google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/constructs/component_test.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9121 2023-08-04 17:14:51.000000 google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/constructs/pipeline_test.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    24645 2023-08-07 17:52:26.000000 google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/constructs/scripts_test.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9017 2023-08-04 17:14:51.000000 google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/scaffold_test.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-08-07 17:58:24.875403 google-cloud-automlops-1.1.5/tests/unit/utils/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2023-07-13 15:20:21.000000 google-cloud-automlops-1.1.5/tests/unit/utils/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    18066 2023-08-07 17:52:26.000000 google-cloud-automlops-1.1.5/tests/unit/utils/utils_test.py
```

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/AutoMLOps.py` & `google-cloud-automlops-1.1.5/AutoMLOps/AutoMLOps.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from AutoMLOps.deployments.cloudbuild import builder as CloudBuildBuilder
 
 logging.basicConfig(stream=sys.stdout, level=logging.INFO, format='%(message)s')
 logger = logging.getLogger()
 
 make_dirs([OUTPUT_DIR])
 
+
 def go(project_id: str,
        pipeline_params: Dict,
        af_registry_location: Optional[str] = 'us-central1',
        af_registry_name: Optional[str] = 'vertex-mlops-af',
        base_image: Optional[str] = 'python:3.9-slim',
        cb_trigger_location: Optional[str] = 'us-central1',
        cb_trigger_name: Optional[str] = 'automlops-trigger',
@@ -102,14 +103,15 @@
              cloud_run_location, cloud_run_name, cloud_tasks_queue_location,
              cloud_tasks_queue_name, csr_branch_name, csr_name,
              custom_training_job_specs, gs_bucket_location, gs_bucket_name,
              pipeline_runner_sa, run_local, schedule_location,
              schedule_name, schedule_pattern, vpc_connector)
     run(run_local)
 
+
 def generate(project_id: str,
              pipeline_params: Dict,
              af_registry_location: Optional[str] = 'us-central1',
              af_registry_name: Optional[str] = 'vertex-mlops-af',
              base_image: Optional[str] = 'python:3.9-slim',
              cb_trigger_location: Optional[str] = 'us-central1',
              cb_trigger_name: Optional[str] = 'automlops-trigger',
@@ -153,14 +155,15 @@
         default_pipeline_runner_sa, run_local, schedule_location,
         schedule_name, schedule_pattern, vpc_connector)
 
     CloudBuildBuilder.build(af_registry_location, af_registry_name, cloud_run_location,
         cloud_run_name, default_pipeline_runner_sa, project_id,
         run_local, schedule_pattern, vpc_connector)
 
+
 def run(run_local: bool):
     """Builds, compiles, and submits the PipelineJob.
 
     Args:
         run_local: Flag that determines whether to use Cloud Run CI/CD.
     """
     # Build resources
@@ -176,14 +179,15 @@
         os.chdir('../')
     else:
         _push_to_csr()
 
     # Log generated resources
     _resources_generation_manifest(run_local)
 
+
 def _resources_generation_manifest(run_local: bool):
     """Logs urls of generated resources.
 
     Args:
         run_local: Flag that determines whether to use Cloud Run CI/CD.
     """
     defaults = read_yaml_file(GENERATED_DEFAULTS_FILE)
@@ -206,14 +210,15 @@
     if not run_local:
         logging.info(f'''Cloud Build Trigger: https://console.cloud.google.com/cloud-build/triggers;region={defaults['gcp']['cb_trigger_location']}''')
         logging.info(f'''Cloud Run Service: https://console.cloud.google.com/run/detail/{defaults['gcp']['cloud_run_location']}/{defaults['gcp']['cloud_run_name']}''')
         logging.info(f'''Cloud Tasks Queue: https://console.cloud.google.com/cloudtasks/queue/{defaults['gcp']['cloud_tasks_queue_location']}/{defaults['gcp']['cloud_tasks_queue_name']}/tasks''')
     if defaults['gcp']['cloud_schedule_pattern'] != 'No Schedule Specified':
         logging.info('Cloud Scheduler Job: https://console.cloud.google.com/cloudscheduler')
 
+
 def _push_to_csr():
     """Initializes a git repo if one doesn't already exist,
        then pushes to the specified branch and triggers the cloudbuild job.
     """
     defaults = read_yaml_file(GENERATED_DEFAULTS_FILE)
     csr_remote_origin_url = f'''https://source.developers.google.com/p/{defaults['gcp']['project_id']}/r/{defaults['gcp']['cloud_source_repository']}'''
 
@@ -244,14 +249,15 @@
     execute_process('git add .', to_null=False)
     execute_process('''git commit -m 'Run AutoMLOps' ''', to_null=False)
     execute_process(f'''git push origin {defaults['gcp']['cloud_source_repository_branch']} --force''', to_null=False)
     # pylint: disable=logging-fstring-interpolation
     logging.info(f'''Pushing code to {defaults['gcp']['cloud_source_repository_branch']} branch, triggering cloudbuild...''')
     logging.info(f'''Cloudbuild job running at: https://console.cloud.google.com/cloud-build/builds;region={defaults['gcp']['cb_trigger_location']}''')
 
+
 def component(func: Optional[Callable] = None,
               *,
               packages_to_install: Optional[List[str]] = None):
     """Decorator for Python-function based components in AutoMLOps.
 
     Example usage:
     from AutoMLOps import AutoMLOps
@@ -271,14 +277,15 @@
             component,
             packages_to_install=packages_to_install)
     else:
         return KfpScaffold.create_component_scaffold(
             func=func,
             packages_to_install=packages_to_install)
 
+
 def pipeline(func: Optional[Callable] = None,
              *,
              name: Optional[str] = None,
              description: Optional[str] = None):
     """Decorator for Python-function based pipelines in AutoMLOps.
 
     Example usage:
@@ -309,12 +316,13 @@
             description=description)
     else:
         return KfpScaffold.create_pipeline_scaffold(
             func=func,
             name=name,
             description=description)
 
+
 def clear_cache():
     """Deletes all temporary files stored in the cache directory."""
     execute_process(f'rm -rf {OUTPUT_DIR}', to_null=False)
     make_dirs([OUTPUT_DIR])
     logging.info('Cache cleared.')
```

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/__init__.py` & `google-cloud-automlops-1.1.5/AutoMLOps/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 import, with the end goal of becoming a Jupyter plugin to Vertex
 Workbench managed notebooks. The tool will generate yaml-component
 definitions, complete with Dockerfiles and requirements.txts for all
 Kubeflow components defined in a notebook. It will also generate a
 series of directories to support the creation of Vertex Pipelines.
 """
 # pylint: disable=invalid-name
-__version__ = '1.1.4'
+__version__ = '1.1.5'
 __author__ = 'Sean Rastatter'
 __credits__ = 'Google'
```

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/deployments/__init__.py` & `google-cloud-automlops-1.1.5/AutoMLOps/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/__init__.py` & `google-cloud-automlops-1.1.5/AutoMLOps/deployments/cloudbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/builder.py` & `google-cloud-automlops-1.1.5/AutoMLOps/deployments/cloudbuild/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from AutoMLOps.utils.utils import write_file
 from AutoMLOps.utils.constants import (
     BASE_DIR,
     GENERATED_CLOUDBUILD_FILE
 )
 from AutoMLOps.deployments.cloudbuild.constructs.scripts import CloudBuildScripts
 
+
 def build(af_registry_location: str,
           af_registry_name: str,
           cloud_run_location: str,
           cloud_run_name: str,
           pipeline_runner_sa: str,
           project_id: str,
           run_local: bool,
```

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/deployments/cloudbuild/constructs/scripts.py` & `google-cloud-automlops-1.1.5/AutoMLOps/deployments/cloudbuild/constructs/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 """Code strings for Cloudbuild scripts."""
 
 # pylint: disable=line-too-long
 
 from AutoMLOps.utils.constants import GENERATED_LICENSE
 
+
 class CloudBuildScripts():
     """Generates CloudBuild yaml config file."""
     def __init__(self,
                  af_registry_location: str,
                  af_registry_name: str,
                  cloud_run_location: str,
                  cloud_run_name: str,
```

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/__init__.py` & `google-cloud-automlops-1.1.5/AutoMLOps/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/base.py` & `google-cloud-automlops-1.1.5/AutoMLOps/frameworks/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 
 """Defines parent classes for a Component and Pipeline."""
 
 # pylint: disable=C0103
 # pylint: disable=line-too-long
 
 from typing import Dict, List
+
 from AutoMLOps.utils.utils import read_yaml_file
 
+
 class Component():
     """Parent class that defines a general abstraction of a Component."""
     def __init__(self, component_spec: dict, defaults_file: str):
         """Instantiate Component scripts object with all necessary attributes.
 
         Args:
             component_spec (dict): Dictionary of component specs including details
@@ -34,14 +36,15 @@
 
         # Parse defaults file for hidden class attributes
         defaults = read_yaml_file(defaults_file)
         self._af_registry_location = defaults['gcp']['af_registry_location']
         self._project_id = defaults['gcp']['project_id']
         self._af_registry_name = defaults['gcp']['af_registry_name']
 
+
 class Pipeline():
     """Parent class that defines a general abstraction of a Pipeline """
     def __init__(self, custom_training_job_specs: List[Dict], defaults_file: str):
         """Instantiate Pipeline scripts object with all necessary attributes.
 
         Args:
             custom_training_job_specs (List[Dict]): Specifies the specs to run the training job with.
```

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/__init__.py` & `google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/builder.py` & `google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     GENERATED_PARAMETER_VALUES_PATH
 )
 from AutoMLOps.frameworks.kfp.constructs.cloudrun import KfpCloudRun
 from AutoMLOps.frameworks.kfp.constructs.component import KfpComponent
 from AutoMLOps.frameworks.kfp.constructs.pipeline import KfpPipeline
 from AutoMLOps.frameworks.kfp.constructs.scripts import KfpScripts
 
+
 def build(project_id: str,
           pipeline_params: Dict,
           af_registry_location: Optional[str],
           af_registry_name: Optional[str],
           base_image: Optional[str],
           cb_trigger_location: Optional[str],
           cb_trigger_name: Optional[str],
@@ -137,14 +138,15 @@
     # Write requirements.txt to the component base directory
     write_file(f'{GENERATED_COMPONENT_BASE}/requirements.txt', kfp_scripts.requirements, 'w')
 
     # Build the cloud run files
     if not run_local:
         build_cloudrun()
 
+
 def build_component(component_path: str):
     """Constructs and writes component.yaml and {component_name}.py files.
         component.yaml: Contains the Kubeflow custom component definition.
         {component_name}.py: Contains the python code from the Jupyter cell.
 
     Args:
         component_path: Path to the temporary component yaml. This file
@@ -179,14 +181,15 @@
         f'''/pipelines/component/src/{component_spec['name']+'.py'}''']
 
     # Write license and component spec to the appropriate component.yaml file
     filename = component_dir + '/component.yaml'
     write_file(filename, GENERATED_LICENSE, 'w')
     write_yaml_file(filename, component_spec, 'a')
 
+
 def build_pipeline(custom_training_job_specs: List[Dict],
                    pipeline_parameter_values: dict):
     """Constructs and writes pipeline.py, pipeline_runner.py, and pipeline_parameter_values.json files.
         pipeline.py: Generates a Kubeflow pipeline spec from custom components.
         pipeline_runner.py: Sends a PipelineJob to Vertex AI using pipeline spec.
         pipeline_parameter_values.json: Provides runtime parameters for the PipelineJob.
 
@@ -219,14 +222,15 @@
     # Construct pipeline_runner.py
     write_file(pipeline_runner_file, kfp_pipeline.pipeline_runner, 'w+')
 
     # Construct pipeline_parameter_values.json
     serialized_params = json.dumps(pipeline_parameter_values, indent=4)
     write_file(pipeline_params_file, serialized_params, 'w+')
 
+
 def build_cloudrun():
     """Constructs and writes a Dockerfile, requirements.txt, and
        main.py to the cloud_run/run_pipeline directory. Also
        constructs and writes a main.py, requirements.txt, and
        pipeline_parameter_values.json to the
        cloud_run/queueing_svc directory.
     """
```

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/__init__.py` & `google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/cloudrun.py` & `google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/constructs/cloudrun.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     GENERATED_LICENSE,
     GENERATED_PIPELINE_JOB_SPEC_PATH,
     LEFT_BRACKET,
     PINNED_KFP_VERSION,
     RIGHT_BRACKET
 )
 
+
 class KfpCloudRun():
     """Generates files related to cloud runner service."""
     def __init__(self, defaults_file: str):
         """Instantiate Cloud Run scripts object with all necessary attributes.
 
         Args:
             defaults_file (str): Path to the default config variables yaml.
```

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/component.py` & `google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/constructs/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 # pylint: disable=line-too-long
 
 from AutoMLOps.utils.constants import GENERATED_LICENSE
 from AutoMLOps.utils.utils import is_using_kfp_spec
 from AutoMLOps.frameworks.base import Component
 
+
 class KfpComponent(Component):
     """Child class that generates files related to kfp components."""
     def __init__(self, component_spec: dict, defaults_file: str):
         """Instantiate Component scripts object with all necessary attributes.
 
         Args:
             component_spec (dict): Dictionary of component specs including details
```

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/pipeline.py` & `google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/constructs/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from typing import Dict, List
 
 from AutoMLOps.utils.utils import get_components_list, format_spec_dict
 from AutoMLOps.utils.constants import GENERATED_LICENSE
 from AutoMLOps.frameworks.base import Pipeline
 
+
 class KfpPipeline(Pipeline):
     """Child class that generates files related to kfp pipelines."""
     def __init__(self, custom_training_job_specs: List[Dict], defaults_file: str):
         """Instantiate Pipeline scripts object with all necessary attributes.
 
         Args:
             custom_training_job_specs (List[Dict]): Specifies the specs to run the training job with.
@@ -53,29 +54,27 @@
                 f'\n'
                 f'''    {newline_tab.join(f'{spec["component_spec"]}_job_op = create_custom_training_job_op_from_component(**{spec["component_spec"]}_custom_training_job_specs)' for spec in custom_training_job_specs)}'''
                 f'\n'
                 f'''    {newline_tab.join(f'{spec["component_spec"]} = partial({spec["component_spec"]}_job_op, project={quote}{self._project_id}{quote})' for spec in custom_training_job_specs)}'''        
                 f'\n')
         return custom_specs
 
-
     def _get_pipeline_imports(self):
         """Generates python code that imports modules and loads all custom components.
 
         Returns:
             str: Python pipeline_imports code.
         """
         components_list = get_components_list(full_path=False)
         gcpc_imports = (
             'from functools import partial\n'
             'from google_cloud_pipeline_components.v1.custom_job import create_custom_training_job_op_from_component\n')
         quote = '\''
         newline_tab = '\n    '
 
-
         # If there is a custom training job specified, write those to feed to pipeline imports
         custom_specs = self.custom_specs_helper(self._custom_training_job_specs)
 
         # Return standard code and customized specs
         return (
             f'''import argparse\n'''
             f'''import os\n'''
```

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/constructs/scripts.py` & `google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/constructs/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     GENERATED_PIPELINE_JOB_SPEC_PATH,
     LEFT_BRACKET,
     NEWLINE,
     PINNED_KFP_VERSION,
     RIGHT_BRACKET
 )
 
+
 class KfpScripts():
     """Generates files related to running kubeflow pipelines."""
     def __init__(self,
                  af_registry_location: str,
                  af_registry_name: str,
                  base_image: str,
                  cb_trigger_location: str,
```

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/frameworks/kfp/scaffold.py` & `google-cloud-automlops-1.1.5/AutoMLOps/frameworks/kfp/scaffold.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     update_params,
     write_file,
     write_yaml_file
 )
 
 T = TypeVar('T')
 
+
 def create_component_scaffold(func: Optional[Callable] = None,
                               *,
                               packages_to_install: Optional[List[str]] = None):
     """Creates a tmp component scaffold which will be used by the formalize function.
     Code is temporarily stored in component_spec['implementation']['container']['command'].
 
     Args:
@@ -73,14 +74,15 @@
                                                              '--function_to_execute', 
                                                              name]
     # Write component yaml
     filename = CACHE_DIR + f'/{name}.yaml'
     make_dirs([CACHE_DIR])
     write_yaml_file(filename, component_spec, 'w')
 
+
 def get_packages_to_install_command(func: Optional[Callable] = None,
                                     packages_to_install: Optional[List[str]] = None):
     """Returns a list of formatted list of commands, including code for tmp storage.
 
     Args:
         func: The python function to create a component from. The function
             should have type annotations for all its arguments, indicating how
@@ -99,14 +101,15 @@
         f'''fi{newline}'''
         f'''PIP_DISABLE_PIP_VERSION_CHECK=1 python3 -m pip install --quiet \{newline}'''
         f'''    --no-warn-script-location {concat_package_list} && "$0" "$@"{newline}'''
         f'''{newline}''')
     src_code = get_function_source_definition(func)
     return ['sh', '-c', install_python_packages_script, src_code]
 
+
 def get_function_parameters(func: Callable) -> dict:
     """Returns a formatted list of parameters.
 
     Args:
         func: The python function to create a component from. The function
             should have type annotations for all its arguments, indicating how
             it is intended to be used (e.g. as an input/output Artifact object,
@@ -133,14 +136,15 @@
         # pylint: disable=protected-access
         if metadata['type'] == inspect._empty:
             raise TypeError(
                 f'''Missing type hint for parameter "{metadata['name']}". '''
                 f'''Please specify the type for this parameter.''')
     return update_params(parameter_holder)
 
+
 def maybe_strip_optional_from_annotation(annotation: T) -> T:
     """Strips 'Optional' from 'Optional[<type>]' if applicable.
     For example::
         Optional[str] -> str
         str -> str
         List[int] -> List[int]
     Args:
@@ -149,14 +153,15 @@
         The type inside Optional[] if Optional exists, otherwise the original type.
     """
     if getattr(annotation, '__origin__', None) is Union and annotation.__args__[1] is type(None):
         return annotation.__args__[0]
     else:
         return annotation
 
+
 def create_pipeline_scaffold(func: Optional[Callable] = None,
                              *,
                              name: Optional[str] = None,
                              description: Optional[str] = None):
     """Creates a temporary pipeline scaffold which will
     be used by the formalize function.
 
@@ -170,14 +175,15 @@
     """
     pipeline_scaffold = (get_pipeline_decorator(name, description) +
                          get_function_source_definition(func) +
                          get_compile_step(func.__name__))
     make_dirs([CACHE_DIR]) # if it doesn't already exist
     write_file(PIPELINE_CACHE_FILE, pipeline_scaffold, 'w')
 
+
 def get_pipeline_decorator(name: Optional[str] = None,
                            description: Optional[str] = None):
     """Creates the kfp pipeline decorator.
 
     Args:
         name: The name of the pipeline.
         description: Short description of what the pipeline does.
@@ -187,14 +193,15 @@
     """
     default_name = DEFAULT_PIPELINE_NAME if not name else name
     name_str = f'''(\n    name='{default_name}',\n'''
     desc_str = f'''    description='{description}',\n''' if description else ''
     ending_str = ')\n'
     return '@dsl.pipeline' + name_str + desc_str + ending_str
 
+
 def get_compile_step(func_name: str):
     """Creates the compile function call.
 
     Args:
         func_name: The name of the pipeline function.
 
     Returns:
```

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/utils/__init__.py` & `google-cloud-automlops-1.1.5/AutoMLOps/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/utils/constants.py` & `google-cloud-automlops-1.1.5/AutoMLOps/utils/constants.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/AutoMLOps/utils/utils.py` & `google-cloud-automlops-1.1.5/AutoMLOps/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,26 +28,28 @@
 import yaml
 
 from AutoMLOps.utils.constants import (
     CACHE_DIR,
     PLACEHOLDER_IMAGE
 )
 
+
 def make_dirs(directories: list):
     """Makes directories with the specified names.
 
     Args:
         directories: Path of the directories to make.
     """
     for d in directories:
         try:
             os.makedirs(d)
         except FileExistsError:
             pass
 
+
 def read_yaml_file(filepath: str) -> dict:
     """Reads a yaml and returns file contents as a dict.
        Defaults to utf-8 encoding.
 
     Args:
         filepath: Path to the yaml.
     Returns:
@@ -59,14 +61,15 @@
         with open(filepath, 'r', encoding='utf-8') as file:
             file_dict = yaml.safe_load(file)
         file.close()
     except yaml.YAMLError as err:
         raise yaml.YAMLError(f'Error reading file. {err}') from err
     return file_dict
 
+
 def write_yaml_file(filepath: str, contents: dict, mode: str):
     """Writes a dictionary to yaml. Defaults to utf-8 encoding.
 
     Args:
         filepath: Path to the file.
         contents: Dictionary to be written to yaml.
         mode: Read/write mode to be used.
@@ -76,14 +79,15 @@
     try:
         with open(filepath, mode, encoding='utf-8') as file:
             yaml.safe_dump(contents, file, sort_keys=False)
         file.close()
     except yaml.YAMLError as err:
         raise yaml.YAMLError(f'Error writing to file. {err}') from err
 
+
 def read_file(filepath: str) -> str:
     """Reads a file and returns contents as a string.
        Defaults to utf-8 encoding.
 
     Args:
         filepath: Path to the file.
     Returns:
@@ -95,14 +99,15 @@
         with open(filepath, 'r', encoding='utf-8') as file:
             contents = file.read()
         file.close()
     except FileNotFoundError as err:
         raise FileNotFoundError(f'Error reading file. {err}') from err
     return contents
 
+
 def write_file(filepath: str, text: str, mode: str):
     """Writes a file at the specified path. Defaults to utf-8 encoding.
 
     Args:
         filepath: Path to the file.
         text: Text to be written to file.
         mode: Read/write mode to be used.
@@ -112,14 +117,15 @@
     try:
         with open(filepath, mode, encoding='utf-8') as file:
             file.write(text)
         file.close()
     except OSError as err:
         raise OSError(f'Error writing to file. {err}') from err
 
+
 def write_and_chmod(filepath: str, text: str):
     """Writes a file at the specified path and chmods the file
        to allow for execution.
 
     Args:
         filepath: Path to the file.
         text: Text to be written to file.
@@ -129,26 +135,28 @@
     write_file(filepath, text, 'w+')
     try:
         st = os.stat(filepath)
         os.chmod(filepath, st.st_mode | 0o111)
     except OSError as err:
         raise OSError(f'Error chmod-ing file. {err}') from err
 
+
 def delete_file(filepath: str):
     """Deletes a file at the specified path.
        If it does not exist, pass.
 
     Args:
         filepath: Path to the file.
     """
     try:
         os.remove(filepath)
     except OSError:
         pass
 
+
 def get_components_list(full_path: bool = True) -> list:
     """Reads yamls in the cache directory, verifies they are component
        yamls, and returns the name of the files.
 
     Args:
         full_path: Boolean; if false, stores only the filename w/o extension.
     Returns:
@@ -161,26 +169,28 @@
         if is_component_config(path):
             if full_path:
                 components_list.append(path)
             else:
                 components_list.append(os.path.basename(file).split('.')[0])
     return components_list
 
+
 def is_component_config(filepath: str) -> bool:
     """Checks to see if the given file is a component yaml.
 
     Args:
         filepath: Path to a yaml file.
     Returns:
         bool: Whether the given file is a component yaml.
     """
     required_keys = ['name','inputs','implementation']
     file_dict = read_yaml_file(filepath)
     return all(key in file_dict.keys() for key in required_keys)
 
+
 def execute_process(command: str, to_null: bool):
     """Executes an external shell process.
 
     Args:
         command: The string of the command to execute.
         to_null: Determines where to send output.
     Raises:
@@ -192,28 +202,30 @@
                        shell=True,
                        check=True,
                        stdout=stdout,
                        stderr=subprocess.STDOUT)
     except subprocess.CalledProcessError as err:
         raise RuntimeError(f'Error executing process. {err}') from err
 
+
 def validate_schedule(schedule_pattern: str, run_local: str):
     """Validates that the inputted schedule parameter aligns with the run_local configuration.
     Note: this function does not validate that schedule_pattern is a properly formatted cron value.
     Cron format validation is done in the backend by GCP.
     
     Args:
         schedule_pattern: Cron formatted value used to create a Scheduled retrain job.
         run_local: Flag that determines whether to use Cloud Run CI/CD.
     Raises:
         Exception: If schedule is not cron formatted or run_local validation fails.
     """
     if schedule_pattern != 'No Schedule Specified' and run_local:
         raise ValueError('run_local must be set to False to use Cloud Scheduler.')
 
+
 def update_params(params: list) -> list:
     """Converts the parameter types from Python types
        to Kubeflow types. Currently only supports
        Python primitive types.
 
     Args:
         params: Pipeline parameters. A list of dictionaries,
@@ -238,14 +250,15 @@
         try:
             param['type'] = python_kfp_types_mapper[param['type']]
         except KeyError as err:
             raise ValueError(f'Unsupported python type - we only support '
                              f'primitive types at this time. {err}') from err
     return params
 
+
 def get_function_source_definition(func: Callable) -> str:
     """Returns a formatted string of the source code.
 
     Args:
         func: The python function to create a component from. The function
             should have type annotations for all its arguments, indicating how
             it is intended to be used (e.g. as an input/output Artifact object,
@@ -263,14 +276,15 @@
     if not source_code_lines:
         raise ValueError(
             f'Failed to dedent and clean up the source of function "{func.__name__}". '
             f'It is probably not properly indented.')
 
     return '\n'.join(source_code_lines)
 
+
 def format_spec_dict(job_spec: dict) -> str:
     """Takes in a job spec dictionary and removes the quotes around the component op name. 
     e.g. 'component_spec': 'train_model' becomes 'component_spec': train_model.
     This is necessary to in order for the op to be callable within the Python code.
 
     Args:
         job_spec: Dictionary with job spec info.
@@ -284,14 +298,15 @@
     newline = '\n'
 
     return (
         f'''{left_bracket}\n'''
         f'''    {f'{newline}    '.join(f"   {quote}{k}{quote}: {quote if k != 'component_spec' else ''}{v}{quote if k != 'component_spec' else ''}," for k, v in job_spec.items())}{newline}'''
         f'''    {right_bracket}\n''')
 
+
 def is_using_kfp_spec(image: str):
     """Takes in an image string from a component yaml and determines if it came from kfp or not.
 
     Args:
         image: image string.
 
     Returns:
```

### Comparing `google-cloud-automlops-1.1.4/LICENSE` & `google-cloud-automlops-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/PKG-INFO` & `google-cloud-automlops-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-automlops
-Version: 1.1.4
+Version: 1.1.5
 Summary: AutoMLOps is a service that generates a production-style         MLOps pipeline from Jupyter Notebooks.
 Home-page: https://github.com/GoogleCloudPlatform/automlops
 Author: Sean Rastatter
 Author-email: srastatter@google.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `google-cloud-automlops-1.1.4/README.md` & `google-cloud-automlops-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/PKG-INFO` & `google-cloud-automlops-1.1.5/google_cloud_automlops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-automlops
-Version: 1.1.4
+Version: 1.1.5
 Summary: AutoMLOps is a service that generates a production-style         MLOps pipeline from Jupyter Notebooks.
 Home-page: https://github.com/GoogleCloudPlatform/automlops
 Author: Sean Rastatter
 Author-email: srastatter@google.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `google-cloud-automlops-1.1.4/google_cloud_automlops.egg-info/SOURCES.txt` & `google-cloud-automlops-1.1.5/google_cloud_automlops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/setup.py` & `google-cloud-automlops-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as file:
     readme_contents = file.read()
 
 setup(
     name='google-cloud-automlops',
-    version='1.1.4',
+    version='1.1.5',
     description='AutoMLOps is a service that generates a production-style \
         MLOps pipeline from Jupyter Notebooks.',
     long_description=readme_contents,
     long_description_content_type='text/markdown',
     url='https://github.com/GoogleCloudPlatform/automlops',
     author='Sean Rastatter',
     author_email='srastatter@google.com',
     license='Apache-2.0',
     packages=find_packages(),
     install_requires=['docopt==0.6.2',
                       'docstring-parser==0.15',
                       'pipreqs==0.4.11',
-                      'PyYAML==5.4.1',
+                      'PyYAML==6.0.1',
                       'yarg==0.1.9'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS :: MacOS X',
```

### Comparing `google-cloud-automlops-1.1.4/tests/__init__.py` & `google-cloud-automlops-1.1.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/tests/unit/__init__.py` & `google-cloud-automlops-1.1.5/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/tests/unit/deployments/__init__.py` & `google-cloud-automlops-1.1.5/tests/unit/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/tests/unit/frameworks/__init__.py` & `google-cloud-automlops-1.1.5/tests/unit/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/tests/unit/frameworks/base_test.py` & `google-cloud-automlops-1.1.5/tests/unit/frameworks/base_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         {
             'af_registry_location': 'us-central1',
             'project_id': 'my_project',
             'af_registry_name': 'my_af_registry'
         }
     }
 
+
 @pytest.fixture(name='defaults_dict', params=[DEFAULTS1, DEFAULTS2])
 def fixture_defaults_dict(request: pytest.FixtureRequest, tmpdir: pytest.FixtureRequest):
     """Writes temporary yaml file fixture using defaults parameterized
     dictionaries during pytest session scope.
 
     Args:
         request: Pytest fixture special object that provides information
@@ -57,14 +58,15 @@
     Returns:
         str: Path of yaml file.
     """
     yaml_path = tmpdir.join('test.yaml')
     write_yaml_file(yaml_path, request.param, 'w')
     return {'path': yaml_path, 'vals': request.param}
 
+
 @pytest.mark.parametrize(
     'component_spec',
     [{'test1': 'val1'}, {'test2': 'val2'}]
 )
 def test_Component(defaults_dict: pytest.FixtureRequest, component_spec: dict):
     """Tests the Component base class, the parent class that defines a general
     abstraction of a Component.
@@ -79,14 +81,15 @@
 
     my_component = Component(component_spec=component_spec, defaults_file=path)
     assert my_component._af_registry_location == defaults['gcp']['af_registry_location']
     assert my_component._af_registry_name == defaults['gcp']['af_registry_name']
     assert my_component._project_id == defaults['gcp']['project_id']
     assert my_component._component_spec == component_spec
 
+
 @pytest.mark.parametrize(
     'custom_training_job_specs',
     [
         [{'component_spec': 'mycomp1', 'other': 'myother'}],
         [
             {
                 'component_spec': 'train_model',
```

### Comparing `google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/__init__.py` & `google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/builder_test.py` & `google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/builder_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,15 @@
                 '--function_to_execute',
                 'create_dataset',
             ],
         }
     },
 }
 
+
 @pytest.fixture(name='temp_yaml_dict', params=[TEMP_YAML])
 def fixture_temp_yaml_dict(request: pytest.FixtureRequest, tmpdir: pytest.FixtureRequest):
     """Writes temporary yaml file fixture using defaults parameterized
     dictionaries during pytest session scope.
 
     Args:
         request: Pytest fixture special object that provides information
@@ -95,14 +96,15 @@
     Returns:
         dict: Path of yaml file and dictionary it contains.
     """
     yaml_path = tmpdir.join('test.yaml')
     write_yaml_file(yaml_path, request.param, 'w')
     return {'path': yaml_path, 'vals': request.param}
 
+
 @pytest.fixture(name='defaults_dict', params=[DEFAULTS])
 def fixture_defaults_dict(request: pytest.FixtureRequest, tmpdir: pytest.FixtureRequest):
     """Writes temporary yaml file fixture using defaults parameterized
     dictionaries during pytest session scope.
 
     Args:
         request: Pytest fixture special object that provides information
@@ -113,14 +115,15 @@
     Returns:
         dict: Path of yaml file and dictionary it contains.
     """
     yaml_path = tmpdir.join('defaults.yaml')
     write_yaml_file(yaml_path, request.param, 'w')
     return {'path': yaml_path, 'vals': request.param}
 
+
 @pytest.fixture(name='expected_component_dict')
 def fixture_expected_component_dict():
     """Creates the expected component dictionary, which is the temporary yaml
     file with a change to the implementation key.
 
     Returns:
         dict: Expected component dictionary generated from the component
@@ -137,14 +140,15 @@
                 '--function_to_execute',
                 'create_dataset',
             ],
         }
     }
     return expected
 
+
 def test_build_component(mocker: pytest_mock.MockerFixture,
                          tmpdir: pytest.FixtureRequest,
                          temp_yaml_dict: pytest.FixtureRequest,
                          defaults_dict: pytest.FixtureRequest,
                          expected_component_dict: pytest.FixtureRequest):
     """Tests build_component, which Constructs and writes component.yaml and
     {component_name}.py files.
@@ -175,14 +179,15 @@
     assert os.path.exists(f'{tmpdir}/components/{component_name}/component.yaml')
     assert os.path.exists(f'{tmpdir}/components/component_base/src/{component_name}.py')
 
     # Load component.yaml file and compare to the expected output in test_data
     created_component_dict = read_yaml_file(f'{tmpdir}/components/{component_name}/component.yaml')
     assert created_component_dict == expected_component_dict
 
+
 @pytest.mark.parametrize(
     'custom_training_job_specs, pipeline_parameter_values',
     [
         (
             [{'component_spec': 'mycomp1', 'other': 'myother'}],
             {
                 'bq_table': 'automlops-sandbox.test_dataset.dry-beans',
```

### Comparing `google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/__init__.py` & `google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/cloudrun_test.py` & `google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/constructs/cloudrun_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
             'gs_bucket_name': 'automlops-sandbox-bucket',
             'pipeline_runner_service_account': 'vertex-pipelines@automlops-sandbox.iam.gserviceaccount.com',
             'project_id': 'automlops-sandbox',
             'vpc_connector': 'No VPC Specified'
         }
     }
 
+
 @pytest.fixture(name='defaults_dict', params=[DEFAULTS1, DEFAULTS2])
 def fixture_defaults_dict(request: pytest.FixtureRequest, tmpdir: pytest.FixtureRequest):
     """Writes temporary yaml file fixture using defaults parameterized
     dictionaries during pytest session scope.
 
     Args:
         request: Pytest fixture special object that provides information
@@ -91,14 +92,15 @@
     Returns:
         dict: Path of yaml file and dictionary it contains.
     """
     yaml_path = tmpdir.join('test.yaml')
     write_yaml_file(yaml_path, request.param, 'w')
     return {'path': yaml_path, 'vals': request.param}
 
+
 def test_KfpCloudRun(defaults_dict: pytest.FixtureRequest):
     """Tests the KFP Cloud Run class.
     
     Args:
         defaults_dict: Locally defined defaults_dict Pytest fixture.
     """
     path = defaults_dict['path']
```

### Comparing `google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/component_test.py` & `google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/constructs/component_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
                 {
                     'command': 'echo hi',
                     'image': 'AutoMLOps_image_tbd'
                 }
         }
 }
 
+
 @pytest.fixture(name='defaults_dict', params=[DEFAULTS1, DEFAULTS2])
 def fixture_defaults_dict(request: pytest.FixtureRequest, tmpdir: pytest.FixtureRequest):
     """Writes temporary yaml file fixture using defaults parameterized
     dictionaries during pytest session scope.
 
     Args:
         request: Pytest fixture special object that provides information
@@ -79,14 +80,15 @@
     Returns:
         dict: Path of yaml file and dictionary it contains
     """
     yaml_path = tmpdir.join('test.yaml')
     write_yaml_file(yaml_path, request.param, 'w')
     return {'path': yaml_path, 'vals': request.param}
 
+
 @pytest.mark.parametrize(
     'component_spec',
     [COMPONENT_SPEC1, COMPONENT_SPEC2]
 )
 def test_KfpComponent(component_spec: dict, defaults_dict: pytest.FixtureRequest):
     """Tests the KFP child class that generates files related to KFP components.
```

### Comparing `google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/pipeline_test.py` & `google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/constructs/pipeline_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         {
             'af_registry_location': 'us-central1',
             'project_id': 'my_project',
             'af_registry_name': 'my_af_registry'
         }
     }
 
+
 @pytest.fixture(name='defaults_dict', params=[DEFAULTS1, DEFAULTS2])
 def fixture_defaults_dict(request: pytest.FixtureRequest, tmpdir: pytest.FixtureRequest):
     """Writes temporary yaml file fixture using defaults parameterized
     dictionaries during pytest session scope.
 
     Args:
         request: Pytest fixture special object that provides information
@@ -61,14 +62,15 @@
     Returns:
         dict: Path of yaml file and dictionary it contains.
     """
     yaml_path = tmpdir.join('test.yaml')
     write_yaml_file(yaml_path, request.param, 'w')
     return {'path': yaml_path, 'vals': request.param}
 
+
 @pytest.mark.parametrize(
     'custom_training_job_specs',
     [
         [{'component_spec': 'mycomp1', 'other': 'myother'}],
         [
             {
                 'component_spec': 'train_model',
```

### Comparing `google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/constructs/scripts_test.py` & `google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/constructs/scripts_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from AutoMLOps.utils.constants import (
     GENERATED_LICENSE,
     LEFT_BRACKET,
     NEWLINE,
     RIGHT_BRACKET
 )
 
+
 @pytest.mark.parametrize(
     '''af_registry_location, af_registry_name, base_image, cb_trigger_location,'''
     '''cb_trigger_name, cloud_run_location, cloud_run_name, cloud_tasks_queue_location,'''
     '''cloud_tasks_queue_name, csr_branch_name, csr_name, gs_bucket_location,'''
     '''gs_bucket_name, pipeline_runner_sa, project_id, run_local, schedule_location,'''
     '''schedule_name, schedule_pattern, base_dir, vpc_connector, reqs''',
     [
```

### Comparing `google-cloud-automlops-1.1.4/tests/unit/frameworks/kfp/scaffold_test.py` & `google-cloud-automlops-1.1.5/tests/unit/frameworks/kfp/scaffold_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,38 +32,42 @@
     get_function_parameters,
     get_pipeline_decorator,
 )
 from AutoMLOps.utils.constants import DEFAULT_PIPELINE_NAME
 import AutoMLOps.utils.utils
 from AutoMLOps.utils.utils import get_function_source_definition, read_yaml_file
 
+
 def add(a: int, b: int):
     """Testing
 
     Args:
         a (int): Integer a
         b (int): Integer b
 
     Returns:
         int: Sum of a and b
     """
     return a + b
 
+
 def sub(a, b):
     return a - b
 
+
 def div(a: float, b: float):
     """Testing
 
     Args:
         a (float): Float a
         b (float): Float b
     """
     return a/b
 
+
 @pytest.mark.parametrize(
     'func, packages_to_install, expectation',
     [
         (add, None, does_not_raise()),
         (add, ['pandas', 'pytest'], does_not_raise()),
         (sub, None, pytest.raises(TypeError))
     ]
@@ -97,14 +101,15 @@
         assert list(component_spec['implementation'].keys()) == ['container']
         assert list(component_spec['implementation']['container'].keys()) == ['image', 'command', 'args']
 
         # Remove temporary files
         os.remove(func_path)
         os.rmdir('.AutoMLOps-cache')
 
+
 @pytest.mark.parametrize(
     'func, packages_to_install',
     [
         (add, None),
         (add, ['pandas']),
         (sub, ['pandas', 'kfp', 'pytest'])
     ]
@@ -129,14 +134,15 @@
         f'''    python3 -m ensurepip || python3 -m ensurepip --user || apt-get install python3-pip{newline}'''
         f'''fi{newline}'''
         f'''PIP_DISABLE_PIP_VERSION_CHECK=1 python3 -m pip install --quiet \{newline}'''
         f'''    --no-warn-script-location {' '.join([repr(str(package)) for package in packages_to_install])} && "$0" "$@"{newline}'''
         f'''{newline}''')
     assert get_packages_to_install_command(func, packages_to_install) == ['sh', '-c', install_python_packages_script, get_function_source_definition(func=func)]
 
+
 @pytest.mark.parametrize(
     'func, params, expectation',
     [
         (
             add,
             [
                 {'description': 'Integer a', 'name': 'a', 'type': 'Integer'},
@@ -171,14 +177,15 @@
         params (List[dict]): Params list with types converted to kubeflow spec.
         expectation: Any corresponding expected errors for each
             set of parameters.
     """
     with expectation:
         assert params == get_function_parameters(func=func)
 
+
 @pytest.mark.parametrize(
     'func, name, description',
     [
         (add, 'Add', 'This is a test'),
         (sub, 'Sub', 'Test 2'),
         (div, None, None)
     ]
@@ -201,14 +208,15 @@
     create_pipeline_scaffold(func=func, name=name, description=description)
     fold = '.AutoMLOps-cache'
     file_path = 'pipeline_scaffold.py'
     assert os.path.exists(os.path.join(fold, file_path))
     os.remove(os.path.join(fold, file_path))
     os.rmdir(fold)
 
+
 @pytest.mark.parametrize(
     'name, description',
     [
         ('Name1', 'Description1'),
         ('Name2', 'Description2'),
         (None, None),
     ]
@@ -225,14 +233,15 @@
         f'''@dsl.pipeline'''
         f'''(\n    name='{DEFAULT_PIPELINE_NAME if not name else name}',\n'''
         f'''{desc_str}'''
         f''')\n'''
     )
     assert decorator == get_pipeline_decorator(name=name, description=description)
 
+
 @pytest.mark.parametrize(
     'func_name',
     ['func1', 'func2']
 )
 def test_get_compile_step(func_name: str):
     """Tests get_compile_step, which creates the compile function call.
```

### Comparing `google-cloud-automlops-1.1.4/tests/unit/utils/__init__.py` & `google-cloud-automlops-1.1.5/tests/unit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.1.4/tests/unit/utils/utils_test.py` & `google-cloud-automlops-1.1.5/tests/unit/utils/utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,27 +40,37 @@
     update_params,
     validate_schedule,
     write_and_chmod,
     write_file,
     write_yaml_file
 )
 
+
 # Define simple functions to be used in tests
 def func1(x):
     return x + 1
+
+
 def func2(x, y):
     return x + y
+
+
 def func3(x, y, z):
     return x + y + z
+
+
 def func4():
+
     def inner_func():
         res = 1 + 1
         return res
+
     return inner_func()
 
+
 @pytest.mark.parametrize(
     'directories, existance, expectation',
     [
         (['dir1', 'dir2'], [True, True], does_not_raise()),
         (['dir1', 'dir1'], [True, False], does_not_raise()),
         (['\0', 'dir1'], [True, True], pytest.raises(ValueError))
     ]
@@ -81,14 +91,15 @@
     with expectation:
         make_dirs(directories=directories)
         for directory, exist in zip(directories, existance):
             assert os.path.exists(directory) == exist
             if exist:
                 os.rmdir(directory)
 
+
 @pytest.mark.parametrize(
     'filepath, content1, content2, expectation',
     [
         (
             'test.yaml',
             {'key1': 'value1', 'key2': 'value2'},
             None,
@@ -122,14 +133,15 @@
             yaml.dump(content1, file)
         if content2:
             yaml.dump(content2, file)
     with expectation:
         assert read_yaml_file(filepath=filepath) == content1
     os.remove(path=filepath)
 
+
 @pytest.mark.parametrize(
     'filepath, mode, expectation',
     [
         ('test.yaml', 'w', does_not_raise()),
         ('/nonexistent/directory', 'w',  pytest.raises(FileNotFoundError)),
         ('test.yaml', 'r', pytest.raises(IOError))
     ]
@@ -154,14 +166,15 @@
             contents=contents,
             mode=mode
         )
         with open(file=filepath, mode='r', encoding='utf-8') as file:
             assert yaml.safe_load(file) == contents
         os.remove(path=filepath)
 
+
 @pytest.mark.parametrize(
     'filepath, text, write_file_bool, expectation',
     [
         ('test.txt', 'This is a text file.', True, does_not_raise()),
         ('fail', '', False, pytest.raises(FileNotFoundError))
     ]
 )
@@ -184,14 +197,15 @@
         with open(file=filepath, mode='w', encoding='utf-8') as file:
             file.write(text)
     with expectation:
         assert read_file(filepath=filepath) == text
     if os.path.exists(filepath):
         os.remove(filepath)
 
+
 @pytest.mark.parametrize(
     'filepath, text, mode, expectation',
     [
         ('test.txt', 'This is a test file.', 'w', does_not_raise()),
         (15, 'This is a test file.', 'w', pytest.raises(OSError))
     ]
 )
@@ -216,14 +230,15 @@
             mode=mode
         )
         assert os.path.exists(filepath)
         with open(file=filepath, mode='r', encoding='utf-8') as file:
             assert text == file.read()
         os.remove(filepath)
 
+
 def test_write_and_chmod():
     """Tests write_and_chmod, which writes a file at the specified path
     and chmods the file to allow for execution.
     """
     # Create a file.
     with open(file='test.txt', mode='w', encoding='utf-8') as file:
         file.write('This is a test file.')
@@ -237,14 +252,15 @@
 
     # Assert that the contents of the file are correct.
     with open(file='test.txt', mode='r', encoding='utf-8') as file:
         contents = file.read()
     assert contents == 'This is a test file.'
     os.remove('test.txt')
 
+
 @pytest.mark.parametrize(
     'file_to_delete, valid_file',
     [
         ('test.txt', True),
         ('fake.txt', False)
     ]
 )
@@ -262,14 +278,15 @@
             delete_file(file_to_delete)
     else:
         with open(file=file_to_delete, mode='w', encoding='utf-8') as file:
             file.write('This is a test file.')
             delete_file(file_to_delete)
             assert not os.path.exists(file_to_delete)
 
+
 @pytest.mark.parametrize(
     'comp_path, comp_name, patch_cwd, expectation',
     [
         (['component.yaml'], ['component'], True, does_not_raise()),
         ([], [], True, does_not_raise()),
         (['component.yaml'], ['component'], False, pytest.raises(FileNotFoundError))
     ]
@@ -310,14 +327,15 @@
     with expectation:
         assert get_components_list(full_path=False) == comp_name
         assert get_components_list(full_path=True) == [os.path.join('.', file) for file in comp_path]
     for file in comp_path:
         if os.path.exists(file):
             os.remove(file)
 
+
 @pytest.mark.parametrize(
     'yaml_contents, expectation',
     [
         (
             {
                 'name': 'value1',
                 'inputs': 'value2',
@@ -345,14 +363,15 @@
         expected (bool): Expectation of whether or not the configuration is valid.
     """
     with open(file='component.yaml', mode='w', encoding='utf-8') as f:
         yaml.dump(yaml_contents, f)
     assert expectation == is_component_config('component.yaml')
     os.remove('component.yaml')
 
+
 @pytest.mark.parametrize(
     'command, to_null, expectation',
     [
         ('touch test.txt', False, False),
         ('not a real command', False, True),
         ('echo "howdy"', True, False)
     ]
@@ -374,14 +393,15 @@
     elif to_null:
         assert execute_process(command=command, to_null=to_null) is None
     else:
         execute_process(command=command, to_null=to_null)
         assert os.path.exists('test.txt')
         os.remove('test.txt')
 
+
 @pytest.mark.parametrize(
     'sch_pattern, run_local, expectation',
     [
         ('No Schedule Specified', True, does_not_raise()),
         ('No Schedule Specified', False, does_not_raise()),
         ('Schedule', True, pytest.raises(ValueError)),
         ('Schedule', False, does_not_raise())
@@ -396,14 +416,15 @@
         sch_pattern (str): Cron formatted value used to create a Scheduled retrain job.
         run_local (bool): Flag that determines whether to use Cloud Run CI/CD.
         expectation: Any corresponding expected errors for each set of parameters.
     """
     with expectation:
         validate_schedule(schedule_pattern=sch_pattern, run_local=run_local)
 
+
 @pytest.mark.parametrize(
     'params, expected_output',
     [
         ([{'name': 'param1', 'type': int}], [{'name': 'param1', 'type': 'Integer'}]),
         ([{'name': 'param2', 'type': str}], [{'name': 'param2', 'type': 'String'}]),
         ([{'name': 'param3', 'type': float}], [{'name': 'param3', 'type': 'Float'}]),
         ([{'name': 'param4', 'type': bool}], [{'name': 'param4', 'type': 'Bool'}]),
@@ -426,33 +447,35 @@
     """
     if expected_output is not None:
         assert expected_output == update_params(params=params)
     else:
         with pytest.raises(ValueError):
             assert update_params(params=params)
 
+
 @pytest.mark.parametrize(
     'func, expected_output',
     [
         (func1, 'def func1(x):\n    return x + 1\n'),
         (func2, 'def func2(x, y):\n    return x + y\n'),
         (func3, 'def func3(x, y, z):\n    return x + y + z\n'),
-        (func4, 'def func4():\n    def inner_func():\n        res = 1 + 1\n        return res\n    return inner_func()\n')
+        (func4, 'def func4():\n\n    def inner_func():\n        res = 1 + 1\n        return res\n\n    return inner_func()\n')
     ]
 )
 def test_get_function_source_definition(func: Callable, expected_output: str):
     """Tests get_function_source_definition, which returns a formatted string of
     the source code.
 
     Args:
         func (Callable): Function to pull source definition from.
         expected_output (str): Expected source definition of the given function.
     """
     assert expected_output == get_function_source_definition(func=func)
 
+
 @pytest.mark.parametrize(
     'job_spec, expected_output',
     [
         (
             {'component_spec': 'train_model'},
             '''{\n       'component_spec': train_model,\n    }\n'''
         ),
```

