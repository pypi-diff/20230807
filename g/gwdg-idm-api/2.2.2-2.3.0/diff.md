# Comparing `tmp/gwdg_idm_api-2.2.2.tar.gz` & `tmp/gwdg_idm_api-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdg_idm_api-2.2.2.tar", last modified: Tue Aug  1 09:45:45 2023, max compression
+gzip compressed data, was "gwdg_idm_api-2.3.0.tar", last modified: Mon Aug  7 08:50:34 2023, max compression
```

## Comparing `gwdg_idm_api-2.2.2.tar` & `gwdg_idm_api-2.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:45:45.565526 gwdg_idm_api-2.2.2/
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      279 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      685 2023-08-01 09:45:45.565526 gwdg_idm_api-2.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-08-01 09:45:45.569526 gwdg_idm_api-2.2.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:45:45.561526 gwdg_idm_api-2.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:45:45.565526 gwdg_idm_api-2.2.2/src/gwdg_idm_api/
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-08-01 09:45:45.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     5096 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api/benutzerverwaltung.py
--rw-rw-rw-   0 root         (0) root         (0)     6930 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6878 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api/string_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:45:45.565526 gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      685 2023-08-01 09:45:45.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      566 2023-08-01 09:45:45.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 09:45:45.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 09:45:45.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       50 2023-08-01 09:45:45.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-01 09:45:45.000000 gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:45:45.565526 gwdg_idm_api-2.2.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3617 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/tests/examples.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/tests/predict_username.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-08-01 09:45:28.000000 gwdg_idm_api-2.2.2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:50:34.280228 gwdg_idm_api-2.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-08-07 08:50:16.000000 gwdg_idm_api-2.3.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-08-07 08:50:16.000000 gwdg_idm_api-2.3.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2023-08-07 08:50:16.000000 gwdg_idm_api-2.3.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-08-07 08:50:16.000000 gwdg_idm_api-2.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      685 2023-08-07 08:50:34.280228 gwdg_idm_api-2.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-08-07 08:50:16.000000 gwdg_idm_api-2.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-08-07 08:50:16.000000 gwdg_idm_api-2.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-08-07 08:50:34.280228 gwdg_idm_api-2.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:50:34.272229 gwdg_idm_api-2.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:50:34.276229 gwdg_idm_api-2.3.0/src/gwdg_idm_api/
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-08-07 08:50:16.000000 gwdg_idm_api-2.3.0/src/gwdg_idm_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-08-07 08:50:34.000000 gwdg_idm_api-2.3.0/src/gwdg_idm_api/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5240 2023-08-07 08:50:16.000000 gwdg_idm_api-2.3.0/src/gwdg_idm_api/benutzerverwaltung.py
+-rw-rw-rw-   0 root         (0) root         (0)     6930 2023-08-07 08:50:16.000000 gwdg_idm_api-2.3.0/src/gwdg_idm_api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6878 2023-08-07 08:50:16.000000 gwdg_idm_api-2.3.0/src/gwdg_idm_api/string_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-08-07 08:50:16.000000 gwdg_idm_api-2.3.0/src/gwdg_idm_api/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:50:34.280228 gwdg_idm_api-2.3.0/src/gwdg_idm_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      685 2023-08-07 08:50:34.000000 gwdg_idm_api-2.3.0/src/gwdg_idm_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      566 2023-08-07 08:50:34.000000 gwdg_idm_api-2.3.0/src/gwdg_idm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:50:34.000000 gwdg_idm_api-2.3.0/src/gwdg_idm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:50:34.000000 gwdg_idm_api-2.3.0/src/gwdg_idm_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-08-07 08:50:34.000000 gwdg_idm_api-2.3.0/src/gwdg_idm_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 08:50:34.000000 gwdg_idm_api-2.3.0/src/gwdg_idm_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:50:34.280228 gwdg_idm_api-2.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3617 2023-08-07 08:50:16.000000 gwdg_idm_api-2.3.0/tests/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-08-07 08:50:16.000000 gwdg_idm_api-2.3.0/tests/predict_username.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-08-07 08:50:16.000000 gwdg_idm_api-2.3.0/tox.ini
```

### Comparing `gwdg_idm_api-2.2.2/.pre-commit-config.yaml` & `gwdg_idm_api-2.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.2/LICENSE` & `gwdg_idm_api-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.2/PKG-INFO` & `gwdg_idm_api-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdg_idm_api
-Version: 2.2.2
+Version: 2.3.0
 Summary: Interface to the GWDG IDM api
 Home-page: https://gitlab.gwdg.de/mpi-dortmund/ze-edv-public/gwdg_idm_api
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gwdg_idm_api-2.2.2/setup.cfg` & `gwdg_idm_api-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.2/src/gwdg_idm_api/benutzerverwaltung.py` & `gwdg_idm_api-2.3.0/src/gwdg_idm_api/benutzerverwaltung.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,21 +129,25 @@
         else:
             change_data = {
                 "goesternExpirationDate": expire_date.strftime("%d.%m.%Y"),
             }
 
         return self.update_user(user, change_data)  # type: ignore
 
-    def reactivate_user(self, user: ChangeTemplate):
+    def reactivate_user(self, user: ChangeTemplate, create_mailbox: bool = True):
         current_user_status = self.get_single_user(user.id)
 
         if current_user_status.goesternUserStatus == "255":
             raise AlreadyDeletedError
         elif current_user_status.goesternUserStatus != "2":
             return user
 
         if current_user_status.goesternExpirationDate:
             change_data = {"goesternExpirationDate": ""}
             user = self.update_user(user, change_data)  # type: ignore
 
-        change_data = {"goesternUserStatus": "0"}
+        change_data = {
+            "goesternUserStatus": "0",
+        }
+        if create_mailbox:
+            change_data["externalTaskCommand"] = "CreateMailbox"
         return self.update_user(user, change_data)  # type: ignore
```

### Comparing `gwdg_idm_api-2.2.2/src/gwdg_idm_api/models.py` & `gwdg_idm_api-2.3.0/src/gwdg_idm_api/models.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.2/src/gwdg_idm_api/string_cleaner.py` & `gwdg_idm_api-2.3.0/src/gwdg_idm_api/string_cleaner.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.2/src/gwdg_idm_api/util.py` & `gwdg_idm_api-2.3.0/src/gwdg_idm_api/util.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/PKG-INFO` & `gwdg_idm_api-2.3.0/src/gwdg_idm_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdg-idm-api
-Version: 2.2.2
+Version: 2.3.0
 Summary: Interface to the GWDG IDM api
 Home-page: https://gitlab.gwdg.de/mpi-dortmund/ze-edv-public/gwdg_idm_api
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gwdg_idm_api-2.2.2/src/gwdg_idm_api.egg-info/SOURCES.txt` & `gwdg_idm_api-2.3.0/src/gwdg_idm_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.2/tests/examples.py` & `gwdg_idm_api-2.3.0/tests/examples.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.2/tests/predict_username.py` & `gwdg_idm_api-2.3.0/tests/predict_username.py`

 * *Files identical despite different names*

