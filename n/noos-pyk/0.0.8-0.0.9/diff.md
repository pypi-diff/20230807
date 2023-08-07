# Comparing `tmp/noos-pyk-0.0.8.tar.gz` & `tmp/noos_pyk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noos-pyk-0.0.8.tar", last modified: Fri Mar 24 11:10:43 2023, max compression
+gzip compressed data, was "noos_pyk-0.0.9.tar", max compression
```

## Comparing `noos-pyk-0.0.8.tar` & `noos_pyk-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1077 2023-03-24 11:10:33.514142 noos-pyk-0.0.8/LICENSE
--rw-r--r--   0        0        0     2007 2023-03-24 11:10:33.514142 noos-pyk-0.0.8/README.md
--rw-r--r--   0        0        0     1785 2023-03-24 11:10:33.514142 noos-pyk-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-24 11:10:33.514142 noos-pyk-0.0.8/src/noos_pyk/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 11:10:33.514142 noos-pyk-0.0.8/src/noos_pyk/clients/__init__.py
--rw-r--r--   0        0        0     1181 2023-03-24 11:10:33.514142 noos-pyk-0.0.8/src/noos_pyk/clients/auth.py
--rw-r--r--   0        0        0     3671 2023-03-24 11:10:33.514142 noos-pyk-0.0.8/src/noos_pyk/clients/base.py
--rw-r--r--   0        0        0     2539 2023-03-24 11:10:33.514142 noos-pyk-0.0.8/src/noos_pyk/clients/http.py
--rw-r--r--   0        0        0     1131 2023-03-24 11:10:33.514142 noos-pyk-0.0.8/src/noos_pyk/clients/json.py
--rw-r--r--   0        0        0     2662 2023-03-24 11:10:33.514142 noos-pyk-0.0.8/src/noos_pyk/clients/ws.py
--rw-r--r--   0        0        0     2892 2023-03-24 11:10:43.595245 noos-pyk-0.0.8/setup.py
--rw-r--r--   0        0        0     2726 2023-03-24 11:10:43.595523 noos-pyk-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-08-07 11:32:45.908029 noos_pyk-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2007 2023-08-07 11:32:45.908029 noos_pyk-0.0.9/README.md
+-rw-r--r--   0        0        0     1787 2023-08-07 11:32:45.912029 noos_pyk-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-07 11:32:45.912029 noos_pyk-0.0.9/src/noos_pyk/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:32:45.912029 noos_pyk-0.0.9/src/noos_pyk/clients/__init__.py
+-rw-r--r--   0        0        0     1181 2023-08-07 11:32:45.912029 noos_pyk-0.0.9/src/noos_pyk/clients/auth.py
+-rw-r--r--   0        0        0     3671 2023-08-07 11:32:45.912029 noos_pyk-0.0.9/src/noos_pyk/clients/base.py
+-rw-r--r--   0        0        0     2539 2023-08-07 11:32:45.912029 noos_pyk-0.0.9/src/noos_pyk/clients/http.py
+-rw-r--r--   0        0        0     1112 2023-08-07 11:32:45.912029 noos_pyk-0.0.9/src/noos_pyk/clients/json.py
+-rw-r--r--   0        0        0     2662 2023-08-07 11:32:45.912029 noos_pyk-0.0.9/src/noos_pyk/clients/ws.py
+-rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 noos_pyk-0.0.9/PKG-INFO
```

### Comparing `noos-pyk-0.0.8/LICENSE` & `noos_pyk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `noos-pyk-0.0.8/README.md` & `noos_pyk-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![CircleCI](https://circleci.com/gh/noosenergy/noos-requests.svg?style=svg&circle-token=5c5370df196704b1e8a8dd7c6f2ec0731c154beb)](https://circleci.com/gh/noosenergy/noos-requests)
+[![CircleCI](https://circleci.com/gh/noosenergy/noos-requests.svg?style=svg&circle-token=c08ede3341e1b8a80f87df87959f849fe40d148f)](https://circleci.com/gh/noosenergy/noos-requests)
 
 # Noos Energy Request Toolkit
 
 This is a simple, yet useful toolkit that supports you in writing Python clients to microservices-style apps.
 
 ## Installation
```

### Comparing `noos-pyk-0.0.8/pyproject.toml` & `noos_pyk-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry>=1.0.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 # Description
 name = "noos-pyk"
-version = "0.0.8"
+version = "0.0.9"
 description = "A simple, yet useful Python toolkit"
 # Credentials
 license = "MIT"
 authors = ["Noos Energy <contact@noos.energy>"]
 homepage = "https://github.com/noosenergy/noos-python-kit"
 # Package data
 readme = "README.md"
@@ -18,20 +18,20 @@
 ]
 # Distribution
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.11"
 requests = "*"
 websocket-client = { version = "*", optional = true }
 
 [tool.poetry.extras]
 websocket = ["websocket-client"]
 
 [tool.poetry.dev-dependencies]
```

### Comparing `noos-pyk-0.0.8/src/noos_pyk/clients/auth.py` & `noos_pyk-0.0.9/src/noos_pyk/clients/auth.py`

 * *Files identical despite different names*

### Comparing `noos-pyk-0.0.8/src/noos_pyk/clients/base.py` & `noos_pyk-0.0.9/src/noos_pyk/clients/base.py`

 * *Files identical despite different names*

### Comparing `noos-pyk-0.0.8/src/noos_pyk/clients/http.py` & `noos_pyk-0.0.9/src/noos_pyk/clients/http.py`

 * *Files identical despite different names*

### Comparing `noos-pyk-0.0.8/src/noos_pyk/clients/json.py` & `noos_pyk-0.0.9/src/noos_pyk/clients/json.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import cgi
 from http import client as http_client
 from typing import Any, Dict
 
 import requests
 
 from . import base, http
 
@@ -30,16 +29,15 @@
 
 # Helpers:
 
 
 def _deserialize_json_response(
     response: requests.Response, valid_content_type: str = DEFAULT_JSON_CONTENT_TYPE
 ) -> Json:
-    content_type, _ = cgi.parse_header(response.headers.get("content-type", ""))
-
+    content_type = response.headers.get("content-type", "").split(";")[0]
     if content_type == valid_content_type:
         return response.json()
 
     # When 204 is returned, there is explicitly no content.
     if response.status_code == http_client.NO_CONTENT:
         return {}
```

### Comparing `noos-pyk-0.0.8/src/noos_pyk/clients/ws.py` & `noos_pyk-0.0.9/src/noos_pyk/clients/ws.py`

 * *Files identical despite different names*

### Comparing `noos-pyk-0.0.8/setup.py` & `noos_pyk-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,83 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: noos-pyk
+Version: 0.0.9
+Summary: A simple, yet useful Python toolkit
+Home-page: https://github.com/noosenergy/noos-python-kit
+License: MIT
+Author: Noos Energy
+Author-email: contact@noos.energy
+Requires-Python: >=3.11,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Provides-Extra: websocket
+Requires-Dist: requests
+Requires-Dist: websocket-client ; extra == "websocket"
+Description-Content-Type: text/markdown
+
+[![CircleCI](https://circleci.com/gh/noosenergy/noos-requests.svg?style=svg&circle-token=c08ede3341e1b8a80f87df87959f849fe40d148f)](https://circleci.com/gh/noosenergy/noos-requests)
+
+# Noos Energy Request Toolkit
+
+This is a simple, yet useful toolkit that supports you in writing Python clients to microservices-style apps.
+
+## Installation
+
+Package available from the [PyPi repository](https://pypi.org/project/noos-pyk/):
+
+```sh
+pip install noos-pyk
+```
+
+## Usage as a library
+
+The project currently houses a boilerplate to build Python HTTP and WebSocket clients to web services.
+
+As an example, to implement a Python client wrapping up HashiCorp's Terraform Cloud API,
+
+```python
+# Import the namespace within your project
+from noos_pyk.clients import auth, json
+
+
+# Define a bearer token authentication class
+class TerraformAuth(auth.HTTPTokenAuth):
+    default_header = "Authorization"
+    default_value = "Bearer"
+
+
+# Wireup all components for a JSON REST client
+class TerraformClient(json.JSONClient, auth.AuthClient):
+    default_base_url = "https://app.terraform.io/api/"
+    default_content_type = "application/vnd.api+json"
+
+    default_auth_class = TerraformAuth
+```
+
+## Development
+
+On Mac OSX, make sure [poetry](https://python-poetry.org/) has been installed and pre-configured,
+
+```sh
+brew install poetry
+```
+
+This project is shipped with a Makefile, which is ready to do basic common tasks.
+
+```shell
+~$ make
+help                           Display this auto-generated help message
+update                         Lock and install build dependencies
+clean                          Clean project from temp files / dirs
+format                         Run auto-formatting linters
+install                        Install build dependencies from lock file
+lint                           Run python linters
+test                           Run pytest with all tests
+package                        Build project wheel distribution
+release                        Publish wheel distribution to PyPi
+```
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['noos_pyk', 'noos_pyk.clients']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests']
-
-extras_require = \
-{'websocket': ['websocket-client']}
-
-setup_kwargs = {
-    'name': 'noos-pyk',
-    'version': '0.0.8',
-    'description': 'A simple, yet useful Python toolkit',
-    'long_description': '[![CircleCI](https://circleci.com/gh/noosenergy/noos-requests.svg?style=svg&circle-token=5c5370df196704b1e8a8dd7c6f2ec0731c154beb)](https://circleci.com/gh/noosenergy/noos-requests)\n\n# Noos Energy Request Toolkit\n\nThis is a simple, yet useful toolkit that supports you in writing Python clients to microservices-style apps.\n\n## Installation\n\nPackage available from the [PyPi repository](https://pypi.org/project/noos-pyk/):\n\n```sh\npip install noos-pyk\n```\n\n## Usage as a library\n\nThe project currently houses a boilerplate to build Python HTTP and WebSocket clients to web services.\n\nAs an example, to implement a Python client wrapping up HashiCorp\'s Terraform Cloud API,\n\n```python\n# Import the namespace within your project\nfrom noos_pyk.clients import auth, json\n\n\n# Define a bearer token authentication class\nclass TerraformAuth(auth.HTTPTokenAuth):\n    default_header = "Authorization"\n    default_value = "Bearer"\n\n\n# Wireup all components for a JSON REST client\nclass TerraformClient(json.JSONClient, auth.AuthClient):\n    default_base_url = "https://app.terraform.io/api/"\n    default_content_type = "application/vnd.api+json"\n\n    default_auth_class = TerraformAuth\n```\n\n## Development\n\nOn Mac OSX, make sure [poetry](https://python-poetry.org/) has been installed and pre-configured,\n\n```sh\nbrew install poetry\n```\n\nThis project is shipped with a Makefile, which is ready to do basic common tasks.\n\n```shell\n~$ make\nhelp                           Display this auto-generated help message\nupdate                         Lock and install build dependencies\nclean                          Clean project from temp files / dirs\nformat                         Run auto-formatting linters\ninstall                        Install build dependencies from lock file\nlint                           Run python linters\ntest                           Run pytest with all tests\npackage                        Build project wheel distribution\nrelease                        Publish wheel distribution to PyPi\n```\n',
-    'author': 'Noos Energy',
-    'author_email': 'contact@noos.energy',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/noosenergy/noos-python-kit',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

