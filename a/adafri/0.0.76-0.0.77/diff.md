# Comparing `tmp/adafri-0.0.76.tar.gz` & `tmp/adafri-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.76.tar", last modified: Mon Aug  7 02:40:59 2023, max compression
+gzip compressed data, was "adafri-0.0.77.tar", last modified: Mon Aug  7 04:50:38 2023, max compression
```

## Comparing `adafri-0.0.76.tar` & `adafri-0.0.77.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.220259 adafri-0.0.76/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-07 02:40:59.219720 adafri-0.0.76/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.141461 adafri-0.0.76/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-08-07 02:40:52.000000 adafri-0.0.76/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.152719 adafri-0.0.76/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.76/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.76/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.76/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1356 2023-07-31 01:55:04.000000 adafri-0.0.76/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    19136 2023-08-07 02:40:23.000000 adafri-0.0.76/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.154121 adafri-0.0.76/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.76/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.155889 adafri-0.0.76/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.76/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.160644 adafri-0.0.76/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.76/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.76/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.76/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.162315 adafri-0.0.76/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.76/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.164915 adafri-0.0.76/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.76/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.76/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.166685 adafri-0.0.76/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.76/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.168561 adafri-0.0.76/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      965 2023-07-28 08:17:28.000000 adafri-0.0.76/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.193061 adafri-0.0.76/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.76/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7226 2023-08-07 02:16:40.000000 adafri-0.0.76/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.76/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6529 2023-07-31 01:47:56.000000 adafri-0.0.76/adafri/v1/auth/oauth/models/code.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2505 2023-07-31 01:28:33.000000 adafri-0.0.76/adafri/v1/auth/oauth/models/code_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16147 2023-07-31 01:04:27.000000 adafri-0.0.76/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.76/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9468 2023-07-31 01:04:45.000000 adafri-0.0.76/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.76/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.198958 adafri-0.0.76/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.76/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.76/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.76/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.205329 adafri-0.0.76/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.76/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.76/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.207579 adafri-0.0.76/adafri/v1/mailing/
--rw-r--r--   0 ibrahima   (502) staff       (20)    11325 2023-08-01 01:31:24.000000 adafri-0.0.76/adafri/v1/mailing/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.209241 adafri-0.0.76/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.76/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.217103 adafri-0.0.76/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.76/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11624 2023-07-26 07:42:34.000000 adafri-0.0.76/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.76/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 02:40:59.146337 adafri-0.0.76/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-07 02:40:59.000000 adafri-0.0.76/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-08-07 02:40:59.000000 adafri-0.0.76/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-08-07 02:40:59.000000 adafri-0.0.76/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-08-07 02:40:59.000000 adafri-0.0.76/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-08-07 02:40:59.221324 adafri-0.0.76/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.76/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.233183 adafri-0.0.77/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-07 04:50:38.232653 adafri-0.0.77/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.097303 adafri-0.0.77/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-08-07 04:50:30.000000 adafri-0.0.77/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.115338 adafri-0.0.77/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.77/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.77/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.77/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1356 2023-07-31 01:55:04.000000 adafri-0.0.77/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    19174 2023-08-07 04:49:01.000000 adafri-0.0.77/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.116131 adafri-0.0.77/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.77/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.123002 adafri-0.0.77/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.77/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.148213 adafri-0.0.77/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.77/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.77/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.77/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.164955 adafri-0.0.77/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.77/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.180788 adafri-0.0.77/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.77/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.77/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.186193 adafri-0.0.77/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.77/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.186575 adafri-0.0.77/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      965 2023-07-28 08:17:28.000000 adafri-0.0.77/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.208576 adafri-0.0.77/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7226 2023-08-07 02:16:40.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6529 2023-07-31 01:47:56.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/code.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2505 2023-07-31 01:28:33.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/code_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16147 2023-07-31 01:04:27.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9468 2023-07-31 01:04:45.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.224706 adafri-0.0.77/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.77/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.77/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.77/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.226987 adafri-0.0.77/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.77/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.77/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.227657 adafri-0.0.77/adafri/v1/mailing/
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11325 2023-08-01 01:31:24.000000 adafri-0.0.77/adafri/v1/mailing/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.228703 adafri-0.0.77/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.77/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.231382 adafri-0.0.77/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.77/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11720 2023-08-07 04:48:08.000000 adafri-0.0.77/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.77/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.100328 adafri-0.0.77/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-07 04:50:37.000000 adafri-0.0.77/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-08-07 04:50:38.000000 adafri-0.0.77/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-08-07 04:50:37.000000 adafri-0.0.77/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-08-07 04:50:37.000000 adafri-0.0.77/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-08-07 04:50:38.233396 adafri-0.0.77/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.77/setup.py
```

### Comparing `adafri-0.0.76/adafri/utils/country.py` & `adafri-0.0.77/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/utils/phone_number.py` & `adafri-0.0.77/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/utils/response.py` & `adafri-0.0.77/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/utils/utils.py` & `adafri-0.0.77/adafri/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,21 +204,23 @@
 
 def get_object_model_class(object_model, cls, fields=None, property='__match_args__'):
         obj = object_model
         if obj is None:
             obj = {};
         attributes = get_class_properties(cls, property);
         for key in attributes:
-            obj[key] = getattr(cls, key, None)
+            if key not in obj:
+                obj[key] = getattr(cls, key, None)
 
-        data_object = DictUtils.pick_object_values(obj, attributes);
+        data_object = obj
         keys = DictUtils.get_keys(data_object);
         if fields is not None:
             for key in attributes:
                 if key in fields:
+                    # print(data_object[key])
                     if key not in data_object or data_object[key] is None or data_object[key] == 'None':
                         if 'default_value' in fields[key]:
                             data_object[key] = fields[key]['default_value']
         return data_object, attributes
 
 def init_class_kwargs(cls, obj, class_fields, class_fields_props, class_collection_name, ids_key: list[str], **kwargs):
         cls_object, keys = get_object_model_class(obj, cls, class_fields_props);
```

### Comparing `adafri-0.0.76/adafri/v1/account/models/account.py` & `adafri-0.0.77/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/account/models/account_fields.py` & `adafri-0.0.77/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.77/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.77/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.77/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.77/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/auth/oauth/models/code.py` & `adafri-0.0.77/adafri/v1/auth/oauth/models/code.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/auth/oauth/models/code_fields.py` & `adafri-0.0.77/adafri/v1/auth/oauth/models/code_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.77/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.77/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.77/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.77/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.77/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.77/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/base/firebase_collection.py` & `adafri-0.0.77/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/mailing/__init__.py` & `adafri-0.0.77/adafri/v1/mailing/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri/v1/user/models/user.py` & `adafri-0.0.77/adafri/v1/user/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,24 +192,26 @@
         user = {};
         props = UserFieldProps
         for k in DictUtils.get_keys(props):
             user[k] = props[k][_key_];
         return user;
 
     @staticmethod
-    def from_dict(user: Any, db=None, collection_name=USERS_COLLECTION) -> 'User':
+    def from_dict(user: Any=None, db=None, collection_name=USERS_COLLECTION) -> 'User':
         cls_object, keys = get_object_model_class(user, User, UserFieldProps);
+        # print('from dict', cls_object)
         _user = User(cls_object, db=db, collection_name=collection_name)
         return _user
     
     def get(self):
         doc = self.document_reference().get();
         if doc.exists is False:
             return None;
-        return User.from_dict(doc.to_dict(), db=self.db, collection_name=self.collection_name);
+        # print('user found', doc.to_dict())
+        return User.from_dict(user=doc.to_dict(), db=self.db, collection_name=self.collection_name);
 
     def query(self, query_params: list, first=False, limit=None):
         result = [];
         query_result = self.custom_query(query_params, first=first, limit=limit)
         if bool(query_result):
             if first:
                 return User.from_dict(user=query_result, db=self.db, collection_name=self.collection_name)
```

### Comparing `adafri-0.0.76/adafri/v1/user/models/user_fields.py` & `adafri-0.0.77/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/adafri.egg-info/SOURCES.txt` & `adafri-0.0.77/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.76/setup.py` & `adafri-0.0.77/setup.py`

 * *Files identical despite different names*

