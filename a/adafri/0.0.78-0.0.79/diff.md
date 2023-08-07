# Comparing `tmp/adafri-0.0.78.tar.gz` & `tmp/adafri-0.0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.78.tar", last modified: Mon Aug  7 05:10:05 2023, max compression
+gzip compressed data, was "adafri-0.0.79.tar", last modified: Mon Aug  7 05:43:48 2023, max compression
```

## Comparing `adafri-0.0.78.tar` & `adafri-0.0.79.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.588744 adafri-0.0.78/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-07 05:10:05.588158 adafri-0.0.78/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.527676 adafri-0.0.78/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-08-07 05:10:01.000000 adafri-0.0.78/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.536277 adafri-0.0.78/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.78/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.78/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.78/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1356 2023-07-31 01:55:04.000000 adafri-0.0.78/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    19174 2023-08-07 04:49:01.000000 adafri-0.0.78/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.537774 adafri-0.0.78/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.78/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.539000 adafri-0.0.78/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.78/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.543129 adafri-0.0.78/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.78/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.78/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.78/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.544513 adafri-0.0.78/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.78/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.546447 adafri-0.0.78/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.78/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.78/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.548447 adafri-0.0.78/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.78/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.549209 adafri-0.0.78/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      965 2023-07-28 08:17:28.000000 adafri-0.0.78/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.563340 adafri-0.0.78/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7216 2023-08-07 05:09:25.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6540 2023-08-07 05:08:57.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/code.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2505 2023-07-31 01:28:33.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/code_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16152 2023-08-07 05:07:34.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9460 2023-08-07 05:08:18.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.78/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.578369 adafri-0.0.78/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.78/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.78/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.78/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.581193 adafri-0.0.78/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.78/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.78/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.582101 adafri-0.0.78/adafri/v1/mailing/
--rw-r--r--   0 ibrahima   (502) staff       (20)    11325 2023-08-01 01:31:24.000000 adafri-0.0.78/adafri/v1/mailing/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.583261 adafri-0.0.78/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.78/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.586527 adafri-0.0.78/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.78/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11720 2023-08-07 04:48:08.000000 adafri-0.0.78/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.78/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:10:05.530272 adafri-0.0.78/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-07 05:10:05.000000 adafri-0.0.78/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-08-07 05:10:05.000000 adafri-0.0.78/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-08-07 05:10:05.000000 adafri-0.0.78/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-08-07 05:10:05.000000 adafri-0.0.78/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-08-07 05:10:05.589002 adafri-0.0.78/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.78/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.890515 adafri-0.0.79/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-07 05:43:48.889928 adafri-0.0.79/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.839351 adafri-0.0.79/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-08-07 05:43:42.000000 adafri-0.0.79/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.848475 adafri-0.0.79/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.79/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.79/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.79/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1356 2023-07-31 01:55:04.000000 adafri-0.0.79/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    19215 2023-08-07 05:42:43.000000 adafri-0.0.79/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.849375 adafri-0.0.79/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.79/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.850611 adafri-0.0.79/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.79/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.854478 adafri-0.0.79/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.79/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.79/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.79/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.855625 adafri-0.0.79/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.79/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.857265 adafri-0.0.79/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.79/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.79/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.858583 adafri-0.0.79/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.79/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.859119 adafri-0.0.79/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      965 2023-07-28 08:17:28.000000 adafri-0.0.79/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.875364 adafri-0.0.79/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.79/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7216 2023-08-07 05:09:25.000000 adafri-0.0.79/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.79/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6540 2023-08-07 05:08:57.000000 adafri-0.0.79/adafri/v1/auth/oauth/models/code.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2505 2023-07-31 01:28:33.000000 adafri-0.0.79/adafri/v1/auth/oauth/models/code_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16152 2023-08-07 05:07:34.000000 adafri-0.0.79/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.79/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9460 2023-08-07 05:08:18.000000 adafri-0.0.79/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.79/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.879244 adafri-0.0.79/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.79/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.79/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.79/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.882231 adafri-0.0.79/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.79/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.79/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.883054 adafri-0.0.79/adafri/v1/mailing/
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11325 2023-08-01 01:31:24.000000 adafri-0.0.79/adafri/v1/mailing/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.884354 adafri-0.0.79/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.79/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.888231 adafri-0.0.79/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.79/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11720 2023-08-07 04:48:08.000000 adafri-0.0.79/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.79/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:43:48.842103 adafri-0.0.79/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-07 05:43:48.000000 adafri-0.0.79/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-08-07 05:43:48.000000 adafri-0.0.79/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-08-07 05:43:48.000000 adafri-0.0.79/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-08-07 05:43:48.000000 adafri-0.0.79/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-08-07 05:43:48.890897 adafri-0.0.79/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.79/setup.py
```

### Comparing `adafri-0.0.78/adafri/utils/country.py` & `adafri-0.0.79/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/utils/phone_number.py` & `adafri-0.0.79/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/utils/response.py` & `adafri-0.0.79/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/utils/utils.py` & `adafri-0.0.79/adafri/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import (date, datetime)
 from urllib.parse import urlparse, parse_qs
 import re
 import random
 
 hash = hashlib.sha1(str(os.getenv('CRYPTO_KEY')).encode())
 ENCRYPTION_KEY = base64.b64encode(hash.hexdigest()[:32].encode()).decode();
-
+from urllib.parse import unquote
 
 camel_pat = re.compile(r'([A-Z])')
 under_pat = re.compile(r'_([a-z])')
 
 
 def boolean(data):
     if type(data) is bool:
@@ -131,15 +131,15 @@
     base64_string = base64_bytes.decode("ascii")
     return base64_string;
 
 def decode_base64(data_base64: str):
     base64_bytes = data_base64.encode("ascii")
     string_bytes = base64.b64decode(base64_bytes)
     decoded_string = string_bytes.decode("ascii")
-    return decoded_string
+    return unquote(decoded_string)
 
 class Crypto:
 
     print(ENCRYPTION_KEY)
     print(hash.hexdigest())
     fernet = Fernet(ENCRYPTION_KEY);
     def encrypt(self, message:str):
```

### Comparing `adafri-0.0.78/adafri/v1/account/models/account.py` & `adafri-0.0.79/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/account/models/account_fields.py` & `adafri-0.0.79/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.79/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.79/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.79/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.79/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/auth/oauth/models/code.py` & `adafri-0.0.79/adafri/v1/auth/oauth/models/code.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/auth/oauth/models/code_fields.py` & `adafri-0.0.79/adafri/v1/auth/oauth/models/code_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.79/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.79/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.79/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.79/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.79/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.79/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/base/firebase_collection.py` & `adafri-0.0.79/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/mailing/__init__.py` & `adafri-0.0.79/adafri/v1/mailing/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/user/models/user.py` & `adafri-0.0.79/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri/v1/user/models/user_fields.py` & `adafri-0.0.79/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/adafri.egg-info/SOURCES.txt` & `adafri-0.0.79/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.78/setup.py` & `adafri-0.0.79/setup.py`

 * *Files identical despite different names*

