# Comparing `tmp/sotrans_fastapi_keycloak-0.0.8.tar.gz` & `tmp/sotrans_fastapi_keycloak-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotrans_fastapi_keycloak-0.0.8.tar", last modified: Thu Aug  3 14:36:56 2023, max compression
+gzip compressed data, was "sotrans_fastapi_keycloak-0.0.9.tar", last modified: Thu Aug  3 15:13:12 2023, max compression
```

## Comparing `sotrans_fastapi_keycloak-0.0.8.tar` & `sotrans_fastapi_keycloak-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 14:36:56.189527 sotrans_fastapi_keycloak-0.0.8/
--rw-rw-rw-   0        0        0    11564 2023-07-28 12:35:22.000000 sotrans_fastapi_keycloak-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1122 2023-08-03 14:36:56.189527 sotrans_fastapi_keycloak-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.8/README.md
--rw-rw-rw-   0        0        0     1314 2023-08-03 14:36:55.000000 sotrans_fastapi_keycloak-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-03 14:36:56.189527 sotrans_fastapi_keycloak-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      218 2023-07-28 13:49:01.000000 sotrans_fastapi_keycloak-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 14:36:56.157517 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/
--rw-rw-rw-   0        0        0      949 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/__init__.py
--rw-rw-rw-   0        0        0    48510 2023-08-03 13:25:22.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/api.py
--rw-rw-rw-   0        0        0     2732 2023-07-25 23:29:41.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/exceptions.py
--rw-rw-rw-   0        0        0     9124 2023-07-28 13:53:54.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/model.py
--rw-rw-rw-   0        0        0     1041 2023-08-03 14:04:55.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/role.py
--rw-rw-rw-   0        0        0     2096 2023-08-01 12:28:40.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/sotrans_model.py
--rw-rw-rw-   0        0        0      925 2023-08-03 14:04:55.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/sotrans_role.py
-drwxrwxrwx   0        0        0        0 2023-08-03 14:36:56.187397 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-08-03 14:36:56.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2023-08-03 14:36:56.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 14:36:56.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2023-08-03 14:36:56.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-08-03 14:36:56.000000 sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 15:13:12.444018 sotrans_fastapi_keycloak-0.0.9/
+-rw-rw-rw-   0        0        0    11564 2023-07-28 12:35:22.000000 sotrans_fastapi_keycloak-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1122 2023-08-03 15:13:12.443023 sotrans_fastapi_keycloak-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1314 2023-08-03 15:12:02.000000 sotrans_fastapi_keycloak-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 15:13:12.444018 sotrans_fastapi_keycloak-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      218 2023-07-28 13:49:01.000000 sotrans_fastapi_keycloak-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:13:12.425638 sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/
+-rw-rw-rw-   0        0        0      949 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/__init__.py
+-rw-rw-rw-   0        0        0    48570 2023-08-03 15:12:02.000000 sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/api.py
+-rw-rw-rw-   0        0        0     2732 2023-07-25 23:29:41.000000 sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/exceptions.py
+-rw-rw-rw-   0        0        0     9124 2023-07-28 13:53:54.000000 sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/model.py
+-rw-rw-rw-   0        0        0     1041 2023-08-03 14:04:55.000000 sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/role.py
+-rw-rw-rw-   0        0        0     2143 2023-08-03 14:55:54.000000 sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/sotrans_model.py
+-rw-rw-rw-   0        0        0      925 2023-08-03 14:04:55.000000 sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/sotrans_role.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:13:12.442022 sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-08-03 15:13:12.000000 sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2023-08-03 15:13:12.000000 sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 15:13:12.000000 sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2023-08-03 15:13:12.000000 sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-08-03 15:13:12.000000 sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak.egg-info/top_level.txt
```

### Comparing `sotrans_fastapi_keycloak-0.0.8/LICENSE` & `sotrans_fastapi_keycloak-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.8/PKG-INFO` & `sotrans_fastapi_keycloak-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotrans_fastapi_keycloak
-Version: 0.0.8
+Version: 0.0.9
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
```

### Comparing `sotrans_fastapi_keycloak-0.0.8/pyproject.toml` & `sotrans_fastapi_keycloak-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
     "pydantic_core==2.4.0",
     "requests==2.31.0",
     "sniffio==1.3.0",
     "starlette==0.27.0",
     "typing_extensions==4.7.1",
     "urllib3==2.0.4"
 ]
-version = "0.0.8"
+version = "0.0.9"
```

### Comparing `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/__init__.py` & `sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/api.py` & `sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,16 +297,19 @@
                 JWTError: If decoding fails or the signature is invalid
                 JWTClaimsError: If any claim is invalid
                 HTTPException: If any role required is not contained within the roles of the users
             """
             decoded_token = self._decode_token(token = token, audience = "account")
             user = self._oidc_user_type.model_validate(decoded_token)
 
-            if required_role_names:
-                self._assert_roles(user.roles, required_role_names)
+            if required_role_names and not self.check_roles(user.roles, required_role_names):
+                raise HTTPException(
+                    status_code = status.HTTP_403_FORBIDDEN,
+                    detail = f'Roles {required_role_names} is required to perform this action',
+                )
 
             if extra_fields:
                 for field in extra_fields:
                     user.extra_fields[field] = decoded_token.get(field, None)
 
             return user
 
@@ -550,28 +553,26 @@
             KeycloakError: If the resulting response is not a successful HTTP-Code (>299)
         """
         return self._admin_request(
             url = f"{self.roles_uri}/{role_name}",
             method = HTTPMethod.DELETE,
         )
 
-    def _assert_roles(self, available_role_names: list[str], required_role_names: list[str]):
+    def check_roles(self, available_role_names: list[str], required_role_names: list[str]) -> bool:
         # O(n)
         required_roles = [self.roles.get(role_name, Role()) for role_name in required_role_names]
         # O(m)
         user_roles = [self.roles.get(role_name, Role()) for role_name in available_role_names]
 
         # O(n * m * k), can be slightly optimized using checking firstly LCA of all roles.
         # but, considering the fact that n, m ~ 1-2 and roles tree is very simple, not needed
         for role in required_roles:
             if not any([user_role.check(role) for user_role in user_roles]):
-                raise HTTPException(
-                    status_code = status.HTTP_403_FORBIDDEN,
-                    detail = f'Role "{role}" is required to perform this action',
-                )
+                return False
+        return True
 
     @result_or_error(response_model = KeycloakGroupModel, is_list = True)
     def get_all_groups(self, skip: int = 0, limit: int = 20) -> list[KeycloakGroupModel]:
         """Get all base groups of the Keycloak realm
 
         Args:
             skip: paging offset
```

### Comparing `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/exceptions.py` & `sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/exceptions.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/model.py` & `sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/model.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/role.py` & `sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/role.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/sotrans_model.py` & `sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/sotrans_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 class SotransKeycloakUserCreateModel(SotransKeycloakUserBaseModel):
     """Represents a creation Keycloak user object in SOTRANS configuration"""
     name: KeycloakUserStrAttribute
     surname: KeycloakUserStrAttribute
     patronymic: KeycloakUserStrAttribute
     phone: KeycloakUserStrAttribute
+    organisation_id: KeycloakUserStrAttribute
     email: str
     password: str
 
 
 class SotransKeycloakUserModel(KeycloakUserBaseModel, SotransKeycloakUserInfoModel):
     """Represents a full Keycloak user object in SOTRANS configuration"""
     pass
```

### Comparing `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak/sotrans_role.py` & `sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak/sotrans_role.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/PKG-INFO` & `sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotrans-fastapi-keycloak
-Version: 0.0.8
+Version: 0.0.9
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
```

### Comparing `sotrans_fastapi_keycloak-0.0.8/sotrans_fastapi_keycloak.egg-info/SOURCES.txt` & `sotrans_fastapi_keycloak-0.0.9/sotrans_fastapi_keycloak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

