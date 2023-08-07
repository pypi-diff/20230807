# Comparing `tmp/yunzhanghu_sdk-1.0.6.tar.gz` & `tmp/yunzhanghu_sdk-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunzhanghu_sdk-1.0.6.tar", last modified: Fri Mar 24 10:14:34 2023, max compression
+gzip compressed data, was "yunzhanghu_sdk-1.0.7.tar", last modified: Mon Aug  7 11:04:17 2023, max compression
```

## Comparing `yunzhanghu_sdk-1.0.6.tar` & `yunzhanghu_sdk-1.0.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-03-24 10:14:34.734637 yunzhanghu_sdk-1.0.6/
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       39 2023-03-10 08:51:50.000000 yunzhanghu_sdk-1.0.6/MANIFEST.in
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     4036 2023-03-24 10:14:34.734481 yunzhanghu_sdk-1.0.6/PKG-INFO
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     6323 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/README.md
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       38 2023-03-24 10:14:34.734690 yunzhanghu_sdk-1.0.6/setup.cfg
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)      885 2023-03-10 08:51:50.000000 yunzhanghu_sdk-1.0.6/setup.py
-drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-03-24 10:14:34.699602 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       41 2023-03-24 10:14:16.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/__init__.py
-drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-03-24 10:14:34.714630 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       13 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/__init__.py
-drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-03-24 10:14:34.721301 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       10 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/__init__.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     2469 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/apiusersign_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3979 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/authentication_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1115 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/bizlicxjjh5_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1648 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/bizlicxjjh5api_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3511 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/dataservice_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1930 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/h5usersign_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3415 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/invoice_client.py
-drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-03-24 10:14:34.734125 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       12 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/__init__.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     5422 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/apiusersign.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     8459 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/authentication.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     5882 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/bizlicxjjh5.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     8034 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/bizlicxjjh5api.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)    14595 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/dataservice.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     5499 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/h5usersign.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)    13872 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/invoice.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)    25030 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/payment.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     2257 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/tax.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     4605 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/payment_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1079 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/tax_client.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3335 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/base.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1396 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/config.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     6646 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/message.py
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)      157 2023-03-10 08:51:50.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/utils.py
-drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-03-24 10:14:34.707329 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk.egg-info/
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     4036 2023-03-24 10:14:34.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1332 2023-03-24 10:14:34.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)        1 2023-03-24 10:14:34.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       38 2023-03-24 10:14:34.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk.egg-info/requires.txt
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       15 2023-03-24 10:14:34.000000 yunzhanghu_sdk-1.0.6/yunzhanghu_sdk.egg-info/top_level.txt
--rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3774 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.6/云账户SDK-for-Python-pypi.md
+drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-08-07 11:04:17.361261 yunzhanghu_sdk-1.0.7/
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       39 2023-03-10 08:51:50.000000 yunzhanghu_sdk-1.0.7/MANIFEST.in
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3996 2023-08-07 11:04:17.361100 yunzhanghu_sdk-1.0.7/PKG-INFO
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     6252 2023-08-07 10:15:06.000000 yunzhanghu_sdk-1.0.7/README.md
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       38 2023-08-07 11:04:17.361305 yunzhanghu_sdk-1.0.7/setup.cfg
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)      885 2023-04-14 07:35:57.000000 yunzhanghu_sdk-1.0.7/setup.py
+drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-08-07 11:04:17.349101 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       41 2023-08-07 10:15:06.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/__init__.py
+drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-08-07 11:04:17.353386 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       13 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/__init__.py
+drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-08-07 11:04:17.357440 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       10 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/__init__.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     2469 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/apiusersign_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3979 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/authentication_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1115 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/bizlicxjjh5_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1648 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/bizlicxjjh5api_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3511 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/dataservice_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1930 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/h5usersign_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3415 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/invoice_client.py
+drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-08-07 11:04:17.360818 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       12 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/__init__.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     5422 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/apiusersign.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     8459 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/authentication.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     5882 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/bizlicxjjh5.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     8034 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/bizlicxjjh5api.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)    14595 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/dataservice.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     5499 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/h5usersign.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)    13872 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/invoice.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)    25030 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/payment.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     2257 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/tax.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     4605 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/payment_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1079 2023-03-24 10:12:55.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/tax_client.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3137 2023-04-14 07:35:57.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/base.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1396 2023-08-07 10:15:06.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/config.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     6130 2023-08-07 10:15:06.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/message.py
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)      157 2023-04-14 07:35:57.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/utils.py
+drwxr-xr-x   0 yunzhanghu_bj1170   (501) staff       (20)        0 2023-08-07 11:04:17.350676 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk.egg-info/
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3996 2023-08-07 11:04:17.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     1332 2023-08-07 11:04:17.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)        1 2023-08-07 11:04:17.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       38 2023-08-07 11:04:17.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk.egg-info/requires.txt
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)       15 2023-08-07 11:04:17.000000 yunzhanghu_sdk-1.0.7/yunzhanghu_sdk.egg-info/top_level.txt
+-rw-r--r--   0 yunzhanghu_bj1170   (501) staff       (20)     3734 2023-08-07 10:15:06.000000 yunzhanghu_sdk-1.0.7/云账户SDK-for-Python-pypi.md
```

### Comparing `yunzhanghu_sdk-1.0.6/PKG-INFO` & `yunzhanghu_sdk-1.0.7/云账户SDK-for-Python-pypi.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: yunzhanghu_sdk
-Version: 1.0.6
-Summary: 云账户官方 SDK for Python
-Home-page: UNKNOWN
-Author: yunzhanghu
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-
 # 云账户 SDK for Python
 
 欢迎使用云账户 SDK for Python。
 云账户是一家专注为平台企业和新就业形态劳动者提供高质量灵活就业服务的新时代企业。云账户 SDK 对云账户综合服务平台 API 接口进行封装，帮助您快速接入到云账户综合服务平台。云账户 SDK for Python 为您提供签约、下单、回调、数据查询等功能，帮助您完成与云账户综合服务平台的接口对接及业务开发。 如果您在使用过程中遇到任何问题，请在当前 GitHub 提交 Issues，或发送邮件至技术支持组 [techsupport@yunzhanghu.com](mailto:techsupport@yunzhanghu.com)。
 
 ### 环境要求
 
@@ -46,16 +35,16 @@
 from yunzhanghu_sdk.config import *
 
 if __name__ == "__main__":
     # 平台企业 ID，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     dealer_id = "xxx"
     # 综合服务主体 ID，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     broker_id = "xxx"
-    # 签名方式，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取，默认为 RSA 签名方式。
-    # rsa：RSA 签名方式   sha256：HMAC 签名方式
+    # 签名方式，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
+    # 签名方式为 RSA，参数固定为：rsa
     sign_type = "rsa"
     # 平台企业 App Key，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     app_key = "xxx"
     # 平台企业 3DES Key，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     des3key = "xxx"
     # 平台企业私钥，自行生成 RSA 公私钥，私钥请妥善保存，谨防泄露。平台企业公钥请登录云账户综合服务平台配置，选择“业务中心 > 业务管理 > 对接信息”，单击页面右上角的“编辑”，完成平台企业公钥配置。
     dealer_private_key = '''
@@ -88,9 +77,8 @@
     )
     # 建议自定义并将 request-id 记录在日志中
     # request.request_id = "XXXXX"
     client = PaymentClient(config)
     resp = client.get_order(request)
 
     print(resp.code, resp.message, resp.request_id, resp.data)
-```
-
+```
```

### Comparing `yunzhanghu_sdk-1.0.6/README.md` & `yunzhanghu_sdk-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -86,16 +86,16 @@
 from yunzhanghu_sdk.config import *
 
 if __name__ == "__main__":
     # 平台企业 ID，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     dealer_id = "xxx"
     # 综合服务主体 ID，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     broker_id = "xxx"
-    # 签名方式，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取，默认为 RSA 签名方式。
-    # rsa：RSA 签名方式   sha256：HMAC 签名方式
+    # 签名方式，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
+    # 签名方式为 RSA，参数固定为：rsa
     sign_type = "rsa"
     # 平台企业 App Key，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     app_key = "xxx"
     # 平台企业 3DES Key，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     des3key = "xxx"
     # 平台企业私钥，自行生成 RSA 公私钥，私钥请妥善保存，谨防泄露。平台企业公钥请登录云账户综合服务平台配置，选择“业务中心 > 业务管理 > 对接信息”，单击页面右上角的“编辑”，完成平台企业公钥配置。
     dealer_private_key = '''
@@ -118,17 +118,17 @@
         app_key=app_key,
         des3key=des3key,
         dealer_private_key=dealer_private_key,
         yzh_public_key=yzh_public_key,
     )
     # 获取订单详情
     request = GetOrderRequest(
-        order_id="232211231231231",
-        channel="微信",
-        data_type="encryption"
+        order_id="",
+        channel="",
+        data_type=""
     )
     # 建议自定义并将 request-id 记录在日志中
     # request.request_id = "XXXXX"
     client = PaymentClient(config)
     resp = client.get_order(request)
 
     print(resp.code, resp.message, resp.request_id, resp.data)
```

### Comparing `yunzhanghu_sdk-1.0.6/setup.py` & `yunzhanghu_sdk-1.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 from yunzhanghu_sdk import __version__
 
 requirements = [
-    'requests>=2.19.1',
-    'pycryptodome==3.10.1',
+    "requests>=2.19.1",
+    "pycryptodome==3.10.1",
 ]
 
 packages = [
-    'yunzhanghu_sdk',
-    'yunzhanghu_sdk.client',
-    'yunzhanghu_sdk.client.api',
-    'yunzhanghu_sdk.client.api.model',
+    "yunzhanghu_sdk",
+    "yunzhanghu_sdk.client",
+    "yunzhanghu_sdk.client.api",
+    "yunzhanghu_sdk.client.api.model",
 ]
 
 setup(
-    name='yunzhanghu_sdk',
+    name="yunzhanghu_sdk",
     version=__version__,
-    description='云账户官方 SDK for Python',
-    author='yunzhanghu',
+    description="云账户官方 SDK for Python",
+    author="yunzhanghu",
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     packages=packages,
-    long_description=open('云账户SDK-for-Python-pypi.md', encoding='utf-8').read(),
-    long_description_content_type='text/markdown',
+    long_description=open("云账户SDK-for-Python-pypi.md", encoding="utf-8").read(),
+    long_description_content_type="text/markdown",
 )
```

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/apiusersign_client.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/apiusersign_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/authentication_client.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/authentication_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/bizlicxjjh5_client.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/bizlicxjjh5_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/bizlicxjjh5api_client.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/bizlicxjjh5api_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/dataservice_client.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/dataservice_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/h5usersign_client.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/h5usersign_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/invoice_client.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/invoice_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/apiusersign.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/apiusersign.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/authentication.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/authentication.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/bizlicxjjh5.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/bizlicxjjh5.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/bizlicxjjh5api.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/bizlicxjjh5api.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/dataservice.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/dataservice.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/h5usersign.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/h5usersign.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/invoice.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/invoice.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/payment.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/payment.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/model/tax.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/model/tax.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/payment_client.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/payment_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/api/tax_client.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/api/tax_client.py`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/client/base.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/client/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,66 +13,64 @@
         :type config: Config
         :param config: 配置信息
 
         :type timeout: int
         :param timeout: 请求超时时间。非必填，默认 30 秒
         """
 
-        encrypt_type = config.sign_type
-        if encrypt_type not in("sha256", "rsa"):
-            raise ValueError('sign_type error! signType must be rsa or sha256!')
+        sign_type = config.sign_type
 
         self.__des3key = config.des3key
+        self.__app_key = config.app_key
+
         self.__encrypt = None
-        if encrypt_type == "sha256":
-            self.__encrypt = Des3EncryptAndHmacSign (
-                config.app_key, config.des3key)
-        if encrypt_type == "rsa":
-            self.__encrypt = Des3EncryptAndRSASign(
-                config.app_key, config.yzh_public_key, config.dealer_private_key, config.des3key)
+        if sign_type == "sha256":
+            self.__encrypt = HmacSigner(config.app_key)
+        if sign_type == "rsa":
+            self.__encrypt = RSASigner(config.app_key, config.yzh_public_key, config.dealer_private_key)
 
         self.__dealer_id = config.dealer_id
         self.__base_url = config.host
         self.__timeout = timeout
 
     def __header(self, request_id):
         if type(request_id) is not str or request_id == "":
             request_id = str(int(time.time()))
         return {
-            'dealer-id': self.__dealer_id,
-            'request-id': request_id,
+            "dealer-id": self.__dealer_id,
+            "request-id": request_id,
             "Content-Type": "application/x-www-form-urlencoded",
             "User-Agent": "yunzhanghu-sdk-python/%s/%s/%s" % (
                 __version__, platform.platform(), platform.python_version()),
         }
 
     def __request(self, method, url, **kwargs):
-        data = kwargs['data'] if 'data' in kwargs else None
-        param = kwargs['param'] if 'param' in kwargs else None
-        headers = self.__header(kwargs['request_id'])
+        data = kwargs.get("data", None)
+        param = kwargs.get("param", None)
+        headers = self.__header(kwargs["request_id"])
         return self.__handle_resp(
             data, param, headers,
             requests.request(method=method,
                              url=self.__base_url + url,
                              headers=headers,
-                             data=ReqMessage(self.__encrypt, data).pack(),
-                             params=ReqMessage(self.__encrypt, param).pack(),
+                             data=ReqMessage(self.__encrypt, data, self.__des3key).pack(),
+                             params=ReqMessage(self.__encrypt, param, self.__des3key).pack(),
                              timeout=self.__timeout))
 
     def _post(self, url, request_id, data):
-        kwargs = {'data': data, 'request_id': request_id}
-        return self.__request(method='POST', url=url, **kwargs)
+        kwargs = {"data": data, "request_id": request_id}
+        return self.__request(method="POST", url=url, **kwargs)
 
     def _get(self, url, request_id, param):
-        kwargs = {'param': param, 'request_id': request_id}
-        return self.__request(method='GET', url=url, **kwargs)
+        kwargs = {"param": param, "request_id": request_id}
+        return self.__request(method="GET", url=url, **kwargs)
 
     def __handle_resp(self, req_data, req_param, headers, resp):
         if resp is None:
-            raise ValueError('resp is None')
+            raise ValueError("resp is None")
 
         resp.raise_for_status()
         return RespMessage(self.__des3key, resp.text, req_data,
                            req_param, headers).decrypt()
 
 
 class BaseRequest(object):
```

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/config.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     :type host: string
     :param host: 请求域名
 
     :type dealer_id: string
     :param dealer_id: 平台企业 ID
 
     :type sign_type: string
-    :param sign_type: 签名类型
+    :param sign_type: 签名算法
 
     :type app_key: string
     :param app_key: App Key
 
     :type des3key: string
     :param des3key: 3DES Key
 
@@ -35,10 +35,10 @@
 
     def check_config(self):
         if self.dealer_private_key is not None:
             self.dealer_private_key = self.dealer_private_key.strip()
         if self.yzh_public_key is not None:
             self.yzh_public_key = self.yzh_public_key.strip()
         if self.sign_type not in ("sha256", "rsa"):
-            raise ValueError('sign_type error! signType must be rsa or sha256!')
+            raise ValueError("sign_type error! signType must be rsa or sha256!")
         if self.host is None:
             self.host = "https://api-service.yunzhanghu.com"
```

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk/message.py` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,137 +7,163 @@
 import hashlib
 import hmac
 import json
 import random
 import time
 
 import pyDes
-import rsa
 from Crypto.Hash import SHA256
 from Crypto.PublicKey import RSA
 from Crypto.Signature import PKCS1_v1_5 as Signature_pkcs1_v1_5
 
 
+class TripleDes(object):
+    """ 3DES 加解密 """
+
+    def __init__(self, data, de3key):
+        self.__data = data
+        self.__des3key = de3key
+
+    def encrypt(self):
+        data = bytes(self.__data, encoding="utf8")
+        key = bytes(self.__des3key[0:8], encoding="utf8")
+        return base64.b64encode(
+            pyDes.triple_des(self.__des3key, pyDes.CBC, key, pad=None, padmode=pyDes.PAD_PKCS5).encrypt(data))
+
+    def decrypt(self):
+        data = bytes(self.__data, encoding="utf8")
+        key = bytes(self.__des3key[0:8], encoding="utf8")
+        return pyDes.triple_des(self.__des3key, pyDes.CBC, key, pad=None, padmode=pyDes.PAD_PKCS5) \
+            .decrypt(base64.b64decode(data))
+
+
 class Signer(abc.ABC):
+    """ 签名 """
+
     @abc.abstractmethod
-    def encrypt(self, data):
+    def sign_type(self):
         return NotImplemented
 
     @abc.abstractmethod
-    def sign(self, mess, timestamp, data):
+    def sign(self, data, mess, timestamp):
         return NotImplemented
 
     @abc.abstractmethod
-    def encrypt_type(self):
+    def verify_sign(self, data, mess, timestamp, signature):
         return NotImplemented
 
 
-class Des3EncryptAndHmacSign(Signer):
-    def __init__(self, app_key, des3key):
+class HmacSigner(Signer):
+    """ Hmac 签名 """
+
+    def __init__(self, app_key):
         self.__app_key = app_key
-        self.__des3key = des3key
 
-    def encrypt_type(self):
+    def sign_type(self):
         return "sha256"
 
-    def encrypt(self, data):
-        data = bytes(data, encoding="utf8")
-        key = bytes(self.__des3key[0:8], encoding="utf8")
-        return base64.b64encode(
-            pyDes.triple_des(self.__des3key, pyDes.CBC, key, pad=None, padmode=pyDes.PAD_PKCS5).encrypt(data))
+    def sign(self, data, mess, timestamp):
+        sign_pairs = "data=%s&mess=%s&timestamp=%d&key=%s" % (
+            str(data, encoding="utf-8"), mess, timestamp, self.__app_key)
+        app_key = bytes(self.__app_key, encoding="utf8")
+        sign_pairs = bytes(sign_pairs, encoding="utf8")
+        return hmac.new(app_key, msg=sign_pairs, digestmod=hashlib.sha256).hexdigest()
 
-    def sign(self, mess, timestamp, encrypt_data):
-        signPairs = "data=%s&mess=%s&timestamp=%d&key=%s" % (
-            str(encrypt_data, encoding="utf-8"), mess, timestamp, self.__app_key)
+    def verify_sign(self, data, mess, timestamp, signature):
+        sign_pairs = "data=%s&mess=%s&timestamp=%d&key=%s" % (data, mess, timestamp, self.__app_key)
         app_key = bytes(self.__app_key, encoding="utf8")
-        signPairs = bytes(signPairs, encoding="utf8")
-        return hmac.new(app_key, msg=signPairs, digestmod=hashlib.sha256).hexdigest()
+        sign_pairs = bytes(sign_pairs, encoding="utf8")
+        return hmac.new(app_key, msg=sign_pairs, digestmod=hashlib.sha256).hexdigest() == signature
 
 
-class Des3EncryptAndRSASign(Signer):
-    def __init__(self, app_key, public_key, private_key, des3key):
+class RSASigner(Signer):
+    """ RSA 签名 """
+
+    def __init__(self, app_key, public_key, private_key):
         self.__public_key = RSA.importKey(public_key)
-        self.__private_key = RSA.importKey(private_key)
+        if private_key is not None:
+            self.__private_key = RSA.importKey(private_key)
         self.__app_key = app_key
-        self.__des3key = des3key
 
-    def encrypt_type(self):
+    def sign_type(self):
         return "rsa"
 
-    def encrypt(self, data):
-        data = bytes(data, encoding="utf8")
-        key = bytes(self.__des3key[0:8], encoding="utf8")
-        return base64.b64encode(
-            pyDes.triple_des(self.__des3key, pyDes.CBC, key, pad=None, padmode=pyDes.PAD_PKCS5).encrypt(data))
-
-    def sign(self, mess, timestamp, encrypt_data):
+    def sign(self, data, mess, timestamp):
         sign_pairs = "data=%s&mess=%s&timestamp=%d&key=%s" % (
-            bytes.decode(encrypt_data), mess, timestamp, self.__app_key)
+            str(data, encoding="utf-8"), mess, timestamp, self.__app_key)
         signer = Signature_pkcs1_v1_5.new(self.__private_key)
         digest = SHA256.new()
         digest.update(sign_pairs.encode("utf8"))
         sign = signer.sign(digest)
         return base64.b64encode(sign)
 
+    def verify_sign(self, data, mess, timestamp, signature):
+        sign_pairs = "data=%s&mess=%s&timestamp=%d&key=%s" % (data, mess, timestamp, self.__app_key)
+        signature = base64.b64decode(signature)
+        cipher = Signature_pkcs1_v1_5.new(self.__public_key)
+        digest = SHA256.new()
+        digest.update(sign_pairs.encode("utf8"))
+        return cipher.verify(digest, signature)
+
 
 class ReqMessage(object):
     """
     ReqMessage 请求消息体
     """
 
-    def __init__(self, encrypt, data):
+    def __init__(self, encrypt, data, des3key):
         """
-        :param encrypt: 加密方式
+        :param encrypt: 加密算法
         :type data: {} 请求信息
         :param data: 请求信息
         """
         self.__encrypt = encrypt
-        self.data = None
+        self.__data = None
+        self.__des3key = des3key
         if data is not None:
-            self.data = json.dumps(data, ensure_ascii=False)
+            self.__data = json.dumps(data, ensure_ascii=False)
 
     def pack(self):
-        if self.data is None:
+        if self.__data is None:
             return None
         timestamp = int(time.time())
-        mess = ''.join(random.sample('1234567890abcdefghijklmnopqrstuvwxy', 10))
-        encrypt_data = self.__encrypt.encrypt(self.data)
+        mess = "".join(random.sample("1234567890abcdefghijklmnopqrstuvwxy", 10))
+        encrypt_data = TripleDes(self.__data, self.__des3key).encrypt()
         return {
             "data": encrypt_data,
             "mess": mess,
-            'timestamp': timestamp,
-            "sign": self.__encrypt.sign(mess, timestamp, encrypt_data),
-            "sign_type": self.__encrypt.encrypt_type()
+            "timestamp": timestamp,
+            "sign": self.__encrypt.sign(encrypt_data, mess, timestamp),
+            "sign_type": self.__encrypt.sign_type()
         }
 
 
 class RespMessage(object):
     """
     RespMessage 返回信息
     """
 
     def __init__(self, des3key, content, req_data, req_param, headers):
         self.__des3key = des3key
         self.__content = content
         dic = json.loads(content)
         self.__req_param = req_param
         self.__req_data = req_data
-        self.__code = dic['code'] if 'code' in dic else None
-        self.__message = dic['message'] if 'message' in dic else None
-        self.__data = dic['data'] if 'data' in dic else None
-        self.__request_id = headers['request-id']
+        self.__code = dic.get("code", None)
+        self.__message = dic.get("message", None)
+        self.__data = dic.get("data")
+        self.__request_id = headers["request-id"]
 
     def decrypt(self):
         if self.__data is None:
             return self
 
         if self.__des3key is not None and self.__req_param is not None \
-                and 'data_type' in self.__req_param and \
-                self.__req_param['data_type'] == 'encryption':
-            self.__data = json.loads(triple_des_decrypt(self.__des3key, self.__data))
+                and self.__req_param.get("data_type", "") == "encryption":
+            self.__data = json.loads(TripleDes(self.__data, self.__des3key).decrypt())
         return self
 
     @property
     def code(self):
         return self.__code
 
     @property
@@ -153,80 +179,18 @@
         return self.__content
 
     @property
     def request_id(self):
         return self.__request_id
 
 
-def triple_des_decrypt(des3key, data):
-    """ 3DES 解密
-
-    :type des3key: string
-    :param des3key: 3DES 密钥
-
-    :type data: string
-    :param data: 待解密数据
-
-    :return: 解密结果
-    """
-    data = bytes(data, encoding="utf8")
-    key = bytes(des3key[0:8], encoding="utf8")
-    return pyDes.triple_des(des3key, pyDes.CBC, key, pad=None, padmode=pyDes.PAD_PKCS5).decrypt(base64.b64decode(data))
-
-
-def verify_sign_rsa(public_key, app_key, data, mess, timestamp, signature):
-    """ RSA 公钥验签
-
-    :type public_key: string
-    :param public_key: 云账户公钥
-
-    :type app_key: string
-    :param app_key: App Key
-
-    :type data: string
-    :param data: data
-
-    :type mess: string
-    :param data: 随机字符串
-
-    :type timestamp: int
-    :param data: 时间戳
-
-    :type signature: string
-    :param signature: 异步通知签名
-
-    :return: 校验结果
-    """
-    sign_pairs = "data=" + data + "&mess=" + mess + "&timestamp=" + timestamp + "&key=" + app_key
-    rsa.verify(sign_pairs, signature, public_key)
-
-
-def verify_sign_hmac(app_key, data, mess, timestamp, signature):
-    """HMAC 验签
-
-    :type app_key: string
-    :param app_key: App Key
-
-    :type data: string
-    :param data: data
-
-    :type mess: string
-    :param data: 随机字符串
-
-    :type timestamp: int
-    :param data: 时间戳
-
-    :type signature: string
-    :param signature: 异步通知签名
-
-    :return: 校验结果
-    """
-    sign_pairs = "data=%s&mess=%s&timestamp=%d&key=%s" % (data, mess, timestamp, app_key)
-    return hmac.new(app_key.encode('utf-8'), msg=sign_pairs, digestmod=hashlib.sha256).hexdigest() == signature
-
-
-def notify_decoder(public_key, app_key, des3key, data, mess, timestamp, signature):
+def notify_decoder(public_key, app_key, des3key, data, mess, timestamp, signature, sign_type):
     res_data, verify_result = "", False
-    if verify_sign_rsa(public_key, app_key, data, mess, timestamp, signature):
-        res_data = triple_des_decrypt(des3key, data)
-        verify_result = True
+    if sign_type == "sha256":
+        if HmacSigner(app_key).verify_sign(data, mess, timestamp, signature):
+            res_data = TripleDes(data, des3key).decrypt().decode()
+            verify_result = True
+    else:
+        if RSASigner(app_key, public_key, None).verify_sign(data, mess, timestamp, signature):
+            res_data = TripleDes(data, des3key).decrypt().decode()
+            verify_result = True
     return verify_result, res_data
```

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk.egg-info/PKG-INFO` & `yunzhanghu_sdk-1.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yunzhanghu-sdk
-Version: 1.0.6
+Name: yunzhanghu_sdk
+Version: 1.0.7
 Summary: 云账户官方 SDK for Python
 Home-page: UNKNOWN
 Author: yunzhanghu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -46,16 +46,16 @@
 from yunzhanghu_sdk.config import *
 
 if __name__ == "__main__":
     # 平台企业 ID，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     dealer_id = "xxx"
     # 综合服务主体 ID，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     broker_id = "xxx"
-    # 签名方式，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取，默认为 RSA 签名方式。
-    # rsa：RSA 签名方式   sha256：HMAC 签名方式
+    # 签名方式，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
+    # 签名方式为 RSA，参数固定为：rsa
     sign_type = "rsa"
     # 平台企业 App Key，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     app_key = "xxx"
     # 平台企业 3DES Key，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     des3key = "xxx"
     # 平台企业私钥，自行生成 RSA 公私钥，私钥请妥善保存，谨防泄露。平台企业公钥请登录云账户综合服务平台配置，选择“业务中心 > 业务管理 > 对接信息”，单击页面右上角的“编辑”，完成平台企业公钥配置。
     dealer_private_key = '''
```

### Comparing `yunzhanghu_sdk-1.0.6/yunzhanghu_sdk.egg-info/SOURCES.txt` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yunzhanghu_sdk-1.0.6/云账户SDK-for-Python-pypi.md` & `yunzhanghu_sdk-1.0.7/yunzhanghu_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: yunzhanghu-sdk
+Version: 1.0.7
+Summary: 云账户官方 SDK for Python
+Home-page: UNKNOWN
+Author: yunzhanghu
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+
 # 云账户 SDK for Python
 
 欢迎使用云账户 SDK for Python。
 云账户是一家专注为平台企业和新就业形态劳动者提供高质量灵活就业服务的新时代企业。云账户 SDK 对云账户综合服务平台 API 接口进行封装，帮助您快速接入到云账户综合服务平台。云账户 SDK for Python 为您提供签约、下单、回调、数据查询等功能，帮助您完成与云账户综合服务平台的接口对接及业务开发。 如果您在使用过程中遇到任何问题，请在当前 GitHub 提交 Issues，或发送邮件至技术支持组 [techsupport@yunzhanghu.com](mailto:techsupport@yunzhanghu.com)。
 
 ### 环境要求
 
@@ -35,16 +46,16 @@
 from yunzhanghu_sdk.config import *
 
 if __name__ == "__main__":
     # 平台企业 ID，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     dealer_id = "xxx"
     # 综合服务主体 ID，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     broker_id = "xxx"
-    # 签名方式，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取，默认为 RSA 签名方式。
-    # rsa：RSA 签名方式   sha256：HMAC 签名方式
+    # 签名方式，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
+    # 签名方式为 RSA，参数固定为：rsa
     sign_type = "rsa"
     # 平台企业 App Key，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     app_key = "xxx"
     # 平台企业 3DES Key，登录云账户综合服务平台，选择“业务中心 > 业务管理 > 对接信息”获取
     des3key = "xxx"
     # 平台企业私钥，自行生成 RSA 公私钥，私钥请妥善保存，谨防泄露。平台企业公钥请登录云账户综合服务平台配置，选择“业务中心 > 业务管理 > 对接信息”，单击页面右上角的“编辑”，完成平台企业公钥配置。
     dealer_private_key = '''
@@ -77,8 +88,9 @@
     )
     # 建议自定义并将 request-id 记录在日志中
     # request.request_id = "XXXXX"
     client = PaymentClient(config)
     resp = client.get_order(request)
 
     print(resp.code, resp.message, resp.request_id, resp.data)
-```
+```
+
```

