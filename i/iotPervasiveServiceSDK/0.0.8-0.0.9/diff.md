# Comparing `tmp/iotPervasiveServiceSDK-0.0.8.tar.gz` & `tmp/iotPervasiveServiceSDK-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iotPervasiveServiceSDK-0.0.8.tar", last modified: Mon Aug  7 08:01:38 2023, max compression
+gzip compressed data, was "dist\iotPervasiveServiceSDK-0.0.9.tar", last modified: Mon Aug  7 08:10:22 2023, max compression
```

## Comparing `iotPervasiveServiceSDK-0.0.8.tar` & `iotPervasiveServiceSDK-0.0.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/
--rw-rw-rw-   0        0        0    11357 2023-08-02 09:48:52.000000 iotPervasiveServiceSDK-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       68 2023-08-03 06:38:15.000000 iotPervasiveServiceSDK-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      564 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-08-02 10:00:57.000000 iotPervasiveServiceSDK-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/
--rw-rw-rw-   0        0        0      123 2023-08-03 06:44:05.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/__init__.py
--rw-rw-rw-   0        0        0     2315 2023-08-03 10:06:05.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/config.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/
--rw-rw-rw-   0        0        0     1243 2023-08-06 08:33:51.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/applicationContext.py
--rw-rw-rw-   0        0        0     3414 2023-08-04 05:44:12.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/eventInvoker.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/exception/
--rw-rw-rw-   0        0        0      176 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/exception/commonException.py
--rw-rw-rw-   0        0        0        0 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/exception/sdkException.py
--rw-rw-rw-   0        0        0     2327 2023-07-24 10:35:34.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/exception/serviceException.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/job/
--rw-rw-rw-   0        0        0      905 2023-07-20 08:12:22.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/job/contextUpLoadJob.py
--rw-rw-rw-   0        0        0      475 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/job/eventListenerJob.py
--rw-rw-rw-   0        0        0      271 2023-07-21 08:49:20.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/job/mqttCheckMessageJob.py
--rw-rw-rw-   0        0        0      256 2023-07-21 02:43:53.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/job/mqttHealthJob.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/loader/
--rw-rw-rw-   0        0        0     1380 2023-08-03 08:07:20.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/loader/hardwareInfoLoader.py
--rw-rw-rw-   0        0        0     1541 2023-08-03 07:49:26.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/loader/proxyLoader.py
--rw-rw-rw-   0        0        0     8275 2023-08-03 07:50:28.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/loader/serversLoader.py
--rw-rw-rw-   0        0        0      210 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/loader/thingProxyFuncLoader.py
--rw-rw-rw-   0        0        0     2303 2023-07-21 03:01:27.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/scheduleService.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/sender/
--rw-rw-rw-   0        0        0       67 2023-07-27 02:11:41.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/sender/baseSender.py
--rw-rw-rw-   0        0        0      369 2023-07-27 02:49:45.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/sender/hardwareUpLoadSender.py
--rw-rw-rw-   0        0        0     3642 2023-08-07 07:59:36.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/serverInvoker.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/factory/
--rw-rw-rw-   0        0        0      392 2023-06-15 10:40:11.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/factory/systemEventFactory.py
--rw-rw-rw-   0        0        0      690 2023-06-27 09:17:54.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/factory/systemServiceFactory.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/model/
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/model/ujinja/
--rw-rw-rw-   0        0        0     7700 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/model/ujinja/source.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/pojo/
--rw-rw-rw-   0        0        0      746 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/pojo/capabilityBean.py
--rw-rw-rw-   0        0        0      545 2023-06-12 06:53:14.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/pojo/eventBean.py
--rw-rw-rw-   0        0        0      892 2023-07-20 10:25:24.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/pojo/serviceBean.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/proxy/
--rw-rw-rw-   0        0        0      166 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/proxy/proxyBase.py
--rw-rw-rw-   0        0        0      696 2023-08-06 08:30:31.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/proxy/pythonServiceProxy.py
--rw-rw-rw-   0        0        0      589 2023-08-06 08:30:47.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/proxy/thingProxy.py
--rw-rw-rw-   0        0        0     4315 2023-08-03 10:10:09.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/proxySDK.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/router/
--rw-rw-rw-   0        0        0     1175 2023-08-03 08:02:13.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/router/httpRouter.py
--rw-rw-rw-   0        0        0     2996 2023-07-24 07:55:12.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/router/mqttRouter.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/systemService/
--rw-rw-rw-   0        0        0      153 2023-07-25 09:53:27.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/systemService/httpService.py
--rw-rw-rw-   0        0        0     3176 2023-07-25 14:18:36.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/systemService/mqttService.py
--rw-rw-rw-   0        0        0     3274 2023-07-24 08:17:36.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/systemService/updateService.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/
--rw-rw-rw-   0        0        0      191 2023-07-20 08:17:40.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/TimeUtil.py
--rw-rw-rw-   0        0        0      247 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/copyUtils.py
--rw-rw-rw-   0        0        0     1014 2023-07-26 10:19:45.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/fileUtils.py
--rw-rw-rw-   0        0        0      619 2023-07-24 07:47:42.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/logutil.py
--rw-rw-rw-   0        0        0     1304 2023-07-24 03:42:08.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/netUtils.py
--rw-rw-rw-   0        0        0      128 2023-07-24 08:13:35.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/pathUtils.py
--rw-rw-rw-   0        0        0      859 2023-07-24 07:35:22.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/tarGzUtils.py
--rw-rw-rw-   0        0        0     1441 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/taskUtils.py
--rw-rw-rw-   0        0        0      955 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/templateUtils.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK.egg-info/
--rw-rw-rw-   0        0        0      564 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2349 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       87 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1259 2023-08-07 08:01:06.000000 iotPervasiveServiceSDK-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/
+-rw-rw-rw-   0        0        0    11357 2023-08-02 09:48:52.000000 iotPervasiveServiceSDK-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       68 2023-08-03 06:38:15.000000 iotPervasiveServiceSDK-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      564 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-08-02 10:00:57.000000 iotPervasiveServiceSDK-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/
+-rw-rw-rw-   0        0        0      123 2023-08-03 06:44:05.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/__init__.py
+-rw-rw-rw-   0        0        0     2315 2023-08-03 10:06:05.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/config.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/
+-rw-rw-rw-   0        0        0     1243 2023-08-06 08:33:51.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/applicationContext.py
+-rw-rw-rw-   0        0        0     3454 2023-08-07 08:07:20.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/eventInvoker.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/exception/
+-rw-rw-rw-   0        0        0      176 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/exception/commonException.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/exception/sdkException.py
+-rw-rw-rw-   0        0        0     2327 2023-07-24 10:35:34.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/exception/serviceException.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/job/
+-rw-rw-rw-   0        0        0      925 2023-08-07 08:07:33.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/job/contextUpLoadJob.py
+-rw-rw-rw-   0        0        0      475 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/job/eventListenerJob.py
+-rw-rw-rw-   0        0        0      271 2023-07-21 08:49:20.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/job/mqttCheckMessageJob.py
+-rw-rw-rw-   0        0        0      256 2023-07-21 02:43:53.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/job/mqttHealthJob.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/loader/
+-rw-rw-rw-   0        0        0     1380 2023-08-03 08:07:20.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/loader/hardwareInfoLoader.py
+-rw-rw-rw-   0        0        0     1541 2023-08-03 07:49:26.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/loader/proxyLoader.py
+-rw-rw-rw-   0        0        0     8275 2023-08-03 07:50:28.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/loader/serversLoader.py
+-rw-rw-rw-   0        0        0      210 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/loader/thingProxyFuncLoader.py
+-rw-rw-rw-   0        0        0     2303 2023-07-21 03:01:27.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/scheduleService.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/sender/
+-rw-rw-rw-   0        0        0       67 2023-07-27 02:11:41.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/sender/baseSender.py
+-rw-rw-rw-   0        0        0      369 2023-07-27 02:49:45.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/sender/hardwareUpLoadSender.py
+-rw-rw-rw-   0        0        0     3820 2023-08-07 08:09:55.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/serverInvoker.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/factory/
+-rw-rw-rw-   0        0        0      392 2023-06-15 10:40:11.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/factory/systemEventFactory.py
+-rw-rw-rw-   0        0        0      690 2023-06-27 09:17:54.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/factory/systemServiceFactory.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/model/
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/model/ujinja/
+-rw-rw-rw-   0        0        0     7700 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/model/ujinja/source.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/pojo/
+-rw-rw-rw-   0        0        0      746 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/pojo/capabilityBean.py
+-rw-rw-rw-   0        0        0      545 2023-06-12 06:53:14.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/pojo/eventBean.py
+-rw-rw-rw-   0        0        0      892 2023-07-20 10:25:24.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/pojo/serviceBean.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/proxy/
+-rw-rw-rw-   0        0        0      166 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/proxy/proxyBase.py
+-rw-rw-rw-   0        0        0      696 2023-08-06 08:30:31.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/proxy/pythonServiceProxy.py
+-rw-rw-rw-   0        0        0      589 2023-08-06 08:30:47.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/proxy/thingProxy.py
+-rw-rw-rw-   0        0        0     4335 2023-08-07 08:07:09.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/proxySDK.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/router/
+-rw-rw-rw-   0        0        0     1195 2023-08-07 08:07:42.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/router/httpRouter.py
+-rw-rw-rw-   0        0        0     3036 2023-08-07 08:07:52.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/router/mqttRouter.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/systemService/
+-rw-rw-rw-   0        0        0      153 2023-07-25 09:53:27.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/systemService/httpService.py
+-rw-rw-rw-   0        0        0     3196 2023-08-07 08:07:56.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/systemService/mqttService.py
+-rw-rw-rw-   0        0        0     3274 2023-07-24 08:17:36.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/systemService/updateService.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/
+-rw-rw-rw-   0        0        0      191 2023-07-20 08:17:40.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/TimeUtil.py
+-rw-rw-rw-   0        0        0      247 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/copyUtils.py
+-rw-rw-rw-   0        0        0     1014 2023-07-26 10:19:45.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/fileUtils.py
+-rw-rw-rw-   0        0        0      619 2023-07-24 07:47:42.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/logutil.py
+-rw-rw-rw-   0        0        0     1304 2023-07-24 03:42:08.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/netUtils.py
+-rw-rw-rw-   0        0        0      128 2023-07-24 08:13:35.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/pathUtils.py
+-rw-rw-rw-   0        0        0      859 2023-07-24 07:35:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/tarGzUtils.py
+-rw-rw-rw-   0        0        0     1441 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/taskUtils.py
+-rw-rw-rw-   0        0        0      955 2023-06-07 09:59:47.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/templateUtils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK.egg-info/
+-rw-rw-rw-   0        0        0      564 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2349 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 08:01:38.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       87 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 08:10:22.000000 iotPervasiveServiceSDK-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1259 2023-08-07 08:10:08.000000 iotPervasiveServiceSDK-0.0.9/setup.py
```

### Comparing `iotPervasiveServiceSDK-0.0.8/LICENSE` & `iotPervasiveServiceSDK-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/PKG-INFO` & `iotPervasiveServiceSDK-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotPervasiveServiceSDK
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Author: HFC
 Author-email: 2898534520@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/config.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/config.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/applicationContext.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/applicationContext.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/eventInvoker.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/eventInvoker.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,29 +81,29 @@
       "deviceInstanceId":config.DEVICE_ID,
       "serviceUrl": service.url,
       "versionCode": service.versionCode,
       "eventId":event.eventId,
       "msg": eventMsg
     }
 
-    mqttClient.sendMsg(topic,ujson.dumps(msgJsonDict))
+    mqttClient.sendMsg(topic,ujson.dumps(msgJsonDict, ensure_ascii=False))
     # 如果非系统的mqtt客户端则关闭
     if not isSystemMqtt:
       mqttClient.close()
 
 
   def getEventMsgStr(service:ServiceBean,event:EventBean,eventMsg:str):
     msgJsonDict = {
       "deviceInstanceId":config.DEVICE_ID,
       "serviceUrl": service.url,
       "versionCode": service.versionCode,
       "eventId":event.eventId,
       "msg": eventMsg
     }
-    return ujson.dumps(msgJsonDict)
+    return ujson.dumps(msgJsonDict, ensure_ascii=False)
```

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/exception/serviceException.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/exception/serviceException.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/job/contextUpLoadJob.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/job/contextUpLoadJob.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     # 拼接msg
     msgDict = {
       "timestamp": TimeUtil.getTimerMs(),
       # "lanIp" : wlan.ifconfig()[0],
       "thingModel":thingModel,
       "serviceList":services
     }
-    applicationContext.pervasiveMqttClient.sendMsg(config.UPLOAD_CONTEXT_TOPIC,ujson.dumps(msgDict))
+    applicationContext.pervasiveMqttClient.sendMsg(config.UPLOAD_CONTEXT_TOPIC,ujson.dumps(msgDict), ensure_ascii=False)
     
   def upLoadServiceList(self):
     services = applicationContext.getServiceListInfo()
```

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/loader/hardwareInfoLoader.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/loader/hardwareInfoLoader.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/loader/proxyLoader.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/loader/proxyLoader.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/loader/serversLoader.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/loader/serversLoader.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/scheduleService.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/scheduleService.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/core/serverInvoker.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/core/serverInvoker.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,22 +55,26 @@
     if(capability.outputMapper != None):
       if(capability.outputLanguage == "jinja2"):
         outputTemplateEngine = TemplateEngine()
         outputTemplateEngine.load_template(capability.outputMapper)
         try:
           if(isinstance(response, str)):
             response = json.loads(response)
+          print("wwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwww")
+          print(response)
           response = outputTemplateEngine.render_template(response)
+          print(response)
           if(isinstance(response, str)):
             response = json.loads(response)
+          print(response)
         except Exception as e:
           raise InvokeServiceException(json.dumps({
             "response":response,
             "systemInfo":"服务定义错误,输出消息映射错误,请联系服务开发者"+str(e)
-            }))
+            }, ensure_ascii=False))
           
         print(response)
     return response
 
 
   '''
   * 运行代理
```

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/factory/systemServiceFactory.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/factory/systemServiceFactory.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/model/ujinja/source.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/model/ujinja/source.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/pojo/capabilityBean.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/pojo/capabilityBean.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/pojo/eventBean.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/pojo/eventBean.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/pojo/serviceBean.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/pojo/serviceBean.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/proxy/pythonServiceProxy.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/proxy/pythonServiceProxy.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/proxy/thingProxy.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/proxy/thingProxy.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/proxySDK.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/proxySDK.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     deviceInfo["ipAddress"] = ip.lower()
     deviceInfo["serviceList"] = serviceList
     deviceInfo["deviceTypeId"] = deviceTypeId
     log.info(deviceInfo)
     applicationContext.stateInfo = deviceInfo
     config.deviceInfo = deviceInfo
 
-    applicationContext.pervasiveMqttClient.sendMsg(config.UPLOAD_SERVICE_LIST_TOPIC,ujson.dumps(deviceInfo))
+    applicationContext.pervasiveMqttClient.sendMsg(config.UPLOAD_SERVICE_LIST_TOPIC,ujson.dumps(deviceInfo, ensure_ascii=False))
 
     # 初始化定时任务  
     tasks = []
     # tasks.append(MqttHealthJob(intervalTime=60000))
     tasks.append(ContextUploadJob(intervalTime=10000))
     tasks.append(MqttCheckMessageJob(intervalTime=500))
     tasks.append(EventListenerJob(intervalTime=5000))
```

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/router/httpRouter.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/router/httpRouter.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # 拼接msg
     msgDict = {
         "success": runSuccess,
         "data": res,
         "timestamp": TimeUtil.getTimerMs(),
     }
     print(msgDict)
-    return template(json.dumps(msgDict), name=__name__);
+    return template(json.dumps(msgDict, ensure_ascii=False), name=__name__);
 
 def _runServer():
     run(app, host='localhost', port=1024, debug=True)
 
 def runWebServer():
         # 创建一个新线程来运行 Bottle 服务
     server_thread = threading.Thread(target=_runServer)
```

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/router/mqttRouter.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/router/mqttRouter.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     # 拼接msg
     msgDict = {
       "success" : runSuccess,
       "data" : responce,
       "timestamp": TimeUtil.getTimerMs()
     }
     routerLog.info(msgDict)
-    applicationContext.pervasiveMqttClient.sendMsg(callbackTopic,json.dumps(msgDict))
+    applicationContext.pervasiveMqttClient.sendMsg(callbackTopic,json.dumps(msgDict, ensure_ascii=False))
   # 脚本更新能力
   elif topic[2] == config.UPDATE_ENUM:
     msgJson = json.loads(msg)
     print(msgJson)
     msgId = msgJson.get("messageId","null")
     isInstall = msgJson.get("installStatus",True)
     # 拼接topic
@@ -74,13 +74,13 @@
         # sys.print_exception(e)
         responce = {"errorMsg":str(e)}
     msgDict = {
       "success" : runSuccess,
       "timestamp": TimeUtil.getTimerMs(),
       "data":responce
     }
-    applicationContext.pervasiveMqttClient.sendMsg(callbackTopic,json.dumps(msgDict))
+    applicationContext.pervasiveMqttClient.sendMsg(callbackTopic,json.dumps(msgDict, ensure_ascii=False))
   else:
     routerLog.error("no topic path")
```

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/systemService/mqttService.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/systemService/mqttService.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     willMsg = {
       "deviceInstanceId":config.DEVICE_ID,
       "serviceUrl": "systemService",
 	    "versionCode": 0,
 	    "eventId": "OFFLINE",
 	    "msg": None
       }
-    self.client.will_set(topic = config.ON_EVENT_TOPIC, payload=json.dumps(willMsg))
+    self.client.will_set(topic = config.ON_EVENT_TOPIC, payload=json.dumps(willMsg, ensure_ascii=False))
 
     # 设置连接和消息回调函数
     self.client.on_connect = self.on_connect
     self.client.on_message = self.sub_cb
 
     self.client.connect(host = config.MQTT_ADDRESS, port = config.MQTT_PORT, keepalive = 60)
     # 开始循环处理网络流量和消息回调
```

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/systemService/updateService.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/systemService/updateService.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/fileUtils.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/fileUtils.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/logutil.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/logutil.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/netUtils.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/netUtils.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/tarGzUtils.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/tarGzUtils.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/taskUtils.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/taskUtils.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK/utils/templateUtils.py` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK/utils/templateUtils.py`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK.egg-info/PKG-INFO` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotPervasiveServiceSDK
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Author: HFC
 Author-email: 2898534520@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `iotPervasiveServiceSDK-0.0.8/iotPervasiveServiceSDK.egg-info/SOURCES.txt` & `iotPervasiveServiceSDK-0.0.9/iotPervasiveServiceSDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iotPervasiveServiceSDK-0.0.8/setup.py` & `iotPervasiveServiceSDK-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools #导入setuptools打包工具
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="iotPervasiveServiceSDK", # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.8",    #包版本号，便于维护版本
+    version="0.0.9",    #包版本号，便于维护版本
     author="HFC",    #作者，可以写自己的姓名
     author_email="2898534520@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="A small example package",#包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),  # Make sure to include 'where' argument
     zip_safe=False,  # Disable zip-safe mode for easier debugging
```

