# Comparing `tmp/flasgger_marshmallow-0.0.9.tar.gz` & `tmp/flasgger_marshmallow-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flasgger_marshmallow-0.0.9.tar", last modified: Thu Sep 22 06:23:53 2022, max compression
+gzip compressed data, was "dist/flasgger_marshmallow-0.2.0.tar", last modified: Mon Aug  7 08:42:51 2023, max compression
```

## Comparing `flasgger_marshmallow-0.0.9.tar` & `flasgger_marshmallow-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 chenxl    (1000) chenxl    (1000)        0 2022-09-22 06:23:53.000000 flasgger_marshmallow-0.0.9/
-drwxrwxr-x   0 chenxl    (1000) chenxl    (1000)        0 2022-09-22 06:23:53.000000 flasgger_marshmallow-0.0.9/flasgger_marshmallow.egg-info/
--rwxrwxrwx   0 chenxl    (1000) chenxl    (1000)      317 2022-09-22 06:23:53.000000 flasgger_marshmallow-0.0.9/flasgger_marshmallow.egg-info/SOURCES.txt
--rwxrwxrwx   0 chenxl    (1000) chenxl    (1000)       21 2022-09-22 06:23:53.000000 flasgger_marshmallow-0.0.9/flasgger_marshmallow.egg-info/top_level.txt
--rwxrwxrwx   0 chenxl    (1000) chenxl    (1000)     6137 2022-09-22 06:23:53.000000 flasgger_marshmallow-0.0.9/flasgger_marshmallow.egg-info/PKG-INFO
--rwxrwxrwx   0 chenxl    (1000) chenxl    (1000)        1 2022-09-22 06:23:53.000000 flasgger_marshmallow-0.0.9/flasgger_marshmallow.egg-info/dependency_links.txt
--rwxrwxrwx   0 chenxl    (1000) chenxl    (1000)        1 2020-11-21 07:00:08.000000 flasgger_marshmallow-0.0.9/flasgger_marshmallow.egg-info/zip-safe
--rwxrwxrwx   0 chenxl    (1000) chenxl    (1000)       83 2022-09-22 06:23:53.000000 flasgger_marshmallow-0.0.9/flasgger_marshmallow.egg-info/requires.txt
-drwxrwxr-x   0 chenxl    (1000) chenxl    (1000)        0 2022-09-22 06:23:53.000000 flasgger_marshmallow-0.0.9/flasgger_marshmallow/
--rw-rw-r--   0 chenxl    (1000) chenxl    (1000)    21071 2022-09-22 06:20:24.000000 flasgger_marshmallow-0.0.9/flasgger_marshmallow/__init__.py
--rw-rw-r--   0 chenxl    (1000) chenxl    (1000)     6137 2022-09-22 06:23:53.000000 flasgger_marshmallow-0.0.9/PKG-INFO
--rw-rw-r--   0 chenxl    (1000) chenxl    (1000)       38 2022-09-22 06:23:53.000000 flasgger_marshmallow-0.0.9/setup.cfg
--rw-rw-r--   0 chenxl    (1000) chenxl    (1000)     1073 2022-07-27 06:20:45.000000 flasgger_marshmallow-0.0.9/LICENSE
--rw-rw-r--   0 chenxl    (1000) chenxl    (1000)     1359 2022-09-22 06:11:57.000000 flasgger_marshmallow-0.0.9/setup.py
--rw-rw-r--   0 chenxl    (1000) chenxl    (1000)     5500 2022-07-27 06:20:45.000000 flasgger_marshmallow-0.0.9/README.md
+drwxrwxr-x   0 chenxl    (1000) chenxl    (1000)        0 2023-08-07 08:42:51.000000 flasgger_marshmallow-0.2.0/
+drwxrwxr-x   0 chenxl    (1000) chenxl    (1000)        0 2023-08-07 08:42:51.000000 flasgger_marshmallow-0.2.0/flasgger_marshmallow.egg-info/
+-rwxrwxrwx   0 chenxl    (1000) chenxl    (1000)      317 2023-08-07 08:42:51.000000 flasgger_marshmallow-0.2.0/flasgger_marshmallow.egg-info/SOURCES.txt
+-rwxrwxrwx   0 chenxl    (1000) chenxl    (1000)       21 2023-08-07 08:42:51.000000 flasgger_marshmallow-0.2.0/flasgger_marshmallow.egg-info/top_level.txt
+-rwxrwxrwx   0 chenxl    (1000) chenxl    (1000)     5765 2023-08-07 08:42:51.000000 flasgger_marshmallow-0.2.0/flasgger_marshmallow.egg-info/PKG-INFO
+-rwxrwxrwx   0 chenxl    (1000) chenxl    (1000)        1 2023-08-07 08:42:51.000000 flasgger_marshmallow-0.2.0/flasgger_marshmallow.egg-info/dependency_links.txt
+-rwxrwxrwx   0 chenxl    (1000) chenxl    (1000)        1 2020-11-21 07:00:08.000000 flasgger_marshmallow-0.2.0/flasgger_marshmallow.egg-info/zip-safe
+-rwxrwxrwx   0 chenxl    (1000) chenxl    (1000)       63 2023-08-07 08:42:51.000000 flasgger_marshmallow-0.2.0/flasgger_marshmallow.egg-info/requires.txt
+drwxrwxr-x   0 chenxl    (1000) chenxl    (1000)        0 2023-08-07 08:42:51.000000 flasgger_marshmallow-0.2.0/flasgger_marshmallow/
+-rw-rw-r--   0 chenxl    (1000) chenxl    (1000)    20740 2023-08-07 08:09:30.000000 flasgger_marshmallow-0.2.0/flasgger_marshmallow/__init__.py
+-rw-rw-r--   0 chenxl    (1000) chenxl    (1000)     5765 2023-08-07 08:42:51.000000 flasgger_marshmallow-0.2.0/PKG-INFO
+-rw-rw-r--   0 chenxl    (1000) chenxl    (1000)       38 2023-08-07 08:42:51.000000 flasgger_marshmallow-0.2.0/setup.cfg
+-rw-rw-r--   0 chenxl    (1000) chenxl    (1000)     1073 2022-07-27 06:20:45.000000 flasgger_marshmallow-0.2.0/LICENSE
+-rw-rw-r--   0 chenxl    (1000) chenxl    (1000)     1335 2023-08-07 08:33:47.000000 flasgger_marshmallow-0.2.0/setup.py
+-rw-rw-r--   0 chenxl    (1000) chenxl    (1000)     5128 2023-08-07 07:42:15.000000 flasgger_marshmallow-0.2.0/README.md
```

### Comparing `flasgger_marshmallow-0.0.9/flasgger_marshmallow.egg-info/PKG-INFO` & `flasgger_marshmallow-0.2.0/flasgger_marshmallow.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flasgger-marshmallow
-Version: 0.0.9
+Version: 0.2.0
 Summary: code to swagger document.
 Home-page: https://github.com/flask-rabmq/Flasgger-Marshmallow
 Author: chenxiaolong
 Author-email: cxiaolong6@gmail.com
 License: MIT
 Keywords: python flask swagger flasgger marshmallow restfull
 Platform: UNKNOWN
@@ -32,15 +32,14 @@
 
 ## A Simple Example
 
 ```python
 import logging
 
 from flasgger import Swagger
-# use basePath   from flasgger_marshmallow import Swagger
 from flask import Flask, request
 from flask_restful import Api, Resource
 from marshmallow import Schema, fields
 from flasgger_marshmallow import swagger_decorator
 
 logging.basicConfig(
     filemode="w",
@@ -119,19 +118,15 @@
 
 
 class responseHeadersSchema(Schema):
     Location = fields.String(required=True, default=1, doc='跳转地址')
     X_RateLimit_Limit = fields.Integer(
         required=True, default=1, doc='Request limit per hour',
         data_key='X-RateLimit-Limit'
-    )  # marshmallow 3
-    # X_RateLimit_Limit = fields.Integer(
-    #     required=True, default=1, doc='Request limit per hour',
-    #     load_from='X-RateLimit-Limit', dump_to='X-RateLimit-Limit'
-    # ) # marshmallow 2
+    )
 
     class Meta:
         strict = True
 
 
 class HeadersSchema(Schema):
     Login_Credential = fields.String(
@@ -170,15 +165,15 @@
     def get(self):
         """
         查询用户
         """
 
         # 获取校验后的数据
         logger.info('%s, %s', type(request.query_schema), request.query_schema)
-        return {"count": 1, "page": 1, "users": [{'username': '陈小龙'}]}
+        return {'user_name': '陈小龙'}
 
     @swagger_decorator(query_schema=QueryUserSchema, response_schema={302: RedirectResponseSchema})
     def put(self):
         """重定向实例"""
         return None, 302, {'Location': 'http://www.baidu.com', 'X-RateLimit-Limit': 2000}
 
 
@@ -211,17 +206,15 @@
 
         # 获取校验后的数据
         logger.info('%s, %s', type(request.path_schema), request.path_schema)
         return {'username': username}, 200
 
     @swagger_decorator(path_schema=UsernamePathSchema,
                        form_schema=UpdateUserSchema,
-                       response_schema={200: UserDetailResponseSchema},
-                       tags=["AAA"]
-                       )
+                       response_schema={200: UserDetailResponseSchema})
     def put(self, username):
         """
         更新用户信息
         """
         return {'username': username}, 200
```

### Comparing `flasgger_marshmallow-0.0.9/flasgger_marshmallow/__init__.py` & `flasgger_marshmallow-0.2.0/flasgger_marshmallow/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,17 @@
-import copy
 import functools
 import logging
 import re
 from collections import defaultdict
 
 import marshmallow
 import yaml
 from flasgger.base import Swagger as FSwagger
 from flasgger.constants import OPTIONAL_FIELDS
-try:
-    from flasgger.constants import OPTIONAL_OAS3_FIELDS
-except :
-    OPTIONAL_OAS3_FIELDS = [
-        'components', 'servers'
-    ]
+from flasgger.constants import OPTIONAL_OAS3_FIELDS
 from flasgger.utils import extract_definitions
 from flasgger.utils import get_specs
 from flasgger.utils import get_vendor_extension_fields
 from flasgger.utils import parse_definition_docstring
 from flask import request
 from marshmallow import __version__
 from marshmallow import fields
@@ -46,49 +40,36 @@
     fields.URL: 'string',
     fields.Email: 'string',
     fields.Str: 'string',
     fields.Bool: 'bool',
     fields.Int: 'number',
 }
 
-if int(marshmallow.__version__.split('.')[0]) == 3:
+if int(marshmallow.__version__.split('.')[1]) == 3:
     FIELDS_JSON_TYPE_MAP.update({
         fields.NaiveDateTime: 'string',
         fields.AwareDateTime: 'string',
         fields.Tuple: 'array',
     })
 
 
-def is_marsh_v3():
-    return int(marshmallow.__version__.split('.')[0]) == 3
-
-
-def data_schema(schema, data):
-    data = schema().load(data or {})
-    if not is_marsh_v3():
-        data = schema().dump(data.data).data
-    else:
-        data = schema().dump(data)
-    return data
-
-
 class Swagger(FSwagger):
 
     def get_apispecs(self, endpoint='apispec_1'):
         if not self.app.debug and endpoint in self.apispecs:
             return self.apispecs[endpoint]
 
         spec = None
         for _spec in self.config['specs']:
             if _spec['endpoint'] == endpoint:
                 spec = _spec
                 break
         if not spec:
             raise RuntimeError(
-                'Can`t find specs by endpoint {:d},'
+                'Can`t find specs by endpoint {:s},'
                 ' check your flasger`s config'.format(endpoint))
 
         data = {
             # try to get from config['SWAGGER']['info']
             # then config['SWAGGER']['specs'][x]
             # then config['SWAGGER']
             # then default
@@ -327,40 +308,26 @@
     return value, 200, {}
 
 
 def swagger_decorator(
         path_schema=None, query_schema=None,
         form_schema=None, json_schema=None,
         headers_schema=None, response_schema=None,
-        tags=None, max_length_log=None
+        tags=None
 ):
     def decorator(func):
 
-        def limit_log_length(content):
-            current_content = copy.deepcopy(content)
-            if max_length_log and len(current_content.__str__()) > max_length_log:
-                current_content = current_content.__str__()
-                return "%s...%s" % (current_content[:int(max_length_log/2)], current_content[-int(max_length_log/2):])
-            return current_content
-
-        def log_format(content):
-            content = limit_log_length(content)
-            return content
-
         def parse_simple_schema(c_schema, location):
             ret = []
             for key, value in c_schema.__dict__.get('_declared_fields').items():
                 values_real_types = list(set(FIELDS_JSON_TYPE_MAP) & set(value.__class__.__mro__))
                 values_real_types.sort(key=value.__class__.__mro__.index)
                 if not values_real_types:
                     raise '不支持的%s类型' % str(type(value))
-                if is_marsh_v3():
-                    name = getattr(value, 'data_key', None) or key
-                else:
-                    name = getattr(value, 'load_from', None) or key
+                name = value.metadata.get('data_key', '') or getattr(value, 'load_from', None) or key
                 tmp = {
                     'in': location,
                     'name': name,
                     'type': FIELDS_JSON_TYPE_MAP.get(values_real_types[0]),
                     'required': value.required if location != 'path' else True,
                     'description': value.metadata.get('doc', '')
                 }
@@ -369,18 +336,15 @@
                 ret.append(tmp)
             return ret
 
         def parse_json_schema(r_s):
             tmp = {}
             for key, value in (
                     r_s.__dict__.get('_declared_fields') or r_s.__dict__.get('declared_fields') or {}).items():
-                if is_marsh_v3():
-                    key = getattr(value, 'data_key', None) or key
-                else:
-                    key = getattr(value, 'load_from', None) or key
+                key = value.metadata.get('data_key', '') or getattr(value, 'load_from', None) or key
                 if isinstance(value, fields.Nested):
                     if value.many:
                         tmp[key] = {
                             'type': 'array',
                             'description': value.metadata.get('doc', ''),
                             'items': {
                                 'type': 'object',
@@ -480,37 +444,47 @@
             path_params = request.view_args
             query_params = request.args
             form_params = request.form
             json_params = request.get_json(silent=True) or {}
             header_params = request.headers
             logger.info(
                 'request params\npath params: %s\nquery params: %s\nform params: %s\njson params: %s\n',
-                log_format(path_params), log_format(query_params), log_format(form_params), log_format(json_params)
+                path_params, query_params, form_params, json_params
             )
             logger.info('headers: %s\n', header_params)
             request.path_schema, request.path_schema, request.form_schema = [None] * 3
             request.json_schema, request.headers_schema = [None] * 2
             try:
-                path_schema and setattr(request, 'path_schema', data_schema(path_schema, path_params))
-                query_schema and setattr(request, 'query_schema', data_schema(query_schema, query_params))
-                form_schema and setattr(request, 'form_schema', data_schema(form_schema, form_params))
-                json_schema and setattr(request, 'json_schema', data_schema(json_schema, json_params))
-                headers_schema and setattr(request, 'headers_schema', data_schema(headers_schema, dict(header_params)))
+                if __version__.startswith('3.'):
+                    path_schema and setattr(request, 'path_schema', path_schema().load(path_params or {}))
+                    query_schema and setattr(request, 'query_schema', query_schema().load(query_params or {}))
+                    form_schema and setattr(request, 'form_schema', form_schema().load(form_params or {}))
+                    json_schema and setattr(request, 'json_schema', json_schema().load(json_params or {}))
+                    headers_schema and setattr(request, 'headers_schema', headers_schema().load(dict(header_params)))
+                else:
+                    path_schema and setattr(request, 'path_schema', path_schema().load(path_params or {}).data)
+                    query_schema and setattr(request, 'query_schema', query_schema().load(query_params or {}).data)
+                    form_schema and setattr(request, 'form_schema', form_schema().load(form_params or {}).data)
+                    json_schema and setattr(request, 'json_schema', json_schema().load(json_params or {}).data)
+                    headers_schema and setattr(request, 'headers_schema',
+                                               headers_schema().load(dict(header_params)).data)
             except Exception as e:
                 return 'request error: %s' % ''.join(
                     [('%s: %s; ' % (x, ''.join(y))) for x, y in e.messages.items()]), 400
             f_result = func(*args, **kw)
             data, code, headers = unpack(f_result)
-            logger.info('response data\ndata: %s\ncode: %s\nheaders: %s\n', log_format(data), code, headers)
+            logger.info('response data\ndata: %s\ncode: %s\nheaders: %s\n', data, code, headers)
             try:
                 if response_schema and response_schema.get(code):
-                    data = data_schema(response_schema.get(code), data)
+                    data = response_schema.get(code)().load(data or {})
+                    if not __version__.startswith('3.'):
+                        data = data.data
                     r_headers_schema = getattr(response_schema.get(code).Meta, 'headers', None)
                     if r_headers_schema:
-                        headers = data_schema(r_headers_schema, headers)
+                        headers = r_headers_schema().load(headers or {})
             except Exception as e:
                 return 'response error: %s' % ''.join(
                     [('%s: %s; ' % (x, ''.join(y))) for x, y in e.messages.items()]), 400
             return data, code, headers
 
         return wrapper
```

### Comparing `flasgger_marshmallow-0.0.9/PKG-INFO` & `flasgger_marshmallow-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flasgger_marshmallow
-Version: 0.0.9
+Version: 0.2.0
 Summary: code to swagger document.
 Home-page: https://github.com/flask-rabmq/Flasgger-Marshmallow
 Author: chenxiaolong
 Author-email: cxiaolong6@gmail.com
 License: MIT
 Keywords: python flask swagger flasgger marshmallow restfull
 Platform: UNKNOWN
@@ -32,15 +32,14 @@
 
 ## A Simple Example
 
 ```python
 import logging
 
 from flasgger import Swagger
-# use basePath   from flasgger_marshmallow import Swagger
 from flask import Flask, request
 from flask_restful import Api, Resource
 from marshmallow import Schema, fields
 from flasgger_marshmallow import swagger_decorator
 
 logging.basicConfig(
     filemode="w",
@@ -119,19 +118,15 @@
 
 
 class responseHeadersSchema(Schema):
     Location = fields.String(required=True, default=1, doc='跳转地址')
     X_RateLimit_Limit = fields.Integer(
         required=True, default=1, doc='Request limit per hour',
         data_key='X-RateLimit-Limit'
-    )  # marshmallow 3
-    # X_RateLimit_Limit = fields.Integer(
-    #     required=True, default=1, doc='Request limit per hour',
-    #     load_from='X-RateLimit-Limit', dump_to='X-RateLimit-Limit'
-    # ) # marshmallow 2
+    )
 
     class Meta:
         strict = True
 
 
 class HeadersSchema(Schema):
     Login_Credential = fields.String(
@@ -170,15 +165,15 @@
     def get(self):
         """
         查询用户
         """
 
         # 获取校验后的数据
         logger.info('%s, %s', type(request.query_schema), request.query_schema)
-        return {"count": 1, "page": 1, "users": [{'username': '陈小龙'}]}
+        return {'user_name': '陈小龙'}
 
     @swagger_decorator(query_schema=QueryUserSchema, response_schema={302: RedirectResponseSchema})
     def put(self):
         """重定向实例"""
         return None, 302, {'Location': 'http://www.baidu.com', 'X-RateLimit-Limit': 2000}
 
 
@@ -211,17 +206,15 @@
 
         # 获取校验后的数据
         logger.info('%s, %s', type(request.path_schema), request.path_schema)
         return {'username': username}, 200
 
     @swagger_decorator(path_schema=UsernamePathSchema,
                        form_schema=UpdateUserSchema,
-                       response_schema={200: UserDetailResponseSchema},
-                       tags=["AAA"]
-                       )
+                       response_schema={200: UserDetailResponseSchema})
     def put(self, username):
         """
         更新用户信息
         """
         return {'username': username}, 200
```

### Comparing `flasgger_marshmallow-0.0.9/LICENSE` & `flasgger_marshmallow-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flasgger_marshmallow-0.0.9/setup.py` & `flasgger_marshmallow-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 AUTHOR = "chenxiaolong"
 
 AUTHOR_EMAIL = "cxiaolong6@gmail.com"
 
 
 URL = 'https://github.com/flask-rabmq/Flasgger-Marshmallow'
 
-VERSION = "0.0.9"
+VERSION = "0.2.0"
 
 LICENSE = "MIT"
 
-INSTALL_REQUIRES = ["flask>=1.0.0, <2.0.0", "Jinja2>=2.10.1, <3.0", "flasgger>=0.9.3", "marshmallow>=2.18.1", "PyYAML"]
+INSTALL_REQUIRES = ["flask>=1.0.0", "flasgger>=0.9.5", "marshmallow>=2.18.1, <3.0.0", "PyYAML"]
 
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type=LONG_DESCRIPTION_CONTENT_TYPE,
```

### Comparing `flasgger_marshmallow-0.0.9/README.md` & `flasgger_marshmallow-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 ## A Simple Example
 
 ```python
 import logging
 
 from flasgger import Swagger
-# use basePath   from flasgger_marshmallow import Swagger
 from flask import Flask, request
 from flask_restful import Api, Resource
 from marshmallow import Schema, fields
 from flasgger_marshmallow import swagger_decorator
 
 logging.basicConfig(
     filemode="w",
@@ -101,19 +100,15 @@
 
 
 class responseHeadersSchema(Schema):
     Location = fields.String(required=True, default=1, doc='跳转地址')
     X_RateLimit_Limit = fields.Integer(
         required=True, default=1, doc='Request limit per hour',
         data_key='X-RateLimit-Limit'
-    )  # marshmallow 3
-    # X_RateLimit_Limit = fields.Integer(
-    #     required=True, default=1, doc='Request limit per hour',
-    #     load_from='X-RateLimit-Limit', dump_to='X-RateLimit-Limit'
-    # ) # marshmallow 2
+    )
 
     class Meta:
         strict = True
 
 
 class HeadersSchema(Schema):
     Login_Credential = fields.String(
@@ -152,15 +147,15 @@
     def get(self):
         """
         查询用户
         """
 
         # 获取校验后的数据
         logger.info('%s, %s', type(request.query_schema), request.query_schema)
-        return {"count": 1, "page": 1, "users": [{'username': '陈小龙'}]}
+        return {'user_name': '陈小龙'}
 
     @swagger_decorator(query_schema=QueryUserSchema, response_schema={302: RedirectResponseSchema})
     def put(self):
         """重定向实例"""
         return None, 302, {'Location': 'http://www.baidu.com', 'X-RateLimit-Limit': 2000}
 
 
@@ -193,17 +188,15 @@
 
         # 获取校验后的数据
         logger.info('%s, %s', type(request.path_schema), request.path_schema)
         return {'username': username}, 200
 
     @swagger_decorator(path_schema=UsernamePathSchema,
                        form_schema=UpdateUserSchema,
-                       response_schema={200: UserDetailResponseSchema},
-                       tags=["AAA"]
-                       )
+                       response_schema={200: UserDetailResponseSchema})
     def put(self, username):
         """
         更新用户信息
         """
         return {'username': username}, 200
```

