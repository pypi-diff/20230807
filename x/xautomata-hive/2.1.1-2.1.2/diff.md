# Comparing `tmp/xautomata-hive-2.1.1.tar.gz` & `tmp/xautomata-hive-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xautomata-hive-2.1.1.tar", last modified: Fri Aug  4 07:52:59 2023, max compression
+gzip compressed data, was "xautomata-hive-2.1.2.tar", last modified: Mon Aug  7 12:11:25 2023, max compression
```

## Comparing `xautomata-hive-2.1.1.tar` & `xautomata-hive-2.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 07:52:59.582081 xautomata-hive-2.1.1/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10656 2023-08-04 07:52:59.582081 xautomata-hive-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10385 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 07:52:59.578081 xautomata-hive-2.1.1/hive/
--rw-r--r--   0 root         (0) root         (0)       68 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32020 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 07:52:59.582081 xautomata-hive-2.1.1/hive/cookbook/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2436 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/analytics.py
--rw-r--r--   0 root         (0) root         (0)     8313 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/anomalies.py
--rw-r--r--   0 root         (0) root         (0)    13912 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/customers.py
--rw-r--r--   0 root         (0) root         (0)     8933 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/external_tickets.py
--rw-r--r--   0 root         (0) root         (0)    31415 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/groups.py
--rw-r--r--   0 root         (0) root         (0)     4324 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/ingest.py
--rw-r--r--   0 root         (0) root         (0)     6845 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/last_status.py
--rw-r--r--   0 root         (0) root         (0)    23714 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/metric_types.py
--rw-r--r--   0 root         (0) root         (0)    26096 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/metrics.py
--rw-r--r--   0 root         (0) root         (0)    33742 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/objects.py
--rw-r--r--   0 root         (0) root         (0)     7509 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/probes.py
--rw-r--r--   0 root         (0) root         (0)     3234 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/profile_topics.py
--rw-r--r--   0 root         (0) root         (0)    20710 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/services.py
--rw-r--r--   0 root         (0) root         (0)    23773 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/sites.py
--rw-r--r--   0 root         (0) root         (0)    14591 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/tree_hierarchy.py
--rw-r--r--   0 root         (0) root         (0)    10076 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/ts_cost_management.py
--rw-r--r--   0 root         (0) root         (0)     5111 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/ts_metric.py
--rw-r--r--   0 root         (0) root         (0)    10332 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/ts_service.py
--rw-r--r--   0 root         (0) root         (0)     9053 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/users.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/virtual_domains.py
--rw-r--r--   0 root         (0) root         (0)     4102 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/webhooks.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/cookbook/widget_groups.py
--rw-r--r--   0 root         (0) root         (0)     8770 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/decorators.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3570 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/infrastrucure_keys.py
--rw-r--r--   0 root         (0) root         (0)       17 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/hive/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 07:52:59.582081 xautomata-hive-2.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      884 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 07:52:59.582081 xautomata-hive-2.1.1/xautomata_hive.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10656 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/xautomata_hive.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      964 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/xautomata_hive.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/xautomata_hive.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/xautomata_hive.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-08-04 07:52:59.000000 xautomata-hive-2.1.1/xautomata_hive.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:11:25.178283 xautomata-hive-2.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10656 2023-08-07 12:11:25.178283 xautomata-hive-2.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10385 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:11:25.174283 xautomata-hive-2.1.2/hive/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32016 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:11:25.178283 xautomata-hive-2.1.2/hive/cookbook/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/analytics.py
+-rw-r--r--   0 root         (0) root         (0)     8313 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/anomalies.py
+-rw-r--r--   0 root         (0) root         (0)    13912 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/customers.py
+-rw-r--r--   0 root         (0) root         (0)     8933 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/external_tickets.py
+-rw-r--r--   0 root         (0) root         (0)    31415 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/groups.py
+-rw-r--r--   0 root         (0) root         (0)     4324 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/ingest.py
+-rw-r--r--   0 root         (0) root         (0)     6845 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/last_status.py
+-rw-r--r--   0 root         (0) root         (0)    23714 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/metric_types.py
+-rw-r--r--   0 root         (0) root         (0)    26096 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    33742 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7509 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/probes.py
+-rw-r--r--   0 root         (0) root         (0)     3234 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/profile_topics.py
+-rw-r--r--   0 root         (0) root         (0)    20710 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/services.py
+-rw-r--r--   0 root         (0) root         (0)    23773 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/sites.py
+-rw-r--r--   0 root         (0) root         (0)    14591 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/tree_hierarchy.py
+-rw-r--r--   0 root         (0) root         (0)    10076 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/ts_cost_management.py
+-rw-r--r--   0 root         (0) root         (0)     5111 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/ts_metric.py
+-rw-r--r--   0 root         (0) root         (0)    10332 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/ts_service.py
+-rw-r--r--   0 root         (0) root         (0)     9053 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/users.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/virtual_domains.py
+-rw-r--r--   0 root         (0) root         (0)     4102 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/webhooks.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/cookbook/widget_groups.py
+-rw-r--r--   0 root         (0) root         (0)     8770 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3570 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/infrastrucure_keys.py
+-rw-r--r--   0 root         (0) root         (0)       17 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/hive/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 12:11:25.178283 xautomata-hive-2.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      884 2023-08-07 12:11:24.000000 xautomata-hive-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 12:11:25.178283 xautomata-hive-2.1.2/xautomata_hive.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10656 2023-08-07 12:11:25.000000 xautomata-hive-2.1.2/xautomata_hive.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      964 2023-08-07 12:11:25.000000 xautomata-hive-2.1.2/xautomata_hive.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 12:11:25.000000 xautomata-hive-2.1.2/xautomata_hive.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-08-07 12:11:25.000000 xautomata-hive-2.1.2/xautomata_hive.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-07 12:11:25.000000 xautomata-hive-2.1.2/xautomata_hive.egg-info/top_level.txt
```

### Comparing `xautomata-hive-2.1.1/LICENSE` & `xautomata-hive-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/PKG-INFO` & `xautomata-hive-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xautomata-hive
-Version: 2.1.1
+Version: 2.1.2
 Home-page: https://github.com/sherlogic/xautomata-hive.git
 Author: Enrico Ferro - Andrea Jacassi
 Author-email: 
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `xautomata-hive-2.1.1/README.md` & `xautomata-hive-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/api.py` & `xautomata-hive-2.1.2/hive/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,16 @@
             # tutto quello che non è bulk e query gli viene impedito di paginare
             # mentre le bulk e query post/delete possono paginare come le get
             if not bulk and not query:
                 single_page = True
                 warm_start = False
                 _params_.pop('count')
 
-            # le bulk o query post/delete non devono poter fare warm_start mai, se viene impostato a True è per errore e qui viene forzato a False
-            if bulk or query: warm_start = False
+            # le bulk post/delete non devono poter fare warm_start mai, se viene impostato a True è per errore e qui viene forzato a False
+            if bulk and not read: warm_start = False
 
         url = f'{self.root}{path}'
 
         @warmstart(active=warm_start, args_ex=[2], verbose=False)
         @paginate(single_page=single_page, page_size=page_size, skip=_params_['skip'], limit=_params_['limit'], bulk=bulk)
         @ratelimiter
         def run_request(_mode, _url, _headers, _payload, _params, **_kwargs):
```

### Comparing `xautomata-hive-2.1.1/hive/cookbook/analytics.py` & `xautomata-hive-2.1.2/hive/cookbook/analytics.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/anomalies.py` & `xautomata-hive-2.1.2/hive/cookbook/anomalies.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/customers.py` & `xautomata-hive-2.1.2/hive/cookbook/customers.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/external_tickets.py` & `xautomata-hive-2.1.2/hive/cookbook/external_tickets.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/groups.py` & `xautomata-hive-2.1.2/hive/cookbook/groups.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/ingest.py` & `xautomata-hive-2.1.2/hive/cookbook/ingest.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/last_status.py` & `xautomata-hive-2.1.2/hive/cookbook/last_status.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/metric_types.py` & `xautomata-hive-2.1.2/hive/cookbook/metric_types.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/metrics.py` & `xautomata-hive-2.1.2/hive/cookbook/metrics.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/objects.py` & `xautomata-hive-2.1.2/hive/cookbook/objects.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/probes.py` & `xautomata-hive-2.1.2/hive/cookbook/probes.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/profile_topics.py` & `xautomata-hive-2.1.2/hive/cookbook/profile_topics.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/services.py` & `xautomata-hive-2.1.2/hive/cookbook/services.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/sites.py` & `xautomata-hive-2.1.2/hive/cookbook/sites.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/tree_hierarchy.py` & `xautomata-hive-2.1.2/hive/cookbook/tree_hierarchy.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/ts_cost_management.py` & `xautomata-hive-2.1.2/hive/cookbook/ts_cost_management.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/ts_metric.py` & `xautomata-hive-2.1.2/hive/cookbook/ts_metric.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/ts_service.py` & `xautomata-hive-2.1.2/hive/cookbook/ts_service.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/users.py` & `xautomata-hive-2.1.2/hive/cookbook/users.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/virtual_domains.py` & `xautomata-hive-2.1.2/hive/cookbook/virtual_domains.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/webhooks.py` & `xautomata-hive-2.1.2/hive/cookbook/webhooks.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/cookbook/widget_groups.py` & `xautomata-hive-2.1.2/hive/cookbook/widget_groups.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/decorators.py` & `xautomata-hive-2.1.2/hive/decorators.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/hive/infrastrucure_keys.py` & `xautomata-hive-2.1.2/hive/infrastrucure_keys.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/setup.py` & `xautomata-hive-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-2.1.1/xautomata_hive.egg-info/PKG-INFO` & `xautomata-hive-2.1.2/xautomata_hive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xautomata-hive
-Version: 2.1.1
+Version: 2.1.2
 Home-page: https://github.com/sherlogic/xautomata-hive.git
 Author: Enrico Ferro - Andrea Jacassi
 Author-email: 
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `xautomata-hive-2.1.1/xautomata_hive.egg-info/SOURCES.txt` & `xautomata-hive-2.1.2/xautomata_hive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

