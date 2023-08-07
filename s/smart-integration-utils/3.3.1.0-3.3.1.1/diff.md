# Comparing `tmp/smart-integration-utils-3.3.1.0.tar.gz` & `tmp/smart-integration-utils-3.3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart-integration-utils-3.3.1.0.tar", last modified: Mon Aug  7 09:04:39 2023, max compression
+gzip compressed data, was "smart-integration-utils-3.3.1.1.tar", last modified: Mon Aug  7 09:40:27 2023, max compression
```

## Comparing `smart-integration-utils-3.3.1.0.tar` & `smart-integration-utils-3.3.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-08-07 09:04:39.679834 smart-integration-utils-3.3.1.0/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       92 2023-08-07 09:04:39.679834 smart-integration-utils-3.3.1.0/PKG-INFO
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    11397 2023-08-07 09:04:34.000000 smart-integration-utils-3.3.1.0/README.md
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-08-07 09:04:39.679834 smart-integration-utils-3.3.1.0/integration_utils/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       46 2023-08-07 09:04:34.000000 smart-integration-utils-3.3.1.0/integration_utils/__init__.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1818 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.1.0/integration_utils/comparison.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      814 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.1.0/integration_utils/exceptions.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      912 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.0/integration_utils/fields.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7867 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.0/integration_utils/filters.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4755 2023-08-07 09:04:34.000000 smart-integration-utils-3.3.1.0/integration_utils/mixins.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3333 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.1.0/integration_utils/pagination.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1970 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.0/integration_utils/serializers.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7266 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.0/integration_utils/services.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    14505 2023-08-07 09:04:34.000000 smart-integration-utils-3.3.1.0/integration_utils/tools.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3341 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.0/integration_utils/utils.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4668 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.1.0/integration_utils/views.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       38 2023-08-07 09:04:39.679834 smart-integration-utils-3.3.1.0/setup.cfg
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      535 2022-10-25 14:02:55.000000 smart-integration-utils-3.3.1.0/setup.py
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-08-07 09:04:39.679834 smart-integration-utils-3.3.1.0/smart_integration_utils.egg-info/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       92 2023-08-07 09:04:39.000000 smart-integration-utils-3.3.1.0/smart_integration_utils.egg-info/PKG-INFO
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      607 2023-08-07 09:04:39.000000 smart-integration-utils-3.3.1.0/smart_integration_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        1 2023-08-07 09:04:39.000000 smart-integration-utils-3.3.1.0/smart_integration_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      104 2023-08-07 09:04:39.000000 smart-integration-utils-3.3.1.0/smart_integration_utils.egg-info/requires.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       18 2023-08-07 09:04:39.000000 smart-integration-utils-3.3.1.0/smart_integration_utils.egg-info/top_level.txt
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-08-07 09:40:27.599614 smart-integration-utils-3.3.1.1/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       92 2023-08-07 09:40:27.599614 smart-integration-utils-3.3.1.1/PKG-INFO
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    11397 2023-08-07 09:04:34.000000 smart-integration-utils-3.3.1.1/README.md
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-08-07 09:40:27.599614 smart-integration-utils-3.3.1.1/integration_utils/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       46 2023-08-07 09:40:20.000000 smart-integration-utils-3.3.1.1/integration_utils/__init__.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1818 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.1.1/integration_utils/comparison.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      814 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.1.1/integration_utils/exceptions.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      912 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.1/integration_utils/fields.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7867 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.1/integration_utils/filters.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4755 2023-08-07 09:04:34.000000 smart-integration-utils-3.3.1.1/integration_utils/mixins.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3399 2023-08-07 09:40:20.000000 smart-integration-utils-3.3.1.1/integration_utils/pagination.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1970 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.1/integration_utils/serializers.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7266 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.1/integration_utils/services.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    14505 2023-08-07 09:04:34.000000 smart-integration-utils-3.3.1.1/integration_utils/tools.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3341 2022-10-25 11:05:32.000000 smart-integration-utils-3.3.1.1/integration_utils/utils.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4668 2022-10-25 12:44:54.000000 smart-integration-utils-3.3.1.1/integration_utils/views.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       38 2023-08-07 09:40:27.599614 smart-integration-utils-3.3.1.1/setup.cfg
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      535 2022-10-25 14:02:55.000000 smart-integration-utils-3.3.1.1/setup.py
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-08-07 09:40:27.599614 smart-integration-utils-3.3.1.1/smart_integration_utils.egg-info/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       92 2023-08-07 09:40:27.000000 smart-integration-utils-3.3.1.1/smart_integration_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      607 2023-08-07 09:40:27.000000 smart-integration-utils-3.3.1.1/smart_integration_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        1 2023-08-07 09:40:27.000000 smart-integration-utils-3.3.1.1/smart_integration_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      104 2023-08-07 09:40:27.000000 smart-integration-utils-3.3.1.1/smart_integration_utils.egg-info/requires.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       18 2023-08-07 09:40:27.000000 smart-integration-utils-3.3.1.1/smart_integration_utils.egg-info/top_level.txt
```

### Comparing `smart-integration-utils-3.3.1.0/README.md` & `smart-integration-utils-3.3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.1.0/integration_utils/comparison.py` & `smart-integration-utils-3.3.1.1/integration_utils/comparison.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.1.0/integration_utils/exceptions.py` & `smart-integration-utils-3.3.1.1/integration_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.1.0/integration_utils/fields.py` & `smart-integration-utils-3.3.1.1/integration_utils/fields.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.1.0/integration_utils/filters.py` & `smart-integration-utils-3.3.1.1/integration_utils/filters.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.1.0/integration_utils/mixins.py` & `smart-integration-utils-3.3.1.1/integration_utils/mixins.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.1.0/integration_utils/pagination.py` & `smart-integration-utils-3.3.1.1/integration_utils/pagination.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     you always have:
     self.integration_id
     self.date_form
     self.date_to
     """
 
     check_credential = False
+    with_smart_auth = False
     limit = None
     offset = None
     max_limit = None
     pagination_class = StandardResultsPagination
 
     def _ensure_limit_param(self):
         if self.limit:
@@ -73,14 +74,15 @@
 
     def get_fields(self) -> list:
         return []
 
     def list(self, request, format=None):
         self._get_params()
         self._ensure_limit_param()
+        self.get_check_admin(request)
         queryset = self.get_queryset()
         page = self.paginate_queryset(queryset)
         if page is not None:
             serializer = self.get_serializer(
                 page,
                 many=True,
                 context={
```

### Comparing `smart-integration-utils-3.3.1.0/integration_utils/serializers.py` & `smart-integration-utils-3.3.1.1/integration_utils/serializers.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.1.0/integration_utils/services.py` & `smart-integration-utils-3.3.1.1/integration_utils/services.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.1.0/integration_utils/tools.py` & `smart-integration-utils-3.3.1.1/integration_utils/tools.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.1.0/integration_utils/utils.py` & `smart-integration-utils-3.3.1.1/integration_utils/utils.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.1.0/integration_utils/views.py` & `smart-integration-utils-3.3.1.1/integration_utils/views.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.1.0/setup.py` & `smart-integration-utils-3.3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `smart-integration-utils-3.3.1.0/smart_integration_utils.egg-info/SOURCES.txt` & `smart-integration-utils-3.3.1.1/smart_integration_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

