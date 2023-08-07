# Comparing `tmp/tutor-contrib-k8s-deploy-tasks-15.0.0.tar.gz` & `tmp/tutor-contrib-k8s-deploy-tasks-15.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-k8s-deploy-tasks-15.0.0.tar", last modified: Sat Jun 17 16:10:36 2023, max compression
+gzip compressed data, was "tutor-contrib-k8s-deploy-tasks-15.0.1.tar", last modified: Mon Aug  7 19:21:49 2023, max compression
```

## Comparing `tutor-contrib-k8s-deploy-tasks-15.0.0.tar` & `tutor-contrib-k8s-deploy-tasks-15.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.072049 tutor-contrib-k8s-deploy-tasks-15.0.0/
--rw-r--r--   0 mcdaniel   (501) staff       (20)      102 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/MANIFEST.in
--rw-r--r--   0 mcdaniel   (501) staff       (20)     3955 2023-06-17 16:10:36.072146 tutor-contrib-k8s-deploy-tasks-15.0.0/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2694 2023-06-17 16:09:28.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/README.rst
--rw-r--r--   0 mcdaniel   (501) staff       (20)      278 2023-06-17 14:35:54.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/pyproject.toml
--rw-r--r--   0 mcdaniel   (501) staff       (20)       67 2023-06-17 16:10:36.072515 tutor-contrib-k8s-deploy-tasks-15.0.0/setup.cfg
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2118 2023-06-17 16:05:49.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/setup.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.068588 tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/
--rw-r--r--   0 mcdaniel   (501) staff       (20)     3955 2023-06-17 16:10:35.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)     1177 2023-06-17 16:10:36.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/SOURCES.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-06-17 16:10:35.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/dependency_links.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       66 2023-06-17 16:10:35.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/entry_points.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       22 2023-06-17 16:10:35.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/requires.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       27 2023-06-17 16:10:35.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/top_level.txt
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.069271 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/
--rw-r--r--   0 mcdaniel   (501) staff       (20)       23 2023-06-17 13:31:26.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/__about__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/__init__.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.070101 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/patches/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/patches/.gitignore
--rw-r--r--   0 mcdaniel   (501) staff       (20)      915 2023-06-15 18:15:08.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/patches/openedx-common-settings
--rw-r--r--   0 mcdaniel   (501) staff       (20)     3066 2023-06-15 18:22:20.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/patches/openedx-lms-production-settings
--rw-r--r--   0 mcdaniel   (501) staff       (20)     7845 2023-06-17 14:27:24.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/plugin.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.065430 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.065754 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.070466 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/apps/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/apps/.gitignore
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.070649 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/build/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/build/.gitignore
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.065835 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.070825 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-17 13:31:26.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/.gitignore
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.071003 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/cms/
--rw-r--r--   0 mcdaniel   (501) staff       (20)       71 2023-06-17 13:31:26.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/cms/nutmeg_deploy_tasks
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.071612 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2895 2023-06-17 13:31:26.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/fix_oauth_redirect_uris
--rw-r--r--   0 mcdaniel   (501) staff       (20)       74 2023-06-17 13:31:26.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/nutmeg_deploy_tasks
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.071842 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/mysql/
--rw-r--r--   0 mcdaniel   (501) staff       (20)      472 2023-06-17 13:31:26.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/mysql/add_user_profiles
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 19:21:49.838937 tutor-contrib-k8s-deploy-tasks-15.0.1/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      102 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/MANIFEST.in
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     3714 2023-08-07 19:21:49.838989 tutor-contrib-k8s-deploy-tasks-15.0.1/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2728 2023-08-07 14:27:09.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/README.rst
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     1923 2023-08-07 19:20:41.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/pyproject.toml
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       67 2023-08-07 19:21:49.839184 tutor-contrib-k8s-deploy-tasks-15.0.1/setup.cfg
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2090 2023-08-07 14:48:27.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/setup.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 19:21:49.836336 tutor-contrib-k8s-deploy-tasks-15.0.1/tutor_contrib_k8s_deploy_tasks.egg-info/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     3714 2023-08-07 19:21:49.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutor_contrib_k8s_deploy_tasks.egg-info/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     1177 2023-08-07 19:21:49.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutor_contrib_k8s_deploy_tasks.egg-info/SOURCES.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-08-07 19:21:49.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutor_contrib_k8s_deploy_tasks.egg-info/dependency_links.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       66 2023-08-07 19:21:49.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutor_contrib_k8s_deploy_tasks.egg-info/entry_points.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       41 2023-08-07 19:21:49.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutor_contrib_k8s_deploy_tasks.egg-info/requires.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       22 2023-08-07 19:21:49.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutor_contrib_k8s_deploy_tasks.egg-info/top_level.txt
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 19:21:49.836729 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       23 2023-08-07 19:18:51.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/__about__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/__init__.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 19:21:49.837379 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/patches/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/patches/.gitignore
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      915 2023-06-15 18:15:08.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/patches/openedx-common-settings
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     3589 2023-08-07 19:16:24.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/patches/openedx-lms-production-settings
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     7845 2023-08-07 14:48:27.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/plugin.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 19:21:49.834510 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 19:21:49.834715 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 19:21:49.837644 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/apps/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/apps/.gitignore
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 19:21:49.837759 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/build/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/build/.gitignore
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 19:21:49.834766 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 19:21:49.837874 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-08-07 14:48:27.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/.gitignore
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 19:21:49.837997 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/cms/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       71 2023-08-07 14:48:27.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/cms/nutmeg_deploy_tasks
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 19:21:49.838513 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2895 2023-08-07 14:48:27.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/fix_oauth_redirect_uris
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       74 2023-08-07 14:48:27.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/nutmeg_deploy_tasks
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 19:21:49.838813 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/mysql/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      472 2023-08-07 14:48:27.000000 tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/mysql/add_user_profiles
```

### Comparing `tutor-contrib-k8s-deploy-tasks-15.0.0/PKG-INFO` & `tutor-contrib-k8s-deploy-tasks-15.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-k8s-deploy-tasks
-Version: 15.0.0
+Version: 15.0.1
 Summary: A Tutor plugin to manage deployment tasks that are exclusively (or mostly) specific to Kubernetes deployments
 Home-page: https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
 Author: Lawrence McDaniel
+Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 Maintainer: Lawrence McDaniel
 Maintainer-email: lpm0073@gmail.com
 License: AGPLv3
-Project-URL: Code, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
-Project-URL: Issue tracker, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks/issues
-Project-URL: Community, https://github.com/cookiecutter-openedx
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Project-URL: Homepage, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
+Project-URL: Bug Tracker, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks/issues
+Project-URL: Repository, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
+Keywords: Python,Open edX
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
+Provides-Extra: local
 
 k8s_deploy_tasks plugin for `Tutor <https://docs.tutor.overhang.io>`__
 ===================================================================================
 
 tutor plugin to manage deployment tasks that are exclusively (or mostly) specific to Kubernetes deployments.
 
 
@@ -37,15 +32,15 @@
 - *Xblock storage configuration*. creates this `custom storage configuration <./tutork8s_deploy_tasks/patches/openedx-common-settings>`_ designed to leverage this `custom kubernetes ExternalService <https://github.com/lpm0073/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/terraform/environments/modules/kubernetes_ingress_clb/manifests/proxy-service.yml.tpl>`_ and `ingress <https://github.com/lpm0073/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/terraform/environments/modules/kubernetes_ingress_clb/manifests/ingress-scorm-proxy-service.yml.tpl>`_ created by Cookiecutter for supporting AWS S3 storage for Xblocks.
 
 Installation
 ------------
 
 ::
 
-    pip install tutor-contrib-k8s-deploy-tasks
+    pip install git+https://github.com/myusername/tutor-contrib-k8s-deploy-tasks
 
 Usage
 -----
 
 ::
 
     tutor plugins enable k8s_deploy_tasks
```

### Comparing `tutor-contrib-k8s-deploy-tasks-15.0.0/README.rst` & `tutor-contrib-k8s-deploy-tasks-15.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 - *Xblock storage configuration*. creates this `custom storage configuration <./tutork8s_deploy_tasks/patches/openedx-common-settings>`_ designed to leverage this `custom kubernetes ExternalService <https://github.com/lpm0073/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/terraform/environments/modules/kubernetes_ingress_clb/manifests/proxy-service.yml.tpl>`_ and `ingress <https://github.com/lpm0073/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/terraform/environments/modules/kubernetes_ingress_clb/manifests/ingress-scorm-proxy-service.yml.tpl>`_ created by Cookiecutter for supporting AWS S3 storage for Xblocks.
 
 Installation
 ------------
 
 ::
 
-    pip install tutor-contrib-k8s-deploy-tasks
+    pip install git+https://github.com/myusername/tutor-contrib-k8s-deploy-tasks
 
 Usage
 -----
 
 ::
 
     tutor plugins enable k8s_deploy_tasks
```

### Comparing `tutor-contrib-k8s-deploy-tasks-15.0.0/setup.py` & `tutor-contrib-k8s-deploy-tasks-15.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import io
 import os
-from setuptools import setup, find_namespace_packages
+from setuptools import setup, find_packages
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 
 def load_readme():
     with io.open(os.path.join(HERE, "README.rst"), "rt", encoding="utf8") as f:
         return f.read()
@@ -31,18 +31,18 @@
     license="AGPLv3",
     author="Lawrence McDaniel",
     maintainer="Lawrence McDaniel",
     maintainer_email="lpm0073@gmail.com",
     description="A Tutor plugin to manage deployment tasks that are exclusively (or mostly) specific to Kubernetes deployments",
     long_description=load_readme(),
     long_description_content_type="text/x-rst",
-    packages=find_namespace_packages(exclude=["tests*"]),
+    packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     python_requires=">=3.5",
-    install_requires=["tutor>=15.0.0,<16.0.0"],
+    install_requires=["tutor>=15.0.0"],
     entry_points={"tutor.plugin.v1": ["k8s_deploy_tasks = tutork8s_deploy_tasks.plugin"]},
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

### Comparing `tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/PKG-INFO` & `tutor-contrib-k8s-deploy-tasks-15.0.1/tutor_contrib_k8s_deploy_tasks.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-k8s-deploy-tasks
-Version: 15.0.0
+Version: 15.0.1
 Summary: A Tutor plugin to manage deployment tasks that are exclusively (or mostly) specific to Kubernetes deployments
 Home-page: https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
 Author: Lawrence McDaniel
+Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 Maintainer: Lawrence McDaniel
 Maintainer-email: lpm0073@gmail.com
 License: AGPLv3
-Project-URL: Code, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
-Project-URL: Issue tracker, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks/issues
-Project-URL: Community, https://github.com/cookiecutter-openedx
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Project-URL: Homepage, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
+Project-URL: Bug Tracker, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks/issues
+Project-URL: Repository, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
+Keywords: Python,Open edX
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
+Provides-Extra: local
 
 k8s_deploy_tasks plugin for `Tutor <https://docs.tutor.overhang.io>`__
 ===================================================================================
 
 tutor plugin to manage deployment tasks that are exclusively (or mostly) specific to Kubernetes deployments.
 
 
@@ -37,15 +32,15 @@
 - *Xblock storage configuration*. creates this `custom storage configuration <./tutork8s_deploy_tasks/patches/openedx-common-settings>`_ designed to leverage this `custom kubernetes ExternalService <https://github.com/lpm0073/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/terraform/environments/modules/kubernetes_ingress_clb/manifests/proxy-service.yml.tpl>`_ and `ingress <https://github.com/lpm0073/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/terraform/environments/modules/kubernetes_ingress_clb/manifests/ingress-scorm-proxy-service.yml.tpl>`_ created by Cookiecutter for supporting AWS S3 storage for Xblocks.
 
 Installation
 ------------
 
 ::
 
-    pip install tutor-contrib-k8s-deploy-tasks
+    pip install git+https://github.com/myusername/tutor-contrib-k8s-deploy-tasks
 
 Usage
 -----
 
 ::
 
     tutor plugins enable k8s_deploy_tasks
```

### Comparing `tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/SOURCES.txt` & `tutor-contrib-k8s-deploy-tasks-15.0.1/tutor_contrib_k8s_deploy_tasks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/patches/openedx-common-settings` & `tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/patches/openedx-common-settings`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/patches/openedx-lms-production-settings` & `tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/patches/openedx-lms-production-settings`

 * *Files 16% similar despite different names*

```diff
@@ -25,17 +25,33 @@
 
 {% if MFE_AUTHN_MFE_APP %}
 AUTHN_MICROFRONTEND_URL = "https://{{ MFE_HOST }}/{{ MFE_AUTHN_MFE_APP["name"] }}"
 AUTHN_MICROFRONTEND_DOMAIN  = "{{ MFE_HOST }}/{{ MFE_AUTHN_MFE_APP["name"] }}"
 {% endif %}
 
 LOGIN_REDIRECT_WHITELIST.append("{{ MFE_HOST }}")
-CORS_ORIGIN_WHITELIST.append("https://{{ MFE_HOST }}")
 CSRF_TRUSTED_ORIGINS.append("{{ MFE_HOST }}")
 
+# add missing CORS_ORIGIN_WHITELIST hosts
+CORS_ORIGIN_WHITELIST.append("https://{{ LMS_HOST }}")
+CORS_ORIGIN_WHITELIST.append("https://{{ CMS_HOST }}")
+{% if MFE_HOST is defined %}
+CORS_ORIGIN_WHITELIST.append("https://{{ MFE_HOST }}")
+{% endif %}
+{% if DISCOVERY_HOST is defined %}
+CORS_ORIGIN_WHITELIST.append("https://{{ DISCOVERY_HOST }}")
+{% endif %}
+{% if ECOMMERCE_HOST is defined %}
+CORS_ORIGIN_WHITELIST.append("https://{{ ECOMMERCE_HOST }}")
+{% endif %}
+{% if CREDENTIALS_HOST is defined %}
+CORS_ORIGIN_WHITELIST.append("https://{{ CREDENTIALS_HOST }}")
+{% endif %}
+
+
 # Dynamic config API settings
 # https://openedx.github.io/frontend-platform/module-Config.html
 MFE_CONFIG = {
     "BASE_URL": "{{ MFE_HOST }}",
     "CSRF_TOKEN_API_PATH": "/csrf/api/v1/token",
 {%- if MFE_PROFILE_MFE_APP %}
     "ACCOUNT_PROFILE_URL": "https://{{ MFE_HOST }}/{{ MFE_PROFILE_MFE_APP["name"] }}",
```

### Comparing `tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/plugin.py` & `tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/fix_oauth_redirect_uris` & `tutor-contrib-k8s-deploy-tasks-15.0.1/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/fix_oauth_redirect_uris`

 * *Files identical despite different names*

