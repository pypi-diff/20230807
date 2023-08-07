# Comparing `tmp/pyakeneo-0.5.2.tar.gz` & `tmp/pyakeneo-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyakeneo-0.5.2.tar", max compression
+gzip compressed data, was "pyakeneo-0.6.0.tar", max compression
```

## Comparing `pyakeneo-0.5.2.tar` & `pyakeneo-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1860 2023-03-09 14:25:59.812086 pyakeneo-0.5.2/README.rst
--rw-r--r--   0        0        0        0 2023-03-09 14:25:59.816086 pyakeneo-0.5.2/pyakeneo/__init__.py
--rw-r--r--   0        0        0     3526 2023-03-09 14:25:59.816086 pyakeneo-0.5.2/pyakeneo/auth.py
--rw-r--r--   0        0        0     5817 2023-03-09 14:25:59.816086 pyakeneo-0.5.2/pyakeneo/client.py
--rw-r--r--   0        0        0      888 2023-03-09 14:25:59.816086 pyakeneo-0.5.2/pyakeneo/interfaces.py
--rw-r--r--   0        0        0    10770 2023-03-09 14:25:59.816086 pyakeneo-0.5.2/pyakeneo/resources.py
--rw-r--r--   0        0        0     4254 2023-03-09 14:25:59.816086 pyakeneo-0.5.2/pyakeneo/result.py
--rw-r--r--   0        0        0      772 2023-03-09 14:25:59.816086 pyakeneo-0.5.2/pyakeneo/utils.py
--rw-r--r--   0        0        0      536 2023-03-09 14:26:36.216372 pyakeneo-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2627 1970-01-01 00:00:00.000000 pyakeneo-0.5.2/setup.py
--rw-r--r--   0        0        0     2587 1970-01-01 00:00:00.000000 pyakeneo-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1860 2023-08-07 08:46:02.149987 pyakeneo-0.6.0/README.rst
+-rw-r--r--   0        0        0        0 2023-08-07 08:46:02.153987 pyakeneo-0.6.0/pyakeneo/__init__.py
+-rw-r--r--   0        0        0     3726 2023-08-07 08:46:02.153987 pyakeneo-0.6.0/pyakeneo/auth.py
+-rw-r--r--   0        0        0     5635 2023-08-07 08:46:02.153987 pyakeneo-0.6.0/pyakeneo/client.py
+-rw-r--r--   0        0        0      888 2023-08-07 08:46:02.153987 pyakeneo-0.6.0/pyakeneo/interfaces.py
+-rw-r--r--   0        0        0    10770 2023-08-07 08:46:02.153987 pyakeneo-0.6.0/pyakeneo/resources.py
+-rw-r--r--   0        0        0     4254 2023-08-07 08:46:02.153987 pyakeneo-0.6.0/pyakeneo/result.py
+-rw-r--r--   0        0        0      772 2023-08-07 08:46:02.153987 pyakeneo-0.6.0/pyakeneo/utils.py
+-rw-r--r--   0        0        0      536 2023-08-07 08:46:22.813867 pyakeneo-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2627 1970-01-01 00:00:00.000000 pyakeneo-0.6.0/setup.py
+-rw-r--r--   0        0        0     2587 1970-01-01 00:00:00.000000 pyakeneo-0.6.0/PKG-INFO
```

### Comparing `pyakeneo-0.5.2/README.rst` & `pyakeneo-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyakeneo-0.5.2/pyakeneo/auth.py` & `pyakeneo-0.6.0/pyakeneo/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,19 +20,28 @@
         self._client_id = client_id
         self._secret = secret
         self._username = username
         self._password = password
         self._token = None
         self._refresh_token = None
         self._expiry_date = None
+        self._session = requests.Session()
 
     @property
     def authorization(self):
         return "Bearer {0}".format(self._token)
 
+    @property
+    def session(self):
+        return self._session
+
+    @session.setter
+    def session(self, session):
+        self._session = session
+
     def _request_a_token(self, grant_type="password"):
         """Requests a token. Throws in case of error"""
         authorization = "Basic {0}".format(
             base64.b64encode(
                 "{0}:{1}".format(self._client_id, self._secret).encode("ascii")
             ).decode("utf-8")
         )
@@ -54,15 +63,15 @@
         else:
             raise ValueError(
                 "grant_type parameter is expected to be either "
                 + '"password" or "refresh_token". {0} provided'.format(grant_type)
             )
 
         url = urljoin(self._base_url, self.TOKEN_PATH)
-        r = requests.post(url, data=data, headers=headers)
+        r = self._session.post(url, data=data, headers=headers)
         r.raise_for_status()
 
         try:
             json_data = json.loads(r.text)
         except json.decoder.JSONDecodeError as e:
             raise SyntaxError(
                 "The server did not return expected json: {0}".format(r.text)
```

### Comparing `pyakeneo-0.5.2/pyakeneo/client.py` & `pyakeneo-0.6.0/pyakeneo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,52 +10,42 @@
 from pyakeneo.utils import urljoin
 
 
 class Client:
     BASIC_API_PATH = "/api/rest/v1/"
 
     def __init__(
-        self,
-        base_url,
-        client_id=None,
-        secret=None,
-        username=None,
-        password=None,
-        session=None,
-        auth=None,
+            self,
+            base_url: str,
+            client_id: str = None,
+            secret: str = None,
+            username: str = None,
+            password: str = None,
+            session: requests.Session = None,
     ):
-        """Expect credential
-        1) as auth, or
-        2) as client_id+secret+username+password, or
-        3) as session having an authentication."""
-        provided_auth = False
-        if not auth:
-            if client_id or secret or username or password:
-                if client_id and secret and username and password:
-                    provided_auth = True
-                    auth = Auth(base_url, client_id, secret, username, password)
-            elif session:
-                provided_auth = True
-        else:
-            provided_auth = True
-        if not provided_auth:
+        if not session and not (client_id and secret and username and password):
+            # No credentials provided neither via client_id+secret+username+password nor via session
             raise ValueError(
-                "Expect credential 1) as auth, or "
-                + "2) as client_id+secret+username+password, or "
-                + "3) as session having an authentication."
+                "Expect credentials via "
+                + "1) as client_id+secret+username+password, or "
+                + "2) as session having an authentication."
             )
+
         if not session:
             session = requests.Session()
-        self._init(base_url, session, auth)
+            session.auth = self._make_auth(base_url, client_id, secret, username, password)
+
+        self._init(base_url, session)
+
+    def _make_auth(self, base_url, client_id, secret, username, password) -> Auth:
+        return Auth(base_url, client_id, secret, username, password)
 
-    def _init(self, base_url, session, auth):
+    def _init(self, base_url, session):
         self._base_url = base_url
         self._session = session
-        if auth:
-            self._session.auth = auth
         self._session.headers.update({"Content-Type": "application/json"})
         self._resources = {
             "association_types": AssociationTypesPool(
                 urljoin(self._base_url, self.BASIC_API_PATH, "association-types/"),
                 session,
             ),
             "attributes": AttributesPool(
```

### Comparing `pyakeneo-0.5.2/pyakeneo/interfaces.py` & `pyakeneo-0.6.0/pyakeneo/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyakeneo-0.5.2/pyakeneo/resources.py` & `pyakeneo-0.6.0/pyakeneo/resources.py`

 * *Files identical despite different names*

### Comparing `pyakeneo-0.5.2/pyakeneo/result.py` & `pyakeneo-0.6.0/pyakeneo/result.py`

 * *Files identical despite different names*

### Comparing `pyakeneo-0.5.2/pyakeneo/utils.py` & `pyakeneo-0.6.0/pyakeneo/utils.py`

 * *Files identical despite different names*

### Comparing `pyakeneo-0.5.2/pyproject.toml` & `pyakeneo-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyakeneo"
-version = "0.5.2"
+version = "0.6.0"
 description = "Python client for the Akeneo API REST"
 authors = ["Kave Tech <kavetech@kavehome.com>"]
 readme = "README.rst"
 license = "MIT"
 homepage = "https://github.com/KaveTech/akeneo_api_client"
 
 [tool.poetry.dependencies]
```

### Comparing `pyakeneo-0.5.2/setup.py` & `pyakeneo-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.2,<3.0.0', 'structlog>=22.3.0,<23.0.0']
 
 setup_kwargs = {
     'name': 'pyakeneo',
-    'version': '0.5.2',
+    'version': '0.6.0',
     'description': 'Python client for the Akeneo API REST',
     'long_description': "|Build Status|\n|Documentation Status|\n\n\nPython client for Akeneo PIM API\n================================\n\nA simple Python client to use the `Akeneo PIM API`_.\n\nDependencies are managed with `poetry`_\n(list of dependencies available in `pyproject.toml`_).\n\nYou may install them with:\n\n.. code:: bashasda\n\n        poetry install --dev\n\nInstallation\n------------\n\n.. code:: bash\n\n        poetry install pyakeneo\n        \nUsage\n-----\n\nA simple example is provided in `docs/example_exporter.py`_.\n\nIf you experience issues when importing modules, run the examples as follow:\n\n.. code:: bash\n\n        cd docs\n        poetry run python example_exporter.py\n        \n\n.. _docs/example_exporter.py: https://raw.githubusercontent.com/kavetech/akeneo_api_client/master/docs/example.py\n\nTests\n-----\n\nRun tests as follow:\n\n.. code:: bash\n\n        poetry run nosetests\n        \nIf tests don't pass in your environment, please check that dependencies match those described in pyproject.toml. One way to do it is to ensure that poetry runs commands in a dedicated virtualenv by setting environment variable as follow:\n\n.. code:: bash\n\n        poetry install --dev\n\n\nTests are provided with mocks, recorded with `VCR.py`_. In case you need\nto (re)run tests, you should install the dataset in you PIM instance as\nfollow:\n\n.. _Akeneo PIM API: https://api.akeneo.com/\n.. _poetry: https://github.com/python-poetry/poetry\n.. _VCR.py: http://vcrpy.readthedocs.io/en/latest/index.html\n.. _pyproject.toml: https://python-poetry.org/docs/pyproject/\n\n.. |Build Status| image:: https://travis-ci.org/matthieudelaro/akeneo_api_client.svg?branch=master\n   :target: https://travis-ci.org/matthieudelaro/akeneo_api_client\n.. |Documentation Status| image:: https://readthedocs.org/projects/akeneo-api-client/badge/?version=latest\n   :target: http://akeneo-api-client.readthedocs.io/en/latest/\n",
     'author': 'Kave Tech',
     'author_email': 'kavetech@kavehome.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/KaveTech/akeneo_api_client',
```

### Comparing `pyakeneo-0.5.2/PKG-INFO` & `pyakeneo-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyakeneo
-Version: 0.5.2
+Version: 0.6.0
 Summary: Python client for the Akeneo API REST
 Home-page: https://github.com/KaveTech/akeneo_api_client
 License: MIT
 Author: Kave Tech
 Author-email: kavetech@kavehome.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

