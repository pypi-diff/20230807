# Comparing `tmp/ecs_composex_msk_cluster-0.3.1.tar.gz` & `tmp/ecs_composex_msk_cluster-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_composex_msk_cluster-0.3.1.tar", max compression
+gzip compressed data, was "ecs_composex_msk_cluster-0.3.2.tar", max compression
```

## Comparing `ecs_composex_msk_cluster-0.3.1.tar` & `ecs_composex_msk_cluster-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0    16725 2022-04-24 10:25:44.149879 ecs_composex_msk_cluster-0.3.1/LICENSE
--rw-r--r--   0        0        0      392 2022-04-24 10:25:44.055880 ecs_composex_msk_cluster-0.3.1/MANIFEST.in
--rw-r--r--   0        0        0     1165 2023-03-16 20:50:05.293054 ecs_composex_msk_cluster-0.3.1/README.rst
--rw-r--r--   0        0        0      170 2023-04-10 21:43:06.725304 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/__init__.py
--rw-r--r--   0        0        0     6556 2023-01-12 10:42:26.973223 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster.py
--rw-r--r--   0        0        0     1064 2022-11-21 21:44:03.087655 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_conditions.py
--rw-r--r--   0        0        0     1114 2022-11-21 21:44:03.103654 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_ecs.py
--rw-r--r--   0        0        0     7943 2022-11-21 21:44:03.104655 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_ecs_iam.py
--rw-r--r--   0        0        0     2816 2023-03-11 22:46:19.588524 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_logging.py
--rw-r--r--   0        0        0      501 2022-11-21 21:44:03.144654 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_module.py
--rw-r--r--   0        0        0     2843 2023-04-10 21:42:45.826048 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_params.py
--rw-r--r--   0        0        0      212 2023-04-10 21:43:07.170309 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_perms.json
--rw-r--r--   0        0        0     1731 2022-11-21 21:44:03.163654 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_stack.py
--rw-r--r--   0        0        0     9535 2023-04-10 21:42:45.826048 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_template.py
--rw-r--r--   0        0        0     1401 2022-11-21 21:44:03.186653 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_configuration.py
--rw-r--r--   0        0        0     8504 2023-03-11 22:44:53.532492 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_sg_ingress.py
--rw-r--r--   0        0        0     3144 2022-11-21 21:44:03.188653 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_storage_scaling.py
--rw-r--r--   0        0        0     8392 2023-04-10 21:43:07.170309 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/x-msk_cluster.spec.json
--rw-r--r--   0        0        0     2329 2023-04-10 21:43:06.725304 ecs_composex_msk_cluster-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1924 1970-01-01 00:00:00.000000 ecs_composex_msk_cluster-0.3.1/setup.py
--rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 ecs_composex_msk_cluster-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    16725 2022-04-24 10:25:44.149879 ecs_composex_msk_cluster-0.3.2/LICENSE
+-rw-r--r--   0        0        0      392 2022-04-24 10:25:44.055880 ecs_composex_msk_cluster-0.3.2/MANIFEST.in
+-rw-r--r--   0        0        0     1165 2023-03-16 20:50:05.293054 ecs_composex_msk_cluster-0.3.2/README.rst
+-rw-r--r--   0        0        0      170 2023-08-07 19:49:58.250573 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/__init__.py
+-rw-r--r--   0        0        0     6556 2023-01-12 10:42:26.973223 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster.py
+-rw-r--r--   0        0        0     1064 2022-11-21 21:44:03.087655 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_conditions.py
+-rw-r--r--   0        0        0     1114 2022-11-21 21:44:03.103654 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_ecs.py
+-rw-r--r--   0        0        0     7943 2022-11-21 21:44:03.104655 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_ecs_iam.py
+-rw-r--r--   0        0        0     2816 2023-03-11 22:46:19.588524 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_logging.py
+-rw-r--r--   0        0        0      501 2022-11-21 21:44:03.144654 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_module.py
+-rw-r--r--   0        0        0     2843 2023-04-10 21:42:45.826048 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_params.py
+-rw-r--r--   0        0        0      212 2023-08-07 19:49:58.804580 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_perms.json
+-rw-r--r--   0        0        0     1731 2022-11-21 21:44:03.163654 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_stack.py
+-rw-r--r--   0        0        0     9535 2023-04-10 21:42:45.826048 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_template.py
+-rw-r--r--   0        0        0     1401 2022-11-21 21:44:03.186653 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_configuration.py
+-rw-r--r--   0        0        0     8504 2023-03-11 22:44:53.532492 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_sg_ingress.py
+-rw-r--r--   0        0        0     3144 2022-11-21 21:44:03.188653 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_storage_scaling.py
+-rw-r--r--   0        0        0     8392 2023-08-07 19:49:58.805580 ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/x-msk_cluster.spec.json
+-rw-r--r--   0        0        0     2323 2023-08-07 19:49:58.250573 ecs_composex_msk_cluster-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 ecs_composex_msk_cluster-0.3.2/PKG-INFO
```

### Comparing `ecs_composex_msk_cluster-0.3.1/LICENSE` & `ecs_composex_msk_cluster-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.1/README.rst` & `ecs_composex_msk_cluster-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster.py` & `ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_conditions.py` & `ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_conditions.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_ecs.py` & `ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_ecs_iam.py` & `ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_ecs_iam.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_logging.py` & `ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_logging.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_params.py` & `ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_stack.py` & `ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_template.py` & `ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_cluster_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_configuration.py` & `ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_configuration.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_sg_ingress.py` & `ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_sg_ingress.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_storage_scaling.py` & `ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/msk_storage_scaling.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/x-msk_cluster.spec.json` & `ecs_composex_msk_cluster-0.3.2/ecs_composex_msk_cluster/x-msk_cluster.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.1/pyproject.toml` & `ecs_composex_msk_cluster-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecs_composex_msk_cluster"
-version = "0.3.1"
+version = "0.3.2"
 description = "msk_cluster - AWS MSK Cluster module for ECS Compose-X"
 authors = ["johnpreston <john@compose-x.io>"]
 license = "MPL-2.0"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
@@ -26,15 +26,15 @@
   "NOTICES.rst",
   "ecs_composex/**/*.json"
 ]
 exclude = ["*.pyc", "*~", "*pycache*"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-ecs_composex = "^0.23.7"
+ecs_composex = "^0.23.19"
 compose-x-common = "^1.2"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3"
 isort = "^5.9.3"
 coverage = "^7.0"
 pytest = "^7.2"
@@ -76,15 +76,15 @@
   "*/cli.py"
 ]
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/ecs_composex_msk_cluster"
 
 [tool.tbump.version]
-current = "0.3.1"
+current = "0.3.2"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
@@ -103,9 +103,9 @@
 
 [[tool.tbump.before_commit]]
 name = "Files format"
 cmd = "make conform"
 
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ecs_composex_msk_cluster-0.3.1/PKG-INFO` & `ecs_composex_msk_cluster-0.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecs-composex-msk-cluster
-Version: 0.3.1
+Version: 0.3.2
 Summary: msk_cluster - AWS MSK Cluster module for ECS Compose-X
 License: MPL-2.0
 Author: johnpreston
 Author-email: john@compose-x.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,20 +14,16 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: compose-x-common (>=1.2,<2.0)
-Requires-Dist: ecs_composex (>=0.23.7,<0.24.0)
+Requires-Dist: ecs_composex (>=0.23.19,<0.24.0)
 Project-URL: Compose-X Labs, https://labs.compose-x.io/
 Project-URL: Compose-X Blog, https://blog.compose-x.io/
 Project-URL: ECS ComposeX, https://github.com/compose-x/ecs_composex/
 Description-Content-Type: text/x-rst
 
 
 .. meta::
```

