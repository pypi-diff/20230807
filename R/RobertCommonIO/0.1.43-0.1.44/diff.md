# Comparing `tmp/RobertCommonIO-0.1.43.tar.gz` & `tmp/RobertCommonIO-0.1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonIO-0.1.43.tar", last modified: Tue Aug  1 09:28:36 2023, max compression
+gzip compressed data, was "RobertCommonIO-0.1.44.tar", last modified: Mon Aug  7 14:32:26 2023, max compression
```

## Comparing `RobertCommonIO-0.1.43.tar` & `RobertCommonIO-0.1.44.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.958694 RobertCommonIO-0.1.43/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonIO-0.1.43/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonIO-0.1.43/MANIFEST.in
--rw-rw-rw-   0        0        0      878 2023-08-01 09:28:36.958694 RobertCommonIO-0.1.43/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-06-02 07:57:14.000000 RobertCommonIO-0.1.43/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.913441 RobertCommonIO-0.1.43/RobertCommonIO.egg-info/
--rw-rw-rw-   0        0        0      878 2023-08-01 09:28:36.000000 RobertCommonIO-0.1.43/RobertCommonIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-08-01 09:28:36.000000 RobertCommonIO-0.1.43/RobertCommonIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 09:28:36.000000 RobertCommonIO-0.1.43/RobertCommonIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      262 2023-08-01 09:28:36.000000 RobertCommonIO-0.1.43/RobertCommonIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-08-01 09:28:36.000000 RobertCommonIO-0.1.43/RobertCommonIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      288 2023-08-01 09:17:21.000000 RobertCommonIO-0.1.43/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.914437 RobertCommonIO-0.1.43/robertcommonio/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonIO-0.1.43/robertcommonio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.915439 RobertCommonIO-0.1.43/robertcommonio/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.43/robertcommonio/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.934496 RobertCommonIO-0.1.43/robertcommonio/system/io/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/__init__.py
--rw-rw-rw-   0        0        0    19301 2023-06-13 02:16:52.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/data_storage.py
--rw-rw-rw-   0        0        0     3380 2023-06-13 06:54:18.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/email.py
--rw-rw-rw-   0        0        0     7388 2023-04-19 09:38:00.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/file.py
--rw-rw-rw-   0        0        0     6347 2022-10-09 08:05:49.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/ftp.py
--rw-rw-rw-   0        0        0    10214 2023-02-21 02:59:34.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/http.py
--rw-rw-rw-   0        0        0     3390 2023-08-01 09:18:07.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/ini.py
--rw-rw-rw-   0        0        0     4351 2023-08-01 09:23:18.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/job.py
--rw-rw-rw-   0        0        0     6566 2022-11-24 06:58:34.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/license.py
--rw-rw-rw-   0        0        0    27527 2023-06-13 02:37:00.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/mongo.py
--rw-rw-rw-   0        0        0     7107 2023-08-01 09:27:32.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/mqtt.py
--rw-rw-rw-   0        0        0     6535 2023-01-04 05:46:19.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/mysql.py
--rw-rw-rw-   0        0        0     3900 2022-11-22 07:50:13.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/oss.py
--rw-rw-rw-   0        0        0    19915 2023-06-13 09:03:21.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/rabitmq.py
--rw-rw-rw-   0        0        0    11702 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/redis.py
--rw-rw-rw-   0        0        0     2267 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/redis_cache.py
--rw-rw-rw-   0        0        0     9779 2023-05-25 09:55:20.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/response.py
--rw-rw-rw-   0        0        0    37671 2023-08-01 09:13:24.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/socket.py
--rw-rw-rw-   0        0        0     7306 2023-06-13 02:14:30.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/sqlalche.py
--rw-rw-rw-   0        0        0     6710 2022-11-22 07:58:41.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/transport.py
--rw-rw-rw-   0        0        0      725 2022-12-14 08:37:33.000000 RobertCommonIO-0.1.43/robertcommonio/system/io/version.py
--rw-rw-rw-   0        0        0       42 2023-08-01 09:28:36.958694 RobertCommonIO-0.1.43/setup.cfg
--rw-rw-rw-   0        0        0     3869 2023-08-01 09:18:29.000000 RobertCommonIO-0.1.43/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.935446 RobertCommonIO-0.1.43/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonIO-0.1.43/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.936444 RobertCommonIO-0.1.43/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonIO-0.1.43/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:28:36.957696 RobertCommonIO-0.1.43/tests/test_system/test_io/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:50:10.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-01-04 02:27:37.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test.py
--rw-rw-rw-   0        0        0     1570 2023-01-05 05:43:17.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_data_storage.py
--rw-rw-rw-   0        0        0    14345 2023-06-06 02:41:30.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_email.py
--rw-rw-rw-   0        0        0     3985 2022-07-11 02:23:20.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_file.py
--rw-rw-rw-   0        0        0      978 2022-05-25 08:49:17.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_ftp.py
--rw-rw-rw-   0        0        0      570 2023-07-10 09:37:45.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_http.py
--rw-rw-rw-   0        0        0      413 2022-01-13 06:50:54.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_ini.py
--rw-rw-rw-   0        0        0      381 2023-06-13 07:55:37.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_job.py
--rw-rw-rw-   0        0        0     1187 2023-03-09 08:37:11.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_license.py
--rw-rw-rw-   0        0        0     3141 2023-04-04 06:18:30.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_mongo.py
--rw-rw-rw-   0        0        0     1582 2022-04-20 08:37:11.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_mqtt.py
--rw-rw-rw-   0        0        0    10544 2021-12-24 13:47:06.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_oracle.py
--rw-rw-rw-   0        0        0     1028 2022-09-07 06:12:44.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_rabbitmq.py
--rw-rw-rw-   0        0        0     4221 2022-10-09 07:39:57.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_socket.py
--rw-rw-rw-   0        0        0     3967 2023-06-02 08:41:38.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_sqlalche.py
--rw-rw-rw-   0        0        0     1389 2022-10-13 09:07:08.000000 RobertCommonIO-0.1.43/tests/test_system/test_io/test_transport.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:32:26.483955 RobertCommonIO-0.1.44/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonIO-0.1.44/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonIO-0.1.44/MANIFEST.in
+-rw-rw-rw-   0        0        0      878 2023-08-07 14:32:26.482944 RobertCommonIO-0.1.44/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-06-02 07:57:14.000000 RobertCommonIO-0.1.44/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 14:32:26.414998 RobertCommonIO-0.1.44/RobertCommonIO.egg-info/
+-rw-rw-rw-   0        0        0      878 2023-08-07 14:32:26.000000 RobertCommonIO-0.1.44/RobertCommonIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-08-07 14:32:26.000000 RobertCommonIO-0.1.44/RobertCommonIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 14:32:26.000000 RobertCommonIO-0.1.44/RobertCommonIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      262 2023-08-07 14:32:26.000000 RobertCommonIO-0.1.44/RobertCommonIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-08-07 14:32:26.000000 RobertCommonIO-0.1.44/RobertCommonIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      288 2023-08-01 09:17:21.000000 RobertCommonIO-0.1.44/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 14:32:26.420390 RobertCommonIO-0.1.44/robertcommonio/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonIO-0.1.44/robertcommonio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:32:26.421393 RobertCommonIO-0.1.44/robertcommonio/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.44/robertcommonio/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:32:26.455141 RobertCommonIO-0.1.44/robertcommonio/system/io/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/__init__.py
+-rw-rw-rw-   0        0        0    19301 2023-06-13 02:16:52.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/data_storage.py
+-rw-rw-rw-   0        0        0     3380 2023-06-13 06:54:18.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/email.py
+-rw-rw-rw-   0        0        0     7388 2023-04-19 09:38:00.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/file.py
+-rw-rw-rw-   0        0        0     6347 2022-10-09 08:05:49.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/ftp.py
+-rw-rw-rw-   0        0        0    10214 2023-02-21 02:59:34.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/http.py
+-rw-rw-rw-   0        0        0     3390 2023-08-01 09:18:07.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/ini.py
+-rw-rw-rw-   0        0        0     4351 2023-08-01 09:23:18.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/job.py
+-rw-rw-rw-   0        0        0     6566 2022-11-24 06:58:34.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/license.py
+-rw-rw-rw-   0        0        0    27527 2023-06-13 02:37:00.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/mongo.py
+-rw-rw-rw-   0        0        0     7107 2023-08-01 09:27:32.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/mqtt.py
+-rw-rw-rw-   0        0        0     6535 2023-01-04 05:46:19.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/mysql.py
+-rw-rw-rw-   0        0        0     3900 2022-11-22 07:50:13.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/oss.py
+-rw-rw-rw-   0        0        0    19915 2023-06-13 09:03:21.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/rabitmq.py
+-rw-rw-rw-   0        0        0    11702 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/redis.py
+-rw-rw-rw-   0        0        0     2267 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/redis_cache.py
+-rw-rw-rw-   0        0        0     9779 2023-05-25 09:55:20.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/response.py
+-rw-rw-rw-   0        0        0    37671 2023-08-07 14:31:13.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/socket.py
+-rw-rw-rw-   0        0        0     7899 2023-08-07 14:24:30.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/sqlalche.py
+-rw-rw-rw-   0        0        0     6710 2022-11-22 07:58:41.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/transport.py
+-rw-rw-rw-   0        0        0      725 2022-12-14 08:37:33.000000 RobertCommonIO-0.1.44/robertcommonio/system/io/version.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 14:32:26.483955 RobertCommonIO-0.1.44/setup.cfg
+-rw-rw-rw-   0        0        0     3869 2023-08-07 14:32:03.000000 RobertCommonIO-0.1.44/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:32:26.457141 RobertCommonIO-0.1.44/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonIO-0.1.44/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:32:26.457141 RobertCommonIO-0.1.44/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonIO-0.1.44/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:32:26.481944 RobertCommonIO-0.1.44/tests/test_system/test_io/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:50:10.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-01-04 02:27:37.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test.py
+-rw-rw-rw-   0        0        0     1570 2023-01-05 05:43:17.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_data_storage.py
+-rw-rw-rw-   0        0        0    14345 2023-06-06 02:41:30.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_email.py
+-rw-rw-rw-   0        0        0     3985 2022-07-11 02:23:20.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_file.py
+-rw-rw-rw-   0        0        0      978 2022-05-25 08:49:17.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_ftp.py
+-rw-rw-rw-   0        0        0      570 2023-07-10 09:37:45.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_http.py
+-rw-rw-rw-   0        0        0      413 2022-01-13 06:50:54.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_ini.py
+-rw-rw-rw-   0        0        0      381 2023-06-13 07:55:37.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_job.py
+-rw-rw-rw-   0        0        0     1187 2023-03-09 08:37:11.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_license.py
+-rw-rw-rw-   0        0        0     3141 2023-04-04 06:18:30.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_mongo.py
+-rw-rw-rw-   0        0        0     1582 2022-04-20 08:37:11.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_mqtt.py
+-rw-rw-rw-   0        0        0    10544 2021-12-24 13:47:06.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_oracle.py
+-rw-rw-rw-   0        0        0     1028 2022-09-07 06:12:44.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_rabbitmq.py
+-rw-rw-rw-   0        0        0     4221 2022-10-09 07:39:57.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_socket.py
+-rw-rw-rw-   0        0        0     3967 2023-06-02 08:41:38.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_sqlalche.py
+-rw-rw-rw-   0        0        0     1389 2022-10-13 09:07:08.000000 RobertCommonIO-0.1.44/tests/test_system/test_io/test_transport.py
```

### Comparing `RobertCommonIO-0.1.43/LICENSE` & `RobertCommonIO-0.1.44/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/PKG-INFO` & `RobertCommonIO-0.1.44/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonIO
-Version: 0.1.43
+Version: 0.1.44
 Summary: Robert Common IO Library
 Home-page: https://github.com/hun0423/RobertCommonIO
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonIO-0.1.43/RobertCommonIO.egg-info/PKG-INFO` & `RobertCommonIO-0.1.44/RobertCommonIO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonIO
-Version: 0.1.43
+Version: 0.1.44
 Summary: Robert Common IO Library
 Home-page: https://github.com/hun0423/RobertCommonIO
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonIO-0.1.43/RobertCommonIO.egg-info/SOURCES.txt` & `RobertCommonIO-0.1.44/RobertCommonIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/data_storage.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/data_storage.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/email.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/email.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/file.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/ftp.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/ftp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/http.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/http.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/ini.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/ini.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/job.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/job.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/license.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/license.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/mongo.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/mongo.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/mqtt.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/mqtt.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/mysql.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/mysql.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/oss.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/oss.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/rabitmq.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/rabitmq.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/redis.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/redis.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/redis_cache.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/redis_cache.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/response.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/response.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/socket.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/socket.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/sqlalche.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/sqlalche.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from sqlalchemy.ext.declarative import declarative_base
 
 
 class SQLAlCheAccessor:
 
     def __init__(self):
         self.engine: dict = {}
+        self.engine_factory: dict = {}
 
     def add_engine(self, engine_name: str, engine_conn: str, engine_pool_class: Any = QueuePool, engine_pool_recycle: int = 60, text_factory: Optional[Any] = None, **kwargs):
         """
                 添加一个数据库连接池
                 quote_plus(psw)
                 @Example:
                     PostgreSQL
@@ -50,20 +51,27 @@
 
             """
         if engine_name not in self.engine.keys():
             engine = create_engine(engine_conn, poolclass=engine_pool_class, pool_recycle=engine_pool_recycle, **kwargs)
             if engine:
                 if text_factory is not None:
                     engine.raw_connection().connection.text_factory = text_factory
+                    engine.connect().connection.connection.text_factory = text_factory
+                self.engine_factory[engine_name] = text_factory
                 self.engine[engine_name] = engine
         return self.engine.get(engine_name)
 
     def get_engine(self, engine_name: str):
         return self.engine.get(engine_name)
 
+    def check_text_factory(self, engine_name: str, conn):
+        text_factory = self.engine_factory.get(engine_name)
+        if text_factory is not None and conn.connection.connection.text_factory != text_factory:
+            conn.connection.connection.text_factory = text_factory
+
     def to_dict(self, records: Union[List[Optional[Dict]], Dict]):
         if isinstance(records, Dict):
             values = {}
             for k, v in records.items():
                 values[k] = v
             return values
         elif isinstance(records, List):
@@ -74,21 +82,23 @@
                     value[k] = v
                 values.append(value)
             return values
         return records
 
     def read_sql(self, engine_name: str, sql_cmd: str, to_dict: bool = True):
         with self.get_engine(engine_name).connect() as conn:
+            self.check_text_factory(engine_name, conn)
             records = conn.execute(sql_cmd).mappings().all()
             if to_dict is True:
                 return self.to_dict(records)
             return records
 
     def read_sql_dataframe(self, engine_name: str, sql_cmd: str):
         with self.get_engine(engine_name).connect() as conn:
+            self.check_text_factory(engine_name, conn)
             return pd.read_sql_query(sql_cmd, conn)
 
     def execute_sql(self, engine_name: str, sql_cmd: str, params: Optional[list] = None):
         with self.get_engine(engine_name).connect() as conn:
             return conn.execute(text(sql_cmd), params).rowcount
 
     def execute_multi_sql(self, engine_name: str, cmd_tuple: list):
```

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/transport.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/transport.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/robertcommonio/system/io/version.py` & `RobertCommonIO-0.1.44/robertcommonio/system/io/version.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/setup.py` & `RobertCommonIO-0.1.44/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonIO'
 DESCRIPTION = 'Robert Common IO Library'
 URL = 'https://github.com/hun0423/RobertCommonIO'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.43'
-DATE = '2023-08-01'
+VERSION = '0.1.44'
+DATE = '2023-08-07'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonIO-0.1.43/tests/test_system/test_io/test.py` & `RobertCommonIO-0.1.44/tests/test_system/test_io/test.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/tests/test_system/test_io/test_data_storage.py` & `RobertCommonIO-0.1.44/tests/test_system/test_io/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/tests/test_system/test_io/test_email.py` & `RobertCommonIO-0.1.44/tests/test_system/test_io/test_email.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/tests/test_system/test_io/test_file.py` & `RobertCommonIO-0.1.44/tests/test_system/test_io/test_file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/tests/test_system/test_io/test_ftp.py` & `RobertCommonIO-0.1.44/tests/test_system/test_io/test_ftp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/tests/test_system/test_io/test_http.py` & `RobertCommonIO-0.1.44/tests/test_system/test_io/test_http.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/tests/test_system/test_io/test_license.py` & `RobertCommonIO-0.1.44/tests/test_system/test_io/test_license.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/tests/test_system/test_io/test_mongo.py` & `RobertCommonIO-0.1.44/tests/test_system/test_io/test_mongo.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/tests/test_system/test_io/test_mqtt.py` & `RobertCommonIO-0.1.44/tests/test_system/test_io/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/tests/test_system/test_io/test_oracle.py` & `RobertCommonIO-0.1.44/tests/test_system/test_io/test_oracle.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/tests/test_system/test_io/test_rabbitmq.py` & `RobertCommonIO-0.1.44/tests/test_system/test_io/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/tests/test_system/test_io/test_socket.py` & `RobertCommonIO-0.1.44/tests/test_system/test_io/test_socket.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/tests/test_system/test_io/test_sqlalche.py` & `RobertCommonIO-0.1.44/tests/test_system/test_io/test_sqlalche.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.43/tests/test_system/test_io/test_transport.py` & `RobertCommonIO-0.1.44/tests/test_system/test_io/test_transport.py`

 * *Files identical despite different names*

