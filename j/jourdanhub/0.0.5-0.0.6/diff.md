# Comparing `tmp/jourdanhub-0.0.5.tar.gz` & `tmp/jourdanhub-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jourdanhub-0.0.5.tar", last modified: Mon Aug  7 17:36:55 2023, max compression
+gzip compressed data, was "jourdanhub-0.0.6.tar", last modified: Mon Aug  7 17:40:41 2023, max compression
```

## Comparing `jourdanhub-0.0.5.tar` & `jourdanhub-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 17:36:55.916747 jourdanhub-0.0.5/
--rw-rw-rw-   0        0        0      225 2023-08-07 12:11:20.000000 jourdanhub-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      647 2023-08-07 17:36:55.917747 jourdanhub-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-08-07 15:23:12.000000 jourdanhub-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 17:36:55.842241 jourdanhub-0.0.5/jourdanhub/
--rw-rw-rw-   0        0        0       36 2023-08-07 12:18:23.000000 jourdanhub-0.0.5/jourdanhub/__init__.py
--rw-rw-rw-   0        0        0       63 2023-08-07 12:06:01.000000 jourdanhub-0.0.5/jourdanhub/__main__.py
--rw-rw-rw-   0        0        0       23 2023-08-07 17:36:52.000000 jourdanhub-0.0.5/jourdanhub/_version.py
--rw-rw-rw-   0        0        0      657 2023-08-07 14:11:31.000000 jourdanhub-0.0.5/jourdanhub/app.py
--rw-rw-rw-   0        0        0     2113 2023-08-07 17:36:41.000000 jourdanhub-0.0.5/jourdanhub/userapi_handler.py
-drwxrwxrwx   0        0        0        0 2023-08-07 17:36:55.914782 jourdanhub-0.0.5/jourdanhub.egg-info/
--rw-rw-rw-   0        0        0      647 2023-08-07 17:36:55.000000 jourdanhub-0.0.5/jourdanhub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-08-07 17:36:55.000000 jourdanhub-0.0.5/jourdanhub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 17:36:55.000000 jourdanhub-0.0.5/jourdanhub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-08-07 17:36:55.000000 jourdanhub-0.0.5/jourdanhub.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-08-07 16:00:20.000000 jourdanhub-0.0.5/jourdanhub.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-08-07 17:36:55.000000 jourdanhub-0.0.5/jourdanhub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-07 17:36:55.000000 jourdanhub-0.0.5/jourdanhub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      130 2023-08-07 12:11:10.000000 jourdanhub-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-08-07 17:36:55.920168 jourdanhub-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1327 2023-08-07 16:00:01.000000 jourdanhub-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:40:41.816770 jourdanhub-0.0.6/
+-rw-rw-rw-   0        0        0      225 2023-08-07 12:11:20.000000 jourdanhub-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      647 2023-08-07 17:40:41.816770 jourdanhub-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-08-07 15:23:12.000000 jourdanhub-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 17:40:41.776515 jourdanhub-0.0.6/jourdanhub/
+-rw-rw-rw-   0        0        0       36 2023-08-07 12:18:23.000000 jourdanhub-0.0.6/jourdanhub/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-08-07 12:06:01.000000 jourdanhub-0.0.6/jourdanhub/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-08-07 17:40:35.000000 jourdanhub-0.0.6/jourdanhub/_version.py
+-rw-rw-rw-   0        0        0      657 2023-08-07 14:11:31.000000 jourdanhub-0.0.6/jourdanhub/app.py
+-rw-rw-rw-   0        0        0     2151 2023-08-07 17:40:27.000000 jourdanhub-0.0.6/jourdanhub/userapi_handler.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:40:41.815876 jourdanhub-0.0.6/jourdanhub.egg-info/
+-rw-rw-rw-   0        0        0      647 2023-08-07 17:40:41.000000 jourdanhub-0.0.6/jourdanhub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-08-07 17:40:41.000000 jourdanhub-0.0.6/jourdanhub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 17:40:41.000000 jourdanhub-0.0.6/jourdanhub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-08-07 17:40:41.000000 jourdanhub-0.0.6/jourdanhub.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 16:00:20.000000 jourdanhub-0.0.6/jourdanhub.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-08-07 17:40:41.000000 jourdanhub-0.0.6/jourdanhub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-07 17:40:41.000000 jourdanhub-0.0.6/jourdanhub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      130 2023-08-07 12:11:10.000000 jourdanhub-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-08-07 17:40:41.818754 jourdanhub-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1327 2023-08-07 16:00:01.000000 jourdanhub-0.0.6/setup.py
```

### Comparing `jourdanhub-0.0.5/PKG-INFO` & `jourdanhub-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jourdanhub
-Version: 0.0.5
+Version: 0.0.6
 Summary: Wrapper for JupyterHub
 Home-page: https://github.com/carlosjourdan/jourdanhub
 Author: Carlos Jourdan
 License: AGPL-3.0
 Keywords: JupyterHub,SWAN,CERN
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `jourdanhub-0.0.5/jourdanhub/app.py` & `jourdanhub-0.0.6/jourdanhub/app.py`

 * *Files identical despite different names*

### Comparing `jourdanhub-0.0.5/jourdanhub/userapi_handler.py` & `jourdanhub-0.0.6/jourdanhub/userapi_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,8 +60,10 @@
         else:
             model["session_id"] = None
 
         # add scopes to identify model,
         # but not the scopes we added to ensure we could read our own model
         #model["scopes"] = sorted(self.expanded_scopes.difference(_added_scopes))
         model["scopes"] = sorted(self.expanded_scopes)
+
+        model["jourdan"] = "teste"
         self.write(json.dumps(model))
```

### Comparing `jourdanhub-0.0.5/jourdanhub.egg-info/PKG-INFO` & `jourdanhub-0.0.6/jourdanhub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jourdanhub
-Version: 0.0.5
+Version: 0.0.6
 Summary: Wrapper for JupyterHub
 Home-page: https://github.com/carlosjourdan/jourdanhub
 Author: Carlos Jourdan
 License: AGPL-3.0
 Keywords: JupyterHub,SWAN,CERN
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `jourdanhub-0.0.5/setup.py` & `jourdanhub-0.0.6/setup.py`

 * *Files identical despite different names*

