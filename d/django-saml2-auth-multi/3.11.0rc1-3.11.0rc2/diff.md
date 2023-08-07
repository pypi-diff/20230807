# Comparing `tmp/django_saml2_auth_multi-3.11.0rc1.tar.gz` & `tmp/django_saml2_auth_multi-3.11.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_saml2_auth_multi-3.11.0rc1.tar", max compression
+gzip compressed data, was "django_saml2_auth_multi-3.11.0rc2.tar", max compression
```

## Comparing `django_saml2_auth_multi-3.11.0rc1.tar` & `django_saml2_auth_multi-3.11.0rc2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      552 2023-08-02 12:45:30.206550 django_saml2_auth_multi-3.11.0rc1/LICENSE
--rw-r--r--   0        0        0    47165 2023-08-04 15:21:40.806420 django_saml2_auth_multi-3.11.0rc1/README.md
--rw-r--r--   0        0        0       88 2023-08-04 15:21:40.806420 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/__init__.py
--rw-r--r--   0        0        0     1663 2023-08-07 11:30:44.899915 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/config.py
--rw-r--r--   0        0        0      940 2023-08-04 15:21:40.806420 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/errors.py
--rw-r--r--   0        0        0      585 2023-08-04 15:21:40.806420 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/exceptions.py
--rw-r--r--   0        0        0    17026 2023-08-04 15:23:11.083086 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/saml.py
--rw-r--r--   0        0        0      327 2023-08-04 15:21:40.806420 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/templates/django_saml2_auth_multi/denied.html
--rw-r--r--   0        0        0      493 2023-08-04 15:21:40.806420 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/templates/django_saml2_auth_multi/error.html
--rw-r--r--   0        0        0      308 2023-08-04 15:21:40.806420 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/templates/django_saml2_auth_multi/signout.html
--rw-r--r--   0        0        0       43 2023-08-04 15:21:40.806420 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/tests/__init__.py
--rw-r--r--   0        0        0      416 2023-08-04 16:50:04.809711 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/tests/conftest.py
--rw-r--r--   0        0        0     1567 2023-08-04 15:21:40.809754 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/tests/metadata.xml
--rw-r--r--   0        0        0     3528 2023-08-04 15:21:40.809754 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/tests/settings.py
--rw-r--r--   0        0        0    19588 2023-08-04 16:30:24.306387 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/tests/test_saml.py
--rw-r--r--   0        0        0    23288 2023-08-04 16:25:41.756389 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/tests/test_user.py
--rw-r--r--   0        0        0     4822 2023-08-04 15:21:40.809754 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/tests/test_utils.py
--rw-r--r--   0        0        0      243 2023-08-04 16:27:28.683055 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/tests/utils.py
--rw-r--r--   0        0        0      357 2023-08-04 15:21:40.809754 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/urls.py
--rw-r--r--   0        0        0    16806 2023-08-04 16:30:24.276387 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/user.py
--rw-r--r--   0        0        0     7792 2023-08-04 15:21:40.813087 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/utils.py
--rw-r--r--   0        0        0    11776 2023-08-04 15:47:45.926408 django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/views.py
--rw-r--r--   0        0        0     1484 2023-08-07 11:47:03.996573 django_saml2_auth_multi-3.11.0rc1/pyproject.toml
--rw-r--r--   0        0        0    48649 1970-01-01 00:00:00.000000 django_saml2_auth_multi-3.11.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      552 2023-08-02 12:45:30.206550 django_saml2_auth_multi-3.11.0rc2/LICENSE
+-rw-r--r--   0        0        0    43886 2023-08-07 14:00:38.376509 django_saml2_auth_multi-3.11.0rc2/README.md
+-rw-r--r--   0        0        0       88 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/__init__.py
+-rw-r--r--   0        0        0     1690 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/config.py
+-rw-r--r--   0        0        0      940 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/errors.py
+-rw-r--r--   0        0        0      585 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/exceptions.py
+-rw-r--r--   0        0        0    17151 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/saml.py
+-rw-r--r--   0        0        0      327 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/templates/django_saml2_auth_multi/denied.html
+-rw-r--r--   0        0        0      493 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/templates/django_saml2_auth_multi/error.html
+-rw-r--r--   0        0        0      308 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/templates/django_saml2_auth_multi/signout.html
+-rw-r--r--   0        0        0       43 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/tests/__init__.py
+-rw-r--r--   0        0        0      416 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/tests/conftest.py
+-rw-r--r--   0        0        0     1567 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/tests/metadata.xml
+-rw-r--r--   0        0        0     3528 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/tests/settings.py
+-rw-r--r--   0        0        0    19588 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/tests/test_saml.py
+-rw-r--r--   0        0        0    23304 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/tests/test_user.py
+-rw-r--r--   0        0        0     4953 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/tests/test_utils.py
+-rw-r--r--   0        0        0      244 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/tests/utils.py
+-rw-r--r--   0        0        0      357 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/urls.py
+-rw-r--r--   0        0        0    16854 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/user.py
+-rw-r--r--   0        0        0     7792 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/utils.py
+-rw-r--r--   0        0        0    11843 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/views.py
+-rw-r--r--   0        0        0     1505 2023-08-07 14:02:13.386508 django_saml2_auth_multi-3.11.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    45391 1970-01-01 00:00:00.000000 django_saml2_auth_multi-3.11.0rc2/PKG-INFO
```

### Comparing `django_saml2_auth_multi-3.11.0rc1/LICENSE` & `django_saml2_auth_multi-3.11.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc1/README.md` & `django_saml2_auth_multi-3.11.0rc2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,29 @@
-# Django SAML2 Authentication
+# Django SAML2 Authentication Multi
 
-[![PyPI](https://img.shields.io/pypi/v/grafana-django-saml2-auth?label=version&logo=pypi)](https://pypi.org/project/grafana-django-saml2-auth/) [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/grafana/django-saml2-auth/deploy.yml?branch=main&logo=github)](https://github.com/grafana/django-saml2-auth/actions) [![Coveralls](https://img.shields.io/coveralls/github/grafana/django-saml2-auth?logo=coveralls)](https://coveralls.io/github/grafana/django-saml2-auth) [![Downloads](https://pepy.tech/badge/grafana-django-saml2-auth)](https://pepy.tech/project/grafana-django-saml2-auth)
+[![PyPI](https://img.shields.io/pypi/v/django-saml2-auth-multi?label=version&logo=pypi)](https://pypi.org/project/django-saml2-auth-multi/)
 
 This plugin provides a simple way to integrate SAML2 Authentication into your Django-powered app. SAML SSO is a standard, so practically any SAML2 based SSO identity provider is supported.
 
+This project is a fork of [django-saml2-auth](https://github.com/grafana/django-saml2-auth) and adds support for configuring multiple IDPs with separate configuration parameters. It should be compatible with existing deployments and configurations; nevertheless, unless you need additional features in this package (also which may not compatible with your use case), it is highly suggested to use base package.
+
 This plugin supports both identity provider and service provider-initiated SSO:
 
 - For IdP-initiated SSO, the user should sign in to their identity provider platform, e.g., Okta, and click on the application that authorizes and redirects the user to the service provider, that is your platform.
 - For SP-initiated SSO, the user should first exist on your platform, either by signing in via the first method (IdP-initiated SSO) or any other custom solution. It can be configured to be redirected to the correct application on the identity provider platform.
 
 For IdP-initiated SSO, the user will be created if it doesn't exist. Still, for SP-initiated SSO, the user should exist in your platform for the code to detect and redirect them to the correct application on the identity provider platform.
 
-## Project Information
-
-- Original Author: Fang Li ([@fangli](https://github.com/fangli))
-- Maintainer: Mostafa Moradian ([@mostafa](https://github.com/mostafa))
-- Version support matrix:
-    | **Python**                   | **Django** | **django-saml2-auth** | **End of Support<br/>(django-saml2-auth)** | **End of extended support<br/>(Django)** |
-    | ---------------------------- | ---------- | --------------------- | ------------------------------------------ | ---------------------------------------- |
-    | 3.7.x, 3.8.x, 3.9.x, 3.10.x  | 2.2.x      | >=3.4.0               | 3.10.0                                     | April 11, 2022                           |
-    | 3.7.x, 3.8.x, 3.9.x, 3.10.x  | 3.2.x      | >=3.4.0               |                                            | April 2024                               |
-    | 3.8.x, 3.9.x, 3.10.x         | 4.0.x      | >=3.4.0               | 3.10.0                                     | April 1, 2023                            |
-    | 3.8.x, 3.9.x, 3.10.x         | 4.1.x      | >=3.4.0               |                                            | December 2023                            |
-    | 3.8.x, 3.9.x, 3.10.x, 3.11.x | 4.2.x      | >=3.4.0               |                                            | April 2026                               |
-
-- Release logs are available [here](https://github.com/grafana/django-saml2-auth/releases).
-
-- For contribution, read [contributing guide](CONTRIBUTING.md).
-
-## CycloneDX SBOM
-
-From [v3.6.1](https://github.com/grafana/django-saml2-auth/releases/tag/v3.6.1), CycloneDX SBOMs will be generated for [requirements.txt](./requirements.txt) and [requirements_test.txt](./requirements_test.txt) and it can be accessed from the latest build of GitHub Actions for a tagged release, for example, [this one](https://github.com/grafana/django-saml2-auth/actions/runs/2245422253). The artifacts are only kept for 90 days.
-
-## Donate
-
-Please give us a shiny ![star](https://img.shields.io/github/stars/grafana/django-saml2-auth.svg?style=social&label=Star&maxAge=86400) and help spread the word.
 
 ## Installation
 
 You can install this plugin via `pip`. Make sure you update `pip` to be able to install from git:
 
 ```bash
-pip install grafana-django-saml2-auth
-```
-
-or from source:
-
-```bash
-git clone https://github.com/grafana/django-saml2-auth
-cd django-saml2-auth
-python setup.py install
+pip install django-saml2-auth-multi
 ```
 
 `xmlsec` is also required by `pysaml2`, so it must be installed:
 
 ``` bash
 // RPM-based distributions
 # yum install xmlsec1
@@ -79,132 +49,112 @@
     # These are the SAML2 related URLs. You can change "^saml2_auth/" regex to
     # any path you want, like "^sso/", "^sso_auth/", "^sso_login/", etc. (required)
     url(r'^sso/', include('django_saml2_auth_multi.urls')),
 
     # The following line will replace the default user login with SAML2 (optional)
     # If you want to specific the after-login-redirect-URL, use parameter "?next=/the/path/you/want"
     # with this view.
-    url(r'^accounts/login/$', django_saml2_auth.views.signin),
+    url(r'^accounts/login/$', django_saml2_auth_multi.views.signin),
 
     # The following line will replace the admin login with SAML2 (optional)
     # If you want to specific the after-login-redirect-URL, use parameter "?next=/the/path/you/want"
     # with this view.
-    url(r'^admin/login/$', django_saml2_auth.views.signin),
+    url(r'^admin/login/$', django_saml2_auth_multi.views.signin),
     ```
 
-3. Add `'django_saml2_auth'` to `INSTALLED_APPS` in your django `settings.py`:
+3. Add `'django_saml2_auth_multi'` to `INSTALLED_APPS` in your django `settings.py`:
 
     ```python
     INSTALLED_APPS = [
         '...',
         'django_saml2_auth_multi',
     ]
     ```
 
 4. In `settings.py`, add the SAML2 related configuration:
 
+    `SAML2_AUTH` configuration variable can be a dictionary (for configuring single IDP) or a list (for configuring list of IDPs).
+
     Please note, the only required setting is **METADATA\_AUTO\_CONF\_URL** or the existence of a **GET\_METADATA\_AUTO\_CONF\_URLS** trigger function. The following block shows all required and optional configuration settings and their default values.
 
     ```python
-    SAML2_AUTH = {
-        # Metadata is required, choose either remote url or local file path
-        'METADATA_AUTO_CONF_URL': '[The auto(dynamic) metadata configuration URL of SAML2]',
-        'METADATA_LOCAL_FILE_PATH': '[The metadata configuration file path]',
-        'KEY_FILE': '[The key file path]',
-        'CERT_FILE': '[The certificate file path]',
-
-        'DEBUG': False,  # Send debug information to a log file
-        # Optional logging configuration.
-        # By default, it won't log anything.
-        # The following configuration is an example of how to configure the logger,
-        # which can be used together with the DEBUG option above. Please note that
-        # the logger configuration follows the Python's logging configuration schema:
-        # https://docs.python.org/3/library/logging.config.html#logging-config-dictschema
-        'LOGGING': {
-            'version': 1,
-            'formatters': {
-                'simple': {
-                    'format': '[%(asctime)s] [%(levelname)s] [%(name)s.%(funcName)s] %(message)s',
-                },
+    SAML2_AUTH = [
+        {
+            # Set this to entity ID of IdP. Used when selecting redirection URL in login view and determining issuer IdP in ACS endpoint.
+            # Should be same with Issuer ID in assertions.
+            # Required when a list is provided for SAML2_AUTH (i.e. multiple IDPs are configured). 
+            'IDP_ID': '<Entity ID of IdP>',
+
+            # Metadata is required, choose either remote url or local file path
+            'METADATA_AUTO_CONF_URL': '[The auto(dynamic) metadata configuration URL of SAML2]',
+            'METADATA_LOCAL_FILE_PATH': '[The metadata configuration file path]',
+            'KEY_FILE': '[The key file path]',
+            'CERT_FILE': '[The certificate file path]',
+
+            # Optional settings below
+            'DEFAULT_NEXT_URL': '/admin',  # Custom target redirect URL after the user get logged in. Default to /admin if not set. This setting will be overwritten if you have parameter ?next= specificed in the login URL.
+            'CREATE_USER': True,  # Create a new Django user when a new user logs in. Defaults to True.
+            'NEW_USER_PROFILE': {
+                'USER_GROUPS': [],  # The default group name when a new user logs in
+                'ACTIVE_STATUS': True,  # The default active status for new users
+                'STAFF_STATUS': False,  # The staff status for new users
+                'SUPERUSER_STATUS': False,  # The superuser status for new users
             },
-            'handlers': {
-                'stdout': {
-                    'class': 'logging.StreamHandler',
-                    'stream': 'ext://sys.stdout',
-                    'level': 'DEBUG',
-                    'formatter': 'simple',
-                },
+            'ATTRIBUTES_MAP': {  # Change Email/UserName/FirstName/LastName to corresponding SAML2 userprofile attributes.
+                'email': 'user.email',
+                'username': 'user.username',
+                'first_name': 'user.first_name',
+                'last_name': 'user.last_name',
+                'token': 'Token',  # Mandatory, can be unrequired if TOKEN_REQUIRED is False
+                'groups': 'Groups',  # Optional
             },
-            'loggers': {
-                'saml2': {
-                    'level': 'DEBUG'
-                },
+            'GROUPS_MAP': {  # Optionally allow mapping SAML2 Groups to Django Groups
+                'SAML Group Name': 'Django Group Name',
             },
-            'root': {
-                'level': 'DEBUG',
-                'handlers': [
-                    'stdout',
-                ],
+            'TRIGGER': {
+                # Optional: needs to return a User Model instance or None
+                'GET_USER': 'path.to.your.get.user.hook.method',
+                'CREATE_USER': 'path.to.your.new.user.hook.method',
+                'BEFORE_LOGIN': 'path.to.your.login.hook.method',
+                'AFTER_LOGIN': 'path.to.your.after.login.hook.method',
+                # Optional. This is executed right before METADATA_AUTO_CONF_URL.
+                # For systems with many metadata files registered allows to narrow the search scope.
+                'GET_USER_ID_FROM_SAML_RESPONSE': 'path.to.your.get.user.from.saml.hook.method',
+                # This can override the METADATA_AUTO_CONF_URL to enumerate all existing metadata autoconf URLs
+                'GET_METADATA_AUTO_CONF_URLS': 'path.to.your.get.metadata.conf.hook.method',
             },
-        },
-
-        # Optional settings below
-        'DEFAULT_NEXT_URL': '/admin',  # Custom target redirect URL after the user get logged in. Default to /admin if not set. This setting will be overwritten if you have parameter ?next= specificed in the login URL.
-        'CREATE_USER': True,  # Create a new Django user when a new user logs in. Defaults to True.
-        'NEW_USER_PROFILE': {
-            'USER_GROUPS': [],  # The default group name when a new user logs in
-            'ACTIVE_STATUS': True,  # The default active status for new users
-            'STAFF_STATUS': False,  # The staff status for new users
-            'SUPERUSER_STATUS': False,  # The superuser status for new users
-        },
-        'ATTRIBUTES_MAP': {  # Change Email/UserName/FirstName/LastName to corresponding SAML2 userprofile attributes.
-            'email': 'user.email',
-            'username': 'user.username',
-            'first_name': 'user.first_name',
-            'last_name': 'user.last_name',
-            'token': 'Token',  # Mandatory, can be unrequired if TOKEN_REQUIRED is False
-            'groups': 'Groups',  # Optional
-        },
-        'GROUPS_MAP': {  # Optionally allow mapping SAML2 Groups to Django Groups
-            'SAML Group Name': 'Django Group Name',
-        },
-        'TRIGGER': {
-            # Optional: needs to return a User Model instance or None
-            'GET_USER': 'path.to.your.get.user.hook.method',
-            'CREATE_USER': 'path.to.your.new.user.hook.method',
-            'BEFORE_LOGIN': 'path.to.your.login.hook.method',
-            'AFTER_LOGIN': 'path.to.your.after.login.hook.method',
-            # Optional. This is executed right before METADATA_AUTO_CONF_URL.
-            # For systems with many metadata files registered allows to narrow the search scope.
-            'GET_USER_ID_FROM_SAML_RESPONSE': 'path.to.your.get.user.from.saml.hook.method',
-            # This can override the METADATA_AUTO_CONF_URL to enumerate all existing metadata autoconf URLs
-            'GET_METADATA_AUTO_CONF_URLS': 'path.to.your.get.metadata.conf.hook.method',
-        },
-        'ASSERTION_URL': 'https://mysite.com',  # Custom URL to validate incoming SAML requests against
-        'ENTITY_ID': 'https://mysite.com/saml2_auth/acs/',  # Populates the Issuer element in authn request
-        'NAME_ID_FORMAT': FormatString,  # Sets the Format property of authn NameIDPolicy element, e.g. 'user.email'
-        'USE_JWT': True,  # Set this to True if you are running a Single Page Application (SPA) with Django Rest Framework (DRF), and are using JWT authentication to authorize client users
-        'JWT_ALGORITHM': 'HS256',  # JWT algorithm to sign the message with
-        'JWT_SECRET': 'your.jwt.secret',  # JWT secret to sign the message with
-        'JWT_PRIVATE_KEY': '--- YOUR PRIVATE KEY ---',  # Private key to sign the message with. The algorithm should be set to RSA256 or a more secure alternative.
-        'JWT_PRIVATE_KEY_PASSPHRASE': 'your.passphrase',  # If your private key is encrypted, you might need to provide a passphrase for decryption
-        'JWT_PUBLIC_KEY': '--- YOUR PUBLIC KEY ---',  # Public key to decode the signed JWT token
-        'JWT_EXP': 60,  # JWT expiry time in seconds
-        'FRONTEND_URL': 'https://myfrontendclient.com',  # Redirect URL for the client if you are using JWT auth with DRF. See explanation below
-        'LOGIN_CASE_SENSITIVE': True,  # whether of not to get the user in case_sentive mode
-        'AUTHN_REQUESTS_SIGNED': True, # Require each authentication request to be signed
-        'LOGOUT_REQUESTS_SIGNED': True,  # Require each logout request to be signed
-        'WANT_ASSERTIONS_SIGNED': True,  # Require each assertion to be signed
-        'WANT_RESPONSE_SIGNED': True,  # Require response to be signed
-        'ACCEPTED_TIME_DIFF': None,  # Accepted time difference between your server and the Identity Provider
-        'ALLOWED_REDIRECT_HOSTS': ["https://myfrontendclient.com"], # Allowed hosts to redirect to using the ?next parameter
-        'TOKEN_REQUIRED': True,  # Whether or not to require the token parameter in the SAML assertion
-    }
+            'ASSERTION_URL': 'https://mysite.com',  # Custom URL to validate incoming SAML requests against
+            'ENTITY_ID': 'https://mysite.com/saml2_auth/acs/',  # Populates the Issuer element in authn request
+            'NAME_ID_FORMAT': FormatString,  # Sets the Format property of authn NameIDPolicy element, e.g. 'user.email'
+            'USE_JWT': True,  # Set this to True if you are running a Single Page Application (SPA) with Django Rest Framework (DRF), and are using JWT authentication to authorize client users
+            'JWT_ALGORITHM': 'HS256',  # JWT algorithm to sign the message with
+            'JWT_SECRET': 'your.jwt.secret',  # JWT secret to sign the message with
+            'JWT_PRIVATE_KEY': '--- YOUR PRIVATE KEY ---',  # Private key to sign the message with. The algorithm should be set to RSA256 or a more secure alternative.
+            'JWT_PRIVATE_KEY_PASSPHRASE': 'your.passphrase',  # If your private key is encrypted, you might need to provide a passphrase for decryption
+            'JWT_PUBLIC_KEY': '--- YOUR PUBLIC KEY ---',  # Public key to decode the signed JWT token
+            'JWT_EXP': 60,  # JWT expiry time in seconds
+            'FRONTEND_URL': 'https://myfrontendclient.com',  # Redirect URL for the client if you are using JWT auth with DRF. See explanation below
+            'LOGIN_CASE_SENSITIVE': True,  # whether of not to get the user in case_sentive mode
+            'AUTHN_REQUESTS_SIGNED': True, # Require each authentication request to be signed
+            'LOGOUT_REQUESTS_SIGNED': True,  # Require each logout request to be signed
+            'WANT_ASSERTIONS_SIGNED': True,  # Require each assertion to be signed
+            'WANT_RESPONSE_SIGNED': True,  # Require response to be signed
+            'ACCEPTED_TIME_DIFF': None,  # Accepted time difference between your server and the Identity Provider
+            'ALLOWED_REDIRECT_HOSTS': ["https://myfrontendclient.com"], # Allowed hosts to redirect to using the ?next parameter
+            'TOKEN_REQUIRED': True,  # Whether or not to require the token parameter in the SAML assertion
+        }
+    ]
     ```
 
+    `SAML2_AUTH_DEFAULTS` configuration variable can be used for specifying common settings for all IdP configurations. Same list of settings can be used for `SAML2_AUTH_DEFAULTS`.
+
+    `SAML2_AUTH_DEBUG` (default: `False`) configuration variable toggles debug flag for logging.
+
+
+
 5. In your SAML2 SSO identity provider, set the Single-sign-on URL and Audience URI (SP Entity ID) to <http://your-domain/saml2_auth/acs/>
 
 ## How to debug?
 
 To debug what's happening between the SAMLP Identity Provider and your Django application, you can use SAML-tracer for [Firefox](https://addons.mozilla.org/en-US/firefox/addon/saml-tracer/) or [Chrome](https://chrome.google.com/webstore/detail/saml-tracer/mpdajninpobndbfcldcmbpnnbhibjmch?hl=en). Using this tool, you can see the SAML requests and responses that are being sent back and forth.
 
 Also, you can enable the debug mode in the `settings.py` file by setting the `DEBUG` flag to `True` and enabling the `LOGGING` configuration. See above for configuration examples.
@@ -213,15 +163,16 @@
 
 ## Module Settings
 
 Some of the following settings are related to how this module operates. The rest are passed as options to the pysaml2 library. For more information on the pysaml2 library, see the [pysaml2 documentation](https://pysaml2.readthedocs.io/en/latest/howto/config.html), which contains examples of available settings. Also, note that all settings are not implemented in this module.
 
 | **Field name**                              | **Description**                                                                                                                                                                                                                                                                                                                                                                                                                                             | **Data type(s)** | **Default value(s)**                                                                                                                     | **Example**                                              |
 | ------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
-| **METADATA\_AUTO\_CONF\_URL**               | Auto SAML2 metadata configuration URL                                                                                                                                                                                                                                                                                                                                                                                                                       | `str`            | `None`                                                                                                                                   | `https://ORG.okta.com/app/APP-ID/sso/saml/metadata`      |
+| **IDP\_ID**               | Entity ID of IdP which is also used as Issuer information in assertions                                                                                                                                                                                                                                                                                                                                                                                                                       | `str`            | `None`                                                                                                                                   | `urn:ORG.eu.auth0.com`      |
+| **METADATA\_AUTO\_CONF\_URL**               | Auto SAML2 metadata configuration URL                                                                                                                                                                                                                                                                                                                                                                                                                       | `str`            | `None`                                                                                                                                   | `https://ORG.eu.auth0.com/samlp/metadata/`      |
 | **METADATA\_LOCAL\_FILE\_PATH**             | SAML2 metadata configuration file path                                                                                                                                                                                                                                                                                                                                                                                                                      | `str`            | `None`                                                                                                                                   | `/path/to/the/metadata.xml`                              |
 | **KEY_FILE**                                | SAML2 private key file path                                                                                                                                                                                                                                                                                                                                                                                                                                 | `str`            | `None`                                                                                                                                   | `/path/to/the/key.pem`                                   |
 | **CERT_FILE**                               | SAML2 public certificate file path                                                                                                                                                                                                                                                                                                                                                                                                                          | `str`            | `None`                                                                                                                                   | `/path/to/the/cert.pem`                                  |
 | **DEBUG**                                   | Send debug information to a log file                                                                                                                                                                                                                                                                                                                                                                                                                        | `bool`           | `False`                                                                                                                                  |                                                          |
 | **LOGGING**                                 | Logging configuration dictionary                                                                                                                                                                                                                                                                                                                                                                                                                            | `dict`           | Not set.                                                                                                                                 |                                                          |
 | **DEFAULT\_NEXT\_URL**                      | Custom target redirect URL after the user get logged in. Default to /admin if not set. This setting will be overwritten if you have parameter `?next=` specificed in the login URL.                                                                                                                                                                                                                                                                         | `str`            | `admin:index`                                                                                                                            | `https://app.example.com/account/login`                  |
 | **CREATE\_USER**                            | Determines if a new Django user should be created for new users                                                                                                                                                                                                                                                                                                                                                                                             | `bool`           | `True`                                                                                                                                   |                                                          |
@@ -338,36 +289,16 @@
 
 If a 'django\_saml2\_auth/welcome.html' template exists, that page will be shown to the user upon login instead of the user being redirected to the previous visited page. This welcome page can contain some first-visit notes and welcome words. The [Django user object](https://docs.djangoproject.com/en/1.9/ref/contrib/auth/#django.contrib.auth.models.User) is available within the template as the `user` template variable.
 
 To enable a logout page, add the following lines to `urls.py`, before any `urlpatterns`:
 
 ```python
 # The following line will replace the default user logout with the signout page (optional)
-url(r'^accounts/logout/$', django_saml2_auth.views.signout),
+url(r'^accounts/logout/$', django_saml2_auth_multi.views.signout),
 
 # The following line will replace the default admin user logout with the signout page (optional)
-url(r'^admin/logout/$', django_saml2_auth.views.signout),
+url(r'^admin/logout/$', django_saml2_auth_multi.views.signout),
 ```
 
 To override the built in signout page put a template named 'django\_saml2\_auth/signout.html' in your project's template folder.
 
 If your SAML2 identity provider uses user attribute names other than the defaults listed in the `settings.py` `ATTRIBUTES_MAP`, update them in `settings.py`.
-
-## For Okta Users
-
-I created this plugin originally for Okta. The `METADATA_AUTO_CONF_URL` needed in `settings.py` can be found in the Okta Web UI by navigating to the SAML2 app's `Sign On` tab. In the `Settings` box, you should see:
-
-    Identity Provider metadata is available if this application supports dynamic configuration.
-
-The `Identity Provider metadata` link is the `METADATA_AUTO_CONF_URL`.
-
-More information can be found in the [Okta Developer Documentation](https://developer.okta.com/docs/guides/saml-application-setup/overview/).
-
-## Release Process
-
-I adopted a reasonably simple release process, which is almost automated, except for two actions that needed to be taken to start a release:
-
-1. Update [setup.py](setup.py) and increase the version number in the `setup` function. Unless something backward-incompatible is introduced, only the minor version is upgraded: 3.8.0 becomes 3.9.0.
-2. Tag the `main` branch with the the `vSEMVER`, e.g. `v3.9.0`, and git-push the tag.
-3. The release and publish to PyPI is handled in the CI/CD using GitHub Actions.
-4. Create a new release with auto-generated (and polished) release notes on the tag.
-5. Download [SBOM artifacts](https://github.com/grafana/django-saml2-auth/actions/runs/3227336576) generated by GitHub Actions for the corresponding run, and add them to the [release files](https://github.com/grafana/django-saml2-auth/releases/tag/v3.9.0).
```

### Comparing `django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/config.py` & `django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
     def load_idp_settings(self, idp_config, defaults):
         idp = {}
         if isinstance(idp_config, list):
             for conf in idp_config:
                 if "IDP_ID" not in conf:
                     raise ImproperlyConfigured(
-                        "Entity ID ('ID') of an IDP config is not set in 'SAML2_AUTH'. Set it to Entity ID of your IDP"
+                        "Entity ID ('ID') of an IDP config is not set in 'SAML2_AUTH'. "
+                        "Set it to Entity ID of your IDP"
                     )
                 idp_id = conf["IDP_ID"]
                 base = deepcopy(defaults)
                 base.update(conf)
                 idp[idp_id] = base
         else:
             base = deepcopy(defaults)
```

### Comparing `django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/errors.py` & `django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/errors.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/exceptions.py` & `django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/saml.py` & `django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/saml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Utility functions for various SAML client functions.
 """
 import base64
-from typing import Any, Callable, Dict, Mapping, Optional, Union
+from typing import Any, Callable, Dict, Mapping, Optional, Tuple
 from xml.etree import ElementTree
 
 from dictor import dictor  # type: ignore
-from django.http import HttpRequest, HttpResponse, HttpResponseRedirect
+from django.http import HttpRequest, HttpResponse
 from django.urls import NoReverseMatch
 
 from django_saml2_auth_multi.config import SAML2_SETTINGS
 from django_saml2_auth_multi.errors import (ERROR_CREATING_SAML_CONFIG_OR_CLIENT,
                                             INVALID_METADATA_URL,
                                             NO_ISSUER_IN_SAML_RESPONSE,
                                             NO_METADATA_URL_ASSOCIATED,
@@ -82,15 +82,15 @@
         metadata.load()
     except Exception:
         return False
 
     return True
 
 
-def get_metadata(user_id: Optional[str] = None, idp: str | None = None) -> Mapping[str, Any]:
+def get_metadata(user_id: Optional[str] = None, idp: Optional[str] = None) -> Mapping[str, Any]:
     """Returns metadata information, either by running the GET_METADATA_AUTO_CONF_URLS hook function
     if available, or by checking and returning a local file path or the METADATA_AUTO_CONF_URL. URLs
     are always validated and invalid URLs will be either filtered or raise a SAMLAuthError
     exception.
 
     Args:
         user_id (str, optional): If passed, it will be further processed by the
@@ -134,32 +134,35 @@
                 "exc_type": ValueError,
                 "error_code": INVALID_METADATA_URL,
                 "reason": "There was an error processing your request.",
                 "status_code": 500
             })
 
 
-def get_idp_from_saml_response(saml_response: str):
+def get_idp_from_saml_response(saml_response: str) -> str:
     try:
         parsed_xml = ElementTree.fromstring(saml_response)
-        entity_id = parsed_xml.find("{urn:oasis:names:tc:SAML:2.0:assertion}Issuer").text
-        idp_settings = SAML2_SETTINGS.get_idp_settings(entity_id)
-        return idp_settings["IDP_ID"]
+        if issuer_node := parsed_xml.find("{urn:oasis:names:tc:SAML:2.0:assertion}Issuer"):
+            entity_id = issuer_node.text
+            idp_settings = SAML2_SETTINGS.get_idp_settings(entity_id)
+            return idp_settings["IDP_ID"]
+        else:
+            raise ValueError("Issuer not found in assertion")
     except Exception as e:
         raise SAMLAuthError("Could not get Issuer from response.", extra={
             "exc_type": e,
             "error_code": NO_ISSUER_IN_SAML_RESPONSE,  # TODO: Different error code?
             "reason": "There was an error processing your request.",
             "status_code": 500
         })
 
 
 def get_saml_client(domain: str,
                     acs: Callable[..., HttpResponse],
-                    idp: str | None = None,
+                    idp: Optional[str] = None,
                     user_id: Optional[str] = None,
                     saml_response: Optional[str] = None) -> Optional[Saml2Client]:
     """Create a new Saml2Config object with the given config and return an initialized Saml2Client
     using the config object. The settings are read from django settings key: SAML2_AUTH.
 
     Args:
         domain (str): Domain name to get SAML config for
@@ -262,16 +265,15 @@
             "reason": "There was an error processing your request.",
             "status_code": 500
         })
 
 
 def decode_saml_response(
         request: HttpRequest,
-        acs: Callable[..., HttpResponse]) -> Union[
-            HttpResponseRedirect, Optional[AuthnResponse], None]:
+        acs: Callable[..., HttpResponse]) -> Tuple[AuthnResponse, Optional[str]]:
     """Given a request, the authentication response inside the SAML response body is parsed,
     decoded and returned. If there are any issues parsing the request, the identity or the issuer,
     an exception is raised.
 
     Args:
         request (HttpRequest): Django request object from identity provider (IdP)
         acs (Callable[..., HttpResponse]): The acs endpoint
@@ -301,15 +303,17 @@
     except Exception:
         saml_response = None
 
     idp = None
     if saml_response:
         idp = get_idp_from_saml_response(saml_response)
 
-    saml_client = get_saml_client(get_assertion_url(request, idp), acs, idp, saml_response=saml_response)
+    saml_client = get_saml_client(
+        get_assertion_url(request, idp), acs, idp, saml_response=saml_response
+    )
     if not saml_client:
         raise SAMLAuthError("There was an error creating the SAML client.", extra={
             "exc_type": ValueError,
             "error_code": NO_SAML_CLIENT,
             "reason": "There was an error processing your request.",
             "status_code": 500
         })
@@ -346,15 +350,16 @@
             "reason": "There was an error processing your request.",
             "status_code": 500
         })
 
     return authn_response, idp
 
 
-def extract_user_identity(user_identity: Dict[str, Any], idp: str | None = None) -> Dict[str, Optional[Any]]:
+def extract_user_identity(user_identity: Dict[str, Any],
+                          idp: Optional[str] = None) -> Dict[str, Optional[Any]]:
     """Extract user information from SAML user identity object
 
     Args:
         user_identity (Dict[str, Any]): SAML user identity object (dict)
 
     Raises:
         SAMLAuthError: No token specified.
```

### Comparing `django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/tests/metadata.xml` & `django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/tests/metadata.xml`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/tests/settings.py` & `django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/tests/test_saml.py` & `django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/tests/test_saml.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/tests/test_user.py` & `django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/tests/test_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
     # Create a group for the users to join
     Group.objects.create(name="users")
     params = {
         "first_name": "test_John",
         "last_name": "test_Doe"
     }
-    user = create_new_user("user_test@example.com", **params)
+    user = create_new_user("user_test@example.com", **params)  # type: ignore
     # It can also be email depending on USERNAME_FIELD setting
     assert user.username == "user_test@example.com"
     assert user.is_active is True
     assert user.has_usable_password() is False
     assert user.groups.get(name="users") == Group.objects.get(name="users")
```

### Comparing `django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/tests/test_utils.py` & `django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 Tests for utils.py
 """
 
 import pytest
 from django.http import HttpRequest, HttpResponse
 from django.urls import NoReverseMatch
 from django_saml2_auth_multi.exceptions import SAMLAuthError
-from django_saml2_auth_multi.utils import exception_handler, get_reverse, run_hook, is_jwt_well_formed
+from django_saml2_auth_multi.utils import (exception_handler,
+                                           get_reverse,
+                                           run_hook,
+                                           is_jwt_well_formed)
 
 
 def divide(a: int, b: int = 1) -> int:
     """Simple division function for testing run_hook
 
     Args:
         a (int): Dividend
```

### Comparing `django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/user.py` & `django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     user.save()
     user.refresh_from_db()
 
     return user
 
 
-def get_or_create_user(user: Dict[str, Any], settings: dict | None = None) -> Tuple[bool, User]:
+def get_or_create_user(user: Dict[str, Any], settings: Optional[dict] = None) -> Tuple[bool, User]:
     """Get or create a new user and optionally add it to one or more group(s)
 
     Args:
         user (Dict[str, Any]): User information
 
     Raises:
         SAMLAuthError: Cannot create user. Missing user_id.
@@ -117,15 +117,17 @@
             user_id = get_user_id(user)
             if not user_id:
                 raise SAMLAuthError("Cannot create user. Missing user_id.", extra={
                     "error_code": SHOULD_NOT_CREATE_USER,
                     "reason": "Cannot create user. Missing user_id.",
                     "status_code": 400
                 })
-            target_user = create_new_user(user_id, user["first_name"], user["last_name"], saml2_auth_settings)
+            target_user = create_new_user(
+                user_id, user["first_name"], user["last_name"], saml2_auth_settings
+            )
 
             create_user_trigger = dictor(saml2_auth_settings, "TRIGGER.CREATE_USER")
             if create_user_trigger:
                 run_hook(create_user_trigger, user)  # type: ignore
 
             target_user.refresh_from_db()
             created = True
@@ -181,15 +183,15 @@
 
     if isinstance(user, str):
         user_id = user
 
     return user_id.lower() if user_id else None
 
 
-def get_user(user: Union[str, Dict[str, str]], settings: dict | None = None) -> User:
+def get_user(user: Union[str, Dict[str, str]], settings: Optional[dict] = None) -> User:
     """Get user from database given a cleaned user info object or a user_id
 
     Args:
         user (Union[str, Dict[str, str]]): Either a user_id (as str) or a cleaned user info object
 
     Returns:
         User: An instance of the User model
@@ -296,15 +298,15 @@
             "exc_type": Exception,
             "error_code": NO_JWT_PUBLIC_KEY,
             "reason": "Cannot encode/decode JWT token for login.",
             "status_code": 500
         })
 
 
-def create_jwt_token(user_id: str, settings: dict | None = None) -> Optional[str]:
+def create_jwt_token(user_id: str, settings: Optional[dict] = None) -> Optional[str]:
     """Create a new JWT token
 
     Args:
         user_id (str): User's username or email based on User.USERNAME_FIELD
 
     Returns:
         Optional[str]: JWT token
@@ -347,15 +349,15 @@
     secret = jwt_secret if (
         jwt_secret and
         jwt_algorithm not in requires_cryptography) else jwt_private_key
 
     return jwt.encode(payload, secret, algorithm=jwt_algorithm)
 
 
-def create_custom_or_default_jwt(user: Union[str, User], settings: dict | None = None):
+def create_custom_or_default_jwt(user: Union[str, User], settings: Optional[dict] = None):
     """Create a new JWT token, eventually using custom trigger
 
     Args:
         user (Union[str, User]): User instance or User's username or email
             based on User.USERNAME_FIELD
 
     Raises:
@@ -398,15 +400,15 @@
                 "status_code": 500
             })
         jwt_token = create_jwt_token(user_id, saml2_auth_settings)
 
     return jwt_token
 
 
-def decode_jwt_token(jwt_token: str, settings: dict | None = None) -> Optional[str]:
+def decode_jwt_token(jwt_token: str, settings: Optional[dict] = None) -> Optional[str]:
     """Decode a JWT token
 
     Args:
         jwt_token (str): The token to decode
 
     Raises:
         SAMLAuthError: Cannot decode JWT token.
@@ -439,15 +441,15 @@
             "exc_type": type(exc),
             "error_code": CANNOT_DECODE_JWT_TOKEN,
             "reason": "Cannot decode JWT token.",
             "status_code": 500
         })
 
 
-def decode_custom_or_default_jwt(jwt_token: str, settings: dict | None = None) -> Optional[str]:
+def decode_custom_or_default_jwt(jwt_token: str, settings: Optional[dict] = None) -> Optional[str]:
     """Decode a JWT token, eventually using custom trigger
 
     Args:
         jwt_token (str): The token to decode
 
     Raises:
         SAMLAuthError: Cannot decode JWT token.
```

### Comparing `django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/utils.py` & `django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/utils.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc1/django_saml2_auth_multi/views.py` & `django_saml2_auth_multi-3.11.0rc2/django_saml2_auth_multi/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         except TemplateDoesNotExist:
             return redirect(next_url)
     else:
         return redirect(next_url)
 
 
 @exception_handler
-def sp_initiated_login(request: HttpRequest, idp: str | None = None) -> HttpResponseRedirect:
+def sp_initiated_login(request: HttpRequest, idp: Optional[str] = None) -> HttpResponseRedirect:
     """This view is called by the SP to initiate a login to IdP, aka. SP-initiated SAML SSP.
 
     Args:
         request (HttpRequest): Incoming request from service provider (SP) for authentication
 
     Returns:
         HttpResponseRedirect: Redirect to the IdP login endpoint
@@ -210,21 +210,24 @@
                 raise SAMLAuthError("The token is invalid.", extra={
                     "exc_type": ValueError,
                     "error_code": INVALID_TOKEN,
                     "reason": "The token is invalid.",
                     "status_code": 403
                 })
             saml_client = get_saml_client(get_assertion_url(request, idp), acs, idp, user_id)
-            jwt_token = create_custom_or_default_jwt(user_id) # TODO: NoSettings
+            jwt_token = create_custom_or_default_jwt(user_id)  # TODO: NoSettings
             _, info = saml_client.prepare_for_authenticate(  # type: ignore
                 sign=False, relay_state=jwt_token)
             redirect_url = dict(info["headers"]).get("Location", "")
             if not redirect_url:
                 return HttpResponseRedirect(
-                    get_reverse([denied, "denied", "django_saml2_auth_multi:denied"]))  # type: ignore
+                    get_reverse(
+                        [denied, "denied", "django_saml2_auth_multi:denied"]
+                    )  # type: ignore
+                )
             return HttpResponseRedirect(redirect_url)
     else:
         raise SAMLAuthError("Request method is not supported.", extra={
             "exc_type": Exception,
             "error_code": INVALID_REQUEST_METHOD,
             "reason": "Request method is not supported.",
             "status_code": 404
```

### Comparing `django_saml2_auth_multi-3.11.0rc1/pyproject.toml` & `django_saml2_auth_multi-3.11.0rc2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "django_saml2_auth_multi"
-version = "3.11.0-rc1"
-description = "Django SAML2 Authentication Made Easy."
+version = "3.11.0-rc2"
+description = "Django SAML2 Authentication For Multi IdP Setups Made Easy."
 license = "Apache 2.0"
 keywords = ["django", "saml", "saml2sso", "authentication", "okta", "standard"]
 classifiers = ["Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Topic :: Software Development :: Libraries :: Python Modules", "License :: OSI Approved :: Apache Software License", "Framework :: Django :: 2.2", "Framework :: Django :: 3.2", "Framework :: Django :: 4.0", "Framework :: Django :: 4.1", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3.10", "Programming Language :: Python :: 3.11"]
 homepage = "https://github.com/mfnd/django-saml2-auth-multi"
 authors = ["Fang Li <surivlee+djsaml2auth@gmail.com>", "Mostafa Moradian <mostafa@grafana.com>", "Mustafa Efendioglu <mfnd@protonmail.com>"]
 readme = "README.md"
```

### Comparing `django_saml2_auth_multi-3.11.0rc1/PKG-INFO` & `django_saml2_auth_multi-3.11.0rc2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-saml2-auth-multi
-Version: 3.11.0rc1
-Summary: Django SAML2 Authentication Made Easy.
+Version: 3.11.0rc2
+Summary: Django SAML2 Authentication For Multi IdP Setups Made Easy.
 Home-page: https://github.com/mfnd/django-saml2-auth-multi
 License: Apache 2.0
 Keywords: django,saml,saml2sso,authentication,okta,standard
 Author: Fang Li
 Author-email: surivlee+djsaml2auth@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
@@ -29,66 +29,36 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: dictor (==0.1.11)
 Requires-Dist: pyjwt (==2.7.0)
 Requires-Dist: pysaml2 (==7.3.0)
 Requires-Dist: setuptools (>=67.8.0)
 Description-Content-Type: text/markdown
 
-# Django SAML2 Authentication
+# Django SAML2 Authentication Multi
 
-[![PyPI](https://img.shields.io/pypi/v/grafana-django-saml2-auth?label=version&logo=pypi)](https://pypi.org/project/grafana-django-saml2-auth/) [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/grafana/django-saml2-auth/deploy.yml?branch=main&logo=github)](https://github.com/grafana/django-saml2-auth/actions) [![Coveralls](https://img.shields.io/coveralls/github/grafana/django-saml2-auth?logo=coveralls)](https://coveralls.io/github/grafana/django-saml2-auth) [![Downloads](https://pepy.tech/badge/grafana-django-saml2-auth)](https://pepy.tech/project/grafana-django-saml2-auth)
+[![PyPI](https://img.shields.io/pypi/v/django-saml2-auth-multi?label=version&logo=pypi)](https://pypi.org/project/django-saml2-auth-multi/)
 
 This plugin provides a simple way to integrate SAML2 Authentication into your Django-powered app. SAML SSO is a standard, so practically any SAML2 based SSO identity provider is supported.
 
+This project is a fork of [django-saml2-auth](https://github.com/grafana/django-saml2-auth) and adds support for configuring multiple IDPs with separate configuration parameters. It should be compatible with existing deployments and configurations; nevertheless, unless you need additional features in this package (also which may not compatible with your use case), it is highly suggested to use base package.
+
 This plugin supports both identity provider and service provider-initiated SSO:
 
 - For IdP-initiated SSO, the user should sign in to their identity provider platform, e.g., Okta, and click on the application that authorizes and redirects the user to the service provider, that is your platform.
 - For SP-initiated SSO, the user should first exist on your platform, either by signing in via the first method (IdP-initiated SSO) or any other custom solution. It can be configured to be redirected to the correct application on the identity provider platform.
 
 For IdP-initiated SSO, the user will be created if it doesn't exist. Still, for SP-initiated SSO, the user should exist in your platform for the code to detect and redirect them to the correct application on the identity provider platform.
 
-## Project Information
-
-- Original Author: Fang Li ([@fangli](https://github.com/fangli))
-- Maintainer: Mostafa Moradian ([@mostafa](https://github.com/mostafa))
-- Version support matrix:
-    | **Python**                   | **Django** | **django-saml2-auth** | **End of Support<br/>(django-saml2-auth)** | **End of extended support<br/>(Django)** |
-    | ---------------------------- | ---------- | --------------------- | ------------------------------------------ | ---------------------------------------- |
-    | 3.7.x, 3.8.x, 3.9.x, 3.10.x  | 2.2.x      | >=3.4.0               | 3.10.0                                     | April 11, 2022                           |
-    | 3.7.x, 3.8.x, 3.9.x, 3.10.x  | 3.2.x      | >=3.4.0               |                                            | April 2024                               |
-    | 3.8.x, 3.9.x, 3.10.x         | 4.0.x      | >=3.4.0               | 3.10.0                                     | April 1, 2023                            |
-    | 3.8.x, 3.9.x, 3.10.x         | 4.1.x      | >=3.4.0               |                                            | December 2023                            |
-    | 3.8.x, 3.9.x, 3.10.x, 3.11.x | 4.2.x      | >=3.4.0               |                                            | April 2026                               |
-
-- Release logs are available [here](https://github.com/grafana/django-saml2-auth/releases).
-
-- For contribution, read [contributing guide](CONTRIBUTING.md).
-
-## CycloneDX SBOM
-
-From [v3.6.1](https://github.com/grafana/django-saml2-auth/releases/tag/v3.6.1), CycloneDX SBOMs will be generated for [requirements.txt](./requirements.txt) and [requirements_test.txt](./requirements_test.txt) and it can be accessed from the latest build of GitHub Actions for a tagged release, for example, [this one](https://github.com/grafana/django-saml2-auth/actions/runs/2245422253). The artifacts are only kept for 90 days.
-
-## Donate
-
-Please give us a shiny ![star](https://img.shields.io/github/stars/grafana/django-saml2-auth.svg?style=social&label=Star&maxAge=86400) and help spread the word.
 
 ## Installation
 
 You can install this plugin via `pip`. Make sure you update `pip` to be able to install from git:
 
 ```bash
-pip install grafana-django-saml2-auth
-```
-
-or from source:
-
-```bash
-git clone https://github.com/grafana/django-saml2-auth
-cd django-saml2-auth
-python setup.py install
+pip install django-saml2-auth-multi
 ```
 
 `xmlsec` is also required by `pysaml2`, so it must be installed:
 
 ``` bash
 // RPM-based distributions
 # yum install xmlsec1
@@ -114,132 +84,112 @@
     # These are the SAML2 related URLs. You can change "^saml2_auth/" regex to
     # any path you want, like "^sso/", "^sso_auth/", "^sso_login/", etc. (required)
     url(r'^sso/', include('django_saml2_auth_multi.urls')),
 
     # The following line will replace the default user login with SAML2 (optional)
     # If you want to specific the after-login-redirect-URL, use parameter "?next=/the/path/you/want"
     # with this view.
-    url(r'^accounts/login/$', django_saml2_auth.views.signin),
+    url(r'^accounts/login/$', django_saml2_auth_multi.views.signin),
 
     # The following line will replace the admin login with SAML2 (optional)
     # If you want to specific the after-login-redirect-URL, use parameter "?next=/the/path/you/want"
     # with this view.
-    url(r'^admin/login/$', django_saml2_auth.views.signin),
+    url(r'^admin/login/$', django_saml2_auth_multi.views.signin),
     ```
 
-3. Add `'django_saml2_auth'` to `INSTALLED_APPS` in your django `settings.py`:
+3. Add `'django_saml2_auth_multi'` to `INSTALLED_APPS` in your django `settings.py`:
 
     ```python
     INSTALLED_APPS = [
         '...',
         'django_saml2_auth_multi',
     ]
     ```
 
 4. In `settings.py`, add the SAML2 related configuration:
 
+    `SAML2_AUTH` configuration variable can be a dictionary (for configuring single IDP) or a list (for configuring list of IDPs).
+
     Please note, the only required setting is **METADATA\_AUTO\_CONF\_URL** or the existence of a **GET\_METADATA\_AUTO\_CONF\_URLS** trigger function. The following block shows all required and optional configuration settings and their default values.
 
     ```python
-    SAML2_AUTH = {
-        # Metadata is required, choose either remote url or local file path
-        'METADATA_AUTO_CONF_URL': '[The auto(dynamic) metadata configuration URL of SAML2]',
-        'METADATA_LOCAL_FILE_PATH': '[The metadata configuration file path]',
-        'KEY_FILE': '[The key file path]',
-        'CERT_FILE': '[The certificate file path]',
-
-        'DEBUG': False,  # Send debug information to a log file
-        # Optional logging configuration.
-        # By default, it won't log anything.
-        # The following configuration is an example of how to configure the logger,
-        # which can be used together with the DEBUG option above. Please note that
-        # the logger configuration follows the Python's logging configuration schema:
-        # https://docs.python.org/3/library/logging.config.html#logging-config-dictschema
-        'LOGGING': {
-            'version': 1,
-            'formatters': {
-                'simple': {
-                    'format': '[%(asctime)s] [%(levelname)s] [%(name)s.%(funcName)s] %(message)s',
-                },
+    SAML2_AUTH = [
+        {
+            # Set this to entity ID of IdP. Used when selecting redirection URL in login view and determining issuer IdP in ACS endpoint.
+            # Should be same with Issuer ID in assertions.
+            # Required when a list is provided for SAML2_AUTH (i.e. multiple IDPs are configured). 
+            'IDP_ID': '<Entity ID of IdP>',
+
+            # Metadata is required, choose either remote url or local file path
+            'METADATA_AUTO_CONF_URL': '[The auto(dynamic) metadata configuration URL of SAML2]',
+            'METADATA_LOCAL_FILE_PATH': '[The metadata configuration file path]',
+            'KEY_FILE': '[The key file path]',
+            'CERT_FILE': '[The certificate file path]',
+
+            # Optional settings below
+            'DEFAULT_NEXT_URL': '/admin',  # Custom target redirect URL after the user get logged in. Default to /admin if not set. This setting will be overwritten if you have parameter ?next= specificed in the login URL.
+            'CREATE_USER': True,  # Create a new Django user when a new user logs in. Defaults to True.
+            'NEW_USER_PROFILE': {
+                'USER_GROUPS': [],  # The default group name when a new user logs in
+                'ACTIVE_STATUS': True,  # The default active status for new users
+                'STAFF_STATUS': False,  # The staff status for new users
+                'SUPERUSER_STATUS': False,  # The superuser status for new users
             },
-            'handlers': {
-                'stdout': {
-                    'class': 'logging.StreamHandler',
-                    'stream': 'ext://sys.stdout',
-                    'level': 'DEBUG',
-                    'formatter': 'simple',
-                },
+            'ATTRIBUTES_MAP': {  # Change Email/UserName/FirstName/LastName to corresponding SAML2 userprofile attributes.
+                'email': 'user.email',
+                'username': 'user.username',
+                'first_name': 'user.first_name',
+                'last_name': 'user.last_name',
+                'token': 'Token',  # Mandatory, can be unrequired if TOKEN_REQUIRED is False
+                'groups': 'Groups',  # Optional
             },
-            'loggers': {
-                'saml2': {
-                    'level': 'DEBUG'
-                },
+            'GROUPS_MAP': {  # Optionally allow mapping SAML2 Groups to Django Groups
+                'SAML Group Name': 'Django Group Name',
             },
-            'root': {
-                'level': 'DEBUG',
-                'handlers': [
-                    'stdout',
-                ],
+            'TRIGGER': {
+                # Optional: needs to return a User Model instance or None
+                'GET_USER': 'path.to.your.get.user.hook.method',
+                'CREATE_USER': 'path.to.your.new.user.hook.method',
+                'BEFORE_LOGIN': 'path.to.your.login.hook.method',
+                'AFTER_LOGIN': 'path.to.your.after.login.hook.method',
+                # Optional. This is executed right before METADATA_AUTO_CONF_URL.
+                # For systems with many metadata files registered allows to narrow the search scope.
+                'GET_USER_ID_FROM_SAML_RESPONSE': 'path.to.your.get.user.from.saml.hook.method',
+                # This can override the METADATA_AUTO_CONF_URL to enumerate all existing metadata autoconf URLs
+                'GET_METADATA_AUTO_CONF_URLS': 'path.to.your.get.metadata.conf.hook.method',
             },
-        },
-
-        # Optional settings below
-        'DEFAULT_NEXT_URL': '/admin',  # Custom target redirect URL after the user get logged in. Default to /admin if not set. This setting will be overwritten if you have parameter ?next= specificed in the login URL.
-        'CREATE_USER': True,  # Create a new Django user when a new user logs in. Defaults to True.
-        'NEW_USER_PROFILE': {
-            'USER_GROUPS': [],  # The default group name when a new user logs in
-            'ACTIVE_STATUS': True,  # The default active status for new users
-            'STAFF_STATUS': False,  # The staff status for new users
-            'SUPERUSER_STATUS': False,  # The superuser status for new users
-        },
-        'ATTRIBUTES_MAP': {  # Change Email/UserName/FirstName/LastName to corresponding SAML2 userprofile attributes.
-            'email': 'user.email',
-            'username': 'user.username',
-            'first_name': 'user.first_name',
-            'last_name': 'user.last_name',
-            'token': 'Token',  # Mandatory, can be unrequired if TOKEN_REQUIRED is False
-            'groups': 'Groups',  # Optional
-        },
-        'GROUPS_MAP': {  # Optionally allow mapping SAML2 Groups to Django Groups
-            'SAML Group Name': 'Django Group Name',
-        },
-        'TRIGGER': {
-            # Optional: needs to return a User Model instance or None
-            'GET_USER': 'path.to.your.get.user.hook.method',
-            'CREATE_USER': 'path.to.your.new.user.hook.method',
-            'BEFORE_LOGIN': 'path.to.your.login.hook.method',
-            'AFTER_LOGIN': 'path.to.your.after.login.hook.method',
-            # Optional. This is executed right before METADATA_AUTO_CONF_URL.
-            # For systems with many metadata files registered allows to narrow the search scope.
-            'GET_USER_ID_FROM_SAML_RESPONSE': 'path.to.your.get.user.from.saml.hook.method',
-            # This can override the METADATA_AUTO_CONF_URL to enumerate all existing metadata autoconf URLs
-            'GET_METADATA_AUTO_CONF_URLS': 'path.to.your.get.metadata.conf.hook.method',
-        },
-        'ASSERTION_URL': 'https://mysite.com',  # Custom URL to validate incoming SAML requests against
-        'ENTITY_ID': 'https://mysite.com/saml2_auth/acs/',  # Populates the Issuer element in authn request
-        'NAME_ID_FORMAT': FormatString,  # Sets the Format property of authn NameIDPolicy element, e.g. 'user.email'
-        'USE_JWT': True,  # Set this to True if you are running a Single Page Application (SPA) with Django Rest Framework (DRF), and are using JWT authentication to authorize client users
-        'JWT_ALGORITHM': 'HS256',  # JWT algorithm to sign the message with
-        'JWT_SECRET': 'your.jwt.secret',  # JWT secret to sign the message with
-        'JWT_PRIVATE_KEY': '--- YOUR PRIVATE KEY ---',  # Private key to sign the message with. The algorithm should be set to RSA256 or a more secure alternative.
-        'JWT_PRIVATE_KEY_PASSPHRASE': 'your.passphrase',  # If your private key is encrypted, you might need to provide a passphrase for decryption
-        'JWT_PUBLIC_KEY': '--- YOUR PUBLIC KEY ---',  # Public key to decode the signed JWT token
-        'JWT_EXP': 60,  # JWT expiry time in seconds
-        'FRONTEND_URL': 'https://myfrontendclient.com',  # Redirect URL for the client if you are using JWT auth with DRF. See explanation below
-        'LOGIN_CASE_SENSITIVE': True,  # whether of not to get the user in case_sentive mode
-        'AUTHN_REQUESTS_SIGNED': True, # Require each authentication request to be signed
-        'LOGOUT_REQUESTS_SIGNED': True,  # Require each logout request to be signed
-        'WANT_ASSERTIONS_SIGNED': True,  # Require each assertion to be signed
-        'WANT_RESPONSE_SIGNED': True,  # Require response to be signed
-        'ACCEPTED_TIME_DIFF': None,  # Accepted time difference between your server and the Identity Provider
-        'ALLOWED_REDIRECT_HOSTS': ["https://myfrontendclient.com"], # Allowed hosts to redirect to using the ?next parameter
-        'TOKEN_REQUIRED': True,  # Whether or not to require the token parameter in the SAML assertion
-    }
+            'ASSERTION_URL': 'https://mysite.com',  # Custom URL to validate incoming SAML requests against
+            'ENTITY_ID': 'https://mysite.com/saml2_auth/acs/',  # Populates the Issuer element in authn request
+            'NAME_ID_FORMAT': FormatString,  # Sets the Format property of authn NameIDPolicy element, e.g. 'user.email'
+            'USE_JWT': True,  # Set this to True if you are running a Single Page Application (SPA) with Django Rest Framework (DRF), and are using JWT authentication to authorize client users
+            'JWT_ALGORITHM': 'HS256',  # JWT algorithm to sign the message with
+            'JWT_SECRET': 'your.jwt.secret',  # JWT secret to sign the message with
+            'JWT_PRIVATE_KEY': '--- YOUR PRIVATE KEY ---',  # Private key to sign the message with. The algorithm should be set to RSA256 or a more secure alternative.
+            'JWT_PRIVATE_KEY_PASSPHRASE': 'your.passphrase',  # If your private key is encrypted, you might need to provide a passphrase for decryption
+            'JWT_PUBLIC_KEY': '--- YOUR PUBLIC KEY ---',  # Public key to decode the signed JWT token
+            'JWT_EXP': 60,  # JWT expiry time in seconds
+            'FRONTEND_URL': 'https://myfrontendclient.com',  # Redirect URL for the client if you are using JWT auth with DRF. See explanation below
+            'LOGIN_CASE_SENSITIVE': True,  # whether of not to get the user in case_sentive mode
+            'AUTHN_REQUESTS_SIGNED': True, # Require each authentication request to be signed
+            'LOGOUT_REQUESTS_SIGNED': True,  # Require each logout request to be signed
+            'WANT_ASSERTIONS_SIGNED': True,  # Require each assertion to be signed
+            'WANT_RESPONSE_SIGNED': True,  # Require response to be signed
+            'ACCEPTED_TIME_DIFF': None,  # Accepted time difference between your server and the Identity Provider
+            'ALLOWED_REDIRECT_HOSTS': ["https://myfrontendclient.com"], # Allowed hosts to redirect to using the ?next parameter
+            'TOKEN_REQUIRED': True,  # Whether or not to require the token parameter in the SAML assertion
+        }
+    ]
     ```
 
+    `SAML2_AUTH_DEFAULTS` configuration variable can be used for specifying common settings for all IdP configurations. Same list of settings can be used for `SAML2_AUTH_DEFAULTS`.
+
+    `SAML2_AUTH_DEBUG` (default: `False`) configuration variable toggles debug flag for logging.
+
+
+
 5. In your SAML2 SSO identity provider, set the Single-sign-on URL and Audience URI (SP Entity ID) to <http://your-domain/saml2_auth/acs/>
 
 ## How to debug?
 
 To debug what's happening between the SAMLP Identity Provider and your Django application, you can use SAML-tracer for [Firefox](https://addons.mozilla.org/en-US/firefox/addon/saml-tracer/) or [Chrome](https://chrome.google.com/webstore/detail/saml-tracer/mpdajninpobndbfcldcmbpnnbhibjmch?hl=en). Using this tool, you can see the SAML requests and responses that are being sent back and forth.
 
 Also, you can enable the debug mode in the `settings.py` file by setting the `DEBUG` flag to `True` and enabling the `LOGGING` configuration. See above for configuration examples.
@@ -248,15 +198,16 @@
 
 ## Module Settings
 
 Some of the following settings are related to how this module operates. The rest are passed as options to the pysaml2 library. For more information on the pysaml2 library, see the [pysaml2 documentation](https://pysaml2.readthedocs.io/en/latest/howto/config.html), which contains examples of available settings. Also, note that all settings are not implemented in this module.
 
 | **Field name**                              | **Description**                                                                                                                                                                                                                                                                                                                                                                                                                                             | **Data type(s)** | **Default value(s)**                                                                                                                     | **Example**                                              |
 | ------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
-| **METADATA\_AUTO\_CONF\_URL**               | Auto SAML2 metadata configuration URL                                                                                                                                                                                                                                                                                                                                                                                                                       | `str`            | `None`                                                                                                                                   | `https://ORG.okta.com/app/APP-ID/sso/saml/metadata`      |
+| **IDP\_ID**               | Entity ID of IdP which is also used as Issuer information in assertions                                                                                                                                                                                                                                                                                                                                                                                                                       | `str`            | `None`                                                                                                                                   | `urn:ORG.eu.auth0.com`      |
+| **METADATA\_AUTO\_CONF\_URL**               | Auto SAML2 metadata configuration URL                                                                                                                                                                                                                                                                                                                                                                                                                       | `str`            | `None`                                                                                                                                   | `https://ORG.eu.auth0.com/samlp/metadata/`      |
 | **METADATA\_LOCAL\_FILE\_PATH**             | SAML2 metadata configuration file path                                                                                                                                                                                                                                                                                                                                                                                                                      | `str`            | `None`                                                                                                                                   | `/path/to/the/metadata.xml`                              |
 | **KEY_FILE**                                | SAML2 private key file path                                                                                                                                                                                                                                                                                                                                                                                                                                 | `str`            | `None`                                                                                                                                   | `/path/to/the/key.pem`                                   |
 | **CERT_FILE**                               | SAML2 public certificate file path                                                                                                                                                                                                                                                                                                                                                                                                                          | `str`            | `None`                                                                                                                                   | `/path/to/the/cert.pem`                                  |
 | **DEBUG**                                   | Send debug information to a log file                                                                                                                                                                                                                                                                                                                                                                                                                        | `bool`           | `False`                                                                                                                                  |                                                          |
 | **LOGGING**                                 | Logging configuration dictionary                                                                                                                                                                                                                                                                                                                                                                                                                            | `dict`           | Not set.                                                                                                                                 |                                                          |
 | **DEFAULT\_NEXT\_URL**                      | Custom target redirect URL after the user get logged in. Default to /admin if not set. This setting will be overwritten if you have parameter `?next=` specificed in the login URL.                                                                                                                                                                                                                                                                         | `str`            | `admin:index`                                                                                                                            | `https://app.example.com/account/login`                  |
 | **CREATE\_USER**                            | Determines if a new Django user should be created for new users                                                                                                                                                                                                                                                                                                                                                                                             | `bool`           | `True`                                                                                                                                   |                                                          |
@@ -373,37 +324,17 @@
 
 If a 'django\_saml2\_auth/welcome.html' template exists, that page will be shown to the user upon login instead of the user being redirected to the previous visited page. This welcome page can contain some first-visit notes and welcome words. The [Django user object](https://docs.djangoproject.com/en/1.9/ref/contrib/auth/#django.contrib.auth.models.User) is available within the template as the `user` template variable.
 
 To enable a logout page, add the following lines to `urls.py`, before any `urlpatterns`:
 
 ```python
 # The following line will replace the default user logout with the signout page (optional)
-url(r'^accounts/logout/$', django_saml2_auth.views.signout),
+url(r'^accounts/logout/$', django_saml2_auth_multi.views.signout),
 
 # The following line will replace the default admin user logout with the signout page (optional)
-url(r'^admin/logout/$', django_saml2_auth.views.signout),
+url(r'^admin/logout/$', django_saml2_auth_multi.views.signout),
 ```
 
 To override the built in signout page put a template named 'django\_saml2\_auth/signout.html' in your project's template folder.
 
 If your SAML2 identity provider uses user attribute names other than the defaults listed in the `settings.py` `ATTRIBUTES_MAP`, update them in `settings.py`.
 
-## For Okta Users
-
-I created this plugin originally for Okta. The `METADATA_AUTO_CONF_URL` needed in `settings.py` can be found in the Okta Web UI by navigating to the SAML2 app's `Sign On` tab. In the `Settings` box, you should see:
-
-    Identity Provider metadata is available if this application supports dynamic configuration.
-
-The `Identity Provider metadata` link is the `METADATA_AUTO_CONF_URL`.
-
-More information can be found in the [Okta Developer Documentation](https://developer.okta.com/docs/guides/saml-application-setup/overview/).
-
-## Release Process
-
-I adopted a reasonably simple release process, which is almost automated, except for two actions that needed to be taken to start a release:
-
-1. Update [setup.py](setup.py) and increase the version number in the `setup` function. Unless something backward-incompatible is introduced, only the minor version is upgraded: 3.8.0 becomes 3.9.0.
-2. Tag the `main` branch with the the `vSEMVER`, e.g. `v3.9.0`, and git-push the tag.
-3. The release and publish to PyPI is handled in the CI/CD using GitHub Actions.
-4. Create a new release with auto-generated (and polished) release notes on the tag.
-5. Download [SBOM artifacts](https://github.com/grafana/django-saml2-auth/actions/runs/3227336576) generated by GitHub Actions for the corresponding run, and add them to the [release files](https://github.com/grafana/django-saml2-auth/releases/tag/v3.9.0).
-
```

