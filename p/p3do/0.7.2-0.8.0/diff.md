# Comparing `tmp/p3do-0.7.2.tar.gz` & `tmp/p3do-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p3do-0.7.2.tar", max compression
+gzip compressed data, was "p3do-0.8.0.tar", max compression
```

## Comparing `p3do-0.7.2.tar` & `p3do-0.8.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-07-14 12:34:35.426638 p3do-0.7.2/LICENSE
--rw-r--r--   0        0        0    15444 2023-07-14 12:34:35.426638 p3do-0.7.2/README.md
--rw-r--r--   0        0        0       22 2023-07-14 12:34:35.426638 p3do-0.7.2/p3do/__init__.py
--rw-r--r--   0        0        0    13964 2023-07-14 12:34:35.426638 p3do-0.7.2/p3do/cli.py
--rw-r--r--   0        0        0      274 2023-07-14 12:34:35.426638 p3do-0.7.2/p3do/github.py
--rw-r--r--   0        0        0     1798 2023-07-14 12:34:35.426638 p3do-0.7.2/p3do/jenkins.py
--rw-r--r--   0        0        0     1161 2023-07-14 12:34:35.426638 p3do-0.7.2/p3do/keycloak.py
--rw-r--r--   0        0        0     4626 2023-07-14 12:34:35.426638 p3do-0.7.2/p3do/poolparty.py
--rw-r--r--   0        0        0      938 2023-07-14 12:34:35.426638 p3do-0.7.2/pyproject.toml
--rw-r--r--   0        0        0    16424 1970-01-01 00:00:00.000000 p3do-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-07 14:14:37.560631 p3do-0.8.0/LICENSE
+-rw-r--r--   0        0        0    15981 2023-08-07 14:14:37.560631 p3do-0.8.0/README.md
+-rw-r--r--   0        0        0       22 2023-08-07 14:14:37.560631 p3do-0.8.0/p3do/__init__.py
+-rw-r--r--   0        0        0    14891 2023-08-07 14:14:37.560631 p3do-0.8.0/p3do/cli.py
+-rw-r--r--   0        0        0      274 2023-08-07 14:14:37.560631 p3do-0.8.0/p3do/github.py
+-rw-r--r--   0        0        0     1798 2023-08-07 14:14:37.560631 p3do-0.8.0/p3do/jenkins.py
+-rw-r--r--   0        0        0     1161 2023-08-07 14:14:37.560631 p3do-0.8.0/p3do/keycloak.py
+-rw-r--r--   0        0        0     6482 2023-08-07 14:14:37.560631 p3do-0.8.0/p3do/poolparty.py
+-rw-r--r--   0        0        0      938 2023-08-07 14:14:37.560631 p3do-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    16961 1970-01-01 00:00:00.000000 p3do-0.8.0/PKG-INFO
```

### Comparing `p3do-0.7.2/LICENSE` & `p3do-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `p3do-0.7.2/README.md` & `p3do-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -278,14 +278,28 @@
 The webhook consumer url (to configure in Semantic Middleware Configurator)
 is `http://localhost:5000/hook`.
 
 ``` bash
 p3do pp mock-server
 ```
 
+
+#### encrypt-license
+Encrypts PoolParty license data with the PoolParty standard encryption and the
+given encryption key
+
+KEY must be the base64 encoded encryption key for PoolParty licenses
+LICENSE path to the license data that shall be encrypted as PoolParty license file
+
+#### decrypt-license
+Decrypts a PoolParty license with the PoolParty standard decryption and the given encryption key
+
+KEY must be the base64 encoded encryption key for PoolParty licenses
+LICENSE is the path to an encrypted license file usually ending in .key
+
 ### kc
 
 Commands in this group allow to perform operations for Keycloak. Most of them
 need authentication and server information. Please read [KC
 Configuration](#kc-configuration) first on how to add your configuration.
 
 Commands:
```

### Comparing `p3do-0.7.2/p3do/cli.py` & `p3do-0.8.0/p3do/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -189,14 +189,41 @@
 
     The webhook consumer url (to configure in Semantic Middleware Configurator)
     is `http://localhost:5000/hook`.
     """
 
     poolparty.run_mock_server(port)
 
+
+@pp.command()
+@click.argument("key", type=click.STRING)
+@click.argument("license", type=click.File('r'))
+def decrypt_license(key, license):
+    """Decrypts a PoolParty license with the PoolParty standard decryption and the given encryption key
+
+    KEY must be the base64 encoded encryption key for PoolParty licenses
+    LICENSE is the path to an encrypted license file usually ending in .key
+    """
+
+    print(poolparty.decrypt_license(license, key))
+
+
+@pp.command()
+@click.argument("key", type=click.STRING)
+@click.argument("license", type=click.File('r'))
+def encrypt_license(key, license):
+    """Encrypts PoolParty license data with the PoolParty standard encryption and the given encryption key
+
+    KEY must be the base64 encoded encryption key for PoolParty licenses
+    LICENSE path to the license data that shall be encrypted as PoolParty license file
+    """
+
+    print(poolparty.encrypt_license(license, key))
+
+
 @jk.command()
 @click.option("--branch", help="The branch to build")
 @click.option('--no-autodetect', type=click.BOOL, is_flag=True, default=False, help="Disable autodetection of branch in a git repository")
 @click.option('--api-user', type=click.STRING, help="Jenkins API user (your username)")
 @click.option('--api-key', type=click.STRING, help="Jenkins API key (generate in Jenkins)")
 def build(branch: str, no_autodetect: bool, api_key: str, api_user: str):
     """Run the PoolParty build
```

### Comparing `p3do-0.7.2/p3do/jenkins.py` & `p3do-0.8.0/p3do/jenkins.py`

 * *Files identical despite different names*

### Comparing `p3do-0.7.2/p3do/keycloak.py` & `p3do-0.8.0/p3do/keycloak.py`

 * *Files identical despite different names*

### Comparing `p3do-0.7.2/pyproject.toml` & `p3do-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "p3do"
-version = "0.7.2"
+version = "0.8.0"
 description = "CLI utilities for p3d"
 authors = ["Armin Friedl <armin.friedl@semantic-web.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `p3do-0.7.2/PKG-INFO` & `p3do-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p3do
-Version: 0.7.2
+Version: 0.8.0
 Summary: CLI utilities for p3d
 License: MIT
 Author: Armin Friedl
 Author-email: armin.friedl@semantic-web.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -305,14 +305,28 @@
 The webhook consumer url (to configure in Semantic Middleware Configurator)
 is `http://localhost:5000/hook`.
 
 ``` bash
 p3do pp mock-server
 ```
 
+
+#### encrypt-license
+Encrypts PoolParty license data with the PoolParty standard encryption and the
+given encryption key
+
+KEY must be the base64 encoded encryption key for PoolParty licenses
+LICENSE path to the license data that shall be encrypted as PoolParty license file
+
+#### decrypt-license
+Decrypts a PoolParty license with the PoolParty standard decryption and the given encryption key
+
+KEY must be the base64 encoded encryption key for PoolParty licenses
+LICENSE is the path to an encrypted license file usually ending in .key
+
 ### kc
 
 Commands in this group allow to perform operations for Keycloak. Most of them
 need authentication and server information. Please read [KC
 Configuration](#kc-configuration) first on how to add your configuration.
 
 Commands:
```

