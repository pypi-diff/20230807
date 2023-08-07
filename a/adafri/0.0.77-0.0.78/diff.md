# Comparing `tmp/adafri-0.0.77.tar.gz` & `tmp/adafri-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.77.tar", last modified: Mon Aug  7 04:50:38 2023, max compression
+gzip compressed data, was "adafri-0.0.78.tar", last modified: Mon Aug  7 05:10:05 2023, max compression
```

## Comparing `adafri-0.0.77.tar` & `adafri-0.0.78.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.233183 adafri-0.0.77/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-07 04:50:38.232653 adafri-0.0.77/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.097303 adafri-0.0.77/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-08-07 04:50:30.000000 adafri-0.0.77/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.115338 adafri-0.0.77/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.77/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.77/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.77/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1356 2023-07-31 01:55:04.000000 adafri-0.0.77/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    19174 2023-08-07 04:49:01.000000 adafri-0.0.77/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.116131 adafri-0.0.77/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.77/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.123002 adafri-0.0.77/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.77/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.148213 adafri-0.0.77/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.77/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.77/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.77/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.164955 adafri-0.0.77/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.77/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.180788 adafri-0.0.77/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.77/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.77/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.186193 adafri-0.0.77/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.77/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.186575 adafri-0.0.77/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      965 2023-07-28 08:17:28.000000 adafri-0.0.77/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.208576 adafri-0.0.77/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7226 2023-08-07 02:16:40.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6529 2023-07-31 01:47:56.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/code.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2505 2023-07-31 01:28:33.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/code_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16147 2023-07-31 01:04:27.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9468 2023-07-31 01:04:45.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.77/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.224706 adafri-0.0.77/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.77/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.77/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.77/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.226987 adafri-0.0.77/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.77/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.77/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.227657 adafri-0.0.77/adafri/v1/mailing/
--rw-r--r--   0 ibrahima   (502) staff       (20)    11325 2023-08-01 01:31:24.000000 adafri-0.0.77/adafri/v1/mailing/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.228703 adafri-0.0.77/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.77/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.231382 adafri-0.0.77/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.77/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11720 2023-08-07 04:48:08.000000 adafri-0.0.77/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.77/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 04:50:38.100328 adafri-0.0.77/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-07 04:50:37.000000 adafri-0.0.77/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-08-07 04:50:38.000000 adafri-0.0.77/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-08-07 04:50:37.000000 adafri-0.0.77/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-08-07 04:50:37.000000 adafri-0.0.77/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-08-07 04:50:38.233396 adafri-0.0.77/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.77/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.588744 adafri-0.0.78/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-07 05:10:05.588158 adafri-0.0.78/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.527676 adafri-0.0.78/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-08-07 05:10:01.000000 adafri-0.0.78/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.536277 adafri-0.0.78/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.78/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.78/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.78/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1356 2023-07-31 01:55:04.000000 adafri-0.0.78/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    19174 2023-08-07 04:49:01.000000 adafri-0.0.78/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.537774 adafri-0.0.78/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.78/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.539000 adafri-0.0.78/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.78/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.543129 adafri-0.0.78/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.78/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.78/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.78/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.544513 adafri-0.0.78/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.78/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.546447 adafri-0.0.78/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.78/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.78/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.548447 adafri-0.0.78/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.78/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.549209 adafri-0.0.78/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      965 2023-07-28 08:17:28.000000 adafri-0.0.78/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.563340 adafri-0.0.78/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7216 2023-08-07 05:09:25.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6540 2023-08-07 05:08:57.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/code.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2505 2023-07-31 01:28:33.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/code_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16152 2023-08-07 05:07:34.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9460 2023-08-07 05:08:18.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.578369 adafri-0.0.78/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.78/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.78/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.78/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.581193 adafri-0.0.78/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.78/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.78/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.582101 adafri-0.0.78/adafri/v1/mailing/
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11325 2023-08-01 01:31:24.000000 adafri-0.0.78/adafri/v1/mailing/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.583261 adafri-0.0.78/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.78/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.586527 adafri-0.0.78/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.78/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11720 2023-08-07 04:48:08.000000 adafri-0.0.78/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.78/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.530272 adafri-0.0.78/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-07 05:10:05.000000 adafri-0.0.78/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-08-07 05:10:05.000000 adafri-0.0.78/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-08-07 05:10:05.000000 adafri-0.0.78/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-08-07 05:10:05.000000 adafri-0.0.78/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-08-07 05:10:05.589002 adafri-0.0.78/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.78/setup.py
```

### Comparing `adafri-0.0.77/adafri/utils/country.py` & `adafri-0.0.78/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/utils/phone_number.py` & `adafri-0.0.78/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/utils/response.py` & `adafri-0.0.78/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/utils/utils.py` & `adafri-0.0.78/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/v1/account/models/account.py` & `adafri-0.0.78/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/v1/account/models/account_fields.py` & `adafri-0.0.78/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.78/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.78/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.78/adafri/v1/auth/oauth/models/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         client_model.id = Crypto().generate_id(client_model.name+"~"+client_model.uid+"~"+client_model.client_id);
         client_model.client_id_issued_at = int(time.time())
         
         if client_model.token_endpoint_auth_method == 'none':
             client_model.client_secret = ''
         else:
             client_model.client_secret = gen_salt(48)
-        return ApiResponse(ResponseStatus.OK, StatusCode.status_200, client_model.to_json(), None);
+        return ApiResponse(ResponseStatus.OK, StatusCode.status_200, client_model, None);
     
     def update(self, data):
         try:
             last_value = self.to_json();
             filtered_value = pydash.pick(data, ClientFields.filtered_keys('editable', True));
             new_value = DictUtils.merge_dict(filtered_value, self.to_json());
             changed_fields = DictUtils.get_changed_field(last_value, new_value);
```

### Comparing `adafri-0.0.77/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.78/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/v1/auth/oauth/models/code.py` & `adafri-0.0.78/adafri/v1/auth/oauth/models/code.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,19 +80,19 @@
     
     @staticmethod
     def create(**kwargs):
         authorization_code = Code().generate(**kwargs);
         if authorization_code.status == ResponseStatus.ERROR:
             return authorization_code
         
-        docRef = Code(authorization_code.data).document_reference();
+        authorization_code_model: Code = authorization_code.data;
+        docRef = Code(authorization_code_model.to_json()).document_reference();
         # if docRef.get().exists:
         #     return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Code with name {authorization_code.id} already exist","INVALID_REQUEST", 1));
         
-        authorization_code_model: Code = authorization_code.data;
         docRef.set({**authorization_code_model.to_json(), "createdAt": getTimestamp()}, merge=True);
         created_campaign = authorization_code_model.getCode()
         return ApiResponse(ResponseStatus.OK, StatusCode.status_200, created_campaign.to_json(), None);
     
     def update(self, data):
         try:
             last_value = self.to_json();
```

### Comparing `adafri-0.0.77/adafri/v1/auth/oauth/models/code_fields.py` & `adafri-0.0.78/adafri/v1/auth/oauth/models/code_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.78/adafri/v1/auth/oauth/models/grant.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,22 +116,22 @@
     
     @staticmethod
     def create(**kwargs):
         authorization_code = OAuthGrant().generate(**kwargs);
         if authorization_code.status == ResponseStatus.ERROR:
             return authorization_code
         
-        docRef = OAuthGrant(authorization_code.data).document_reference();
+        authorization_code_model: OAuthGrant = authorization_code.data;
+        docRef = OAuthGrant(authorization_code_model.to_json()).document_reference();
         # if docRef.get().exists:
         #     return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Code with name {authorization_code.id} already exist","INVALID_REQUEST", 1));
         
-        authorization_code_model: OAuthGrant = authorization_code.data;
         docRef.set({**authorization_code_model.to_json(), "createdAt": getTimestamp()}, merge=True);
-        created_campaign = authorization_code_model.getOAuthGrant()
-        return ApiResponse(ResponseStatus.OK, StatusCode.status_200, created_campaign.to_json(), None);
+        created_grant = authorization_code_model.getOAuthGrant()
+        return ApiResponse(ResponseStatus.OK, StatusCode.status_200, created_grant.to_json(), None);
     
     def update(self, data):
         try:
             last_value = self.to_json();
             filtered_value = pydash.pick(data, GrantFields.filtered_keys('editable', True));
             new_value = DictUtils.merge_dict(filtered_value, self.to_json());
             changed_fields = DictUtils.get_changed_field(last_value, new_value);
```

### Comparing `adafri-0.0.77/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.78/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.78/adafri/v1/auth/oauth/models/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,19 +92,19 @@
     def save(self, token, request):
         model = {**token, "client_id": request.client.client_id, "uid": request.user.uid, "revoked": False}
         if 'type' not in model:
             model['type'] = 'app_token'
         token_generate = OAuthToken.generate(**model);
         if token_generate.status == ResponseStatus.ERROR:
             return token_generate
-        docRef = OAuthToken(token_generate.data.to_json()).document_reference();
+        token_model: OAuthToken = token_generate.data;
+        docRef = OAuthToken(token_model.to_json()).document_reference();
         # if docRef.get().exists:
         #     return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Location with name {token_generate.data.id} already exist","INVALID_REQUEST", 1));
         
-        token_model: OAuthToken = token_generate.data;
         docRef.set({**token_model.to_json(), "createdAt": getTimestamp()}, merge=True);
         created_token = token_model.getOAuthToken()
         return ApiResponse(ResponseStatus.OK, StatusCode.status_200, created_token.to_json(), None);
     
     def update(self, data):
         try:
             last_value = self.to_json();
```

### Comparing `adafri-0.0.77/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.78/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.78/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.78/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/v1/base/firebase_collection.py` & `adafri-0.0.78/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/v1/mailing/__init__.py` & `adafri-0.0.78/adafri/v1/mailing/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/v1/user/models/user.py` & `adafri-0.0.78/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri/v1/user/models/user_fields.py` & `adafri-0.0.78/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/adafri.egg-info/SOURCES.txt` & `adafri-0.0.78/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.77/setup.py` & `adafri-0.0.78/setup.py`

 * *Files identical despite different names*

