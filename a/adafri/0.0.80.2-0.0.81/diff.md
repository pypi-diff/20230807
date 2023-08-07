# Comparing `tmp/adafri-0.0.80.2.tar.gz` & `tmp/adafri-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.80.2.tar", last modified: Mon Aug  7 05:59:32 2023, max compression
+gzip compressed data, was "adafri-0.0.81.tar", last modified: Mon Aug  7 06:02:02 2023, max compression
```

## Comparing `adafri-0.0.80.2.tar` & `adafri-0.0.81.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.972013 adafri-0.0.80.2/
--rw-r--r--   0 ibrahima   (502) staff       (20)      179 2023-08-07 05:59:32.971507 adafri-0.0.80.2/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.914523 adafri-0.0.80.2/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       82 2023-08-07 05:59:29.000000 adafri-0.0.80.2/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.923146 adafri-0.0.80.2/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.80.2/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.80.2/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.80.2/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1356 2023-07-31 01:55:04.000000 adafri-0.0.80.2/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    19215 2023-08-07 05:42:43.000000 adafri-0.0.80.2/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.924578 adafri-0.0.80.2/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.80.2/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.925722 adafri-0.0.80.2/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.80.2/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.928817 adafri-0.0.80.2/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.80.2/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.80.2/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.80.2/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.929989 adafri-0.0.80.2/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.80.2/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.931628 adafri-0.0.80.2/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.80.2/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.80.2/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.932937 adafri-0.0.80.2/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.80.2/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.933818 adafri-0.0.80.2/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      965 2023-07-28 08:17:28.000000 adafri-0.0.80.2/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.948256 adafri-0.0.80.2/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.80.2/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7216 2023-08-07 05:09:25.000000 adafri-0.0.80.2/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.80.2/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6540 2023-08-07 05:08:57.000000 adafri-0.0.80.2/adafri/v1/auth/oauth/models/code.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2505 2023-07-31 01:28:33.000000 adafri-0.0.80.2/adafri/v1/auth/oauth/models/code_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16152 2023-08-07 05:07:34.000000 adafri-0.0.80.2/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.80.2/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9460 2023-08-07 05:08:18.000000 adafri-0.0.80.2/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.80.2/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.951392 adafri-0.0.80.2/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.80.2/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.80.2/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.80.2/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.957723 adafri-0.0.80.2/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.80.2/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.80.2/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.958468 adafri-0.0.80.2/adafri/v1/mailing/
--rw-r--r--   0 ibrahima   (502) staff       (20)    11395 2023-08-07 05:59:00.000000 adafri-0.0.80.2/adafri/v1/mailing/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.959153 adafri-0.0.80.2/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.80.2/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.970159 adafri-0.0.80.2/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.80.2/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11720 2023-08-07 04:48:08.000000 adafri-0.0.80.2/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.80.2/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 05:59:32.917771 adafri-0.0.80.2/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      179 2023-08-07 05:59:32.000000 adafri-0.0.80.2/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-08-07 05:59:32.000000 adafri-0.0.80.2/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-08-07 05:59:32.000000 adafri-0.0.80.2/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-08-07 05:59:32.000000 adafri-0.0.80.2/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-08-07 05:59:32.972175 adafri-0.0.80.2/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.80.2/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.685386 adafri-0.0.81/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-07 06:02:02.684861 adafri-0.0.81/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.598083 adafri-0.0.81/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-08-07 06:01:59.000000 adafri-0.0.81/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.626909 adafri-0.0.81/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.81/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.81/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.81/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1356 2023-07-31 01:55:04.000000 adafri-0.0.81/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    19215 2023-08-07 05:42:43.000000 adafri-0.0.81/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.628239 adafri-0.0.81/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.81/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.633731 adafri-0.0.81/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.81/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.653547 adafri-0.0.81/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.81/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.81/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.81/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.655673 adafri-0.0.81/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.81/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.657744 adafri-0.0.81/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.81/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.81/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.659137 adafri-0.0.81/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.81/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.659730 adafri-0.0.81/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      965 2023-07-28 08:17:28.000000 adafri-0.0.81/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.671281 adafri-0.0.81/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.81/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7216 2023-08-07 05:09:25.000000 adafri-0.0.81/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.81/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6540 2023-08-07 05:08:57.000000 adafri-0.0.81/adafri/v1/auth/oauth/models/code.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2505 2023-07-31 01:28:33.000000 adafri-0.0.81/adafri/v1/auth/oauth/models/code_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16152 2023-08-07 05:07:34.000000 adafri-0.0.81/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.81/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9460 2023-08-07 05:08:18.000000 adafri-0.0.81/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.81/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.675113 adafri-0.0.81/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.81/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.81/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.81/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.677873 adafri-0.0.81/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.81/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.81/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.678752 adafri-0.0.81/adafri/v1/mailing/
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11407 2023-08-07 06:01:46.000000 adafri-0.0.81/adafri/v1/mailing/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.679710 adafri-0.0.81/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.81/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.683383 adafri-0.0.81/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.81/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11720 2023-08-07 04:48:08.000000 adafri-0.0.81/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.81/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-07 06:02:02.608172 adafri-0.0.81/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-07 06:02:02.000000 adafri-0.0.81/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-08-07 06:02:02.000000 adafri-0.0.81/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-08-07 06:02:02.000000 adafri-0.0.81/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-08-07 06:02:02.000000 adafri-0.0.81/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-08-07 06:02:02.685624 adafri-0.0.81/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.81/setup.py
```

### Comparing `adafri-0.0.80.2/adafri/utils/country.py` & `adafri-0.0.81/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/utils/phone_number.py` & `adafri-0.0.81/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/utils/response.py` & `adafri-0.0.81/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/utils/utils.py` & `adafri-0.0.81/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/account/models/account.py` & `adafri-0.0.81/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/account/models/account_fields.py` & `adafri-0.0.81/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.81/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.81/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.81/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.81/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/auth/oauth/models/code.py` & `adafri-0.0.81/adafri/v1/auth/oauth/models/code.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/auth/oauth/models/code_fields.py` & `adafri-0.0.81/adafri/v1/auth/oauth/models/code_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.81/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.81/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.81/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.81/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.81/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.81/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/base/firebase_collection.py` & `adafri-0.0.81/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/mailing/__init__.py` & `adafri-0.0.81/adafri/v1/mailing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         uid = user_model.uid;
         code = str(generate_random_code());
         model_ = {
             "target": uid,
             "code_type": "email_validation",
             "code": code
         }
-        id = Code(Code.generate(**model_).data).id
+        id = getattr(Code.generate(**model_).data, 'id',None);
         code_model = Code();
         code_model.id = id;
         code_model.code = code;
         code_model.code_type = 'email_validation'
         code_model.expires_in = 600
         code_model.target = uid;
         code = code_model.getCode();
```

### Comparing `adafri-0.0.80.2/adafri/v1/user/models/user.py` & `adafri-0.0.81/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri/v1/user/models/user_fields.py` & `adafri-0.0.81/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/adafri.egg-info/SOURCES.txt` & `adafri-0.0.81/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.80.2/setup.py` & `adafri-0.0.81/setup.py`

 * *Files identical despite different names*

