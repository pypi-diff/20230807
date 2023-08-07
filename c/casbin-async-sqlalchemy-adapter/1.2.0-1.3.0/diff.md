# Comparing `tmp/casbin_async_sqlalchemy_adapter-1.2.0.tar.gz` & `tmp/casbin_async_sqlalchemy_adapter-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin_async_sqlalchemy_adapter-1.2.0.tar", last modified: Sun Jul 16 15:29:21 2023, max compression
+gzip compressed data, was "casbin_async_sqlalchemy_adapter-1.3.0.tar", last modified: Mon Aug  7 04:04:01 2023, max compression
```

## Comparing `casbin_async_sqlalchemy_adapter-1.2.0.tar` & `casbin_async_sqlalchemy_adapter-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:29:21.138502 casbin_async_sqlalchemy_adapter-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-16 15:28:44.000000 casbin_async_sqlalchemy_adapter-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-16 15:29:21.142502 casbin_async_sqlalchemy_adapter-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-16 15:28:44.000000 casbin_async_sqlalchemy_adapter-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:29:21.138502 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-16 15:28:44.000000 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-16 15:28:44.000000 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:29:21.138502 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-16 15:29:21.000000 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-16 15:29:21.000000 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:29:21.000000 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-16 15:29:21.000000 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-16 15:29:21.000000 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-16 15:29:21.142502 casbin_async_sqlalchemy_adapter-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-16 15:28:44.000000 casbin_async_sqlalchemy_adapter-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:29:21.138502 casbin_async_sqlalchemy_adapter-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-07-16 15:28:44.000000 casbin_async_sqlalchemy_adapter-1.2.0/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:04:01.565668 casbin_async_sqlalchemy_adapter-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 04:03:24.000000 casbin_async_sqlalchemy_adapter-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-08-07 04:04:01.565668 casbin_async_sqlalchemy_adapter-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-08-07 04:03:24.000000 casbin_async_sqlalchemy_adapter-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:04:01.565668 casbin_async_sqlalchemy_adapter-1.3.0/casbin_async_sqlalchemy_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-07 04:03:24.000000 casbin_async_sqlalchemy_adapter-1.3.0/casbin_async_sqlalchemy_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-08-07 04:03:24.000000 casbin_async_sqlalchemy_adapter-1.3.0/casbin_async_sqlalchemy_adapter/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:04:01.565668 casbin_async_sqlalchemy_adapter-1.3.0/casbin_async_sqlalchemy_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-08-07 04:04:01.000000 casbin_async_sqlalchemy_adapter-1.3.0/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-07 04:04:01.000000 casbin_async_sqlalchemy_adapter-1.3.0/casbin_async_sqlalchemy_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 04:04:01.000000 casbin_async_sqlalchemy_adapter-1.3.0/casbin_async_sqlalchemy_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-07 04:04:01.000000 casbin_async_sqlalchemy_adapter-1.3.0/casbin_async_sqlalchemy_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-07 04:04:01.000000 casbin_async_sqlalchemy_adapter-1.3.0/casbin_async_sqlalchemy_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-07 04:04:01.565668 casbin_async_sqlalchemy_adapter-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-08-07 04:03:24.000000 casbin_async_sqlalchemy_adapter-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:04:01.565668 casbin_async_sqlalchemy_adapter-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17768 2023-08-07 04:03:24.000000 casbin_async_sqlalchemy_adapter-1.3.0/tests/test_adapter.py
```

### Comparing `casbin_async_sqlalchemy_adapter-1.2.0/LICENSE` & `casbin_async_sqlalchemy_adapter-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.2.0/PKG-INFO` & `casbin_async_sqlalchemy_adapter-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin_async_sqlalchemy_adapter
-Version: 1.2.0
+Version: 1.3.0
 Summary: Asynchronous SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/async-sqlalchemy-adapter
 Author: wrapping-2000
 Author-email: wenpengchen@njust.edu.cn
 License: Apache 2.0
 Keywords: asynccasbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `casbin_async_sqlalchemy_adapter-1.2.0/README.md` & `casbin_async_sqlalchemy_adapter-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter/__init__.py` & `casbin_async_sqlalchemy_adapter-1.3.0/casbin_async_sqlalchemy_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter/adapter.py` & `casbin_async_sqlalchemy_adapter-1.3.0/casbin_async_sqlalchemy_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO` & `casbin_async_sqlalchemy_adapter-1.3.0/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-async-sqlalchemy-adapter
-Version: 1.2.0
+Version: 1.3.0
 Summary: Asynchronous SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/async-sqlalchemy-adapter
 Author: wrapping-2000
 Author-email: wenpengchen@njust.edu.cn
 License: Apache 2.0
 Keywords: asynccasbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `casbin_async_sqlalchemy_adapter-1.2.0/setup.py` & `casbin_async_sqlalchemy_adapter-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.2.0/tests/test_adapter.py` & `casbin_async_sqlalchemy_adapter-1.3.0/tests/test_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         s.add(CasbinRule(ptype="p", v0="alice", v1="data1", v2="read"))
         s.add(CasbinRule(ptype="p", v0="bob", v1="data2", v2="write"))
         s.add(CasbinRule(ptype="p", v0="data2_admin", v1="data2", v2="read"))
         s.add(CasbinRule(ptype="p", v0="data2_admin", v1="data2", v2="write"))
         s.add(CasbinRule(ptype="g", v0="alice", v1="data2_admin"))
         await s.commit()
 
-    e = casbin.Enforcer(get_fixture("rbac_model.conf"), adapter)
+    e = casbin.AsyncEnforcer(get_fixture("rbac_model.conf"), adapter)
     await e.load_policy()
     return e
 
 
 class TestConfig(IsolatedAsyncioTestCase):
     async def test_custom_db_class(self):
         class CustomRule(Base):
@@ -367,15 +367,14 @@
 
         self.assertFalse(e.enforce("data2_admin", "data2", "read"))
         self.assertTrue(e.enforce("data2_admin", "data_test", "read"))
 
         self.assertFalse(e.enforce("data2_admin", "data2", "write"))
         self.assertTrue(e.enforce("data2_admin", "data_test", "write"))
     
-    @unittest.skip('update_filtered_policies not supported by asynccasbin')
     async def test_update_filtered_policies(self):
         e = await get_enforcer()
 
         await e.update_filtered_policies(
             [
                 ["data2_admin", "data3", "read"],
                 ["data2_admin", "data3", "write"],
```

