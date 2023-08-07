# Comparing `tmp/xj_role-1.0.92.tar.gz` & `tmp/xj_role-1.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xj_role-1.0.92.tar", last modified: Thu Aug  3 08:26:08 2023, max compression
+gzip compressed data, was "dist\xj_role-1.0.94.tar", last modified: Mon Aug  7 06:53:30 2023, max compression
```

## Comparing `xj_role-1.0.92.tar` & `xj_role-1.0.94.tar`

### file list

```diff
@@ -1,61 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.162714 xj_role-1.0.92/
--rw-rw-rw-   0        0        0      354 2023-08-03 08:26:08.161716 xj_role-1.0.92/PKG-INFO
--rw-rw-rw-   0        0        0      212 2022-09-02 08:12:19.000000 xj_role-1.0.92/README.md
--rw-rw-rw-   0        0        0       42 2023-08-03 08:26:08.162714 xj_role-1.0.92/setup.cfg
--rw-rw-rw-   0        0        0     1956 2023-08-03 08:25:02.000000 xj_role-1.0.92/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.098468 xj_role-1.0.92/xj_role/
--rw-rw-rw-   0        0        0        0 2022-09-02 08:12:19.000000 xj_role-1.0.92/xj_role/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/admin.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.111954 xj_role-1.0.92/xj_role/apis/
--rw-rw-rw-   0        0        0        0 2022-09-02 08:12:19.000000 xj_role-1.0.92/xj_role/apis/__init__.py
--rw-rw-rw-   0        0        0     7074 2023-07-20 02:20:21.000000 xj_role-1.0.92/xj_role/apis/group_api.py
--rw-rw-rw-   0        0        0     3879 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/apis/permission_api.py
--rw-rw-rw-   0        0        0     4549 2023-07-20 02:20:21.000000 xj_role-1.0.92/xj_role/apis/role_api.py
--rw-rw-rw-   0        0        0     3638 2023-07-13 00:57:44.000000 xj_role-1.0.92/xj_role/apis/role_menu_apis.py
--rw-rw-rw-   0        0        0     2162 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/apis/role_system_apis.py
--rw-rw-rw-   0        0        0      202 2022-09-06 08:07:54.000000 xj_role-1.0.92/xj_role/apps.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.115574 xj_role-1.0.92/xj_role/library/
--rw-rw-rw-   0        0        0      149 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/library/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.120549 xj_role-1.0.92/xj_role/library/api_interrupter/
--rw-rw-rw-   0        0        0      158 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/library/api_interrupter/__init__.py
--rw-rw-rw-   0        0        0     5573 2023-07-20 02:20:21.000000 xj_role-1.0.92/xj_role/library/api_interrupter/api_interrupter.py
--rw-rw-rw-   0        0        0      973 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/library/api_interrupter/api_interrupter_middleware.py
--rw-rw-rw-   0        0        0     4659 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/library/get_system_apis.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.124807 xj_role-1.0.92/xj_role/library/permission_execute/
--rw-rw-rw-   0        0        0      238 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/library/permission_execute/__init__.py
--rw-rw-rw-   0        0        0      292 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/library/permission_execute/permission_base.py
--rw-rw-rw-   0        0        0      280 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/library/permission_execute/permission_executor.py
--rw-rw-rw-   0        0        0    10442 2023-08-02 08:00:30.000000 xj_role-1.0.92/xj_role/models.py
--rw-rw-rw-   0        0        0     1091 2023-05-12 03:24:05.000000 xj_role-1.0.92/xj_role/service_register.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.136802 xj_role-1.0.92/xj_role/services/
--rw-rw-rw-   0        0        0        0 2022-09-02 08:12:19.000000 xj_role-1.0.92/xj_role/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.139820 xj_role-1.0.92/xj_role/services/abstract/
--rw-rw-rw-   0        0        0      168 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/services/abstract/__init__.py
--rw-rw-rw-   0        0        0      767 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/services/abstract/observer_subject.py
--rw-rw-rw-   0        0        0     6264 2022-10-18 05:55:19.000000 xj_role-1.0.92/xj_role/services/auto_permission_service.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.140817 xj_role-1.0.92/xj_role/services/observer/
--rw-rw-rw-   0        0        0      321 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/services/observer/__init__.py
--rw-rw-rw-   0        0        0    17658 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/services/permission_service.py
--rw-rw-rw-   0        0        0     6454 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/services/role_apis_services.py
--rw-rw-rw-   0        0        0    10049 2023-07-27 01:05:50.000000 xj_role-1.0.92/xj_role/services/role_nemus_services.py
--rw-rw-rw-   0        0        0    23254 2023-07-20 02:20:21.000000 xj_role-1.0.92/xj_role/services/role_service.py
--rw-rw-rw-   0        0        0    12667 2022-10-10 01:30:46.000000 xj_role-1.0.92/xj_role/services/user_group_service [backup].py
--rw-rw-rw-   0        0        0    24433 2023-08-03 08:23:47.000000 xj_role-1.0.92/xj_role/services/user_group_service.py
--rw-rw-rw-   0        0        0     3634 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/urls.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.159721 xj_role-1.0.92/xj_role/utils/
--rw-rw-rw-   0        0        0        0 2022-09-02 08:12:19.000000 xj_role-1.0.92/xj_role/utils/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/utils/api_interrupter_wrapper.py
--rw-rw-rw-   0        0        0     1082 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/utils/custom_authorization.py
--rw-rw-rw-   0        0        0     4618 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/utils/custom_response.py
--rw-rw-rw-   0        0        0    39226 2023-07-20 02:20:21.000000 xj_role-1.0.92/xj_role/utils/custom_tool.py
--rw-rw-rw-   0        0        0      958 2022-10-17 09:29:18.000000 xj_role-1.0.92/xj_role/utils/j_dict.py
--rw-rw-rw-   0        0        0    10256 2023-07-20 02:20:21.000000 xj_role-1.0.92/xj_role/utils/j_recur.py
--rw-rw-rw-   0        0        0      660 2023-05-12 03:24:05.000000 xj_role-1.0.92/xj_role/utils/join_list.py
--rw-rw-rw-   0        0        0     2691 2023-07-12 06:37:35.000000 xj_role-1.0.92/xj_role/utils/omnipotence_wrapper.py
--rw-rw-rw-   0        0        0     5867 2023-07-20 02:20:21.000000 xj_role-1.0.92/xj_role/utils/user_wrapper.py
--rw-rw-rw-   0        0        0     2682 2022-09-02 08:12:19.000000 xj_role-1.0.92/xj_role/utils/validator.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:26:08.103595 xj_role-1.0.92/xj_role.egg-info/
--rw-rw-rw-   0        0        0      354 2023-08-03 08:26:07.000000 xj_role-1.0.92/xj_role.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1577 2023-08-03 08:26:08.000000 xj_role-1.0.92/xj_role.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 08:26:07.000000 xj_role-1.0.92/xj_role.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-03 08:26:07.000000 xj_role-1.0.92/xj_role.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:30.000000 xj_role-1.0.94/
+-rw-rw-rw-   0        0        0      354 2023-08-07 06:53:30.000000 xj_role-1.0.94/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2022-08-25 05:15:54.000000 xj_role-1.0.94/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-07 06:53:30.000000 xj_role-1.0.94/setup.cfg
+-rw-rw-rw-   0        0        0     1956 2023-08-07 06:52:39.000000 xj_role-1.0.94/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role/
+-rw-rw-rw-   0        0        0        0 2023-06-28 10:29:35.000000 xj_role-1.0.94/xj_role/__init__.py
+-rw-rw-rw-   0        0        0     2912 2023-07-05 02:52:04.000000 xj_role-1.0.94/xj_role/admin.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.94/xj_role/apis/__init__.py
+-rw-rw-rw-   0        0        0     7074 2023-07-17 07:31:49.000000 xj_role-1.0.94/xj_role/apis/group_api.py
+-rw-rw-rw-   0        0        0     3879 2023-07-06 06:27:04.000000 xj_role-1.0.94/xj_role/apis/permission_api.py
+-rw-rw-rw-   0        0        0     4549 2023-07-17 07:28:37.000000 xj_role-1.0.94/xj_role/apis/role_api.py
+-rw-rw-rw-   0        0        0     3638 2023-08-07 01:19:41.000000 xj_role-1.0.94/xj_role/apis/role_menu_apis.py
+-rw-rw-rw-   0        0        0     2162 2023-06-30 01:35:19.000000 xj_role-1.0.94/xj_role/apis/role_system_apis.py
+-rw-rw-rw-   0        0        0      202 2022-09-06 06:05:16.000000 xj_role-1.0.94/xj_role/apps.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role/library/
+-rw-rw-rw-   0        0        0      149 2023-06-15 03:18:24.000000 xj_role-1.0.94/xj_role/library/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role/library/api_interrupter/
+-rw-rw-rw-   0        0        0      158 2023-07-05 02:30:03.000000 xj_role-1.0.94/xj_role/library/api_interrupter/__init__.py
+-rw-rw-rw-   0        0        0     5573 2023-07-19 09:27:58.000000 xj_role-1.0.94/xj_role/library/api_interrupter/api_interrupter.py
+-rw-rw-rw-   0        0        0      973 2023-07-06 06:13:34.000000 xj_role-1.0.94/xj_role/library/api_interrupter/api_interrupter_middleware.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role/library/current_limiting_tool/
+-rw-rw-rw-   0        0        0      159 2023-07-30 08:59:12.000000 xj_role-1.0.94/xj_role/library/current_limiting_tool/__init__.py
+-rw-rw-rw-   0        0        0      227 2023-07-31 06:29:41.000000 xj_role-1.0.94/xj_role/library/current_limiting_tool/arithmometer_limiter.py
+-rw-rw-rw-   0        0        0      175 2023-08-07 01:35:21.000000 xj_role-1.0.94/xj_role/library/current_limiting_tool/lease_bucket_limiter.py
+-rw-rw-rw-   0        0        0      178 2023-08-07 01:36:33.000000 xj_role-1.0.94/xj_role/library/current_limiting_tool/token_bucket_limiter.py
+-rw-rw-rw-   0        0        0     4659 2023-06-29 06:33:09.000000 xj_role-1.0.94/xj_role/library/get_system_apis.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role/library/permission_execute/
+-rw-rw-rw-   0        0        0      238 2023-06-28 10:26:56.000000 xj_role-1.0.94/xj_role/library/permission_execute/__init__.py
+-rw-rw-rw-   0        0        0      292 2023-06-28 08:42:31.000000 xj_role-1.0.94/xj_role/library/permission_execute/permission_base.py
+-rw-rw-rw-   0        0        0      280 2023-06-28 10:21:54.000000 xj_role-1.0.94/xj_role/library/permission_execute/permission_executor.py
+-rw-rw-rw-   0        0        0    10442 2023-08-07 01:37:49.000000 xj_role-1.0.94/xj_role/models.py
+-rw-rw-rw-   0        0        0     1091 2023-04-18 01:47:55.000000 xj_role-1.0.94/xj_role/service_register.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role/services/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.94/xj_role/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role/services/abstract/
+-rw-rw-rw-   0        0        0      168 2022-11-15 00:46:06.000000 xj_role-1.0.94/xj_role/services/abstract/__init__.py
+-rw-rw-rw-   0        0        0      767 2023-06-15 03:13:45.000000 xj_role-1.0.94/xj_role/services/abstract/observer_subject.py
+-rw-rw-rw-   0        0        0     6264 2022-10-27 09:43:36.000000 xj_role-1.0.94/xj_role/services/auto_permission_service.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role/services/observer/
+-rw-rw-rw-   0        0        0      321 2023-05-11 03:10:56.000000 xj_role-1.0.94/xj_role/services/observer/__init__.py
+-rw-rw-rw-   0        0        0    17658 2023-07-07 01:42:39.000000 xj_role-1.0.94/xj_role/services/permission_service.py
+-rw-rw-rw-   0        0        0     6454 2023-07-05 08:13:19.000000 xj_role-1.0.94/xj_role/services/role_apis_services.py
+-rw-rw-rw-   0        0        0    10114 2023-08-07 01:19:41.000000 xj_role-1.0.94/xj_role/services/role_nemus_services.py
+-rw-rw-rw-   0        0        0    23447 2023-08-07 06:49:46.000000 xj_role-1.0.94/xj_role/services/role_service.py
+-rw-rw-rw-   0        0        0    12667 2022-10-08 03:39:06.000000 xj_role-1.0.94/xj_role/services/user_group_service [backup].py
+-rw-rw-rw-   0        0        0    24433 2023-08-07 01:37:49.000000 xj_role-1.0.94/xj_role/services/user_group_service.py
+-rw-rw-rw-   0        0        0     3634 2023-06-30 01:15:41.000000 xj_role-1.0.94/xj_role/urls.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_role-1.0.94/xj_role/utils/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-07-04 07:07:56.000000 xj_role-1.0.94/xj_role/utils/api_interrupter_wrapper.py
+-rw-rw-rw-   0        0        0     1082 2023-06-29 09:26:10.000000 xj_role-1.0.94/xj_role/utils/custom_authorization.py
+-rw-rw-rw-   0        0        0     4618 2023-07-05 03:21:30.000000 xj_role-1.0.94/xj_role/utils/custom_response.py
+-rw-rw-rw-   0        0        0    39226 2023-07-17 06:47:39.000000 xj_role-1.0.94/xj_role/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      958 2022-10-25 06:03:08.000000 xj_role-1.0.94/xj_role/utils/j_dict.py
+-rw-rw-rw-   0        0        0    10256 2023-07-17 07:38:21.000000 xj_role-1.0.94/xj_role/utils/j_recur.py
+-rw-rw-rw-   0        0        0      660 2022-11-29 06:32:59.000000 xj_role-1.0.94/xj_role/utils/join_list.py
+-rw-rw-rw-   0        0        0     2691 2023-07-05 01:26:58.000000 xj_role-1.0.94/xj_role/utils/omnipotence_wrapper.py
+-rw-rw-rw-   0        0        0     5867 2023-07-17 01:50:28.000000 xj_role-1.0.94/xj_role/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     2682 2022-08-27 10:02:03.000000 xj_role-1.0.94/xj_role/utils/validator.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role.egg-info/
+-rw-rw-rw-   0        0        0      354 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1813 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-07 06:53:30.000000 xj_role-1.0.94/xj_role.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `xj_role-1.0.92/setup.py` & `xj_role-1.0.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_role',  # 模块名称
-    version='1.0.92',  # 模块版本
+    version='1.0.94',  # 模块版本
     description='权限模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     # author='sieyoo',
     # author_email='sieyoo@163.com',
     packages=find_packages(),  # 系统自动从当前目录开始找包
     # packages=['xj_user'],  # 系指定安装模块
```

### Comparing `xj_role-1.0.92/xj_role/admin.py` & `xj_role-1.0.94/xj_role/admin.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/apis/group_api.py` & `xj_role-1.0.94/xj_role/apis/group_api.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/apis/permission_api.py` & `xj_role-1.0.94/xj_role/apis/permission_api.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/apis/role_api.py` & `xj_role-1.0.94/xj_role/apis/role_api.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/apis/role_menu_apis.py` & `xj_role-1.0.94/xj_role/apis/role_menu_apis.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/apis/role_system_apis.py` & `xj_role-1.0.94/xj_role/apis/role_system_apis.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/library/api_interrupter/api_interrupter.py` & `xj_role-1.0.94/xj_role/library/api_interrupter/api_interrupter.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/library/api_interrupter/api_interrupter_middleware.py` & `xj_role-1.0.94/xj_role/library/api_interrupter/api_interrupter_middleware.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/library/get_system_apis.py` & `xj_role-1.0.94/xj_role/library/get_system_apis.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/models.py` & `xj_role-1.0.94/xj_role/models.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/service_register.py` & `xj_role-1.0.94/xj_role/service_register.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/services/abstract/observer_subject.py` & `xj_role-1.0.94/xj_role/services/abstract/observer_subject.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/services/auto_permission_service.py` & `xj_role-1.0.94/xj_role/services/auto_permission_service.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/services/permission_service.py` & `xj_role-1.0.94/xj_role/services/permission_service.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/services/role_apis_services.py` & `xj_role-1.0.94/xj_role/services/role_apis_services.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/services/role_nemus_services.py` & `xj_role-1.0.94/xj_role/services/role_nemus_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
         role_id = params.pop("role_id", None)
         role_id_list = params.pop("role_id_list", None)
         if role_id or role_id_list:
             permission_obj = RolePermission.objects.filter(type="MENU")
             permission_obj = permission_obj.filter(role_id=role_id) if role_id else permission_obj.filter(role_id__in=role_id_list)
             menu_id_list = permission_obj.values("menu_id").distinct().order_by('menu_id')
+            menu_id_list = [i["menu_id"] for i in menu_id_list]
             params.setdefault("id_list", menu_id_list)
 
         # 字段过滤
         params = format_params_handle(
             param_dict=params,
             filter_filed_list=[
                 "id|int", "id_list|list_int", "menu_id|int", "category_id|int", "parent_id|int", "name", "route", "icon", "link",
```

### Comparing `xj_role-1.0.92/xj_role/services/role_service.py` & `xj_role-1.0.94/xj_role/services/role_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,18 +122,22 @@
         sort = params.pop("sort", "-role_id")
         sort = sort if sort in ["role_id", "-role_id", "sort", "-sort"] else "-role_id"
         filter_tree_params, err = JRecur.get_filter_tree_params(params)
         params = format_params_handle(
             param_dict=params,
             filter_filed_list=[
                 "role_id|int", "role", "role_key|str", "user_group_id|int", "parent_role_id|int", "user_id|int", "is_using|int", "is_delete|int",
-                "user_group_id_list|list_int", "role_id_list|list_int", "user_id_list|list_int", "role_name|str"
+                "user_group_id_list|list_int", "role_id_list|list_int", "user_id_list|list_int", "role_name|str",
+                "created_time_start", "created_time_end"
             ],
             split_list=["user_group_id_list", "role_id_list", "user_id_list"],
-            alias_dict={"user_group_id_list": "user_group_id__in", "role_id_list": "role_id__in", "role": "role_key", "role_name": "role_name__contains"}
+            alias_dict={
+                "user_group_id_list": "user_group_id__in", "role_id_list": "role_id__in", "role": "role_key", "role_name": "role_name__contains",
+                "created_time_start": "created_time__gte", "created_time_end": "created_time__lte",
+            }
         )
         params.setdefault("is_delete", 0)
         user_id = params.pop("user_id", None)
         user_id_list = params.pop("user_id_list", None)
 
         filter_fields = filter_fields_handler(
             input_field_expression=filter_fields,
```

### Comparing `xj_role-1.0.92/xj_role/services/user_group_service [backup].py` & `xj_role-1.0.94/xj_role/services/user_group_service [backup].py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/services/user_group_service.py` & `xj_role-1.0.94/xj_role/services/user_group_service.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/urls.py` & `xj_role-1.0.94/xj_role/urls.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/utils/api_interrupter_wrapper.py` & `xj_role-1.0.94/xj_role/utils/api_interrupter_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/utils/custom_authorization.py` & `xj_role-1.0.94/xj_role/utils/custom_authorization.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/utils/custom_response.py` & `xj_role-1.0.94/xj_role/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/utils/custom_tool.py` & `xj_role-1.0.94/xj_role/utils/custom_tool.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/utils/j_dict.py` & `xj_role-1.0.94/xj_role/utils/j_dict.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/utils/j_recur.py` & `xj_role-1.0.94/xj_role/utils/j_recur.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/utils/join_list.py` & `xj_role-1.0.94/xj_role/utils/join_list.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/utils/omnipotence_wrapper.py` & `xj_role-1.0.94/xj_role/utils/omnipotence_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/utils/user_wrapper.py` & `xj_role-1.0.94/xj_role/utils/user_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role/utils/validator.py` & `xj_role-1.0.94/xj_role/utils/validator.py`

 * *Files identical despite different names*

### Comparing `xj_role-1.0.92/xj_role.egg-info/SOURCES.txt` & `xj_role-1.0.94/xj_role.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 xj_role/apis/role_menu_apis.py
 xj_role/apis/role_system_apis.py
 xj_role/library/__init__.py
 xj_role/library/get_system_apis.py
 xj_role/library/api_interrupter/__init__.py
 xj_role/library/api_interrupter/api_interrupter.py
 xj_role/library/api_interrupter/api_interrupter_middleware.py
+xj_role/library/current_limiting_tool/__init__.py
+xj_role/library/current_limiting_tool/arithmometer_limiter.py
+xj_role/library/current_limiting_tool/lease_bucket_limiter.py
+xj_role/library/current_limiting_tool/token_bucket_limiter.py
 xj_role/library/permission_execute/__init__.py
 xj_role/library/permission_execute/permission_base.py
 xj_role/library/permission_execute/permission_executor.py
 xj_role/services/__init__.py
 xj_role/services/auto_permission_service.py
 xj_role/services/permission_service.py
 xj_role/services/role_apis_services.py
```

