# Comparing `tmp/amazon_ad_sdk-0.2.7.tar.gz` & `tmp/amazon_ad_sdk-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_ad_sdk-0.2.7.tar", last modified: Wed Jun  7 09:13:36 2023, max compression
+gzip compressed data, was "dist/amazon_ad_sdk-0.2.8.tar", last modified: Mon Aug  7 03:19:56 2023, max compression
```

## Comparing `amazon_ad_sdk-0.2.7.tar` & `amazon_ad_sdk-0.2.8.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/
--rw-r--r--   0 linrenwei   (501) staff       (20)     1068 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/LICENSE
--rw-r--r--   0 linrenwei   (501) staff       (20)      242 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/PKG-INFO
--rw-r--r--   0 linrenwei   (501) staff       (20)     1733 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/README.md
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad/
--rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/__init__.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/
--rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/__init__.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/amazon_attribution/
--rw-r--r--   0 linrenwei   (501) staff       (20)        0 2022-08-24 08:21:26.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/amazon_attribution/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      338 2022-08-24 08:56:49.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/amazon_attribution/advertisers.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      334 2022-08-24 08:57:59.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/amazon_attribution/publishers.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     1963 2022-08-24 08:53:29.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/amazon_attribution/reports.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      761 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/auth.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     2638 2023-03-30 12:04:03.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/base.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/dsp/
--rw-r--r--   0 linrenwei   (501) staff       (20)        0 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/dsp/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)    29048 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/dsp/report.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     1323 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/profiles.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     1052 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/report.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/sb/
--rw-r--r--   0 linrenwei   (501) staff       (20)       64 2023-06-07 06:33:01.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/sb/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      503 2022-02-23 08:45:10.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/sb/campaigns.py
--rw-r--r--   0 linrenwei   (501) staff       (20)    58157 2023-06-07 08:37:07.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/sb/report.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/sd/
--rw-r--r--   0 linrenwei   (501) staff       (20)       46 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/sd/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)    40139 2022-10-13 12:52:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/sd/report.py
--rw-r--r--   0 linrenwei   (501) staff       (20)    26080 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/sd/scripts.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/sp/
--rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/sp/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)    27147 2022-03-21 12:32:00.000000 amazon_ad_sdk-0.2.7/amazon_ad/api/sp/report.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad/api_v3/
--rw-r--r--   0 linrenwei   (501) staff       (20)        0 2022-08-17 09:27:17.000000 amazon_ad_sdk-0.2.7/amazon_ad/api_v3/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)    25502 2023-06-07 03:33:10.000000 amazon_ad_sdk-0.2.7/amazon_ad/api_v3/adapters.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      742 2022-08-17 09:31:44.000000 amazon_ad_sdk-0.2.7/amazon_ad/api_v3/base.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      850 2022-08-18 06:39:58.000000 amazon_ad_sdk-0.2.7/amazon_ad/api_v3/report.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad/api_v3/sb/
--rw-r--r--   0 linrenwei   (501) staff       (20)        0 2022-08-23 05:40:22.000000 amazon_ad_sdk-0.2.7/amazon_ad/api_v3/sb/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      846 2022-08-23 08:33:25.000000 amazon_ad_sdk-0.2.7/amazon_ad/api_v3/sb/report.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad/api_v3/sp/
--rw-r--r--   0 linrenwei   (501) staff       (20)       24 2022-08-17 11:44:06.000000 amazon_ad_sdk-0.2.7/amazon_ad/api_v3/sp/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     5308 2022-08-24 11:51:06.000000 amazon_ad_sdk-0.2.7/amazon_ad/api_v3/sp/report.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad/client/
--rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/client/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     1319 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/client/auth.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     8080 2022-08-24 08:18:35.000000 amazon_ad_sdk-0.2.7/amazon_ad/client/base.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     4861 2022-09-19 06:11:33.000000 amazon_ad_sdk-0.2.7/amazon_ad/client/service.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad/core/
--rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/core/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     1437 2023-03-30 12:06:22.000000 amazon_ad_sdk-0.2.7/amazon_ad/core/consts.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     2091 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/core/exceptions.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad/core/utils/
--rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/core/utils/__init__.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      893 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/core/utils/amazon.py
--rw-r--r--   0 linrenwei   (501) staff       (20)      534 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/core/utils/serialize.py
--rw-r--r--   0 linrenwei   (501) staff       (20)     1141 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.7/amazon_ad/core/utils/text.py
-drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad_sdk.egg-info/
--rw-r--r--   0 linrenwei   (501) staff       (20)      242 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad_sdk.egg-info/PKG-INFO
--rw-r--r--   0 linrenwei   (501) staff       (20)     1369 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 linrenwei   (501) staff       (20)        1 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 linrenwei   (501) staff       (20)      158 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad_sdk.egg-info/requires.txt
--rw-r--r--   0 linrenwei   (501) staff       (20)       10 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/amazon_ad_sdk.egg-info/top_level.txt
--rw-r--r--   0 linrenwei   (501) staff       (20)       38 2023-06-07 09:13:36.000000 amazon_ad_sdk-0.2.7/setup.cfg
--rw-r--r--   0 linrenwei   (501) staff       (20)     1067 2023-06-07 09:12:33.000000 amazon_ad_sdk-0.2.7/setup.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1068 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/LICENSE
+-rw-r--r--   0 linrenwei   (501) staff       (20)      242 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/PKG-INFO
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1733 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/README.md
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/__init__.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/__init__.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/amazon_attribution/
+-rw-r--r--   0 linrenwei   (501) staff       (20)        0 2022-08-24 08:21:26.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/amazon_attribution/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      338 2022-08-24 08:56:49.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/amazon_attribution/advertisers.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      334 2022-08-24 08:57:59.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/amazon_attribution/publishers.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1963 2022-08-24 08:53:29.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/amazon_attribution/reports.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      761 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/auth.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     2638 2023-03-30 12:04:03.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/base.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/dsp/
+-rw-r--r--   0 linrenwei   (501) staff       (20)        0 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/dsp/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)    29048 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/dsp/report.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1323 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/profiles.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1052 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/report.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/sb/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       64 2023-06-07 06:33:01.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/sb/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      503 2022-02-23 08:45:10.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/sb/campaigns.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)    58157 2023-06-07 08:37:07.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/sb/report.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/sd/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       46 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/sd/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)    40139 2022-10-13 12:52:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/sd/report.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)    26080 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/sd/scripts.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/sp/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/sp/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)    27147 2022-03-21 12:32:00.000000 amazon_ad_sdk-0.2.8/amazon_ad/api/sp/report.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad/api_v3/
+-rw-r--r--   0 linrenwei   (501) staff       (20)        0 2022-08-17 09:27:17.000000 amazon_ad_sdk-0.2.8/amazon_ad/api_v3/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)    25502 2023-06-07 03:33:10.000000 amazon_ad_sdk-0.2.8/amazon_ad/api_v3/adapters.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      742 2022-08-17 09:31:44.000000 amazon_ad_sdk-0.2.8/amazon_ad/api_v3/base.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      850 2022-08-18 06:39:58.000000 amazon_ad_sdk-0.2.8/amazon_ad/api_v3/report.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad/api_v3/sb/
+-rw-r--r--   0 linrenwei   (501) staff       (20)        0 2022-08-23 05:40:22.000000 amazon_ad_sdk-0.2.8/amazon_ad/api_v3/sb/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      846 2022-08-23 08:33:25.000000 amazon_ad_sdk-0.2.8/amazon_ad/api_v3/sb/report.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad/api_v3/sp/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       24 2022-08-17 11:44:06.000000 amazon_ad_sdk-0.2.8/amazon_ad/api_v3/sp/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     5308 2022-08-24 11:51:06.000000 amazon_ad_sdk-0.2.8/amazon_ad/api_v3/sp/report.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad/client/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/client/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1319 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/client/auth.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     8080 2022-08-24 08:18:35.000000 amazon_ad_sdk-0.2.8/amazon_ad/client/base.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     4861 2022-09-19 06:11:33.000000 amazon_ad_sdk-0.2.8/amazon_ad/client/service.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad/core/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/core/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1437 2023-03-30 12:06:22.000000 amazon_ad_sdk-0.2.8/amazon_ad/core/consts.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     2091 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/core/exceptions.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad/core/utils/
+-rw-r--r--   0 linrenwei   (501) staff       (20)       64 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/core/utils/__init__.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      893 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/core/utils/amazon.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)      534 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/core/utils/serialize.py
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1141 2021-11-23 02:07:40.000000 amazon_ad_sdk-0.2.8/amazon_ad/core/utils/text.py
+drwxr-xr-x   0 linrenwei   (501) staff       (20)        0 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad_sdk.egg-info/
+-rw-r--r--   0 linrenwei   (501) staff       (20)      242 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1369 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 linrenwei   (501) staff       (20)        1 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 linrenwei   (501) staff       (20)      158 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad_sdk.egg-info/requires.txt
+-rw-r--r--   0 linrenwei   (501) staff       (20)       10 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/amazon_ad_sdk.egg-info/top_level.txt
+-rw-r--r--   0 linrenwei   (501) staff       (20)       38 2023-08-07 03:19:56.000000 amazon_ad_sdk-0.2.8/setup.cfg
+-rw-r--r--   0 linrenwei   (501) staff       (20)     1067 2023-08-07 03:18:56.000000 amazon_ad_sdk-0.2.8/setup.py
```

### Comparing `amazon_ad_sdk-0.2.7/LICENSE` & `amazon_ad_sdk-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/README.md` & `amazon_ad_sdk-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api/amazon_attribution/reports.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api/amazon_attribution/reports.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api/auth.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api/auth.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api/base.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api/base.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api/dsp/report.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api/dsp/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api/profiles.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api/profiles.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api/report.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api/sb/report.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api/sb/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api/sd/report.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api/sd/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api/sd/scripts.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api/sd/scripts.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api/sp/report.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api/sp/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api_v3/adapters.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api_v3/adapters.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api_v3/base.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api_v3/base.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api_v3/report.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api_v3/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api_v3/sb/report.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api_v3/sb/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/api_v3/sp/report.py` & `amazon_ad_sdk-0.2.8/amazon_ad/api_v3/sp/report.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/client/auth.py` & `amazon_ad_sdk-0.2.8/amazon_ad/client/auth.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/client/base.py` & `amazon_ad_sdk-0.2.8/amazon_ad/client/base.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/client/service.py` & `amazon_ad_sdk-0.2.8/amazon_ad/client/service.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/core/consts.py` & `amazon_ad_sdk-0.2.8/amazon_ad/core/consts.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/core/exceptions.py` & `amazon_ad_sdk-0.2.8/amazon_ad/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/core/utils/amazon.py` & `amazon_ad_sdk-0.2.8/amazon_ad/core/utils/amazon.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/core/utils/serialize.py` & `amazon_ad_sdk-0.2.8/amazon_ad/core/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad/core/utils/text.py` & `amazon_ad_sdk-0.2.8/amazon_ad/core/utils/text.py`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/amazon_ad_sdk.egg-info/SOURCES.txt` & `amazon_ad_sdk-0.2.8/amazon_ad_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon_ad_sdk-0.2.7/setup.py` & `amazon_ad_sdk-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='amazon_ad_sdk',
-    version='0.2.7',
+    version='0.2.8',
     packages=['amazon_ad',
               'amazon_ad.api',
               'amazon_ad.api.sb',
               'amazon_ad.api.sp',
               'amazon_ad.api.sd',
               'amazon_ad.api.dsp',
               'amazon_ad.api.amazon_attribution',
```

