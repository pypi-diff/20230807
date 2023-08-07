# Comparing `tmp/successfactors_auth-0.0.8.tar.gz` & `tmp/successfactors_auth-0.0.9.tar.gz`

## Comparing `successfactors_auth-0.0.8.tar` & `successfactors_auth-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 successfactors_auth-0.0.8/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 successfactors_auth-0.0.8/src/successfactors_auth/__init__.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 successfactors_auth-0.0.8/src/successfactors_auth/auth.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 successfactors_auth-0.0.8/src/successfactors_auth/templates/sf_saml_template.xml
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 successfactors_auth-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 successfactors_auth-0.0.8/LICENSE
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 successfactors_auth-0.0.8/README.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 successfactors_auth-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 successfactors_auth-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 successfactors_auth-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 successfactors_auth-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 successfactors_auth-0.0.9/src/successfactors_auth/__init__.py
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 successfactors_auth-0.0.9/src/successfactors_auth/auth.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 successfactors_auth-0.0.9/src/successfactors_auth/templates/sf_saml_template.xml
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 successfactors_auth-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 successfactors_auth-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 successfactors_auth-0.0.9/README.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 successfactors_auth-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 successfactors_auth-0.0.9/PKG-INFO
```

### Comparing `successfactors_auth-0.0.8/src/successfactors_auth/auth.py` & `successfactors_auth-0.0.9/src/successfactors_auth/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 import requests
 import xmlsec
 from lxml import etree
 
 from . import templates
 
 
-def get_access_token(sf_url: str, company_id: str, client_id: str,
-                     assertion: str) -> str:
+def request_token(sf_url: str, company_id: str, client_id: str,
+                  assertion: str) -> str:
     """
     Send POST request to SuccessFactors containing the generated
     SAML assertion and other details, then receive a token in response
     """
     # Request body
     token_request = dict(
         client_id=client_id,
@@ -109,16 +109,16 @@
     sign_context.key = key
     sign_context.sign(signature_node)
 
     # Return signed XML string
     return etree.tostring(root)
 
 
-def auth(sf_url: str, sf_company_id: str, sf_oauth_client_id: str,
-         sf_admin_user: str, sf_saml_private_key: str) -> str:
+def get_token(sf_url: str, sf_company_id: str, sf_oauth_client_id: str,
+              sf_admin_user: str, sf_saml_private_key: str) -> str:
     """
     Request an API access token by generating a signed SAML assertion
     and using it to authenticate with SuccessFactors.
     """
 
     template_file = impresources.files(templates) / 'sf_saml_template.xml'
 
@@ -131,13 +131,13 @@
     # Sign the SAML assertion with the private key file
     signed_assertion = sign_assertion(unsigned_assertion, sf_saml_private_key)
 
     # Convert the signed XML string to base64
     signed_assertion_b64 = base64.b64encode(signed_assertion).replace(b'\n', b'')
 
     # Request the API token from SuccessFactors via a POST request
-    access_token = get_access_token(sf_url,
-                                    sf_company_id,
-                                    sf_oauth_client_id,
-                                    signed_assertion_b64)
+    access_token = request_token(sf_url,
+                                 sf_company_id,
+                                 sf_oauth_client_id,
+                                 signed_assertion_b64)
 
     return access_token
```

### Comparing `successfactors_auth-0.0.8/src/successfactors_auth/templates/sf_saml_template.xml` & `successfactors_auth-0.0.9/src/successfactors_auth/templates/sf_saml_template.xml`

 * *Files identical despite different names*

### Comparing `successfactors_auth-0.0.8/.gitignore` & `successfactors_auth-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `successfactors_auth-0.0.8/LICENSE` & `successfactors_auth-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `successfactors_auth-0.0.8/README.md` & `successfactors_auth-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,30 +19,29 @@
 
 ### Example
 
 ``` python
 #!/usr/bin/env python
 
 import requests
-from successfactors_auth import auth as sf_auth
+import successfactors_auth as sf
 
 sf_url = 'https://your.base.url.com'
 sf_company_id = 'your-company-id'
 sf_oauth_client_id = 'your_app_client_id'
 sf_admin_user = 'your_admin_user'
-sf_saml_private_key = 'your_app_private_key.pem'
+sf_saml_private_key = 'app_private_key_file.pem'
 
-token = sf_auth.auth(
-    sf_url,
-    sf_company_id,
-    sf_oauth_client_id,
-    sf_admin_user,
-    sf_saml_private_key,
-    sf_saml_template
-    )
+token = sf.get_token(
+    sf_company_id=company_id,
+    sf_oauth_client_id=oauth_client_id,
+    sf_admin_user=admin_api_user,
+    sf_saml_private_key=oauth_private_key,
+    sf_url=url
+)
 
 headers = {
     "Accept: application/json",
     f"Authorization: {token}"
 }
 
 request = requests.get(f"{sf_url}/User", headers=headers)
```

### Comparing `successfactors_auth-0.0.8/pyproject.toml` & `successfactors_auth-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "successfactors-auth"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Ray Lyon", email="ray@raylyon.net" },
 ]
 description = "Authenticate to the SuccessFactors API."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `successfactors_auth-0.0.8/PKG-INFO` & `successfactors_auth-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: successfactors-auth
-Version: 0.0.8
+Version: 0.0.9
 Summary: Authenticate to the SuccessFactors API.
 Project-URL: Homepage, https://github.com/skoobasteeve/successfactors_auth
 Project-URL: Bug Tracker, https://github.com/skoobasteeve/successfactors_auth/issues
 Author-email: Ray Lyon <ray@raylyon.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -36,30 +36,29 @@
 
 ### Example
 
 ``` python
 #!/usr/bin/env python
 
 import requests
-from successfactors_auth import auth as sf_auth
+import successfactors_auth as sf
 
 sf_url = 'https://your.base.url.com'
 sf_company_id = 'your-company-id'
 sf_oauth_client_id = 'your_app_client_id'
 sf_admin_user = 'your_admin_user'
-sf_saml_private_key = 'your_app_private_key.pem'
+sf_saml_private_key = 'app_private_key_file.pem'
 
-token = sf_auth.auth(
-    sf_url,
-    sf_company_id,
-    sf_oauth_client_id,
-    sf_admin_user,
-    sf_saml_private_key,
-    sf_saml_template
-    )
+token = sf.get_token(
+    sf_company_id=company_id,
+    sf_oauth_client_id=oauth_client_id,
+    sf_admin_user=admin_api_user,
+    sf_saml_private_key=oauth_private_key,
+    sf_url=url
+)
 
 headers = {
     "Accept: application/json",
     f"Authorization: {token}"
 }
 
 request = requests.get(f"{sf_url}/User", headers=headers)
```

