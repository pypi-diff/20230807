# Comparing `tmp/tutor-contrib-k8s-deploy-tasks-14.0.0.tar.gz` & `tmp/tutor-contrib-k8s-deploy-tasks-15.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-k8s-deploy-tasks-14.0.0.tar", last modified: Mon Aug  7 14:36:39 2023, max compression
+gzip compressed data, was "tutor-contrib-k8s-deploy-tasks-15.0.0.tar", last modified: Sat Jun 17 16:10:36 2023, max compression
```

## Comparing `tutor-contrib-k8s-deploy-tasks-14.0.0.tar` & `tutor-contrib-k8s-deploy-tasks-15.0.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 14:36:39.980808 tutor-contrib-k8s-deploy-tasks-14.0.0/
--rw-r--r--   0 mcdaniel   (501) staff       (20)      102 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/MANIFEST.in
--rw-r--r--   0 mcdaniel   (501) staff       (20)     3616 2023-08-07 14:36:39.980695 tutor-contrib-k8s-deploy-tasks-14.0.0/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2728 2023-08-07 14:27:09.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/README.rst
--rw-r--r--   0 mcdaniel   (501) staff       (20)       38 2023-08-07 14:36:39.980845 tutor-contrib-k8s-deploy-tasks-14.0.0/setup.cfg
--rw-r--r--   0 mcdaniel   (501) staff       (20)     1764 2023-08-07 14:28:44.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/setup.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 14:36:39.977994 tutor-contrib-k8s-deploy-tasks-14.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/
--rw-r--r--   0 mcdaniel   (501) staff       (20)     3616 2023-08-07 14:36:39.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)     1132 2023-08-07 14:36:39.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/SOURCES.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-08-07 14:36:39.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/dependency_links.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       66 2023-08-07 14:36:39.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/entry_points.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       14 2023-08-07 14:36:39.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/requires.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       22 2023-08-07 14:36:39.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/top_level.txt
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 14:36:39.978379 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/
--rw-r--r--   0 mcdaniel   (501) staff       (20)       23 2023-08-07 14:31:48.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/__about__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/__init__.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 14:36:39.978996 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/patches/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/patches/.gitignore
--rw-r--r--   0 mcdaniel   (501) staff       (20)      915 2023-06-15 18:15:08.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/patches/openedx-common-settings
--rw-r--r--   0 mcdaniel   (501) staff       (20)     3066 2023-06-15 18:22:20.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/patches/openedx-lms-production-settings
--rw-r--r--   0 mcdaniel   (501) staff       (20)     3007 2023-08-07 14:27:09.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/plugin.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 14:36:39.976499 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 14:36:39.976698 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 14:36:39.979281 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/apps/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/apps/.gitignore
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 14:36:39.979398 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/build/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/build/.gitignore
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 14:36:39.979513 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/tasks/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-08-07 14:27:09.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/tasks/.gitignore
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 14:36:39.979629 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/tasks/cms/
--rw-r--r--   0 mcdaniel   (501) staff       (20)       72 2023-08-07 14:27:09.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/tasks/cms/nutmeg_deploy_tasks
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 14:36:39.980105 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/tasks/lms/
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2896 2023-08-07 14:27:09.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/tasks/lms/fix_oauth_redirect_uris
--rw-r--r--   0 mcdaniel   (501) staff       (20)       75 2023-08-07 14:27:09.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/tasks/lms/nutmeg_deploy_tasks
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-08-07 14:36:39.980510 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/tasks/mysql/
--rw-r--r--   0 mcdaniel   (501) staff       (20)      473 2023-08-07 14:27:09.000000 tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/tasks/mysql/add_user_profiles
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.072049 tutor-contrib-k8s-deploy-tasks-15.0.0/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      102 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/MANIFEST.in
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     3955 2023-06-17 16:10:36.072146 tutor-contrib-k8s-deploy-tasks-15.0.0/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2694 2023-06-17 16:09:28.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/README.rst
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      278 2023-06-17 14:35:54.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/pyproject.toml
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       67 2023-06-17 16:10:36.072515 tutor-contrib-k8s-deploy-tasks-15.0.0/setup.cfg
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2118 2023-06-17 16:05:49.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/setup.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.068588 tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     3955 2023-06-17 16:10:35.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     1177 2023-06-17 16:10:36.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/SOURCES.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-06-17 16:10:35.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/dependency_links.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       66 2023-06-17 16:10:35.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/entry_points.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       22 2023-06-17 16:10:35.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/requires.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       27 2023-06-17 16:10:35.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/top_level.txt
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.069271 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       23 2023-06-17 13:31:26.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/__about__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/__init__.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.070101 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/patches/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/patches/.gitignore
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      915 2023-06-15 18:15:08.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/patches/openedx-common-settings
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     3066 2023-06-15 18:22:20.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/patches/openedx-lms-production-settings
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     7845 2023-06-17 14:27:24.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/plugin.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.065430 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.065754 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.070466 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/apps/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/apps/.gitignore
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.070649 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/build/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-15 18:12:17.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/build/.gitignore
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.065835 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.070825 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-06-17 13:31:26.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/.gitignore
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.071003 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/cms/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       71 2023-06-17 13:31:26.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/cms/nutmeg_deploy_tasks
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.071612 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2895 2023-06-17 13:31:26.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/fix_oauth_redirect_uris
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       74 2023-06-17 13:31:26.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/nutmeg_deploy_tasks
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-06-17 16:10:36.071842 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/mysql/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      472 2023-06-17 13:31:26.000000 tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/mysql/add_user_profiles
```

### Comparing `tutor-contrib-k8s-deploy-tasks-14.0.0/PKG-INFO` & `tutor-contrib-k8s-deploy-tasks-15.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-k8s-deploy-tasks
-Version: 14.0.0
-Summary: k8s_deploy_tasks plugin for Tutor
-Home-page: https://github.com/myusername/tutor-contrib-k8s-deploy-tasks
+Version: 15.0.0
+Summary: A Tutor plugin to manage deployment tasks that are exclusively (or mostly) specific to Kubernetes deployments
+Home-page: https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
 Author: Lawrence McDaniel
+Maintainer: Lawrence McDaniel
+Maintainer-email: lpm0073@gmail.com
 License: AGPLv3
-Project-URL: Code, https://github.com/myusername/tutor-contrib-k8s-deploy-tasks
-Project-URL: Issue tracker, https://github.com/myusername/tutor-contrib-k8s-deploy-tasks/issues
+Project-URL: Code, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
+Project-URL: Issue tracker, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks/issues
+Project-URL: Community, https://github.com/cookiecutter-openedx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.5
+Description-Content-Type: text/x-rst
 
 k8s_deploy_tasks plugin for `Tutor <https://docs.tutor.overhang.io>`__
 ===================================================================================
 
 tutor plugin to manage deployment tasks that are exclusively (or mostly) specific to Kubernetes deployments.
 
 
@@ -31,15 +37,15 @@
 - *Xblock storage configuration*. creates this `custom storage configuration <./tutork8s_deploy_tasks/patches/openedx-common-settings>`_ designed to leverage this `custom kubernetes ExternalService <https://github.com/lpm0073/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/terraform/environments/modules/kubernetes_ingress_clb/manifests/proxy-service.yml.tpl>`_ and `ingress <https://github.com/lpm0073/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/terraform/environments/modules/kubernetes_ingress_clb/manifests/ingress-scorm-proxy-service.yml.tpl>`_ created by Cookiecutter for supporting AWS S3 storage for Xblocks.
 
 Installation
 ------------
 
 ::
 
-    pip install git+https://github.com/myusername/tutor-contrib-k8s-deploy-tasks
+    pip install tutor-contrib-k8s-deploy-tasks
 
 Usage
 -----
 
 ::
 
     tutor plugins enable k8s_deploy_tasks
```

### Comparing `tutor-contrib-k8s-deploy-tasks-14.0.0/README.rst` & `tutor-contrib-k8s-deploy-tasks-15.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 - *Xblock storage configuration*. creates this `custom storage configuration <./tutork8s_deploy_tasks/patches/openedx-common-settings>`_ designed to leverage this `custom kubernetes ExternalService <https://github.com/lpm0073/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/terraform/environments/modules/kubernetes_ingress_clb/manifests/proxy-service.yml.tpl>`_ and `ingress <https://github.com/lpm0073/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/terraform/environments/modules/kubernetes_ingress_clb/manifests/ingress-scorm-proxy-service.yml.tpl>`_ created by Cookiecutter for supporting AWS S3 storage for Xblocks.
 
 Installation
 ------------
 
 ::
 
-    pip install git+https://github.com/myusername/tutor-contrib-k8s-deploy-tasks
+    pip install tutor-contrib-k8s-deploy-tasks
 
 Usage
 -----
 
 ::
 
     tutor plugins enable k8s_deploy_tasks
```

### Comparing `tutor-contrib-k8s-deploy-tasks-14.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/PKG-INFO` & `tutor-contrib-k8s-deploy-tasks-15.0.0/tutor_contrib_k8s_deploy_tasks.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-k8s-deploy-tasks
-Version: 14.0.0
-Summary: k8s_deploy_tasks plugin for Tutor
-Home-page: https://github.com/myusername/tutor-contrib-k8s-deploy-tasks
+Version: 15.0.0
+Summary: A Tutor plugin to manage deployment tasks that are exclusively (or mostly) specific to Kubernetes deployments
+Home-page: https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
 Author: Lawrence McDaniel
+Maintainer: Lawrence McDaniel
+Maintainer-email: lpm0073@gmail.com
 License: AGPLv3
-Project-URL: Code, https://github.com/myusername/tutor-contrib-k8s-deploy-tasks
-Project-URL: Issue tracker, https://github.com/myusername/tutor-contrib-k8s-deploy-tasks/issues
+Project-URL: Code, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks
+Project-URL: Issue tracker, https://github.com/cookiecutter-openedx/tutor-contrib-k8s-deploy-tasks/issues
+Project-URL: Community, https://github.com/cookiecutter-openedx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.5
+Description-Content-Type: text/x-rst
 
 k8s_deploy_tasks plugin for `Tutor <https://docs.tutor.overhang.io>`__
 ===================================================================================
 
 tutor plugin to manage deployment tasks that are exclusively (or mostly) specific to Kubernetes deployments.
 
 
@@ -31,15 +37,15 @@
 - *Xblock storage configuration*. creates this `custom storage configuration <./tutork8s_deploy_tasks/patches/openedx-common-settings>`_ designed to leverage this `custom kubernetes ExternalService <https://github.com/lpm0073/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/terraform/environments/modules/kubernetes_ingress_clb/manifests/proxy-service.yml.tpl>`_ and `ingress <https://github.com/lpm0073/cookiecutter-openedx-devops/blob/main/%7B%7Bcookiecutter.github_repo_name%7D%7D/terraform/environments/modules/kubernetes_ingress_clb/manifests/ingress-scorm-proxy-service.yml.tpl>`_ created by Cookiecutter for supporting AWS S3 storage for Xblocks.
 
 Installation
 ------------
 
 ::
 
-    pip install git+https://github.com/myusername/tutor-contrib-k8s-deploy-tasks
+    pip install tutor-contrib-k8s-deploy-tasks
 
 Usage
 -----
 
 ::
 
     tutor plugins enable k8s_deploy_tasks
```

### Comparing `tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/patches/openedx-common-settings` & `tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/patches/openedx-common-settings`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/patches/openedx-lms-production-settings` & `tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/patches/openedx-lms-production-settings`

 * *Files identical despite different names*

### Comparing `tutor-contrib-k8s-deploy-tasks-14.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/tasks/lms/fix_oauth_redirect_uris` & `tutor-contrib-k8s-deploy-tasks-15.0.0/tutork8s_deploy_tasks/templates/k8s_deploy_tasks/jobs/init/lms/fix_oauth_redirect_uris`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -79,8 +79,8 @@
   --client-id {{ CREDENTIALS_OAUTH2_KEY_SSO }} \
   --client-secret {{ CREDENTIALS_OAUTH2_SECRET_SSO }} \
   --scopes user_id \
   --skip-authorization \
   --update \
   credentials-sso \
   credentials
-{% endif %}
+{% endif %}
```

