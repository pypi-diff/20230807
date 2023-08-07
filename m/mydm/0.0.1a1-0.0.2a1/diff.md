# Comparing `tmp/mydm-0.0.1a1.tar.gz` & `tmp/mydm-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mydm-0.0.1a1.tar", max compression
+gzip compressed data, was "mydm-0.0.2a1.tar", max compression
```

## Comparing `mydm-0.0.1a1.tar` & `mydm-0.0.2a1.tar`

### file list

```diff
@@ -1,5 +1,13 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 mydm-0.0.1a1/LICENSE
--rw-r--r--   0        0        0       21 2023-08-06 04:47:23.174291 mydm-0.0.1a1/mydm/__init__.py
--rw-r--r--   0        0        0      317 2023-08-06 04:46:48.427150 mydm-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0      305 2023-08-06 04:49:31.882721 mydm-0.0.1a1/README.md
--rw-r--r--   0        0        0      781 1970-01-01 00:00:00.000000 mydm-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 mydm-0.0.2a1/LICENSE
+-rw-r--r--   0        0        0       81 2023-08-07 04:19:21.045728 mydm-0.0.2a1/mydm/__init__.py
+-rw-r--r--   0        0        0      417 2023-08-06 11:25:28.254107 mydm-0.0.2a1/mydm/bot.py
+-rw-r--r--   0        0        0        0 2023-08-07 03:42:16.350223 mydm-0.0.2a1/mydm/event.py
+-rw-r--r--   0        0        0     2113 2023-08-06 11:14:22.597860 mydm-0.0.2a1/mydm/interactor/__init__.py
+-rw-r--r--   0        0        0      572 2023-08-07 03:15:54.352056 mydm-0.0.2a1/mydm/interactor/gocqhttp/__init__.py
+-rw-r--r--   0        0        0      934 2023-08-07 04:15:10.970991 mydm-0.0.2a1/mydm/interactor/gocqhttp/cqcode.py
+-rw-r--r--   0        0        0        0 2023-08-07 04:21:03.253715 mydm-0.0.2a1/mydm/interactor/gocqhttp/event.py
+-rw-r--r--   0        0        0        0 2023-08-06 06:10:55.963326 mydm-0.0.2a1/mydm/logger.py
+-rw-r--r--   0        0        0      167 2023-08-07 04:18:44.944129 mydm-0.0.2a1/mydm/tool.py
+-rw-r--r--   0        0        0      460 2023-08-07 04:21:17.681846 mydm-0.0.2a1/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-08-06 05:43:25.803070 mydm-0.0.2a1/README.md
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 mydm-0.0.2a1/PKG-INFO
```

### Comparing `mydm-0.0.1a1/LICENSE` & `mydm-0.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `mydm-0.0.1a1/PKG-INFO` & `mydm-0.0.2a1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: mydm
-Version: 0.0.1a1
-Summary: A qq chatbot framework
+Version: 0.0.2a1
+Summary: 一个使用OneBot v11/12协议的机器人框架
+Home-page: https://github.com/yuyi2439/MyDM
 License: Apache-2.0
 Author: yuyi2439
 Author-email: yuyi2439@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
+Project-URL: Repository, https://github.com/yuyi2439/MyDM
 Description-Content-Type: text/markdown
 
 # MyDM
-### 一个QQ聊天机器人框架
+### 一个使用OneBot v11/12协议的机器人框架
 
 ### 本项目使用Apache2.0开源协议
 - 使用本项目时要求保留原始版权和许可声明。同时向贡献者明确授予专利权。
 - 使用者可以自由修改，进行商业使用，可以使用不同的条款分发，没有开源要求。
```

