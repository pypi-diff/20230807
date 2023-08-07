# Comparing `tmp/dapla_toolbelt-1.8.0.tar.gz` & `tmp/dapla_toolbelt-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt-1.8.0.tar", max compression
+gzip compressed data, was "dapla_toolbelt-1.8.1.tar", max compression
```

## Comparing `dapla_toolbelt-1.8.0.tar` & `dapla_toolbelt-1.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1074 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/LICENSE
--rw-r--r--   0        0        0     6602 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/README.md
--rw-r--r--   0        0        0      432 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/__init__.py
--rw-r--r--   0        0        0     2906 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/auth.py
--rw-r--r--   0        0        0     1576 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/backports.py
--rw-r--r--   0        0        0     1537 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/collector.py
--rw-r--r--   0        0        0     4120 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/converter.py
--rw-r--r--   0        0        0     4185 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/doctor.py
--rw-r--r--   0        0        0     5550 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/files.py
--rw-r--r--   0        0        0     1861 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/gcs.py
--rw-r--r--   0        0        0     1060 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/git.py
--rw-r--r--   0        0        0     2887 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/guardian.py
--rw-r--r--   0        0        0     1140 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/jupyterhub.py
--rw-r--r--   0        0        0     4322 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/pandas.py
--rw-r--r--   0        0        0     6031 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/pubsub.py
--rw-r--r--   0        0        0        0 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/spark/__init__.py
--rw-r--r--   0        0        0      378 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/spark/sparkui.py
--rw-r--r--   0        0        0     3139 2023-07-03 08:37:46.564566 dapla_toolbelt-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     7730 1970-01-01 00:00:00.000000 dapla_toolbelt-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/LICENSE
+-rw-r--r--   0        0        0     6602 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/README.md
+-rw-r--r--   0        0        0      432 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/__init__.py
+-rw-r--r--   0        0        0     3849 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/auth.py
+-rw-r--r--   0        0        0     1576 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/backports.py
+-rw-r--r--   0        0        0     1537 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/collector.py
+-rw-r--r--   0        0        0     4120 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/converter.py
+-rw-r--r--   0        0        0     4185 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/doctor.py
+-rw-r--r--   0        0        0     5550 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/files.py
+-rw-r--r--   0        0        0     1861 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/gcs.py
+-rw-r--r--   0        0        0     1060 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/git.py
+-rw-r--r--   0        0        0     2887 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/guardian.py
+-rw-r--r--   0        0        0     1140 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/jupyterhub.py
+-rw-r--r--   0        0        0     4322 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/pandas.py
+-rw-r--r--   0        0        0     6031 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/pubsub.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/spark/__init__.py
+-rw-r--r--   0        0        0      378 2023-08-07 11:41:53.514575 dapla_toolbelt-1.8.1/dapla/spark/sparkui.py
+-rw-r--r--   0        0        0     3139 2023-08-07 11:41:53.518575 dapla_toolbelt-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     7730 1970-01-01 00:00:00.000000 dapla_toolbelt-1.8.1/PKG-INFO
```

### Comparing `dapla_toolbelt-1.8.0/LICENSE` & `dapla_toolbelt-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.8.0/README.md` & `dapla_toolbelt-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.8.0/dapla/auth.py` & `dapla_toolbelt-1.8.1/dapla/auth.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,24 +11,42 @@
 class AuthClient:
     """
     A client class that connects to the AuthHandler to retrieve user and auth state info
     """
 
     @staticmethod
     def fetch_local_user():
-        # Helps getting the correct ssl configs
-        hub = HubAuth()
-        response = requests.get(os.environ['LOCAL_USER_PATH'],
-                                headers={
-                                    'Authorization': 'token %s' % hub.api_token
-                                }, cert=(hub.certfile, hub.keyfile), verify=hub.client_ca, allow_redirects=False)
-        if response.status_code == 200:
-            return response.json()
+        if AuthClient.is_oidc_token():
+            response = requests.get(os.environ['OIDC_TOKEN_EXCHANGE_URL'],
+                                    headers={
+                                        'Authorization': 'Bearer %s' % os.environ['OIDC_TOKEN']
+                                    })
+            if response.status_code == 200:
+                return {
+                    'access_token': os.environ['OIDC_TOKEN'],
+                    'exchanged_tokens': {
+                        'google': {
+                            'access_token': response.json()['access_token'],
+                            'exp': response.json()['accessTokenExpiration']
+                        }
+                    }
+                }
+            else:
+                raise AuthError
         else:
-            raise AuthError
+            # Helps getting the correct ssl configs
+            hub = HubAuth()
+            response = requests.get(os.environ['LOCAL_USER_PATH'],
+                                    headers={
+                                        'Authorization': 'token %s' % hub.api_token
+                                    }, cert=(hub.certfile, hub.keyfile), verify=hub.client_ca, allow_redirects=False)
+            if response.status_code == 200:
+                return response.json()
+            else:
+                raise AuthError
 
     @staticmethod
     def fetch_personal_token():
         try:
             return AuthClient.fetch_local_user()['access_token']
         except AuthError as err:
             err.print_warning()
@@ -66,15 +84,19 @@
         else:
             # Fetch credentials from Google Cloud SDK
             credentials, _ = google.auth.default()
             return credentials
 
     @staticmethod
     def is_ready():
-        return 'LOCAL_USER_PATH' in os.environ
+        return 'LOCAL_USER_PATH' in os.environ or 'OIDC_TOKEN' in os.environ
+
+    @staticmethod
+    def is_oidc_token():
+        return 'OIDC_TOKEN' in os.environ
 
 
 class AuthError(Exception):
     """This exception class is used when the communication with the custom auth handler fails.
     This is normally due to stale auth session."""
 
     def print_warning(self):
```

### Comparing `dapla_toolbelt-1.8.0/dapla/backports.py` & `dapla_toolbelt-1.8.1/dapla/backports.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.8.0/dapla/collector.py` & `dapla_toolbelt-1.8.1/dapla/collector.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.8.0/dapla/converter.py` & `dapla_toolbelt-1.8.1/dapla/converter.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.8.0/dapla/doctor.py` & `dapla_toolbelt-1.8.1/dapla/doctor.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.8.0/dapla/files.py` & `dapla_toolbelt-1.8.1/dapla/files.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.8.0/dapla/gcs.py` & `dapla_toolbelt-1.8.1/dapla/gcs.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.8.0/dapla/git.py` & `dapla_toolbelt-1.8.1/dapla/git.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.8.0/dapla/guardian.py` & `dapla_toolbelt-1.8.1/dapla/guardian.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.8.0/dapla/jupyterhub.py` & `dapla_toolbelt-1.8.1/dapla/jupyterhub.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.8.0/dapla/pandas.py` & `dapla_toolbelt-1.8.1/dapla/pandas.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.8.0/dapla/pubsub.py` & `dapla_toolbelt-1.8.1/dapla/pubsub.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.8.0/pyproject.toml` & `dapla_toolbelt-1.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt"
-version = "1.8.0"
+version = "1.8.1"
 description = "Python module for use within Jupyterlab notebooks, specifically aimed for Statistics Norway's data platform called Dapla"
 authors = ["Statistics Norway <stat-dev@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt"
 
 classifiers = [
```

### Comparing `dapla_toolbelt-1.8.0/PKG-INFO` & `dapla_toolbelt-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python module for use within Jupyterlab notebooks, specifically aimed for Statistics Norway's data platform called Dapla
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt
 License: MIT
 Author: Statistics Norway
 Author-email: stat-dev@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

