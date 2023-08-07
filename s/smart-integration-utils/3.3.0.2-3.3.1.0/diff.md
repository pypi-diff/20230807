# Comparing `tmp/smart-integration-utils-3.3.0.2.tar.gz` & `tmp/smart-integration-utils-3.3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart-integration-utils-3.3.0.2.tar", last modified: Thu Apr 27 11:41:24 2023, max compression
+gzip compressed data, was "smart-integration-utils-3.3.1.0.tar", last modified: Mon Aug  7 09:04:39 2023, max compression
```

## Comparing `smart-integration-utils-3.3.0.2.tar` & `smart-integration-utils-3.3.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-04-27 11:41:24.171010 smart-integration-utils-3.3.0.2/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       92 2023-04-27 11:41:24.171010 smart-integration-utils-3.3.0.2/PKG-INFO
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    11362 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.0.2/README.md
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-04-27 11:41:24.171010 smart-integration-utils-3.3.0.2/integration_utils/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       46 2023-04-27 11:40:55.000000 smart-integration-utils-3.3.0.2/integration_utils/__init__.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1818 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.0.2/integration_utils/comparison.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      814 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.0.2/integration_utils/exceptions.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      912 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.0.2/integration_utils/fields.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7867 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.0.2/integration_utils/filters.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4708 2023-04-27 11:27:36.000000 smart-integration-utils-3.3.0.2/integration_utils/mixins.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3333 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.0.2/integration_utils/pagination.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1970 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.0.2/integration_utils/serializers.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7266 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.0.2/integration_utils/services.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    14505 2023-04-27 11:41:09.000000 smart-integration-utils-3.3.0.2/integration_utils/tools.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3341 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.0.2/integration_utils/utils.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4668 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.0.2/integration_utils/views.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       38 2023-04-27 11:41:24.171010 smart-integration-utils-3.3.0.2/setup.cfg
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      535 2022-10-25 14:02:55.000000 smart-integration-utils-3.3.0.2/setup.py
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-04-27 11:41:24.171010 smart-integration-utils-3.3.0.2/smart_integration_utils.egg-info/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       92 2023-04-27 11:41:24.000000 smart-integration-utils-3.3.0.2/smart_integration_utils.egg-info/PKG-INFO
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      607 2023-04-27 11:41:24.000000 smart-integration-utils-3.3.0.2/smart_integration_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        1 2023-04-27 11:41:24.000000 smart-integration-utils-3.3.0.2/smart_integration_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      104 2023-04-27 11:41:24.000000 smart-integration-utils-3.3.0.2/smart_integration_utils.egg-info/requires.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       18 2023-04-27 11:41:24.000000 smart-integration-utils-3.3.0.2/smart_integration_utils.egg-info/top_level.txt
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-08-07 09:04:39.679834 smart-integration-utils-3.3.1.0/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       92 2023-08-07 09:04:39.679834 smart-integration-utils-3.3.1.0/PKG-INFO
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    11397 2023-08-07 09:04:34.000000 smart-integration-utils-3.3.1.0/README.md
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-08-07 09:04:39.679834 smart-integration-utils-3.3.1.0/integration_utils/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       46 2023-08-07 09:04:34.000000 smart-integration-utils-3.3.1.0/integration_utils/__init__.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1818 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.1.0/integration_utils/comparison.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      814 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.1.0/integration_utils/exceptions.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      912 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.0/integration_utils/fields.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7867 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.0/integration_utils/filters.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4755 2023-08-07 09:04:34.000000 smart-integration-utils-3.3.1.0/integration_utils/mixins.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3333 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.1.0/integration_utils/pagination.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1970 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.0/integration_utils/serializers.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7266 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.0/integration_utils/services.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    14505 2023-08-07 09:04:34.000000 smart-integration-utils-3.3.1.0/integration_utils/tools.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3341 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.0/integration_utils/utils.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4668 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.1.0/integration_utils/views.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       38 2023-08-07 09:04:39.679834 smart-integration-utils-3.3.1.0/setup.cfg
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      535 2022-10-25 14:02:55.000000 smart-integration-utils-3.3.1.0/setup.py
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-08-07 09:04:39.679834 smart-integration-utils-3.3.1.0/smart_integration_utils.egg-info/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       92 2023-08-07 09:04:39.000000 smart-integration-utils-3.3.1.0/smart_integration_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      607 2023-08-07 09:04:39.000000 smart-integration-utils-3.3.1.0/smart_integration_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        1 2023-08-07 09:04:39.000000 smart-integration-utils-3.3.1.0/smart_integration_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      104 2023-08-07 09:04:39.000000 smart-integration-utils-3.3.1.0/smart_integration_utils.egg-info/requires.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       18 2023-08-07 09:04:39.000000 smart-integration-utils-3.3.1.0/smart_integration_utils.egg-info/top_level.txt
```

### Comparing `smart-integration-utils-3.3.0.2/README.md` & `smart-integration-utils-3.3.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -302,7 +302,8 @@
 - 2.8.9 - fix parse_for_django_query with AND statement
 - 2.8.8 - fix parse_for_mongo_query with OR statement
 - 2.8.7 - upload_to_s3_from_ram now upload from BytesIO and StringIO
 - 2.8.6 - support platform_id in BaseReportListAPIView
 - 2.8.5 - add parse_for_mongo_query, parse_for_django_query tools in filters.py
 - 2.8.4 - fix tools for python3.7
 - 2.8.1 - remove parse_filters, create_filter_results from filters.py, add validate_data func
+- 3.3.1.0 - update get_check_admin
```

### Comparing `smart-integration-utils-3.3.0.2/integration_utils/comparison.py` & `smart-integration-utils-3.3.1.0/integration_utils/comparison.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.0.2/integration_utils/exceptions.py` & `smart-integration-utils-3.3.1.0/integration_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.0.2/integration_utils/fields.py` & `smart-integration-utils-3.3.1.0/integration_utils/fields.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.0.2/integration_utils/filters.py` & `smart-integration-utils-3.3.1.0/integration_utils/filters.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.0.2/integration_utils/mixins.py` & `smart-integration-utils-3.3.1.0/integration_utils/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,16 @@
         if 'auth_info' in json_response:
             return json_response['auth_info']
         return json_response
 
     def get_check_admin(self, request, *args, **kwargs):
         user_info = self.get_user_info(request, *args, **kwargs)
         user_id = user_info["id"]
-        if user_id in (19, 22, 23, 55):
+        status_info = user_info['status_info']
+        if status_info['is_superuser']:
             return user_id
         raise PermissionDenied(
             {"status": "error", "message": "This endpoint only for smart admin users."}
         )
 
 
 class CredentialMixin(BaseCredentialMixin):
```

### Comparing `smart-integration-utils-3.3.0.2/integration_utils/pagination.py` & `smart-integration-utils-3.3.1.0/integration_utils/pagination.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.0.2/integration_utils/serializers.py` & `smart-integration-utils-3.3.1.0/integration_utils/serializers.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.0.2/integration_utils/services.py` & `smart-integration-utils-3.3.1.0/integration_utils/services.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.0.2/integration_utils/tools.py` & `smart-integration-utils-3.3.1.0/integration_utils/tools.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.0.2/integration_utils/utils.py` & `smart-integration-utils-3.3.1.0/integration_utils/utils.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.0.2/integration_utils/views.py` & `smart-integration-utils-3.3.1.0/integration_utils/views.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.0.2/setup.py` & `smart-integration-utils-3.3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.0.2/smart_integration_utils.egg-info/SOURCES.txt` & `smart-integration-utils-3.3.1.0/smart_integration_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

