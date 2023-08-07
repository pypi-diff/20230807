# Comparing `tmp/azurly-0.1.0.tar.gz` & `tmp/azurly-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azurly-0.1.0.tar", last modified: Tue Jul  4 06:55:37 2023, max compression
+gzip compressed data, was "azurly-0.1.1.tar", last modified: Mon Aug  7 20:02:14 2023, max compression
```

## Comparing `azurly-0.1.0.tar` & `azurly-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 06:55:37.178354 azurly-0.1.0/
--rw-rw-rw-   0        0        0      219 2023-07-04 06:55:37.178354 azurly-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-04 06:55:37.178354 azurly-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      316 2023-07-04 06:55:04.000000 azurly-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 06:55:37.162836 azurly-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 06:55:37.178354 azurly-0.1.0/src/azurly/
--rw-rw-rw-   0        0        0     5345 2023-07-04 06:55:04.000000 azurly-0.1.0/src/azurly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 06:55:37.178354 azurly-0.1.0/src/azurly/api/
--rw-rw-rw-   0        0        0    10241 2023-07-04 06:55:04.000000 azurly-0.1.0/src/azurly/api/__init__.py
--rw-rw-rw-   0        0        0    13159 2023-07-04 06:55:04.000000 azurly-0.1.0/src/azurly/api/storage.py
--rw-rw-rw-   0        0        0     4081 2023-07-04 06:55:04.000000 azurly-0.1.0/src/azurly/storage.py
-drwxrwxrwx   0        0        0        0 2023-07-04 06:55:37.178354 azurly-0.1.0/src/azurly.egg-info/
--rw-rw-rw-   0        0        0      219 2023-07-04 06:55:37.000000 azurly-0.1.0/src/azurly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-07-04 06:55:37.000000 azurly-0.1.0/src/azurly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 06:55:37.000000 azurly-0.1.0/src/azurly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-04 06:55:37.000000 azurly-0.1.0/src/azurly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 20:02:14.913130 azurly-0.1.1/
+-rw-rw-rw-   0        0        0     1074 2023-08-07 20:01:33.000000 azurly-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0     4446 2023-08-07 20:02:14.913130 azurly-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4220 2023-08-07 20:01:33.000000 azurly-0.1.1/README.md
+-rw-rw-rw-   0        0        0      336 2023-08-07 20:01:33.000000 azurly-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 20:02:14.913130 azurly-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 20:02:14.897508 azurly-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 20:02:14.913130 azurly-0.1.1/src/azurly/
+-rw-rw-rw-   0        0        0     5393 2023-08-07 20:01:33.000000 azurly-0.1.1/src/azurly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:02:14.913130 azurly-0.1.1/src/azurly/api/
+-rw-rw-rw-   0        0        0    10241 2023-08-07 20:01:33.000000 azurly-0.1.1/src/azurly/api/__init__.py
+-rw-rw-rw-   0        0        0    14866 2023-08-07 20:01:33.000000 azurly-0.1.1/src/azurly/api/batch.py
+-rw-rw-rw-   0        0        0    13159 2023-08-07 20:01:33.000000 azurly-0.1.1/src/azurly/api/storage.py
+-rw-rw-rw-   0        0        0     1599 2023-08-07 20:01:33.000000 azurly-0.1.1/src/azurly/batch.py
+-rw-rw-rw-   0        0        0     4081 2023-08-07 20:01:33.000000 azurly-0.1.1/src/azurly/storage.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:02:14.913130 azurly-0.1.1/src/azurly.egg-info/
+-rw-rw-rw-   0        0        0     4446 2023-08-07 20:02:14.000000 azurly-0.1.1/src/azurly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-08-07 20:02:14.000000 azurly-0.1.1/src/azurly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 20:02:14.000000 azurly-0.1.1/src/azurly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-08-07 20:02:14.000000 azurly-0.1.1/src/azurly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 20:02:14.000000 azurly-0.1.1/src/azurly.egg-info/top_level.txt
```

### Comparing `azurly-0.1.0/src/azurly/__init__.py` & `azurly-0.1.1/src/azurly/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,21 +45,21 @@
 
     def _destroy(self) -> bool:
         # This method will be defined per child class.
         return self._destroy_api()
 
     # Unique methods for each child class.
     def _build_template(self):
-        pass
+        return True
 
     def _deploy_api(self):
-        pass
+        return True
 
     def _destroy_api(self):
-        pass
+        return True
 
 
 class _AzureGroup(_AzureResource):
 
     def __init__(self, name: str, group: 'AzureGroup'):
         super().__init__(name=name, group=group)
 
@@ -139,15 +139,15 @@
         bool:
             True, all the resources have been deployed successfully.
             False, deploying a resource failed.
         """
         try:
             for resource in self._resources:
                 if not resource._deploy():
-                    self._main._logger.warning(f'Deploying {resource._name} failed!')
+                    self._main._logger.warning(f'Deploying {resource._name} failed, because it already exists.')
                     return False
 
             self._main._logger.info(f'Deploying resources for {self._name} succeeded.\n')
             return True
 
         except Exception as e:
             if self.rollback:
```

### Comparing `azurly-0.1.0/src/azurly/api/__init__.py` & `azurly-0.1.1/src/azurly/api/__init__.py`

 * *Files identical despite different names*

### Comparing `azurly-0.1.0/src/azurly/api/storage.py` & `azurly-0.1.1/src/azurly/api/storage.py`

 * *Files identical despite different names*

### Comparing `azurly-0.1.0/src/azurly/storage.py` & `azurly-0.1.1/src/azurly/storage.py`

 * *Files identical despite different names*

