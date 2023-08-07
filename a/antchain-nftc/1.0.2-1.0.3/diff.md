# Comparing `tmp/antchain_nftc-1.0.2.tar.gz` & `tmp/antchain_nftc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_nftc-1.0.2.tar", last modified: Thu May 18 06:59:50 2023, max compression
+gzip compressed data, was "dist/antchain_nftc-1.0.3.tar", last modified: Mon Aug  7 07:38:01 2023, max compression
```

## Comparing `antchain_nftc-1.0.2.tar` & `antchain_nftc-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:59:50.000000 antchain_nftc-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 06:59:49.000000 antchain_nftc-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 06:59:49.000000 antchain_nftc-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-18 06:59:50.000000 antchain_nftc-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-05-18 06:59:49.000000 antchain_nftc-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-05-18 06:59:49.000000 antchain_nftc-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:59:50.000000 antchain_nftc-1.0.2/antchain_nftc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-18 06:59:50.000000 antchain_nftc-1.0.2/antchain_nftc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-05-18 06:59:50.000000 antchain_nftc-1.0.2/antchain_nftc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 06:59:50.000000 antchain_nftc-1.0.2/antchain_nftc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-18 06:59:50.000000 antchain_nftc-1.0.2/antchain_nftc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-18 06:59:50.000000 antchain_nftc-1.0.2/antchain_nftc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:59:50.000000 antchain_nftc-1.0.2/antchain_sdk_nftc/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 06:59:49.000000 antchain_nftc-1.0.2/antchain_sdk_nftc/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16857 2023-05-18 06:59:49.000000 antchain_nftc-1.0.2/antchain_sdk_nftc/client.py
--rw-r--r--   0 root         (0) root         (0)    17006 2023-05-18 06:59:49.000000 antchain_nftc-1.0.2/antchain_sdk_nftc/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 06:59:50.000000 antchain_nftc-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-05-18 06:59:49.000000 antchain_nftc-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 07:38:01.000000 antchain_nftc-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-07 07:38:00.000000 antchain_nftc-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-07 07:38:00.000000 antchain_nftc-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-08-07 07:38:01.000000 antchain_nftc-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-08-07 07:38:00.000000 antchain_nftc-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-08-07 07:38:00.000000 antchain_nftc-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 07:38:01.000000 antchain_nftc-1.0.3/antchain_nftc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-08-07 07:38:01.000000 antchain_nftc-1.0.3/antchain_nftc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-08-07 07:38:01.000000 antchain_nftc-1.0.3/antchain_nftc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 07:38:01.000000 antchain_nftc-1.0.3/antchain_nftc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-08-07 07:38:01.000000 antchain_nftc-1.0.3/antchain_nftc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-07 07:38:01.000000 antchain_nftc-1.0.3/antchain_nftc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 07:38:01.000000 antchain_nftc-1.0.3/antchain_sdk_nftc/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-07 07:38:00.000000 antchain_nftc-1.0.3/antchain_sdk_nftc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19191 2023-08-07 07:38:00.000000 antchain_nftc-1.0.3/antchain_sdk_nftc/client.py
+-rw-r--r--   0 root         (0) root         (0)    20310 2023-08-07 07:38:00.000000 antchain_nftc-1.0.3/antchain_sdk_nftc/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-07 07:38:01.000000 antchain_nftc-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-08-07 07:38:00.000000 antchain_nftc-1.0.3/setup.py
```

### Comparing `antchain_nftc-1.0.2/LICENSE` & `antchain_nftc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_nftc-1.0.2/PKG-INFO` & `antchain_nftc-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_nftc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ant Chain NFTC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftc-1.0.2/README-CN.md` & `antchain_nftc-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_nftc-1.0.2/README.md` & `antchain_nftc-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `antchain_nftc-1.0.2/antchain_nftc.egg-info/PKG-INFO` & `antchain_nftc-1.0.3/antchain_nftc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-nftc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ant Chain NFTC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftc-1.0.2/antchain_sdk_nftc/client.py` & `antchain_nftc-1.0.3/antchain_sdk_nftc/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.2',
+                    'sdk_version': '1.0.3',
                     '_prod_code': 'NFTC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -233,15 +233,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.2',
+                    'sdk_version': '1.0.3',
                     '_prod_code': 'NFTC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -380,7 +380,63 @@
         Summary: DIY藏品发放查询
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             nftc_models.QueryMerchantDiyskuResponse(),
             await self.do_request_async('1.0', 'antchain.nftc.merchant.diysku.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def query_merchant_ugcimages(
+        self,
+        request: nftc_models.QueryMerchantUgcimagesRequest,
+    ) -> nftc_models.QueryMerchantUgcimagesResponse:
+        """
+        Description: 提供ISV  ugc铸造图片查询的openapi服务
+        Summary: ugc铸造图片查询的openapi接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_merchant_ugcimages_ex(request, headers, runtime)
+
+    async def query_merchant_ugcimages_async(
+        self,
+        request: nftc_models.QueryMerchantUgcimagesRequest,
+    ) -> nftc_models.QueryMerchantUgcimagesResponse:
+        """
+        Description: 提供ISV  ugc铸造图片查询的openapi服务
+        Summary: ugc铸造图片查询的openapi接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_merchant_ugcimages_ex_async(request, headers, runtime)
+
+    def query_merchant_ugcimages_ex(
+        self,
+        request: nftc_models.QueryMerchantUgcimagesRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> nftc_models.QueryMerchantUgcimagesResponse:
+        """
+        Description: 提供ISV  ugc铸造图片查询的openapi服务
+        Summary: ugc铸造图片查询的openapi接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            nftc_models.QueryMerchantUgcimagesResponse(),
+            self.do_request('1.0', 'antchain.nftc.merchant.ugcimages.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_merchant_ugcimages_ex_async(
+        self,
+        request: nftc_models.QueryMerchantUgcimagesRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> nftc_models.QueryMerchantUgcimagesResponse:
+        """
+        Description: 提供ISV  ugc铸造图片查询的openapi服务
+        Summary: ugc铸造图片查询的openapi接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            nftc_models.QueryMerchantUgcimagesResponse(),
+            await self.do_request_async('1.0', 'antchain.nftc.merchant.ugcimages.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_nftc-1.0.2/antchain_sdk_nftc/models.py` & `antchain_nftc-1.0.3/antchain_sdk_nftc/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
+from typing import List
 
 
 class Config(TeaModel):
     """
     Model for initing client
     """
     def __init__(
@@ -443,7 +444,105 @@
         if m.get('receive_time') is not None:
             self.receive_time = m.get('receive_time')
         if m.get('send_status') is not None:
             self.send_status = m.get('send_status')
         return self
 
 
+class QueryMerchantUgcimagesRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        record_id_list: List[str] = None,
+        biz_scene: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # ugc资产铸造记录id列表
+        self.record_id_list = record_id_list
+        # 场景
+        self.biz_scene = biz_scene
+
+    def validate(self):
+        self.validate_required(self.record_id_list, 'record_id_list')
+        self.validate_required(self.biz_scene, 'biz_scene')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.record_id_list is not None:
+            result['record_id_list'] = self.record_id_list
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('record_id_list') is not None:
+            self.record_id_list = m.get('record_id_list')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        return self
+
+
+class QueryMerchantUgcimagesResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        img_list: List[str] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 入参中id对应的图片列表
+        self.img_list = img_list
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.img_list is not None:
+            result['img_list'] = self.img_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('img_list') is not None:
+            self.img_list = m.get('img_list')
+        return self
+
+
```

### Comparing `antchain_nftc-1.0.2/setup.py` & `antchain_nftc-1.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_nftc.
 
-Created on 18/05/2023
+Created on 07/08/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_nftc"
 NAME = "antchain_nftc" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain NFTC SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

