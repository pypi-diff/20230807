# Comparing `tmp/keyrings_envvars-1.0.2.tar.gz` & `tmp/keyrings_envvars-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyrings_envvars-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "keyrings_envvars-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `keyrings_envvars-1.0.2.tar` & `keyrings_envvars-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3983 2023-07-23 13:34:22.085752 keyrings_envvars-1.0.2/README.rst
--rw-r--r--   0        0        0     2245 2023-07-23 15:49:52.914723 keyrings_envvars-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       76 2023-07-23 13:08:55.954574 keyrings_envvars-1.0.2/src/keyrings/envvars/__init__.py
--rw-r--r--   0        0        0     3561 2023-07-23 13:08:55.950574 keyrings_envvars-1.0.2/src/keyrings/envvars/keyring.py
--rw-r--r--   0        0        0        0 2023-07-23 13:08:55.946574 keyrings_envvars-1.0.2/src/keyrings/envvars/py.typed
--rw-r--r--   0        0        0       30 2023-07-23 13:08:55.954574 keyrings_envvars-1.0.2/src/keyrings/envvars/tests/__init__.py
--rw-r--r--   0        0        0     1774 2023-07-23 13:08:55.950574 keyrings_envvars-1.0.2/src/keyrings/envvars/tests/conftest.py
--rw-r--r--   0        0        0     2919 2023-07-23 13:08:55.954574 keyrings_envvars-1.0.2/src/keyrings/envvars/tests/keyring_test.py
--rw-r--r--   0        0        0     6866 2023-07-23 13:08:55.954574 keyrings_envvars-1.0.2/src/keyrings/envvars/tests/keyrings_envvars_test.py
--rw-r--r--   0        0        0     5511 1970-01-01 00:00:00.000000 keyrings_envvars-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4251 2023-08-07 03:31:53.658474 keyrings_envvars-1.0.3/README.rst
+-rw-r--r--   0        0        0     2316 2023-08-07 05:08:45.320252 keyrings_envvars-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-08-07 03:31:53.654474 keyrings_envvars-1.0.3/src/keyrings/envvars/__init__.py
+-rw-r--r--   0        0        0     3602 2023-08-07 03:56:16.793920 keyrings_envvars-1.0.3/src/keyrings/envvars/keyring.py
+-rw-r--r--   0        0        0        0 2023-08-07 03:31:53.658474 keyrings_envvars-1.0.3/src/keyrings/envvars/py.typed
+-rw-r--r--   0        0        0       30 2023-08-07 03:31:53.658474 keyrings_envvars-1.0.3/src/keyrings/envvars/tests/__init__.py
+-rw-r--r--   0        0        0     1774 2023-08-07 03:31:53.658474 keyrings_envvars-1.0.3/src/keyrings/envvars/tests/conftest.py
+-rw-r--r--   0        0        0     2919 2023-08-07 03:31:53.658474 keyrings_envvars-1.0.3/src/keyrings/envvars/tests/keyring_test.py
+-rw-r--r--   0        0        0     6866 2023-08-07 03:31:53.658474 keyrings_envvars-1.0.3/src/keyrings/envvars/tests/keyrings_envvars_test.py
+-rw-r--r--   0        0        0     5779 1970-01-01 00:00:00.000000 keyrings_envvars-1.0.3/PKG-INFO
```

### Comparing `keyrings_envvars-1.0.2/README.rst` & `keyrings_envvars-1.0.3/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 keyrings.envvars
 ================
 
 |PyPI| |Status| |Python Version| |License|
 
-|CI| |Codecov|
+|PyPI Downloads| |CI| |Codecov| |SonarCloud|
 
 |pre-commit| |Black|
 
-.. |PyPI| image:: https://img.shields.io/pypi/v/keyrings.envvars.svg
+.. |PyPI| image:: https://img.shields.io/pypi/v/keyrings.envvars
    :target: https://pypi.org/project/keyrings.envvars/
    :alt: PyPI
-.. |Status| image:: https://img.shields.io/pypi/status/keyrings.envvars.svg
+.. |Status| image:: https://img.shields.io/pypi/status/keyrings.envvars
    :target: https://pypi.org/project/keyrings.envvars/
    :alt: Status
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/keyrings.envvars
    :target: https://pypi.org/project/keyrings.envvars
    :alt: Python Version
+.. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/keyrings.envvars
+   :alt: PyPI - Downloads
 .. |License| image:: https://img.shields.io/pypi/l/keyrings.envvars
    :target: https://opensource.org/licenses/MIT
    :alt: License
 .. |CI| image:: https://github.com/wwuck/keyrings.envvars/workflows/CI/badge.svg
    :target: https://github.com/wwuck/keyrings.envvars/actions?workflow=CI
    :alt: CI
 .. |Codecov| image:: https://codecov.io/gh/wwuck/keyrings.envvars/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/wwuck/keyrings.envvars
    :alt: Codecov
+.. |SonarCloud| image:: https://sonarcloud.io/api/project_badges/measure?project=wwuck_keyrings.envvars&metric=alert_status
+   :alt: Sonar Coverage
 .. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
-.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000
    :target: https://github.com/psf/black
    :alt: Black
 
 
 *keyrings.envvars* is a keyring backend plugin for the keyring_ utility that provides credentials via environment variables.
```

### Comparing `keyrings_envvars-1.0.2/pyproject.toml` & `keyrings_envvars-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 dependencies = [
   'keyring>=23.4.0',
 ]
 description = 'keyring backend plugin to retrieve credentials from environment variables.'
 name = 'keyrings.envvars'
 readme = 'README.rst'
 requires-python = '>=3.9,<4'
-version = '1.0.2'
+version = '1.0.3'
 
 [project.entry-points."keyring.backends"]
 envvars = 'keyrings.envvars.keyring:EnvvarsKeyring'
 
 [project.optional-dependencies]
 mypy = [
   'keyring>=23.4.0',
@@ -72,14 +72,18 @@
 strict_equality = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
+[tool.pydoclint]
+arg-type-hints-in-docstring = false
+style = 'sphinx'
+
 [tool.ruff]
 line-length = 120
 
 [tool.ruff.isort]
 known-first-party = ['src']
 
 [tool.tomlsort]
```

### Comparing `keyrings_envvars-1.0.2/src/keyrings/envvars/keyring.py` & `keyrings_envvars-1.0.3/src/keyrings/envvars/keyring.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     priority: int = 1  # type: ignore[assignment]
 
     def __init__(self) -> None:
         super().__init__()  # type: ignore[no-untyped-call]
 
     @staticmethod
     def _get_trailing_number(s: str) -> str | None:
-        m = re.search(r'\d+$', s)
-        return m.group() if m else None
+        m = re.search(r'^KEYRING_SERVICE_NAME_(\d+)$', s)
+        return m.group(1) if m else None
 
     @staticmethod
     def _get_ids(environ_keys: AbstractSet[str]) -> filter[str]:
         return filter(
             None,
             map(
                 EnvvarsKeyring._get_trailing_number,
@@ -63,52 +63,51 @@
 
     def get_password(self, service: str, username: str) -> str | None:
         """
         Get the password for the username of the service.
 
         :param service: keyring service
         :param username: service username
-        :returns: Optional[str]
+        :rtype: str | None
         """
         cred = self.get_credential(service, username)
         if cred is not None:
             return str(cred.password)
         return None
 
     def set_password(self, service: str, username: str, password: str) -> None:
         """
         Set the password for the username of the service.
 
         :param service: keyring service
         :param username: service username
         :param password: service password
-        :returns str: password
         :raises PasswordSetError: error when setting password
         """
         raise PasswordSetError('Environment should not be modified by keyring')
 
     def delete_password(self, service: str, username: str) -> None:
         """
         Delete the password for the username of the service.
 
         :param service: keyring service
         :param username: service username
-        :returns str: password
         :raises PasswordDeleteError: error when deleting password
         """
         raise PasswordDeleteError('Environment should not be modified by keyring')
 
     def get_credential(
         self,
         service: str,
         username: str | None,
     ) -> EnvironCredential | None:
         """
         Get the username and password for the service.
 
         :param service: keyring service
         :param username: service username
-        :returns: EnvironCredential
+        :return: credentials if service/username credentials exist in keyring
+        :rtype: EnvironCredential | None
         """
         if username is not None:
             return EnvvarsKeyring._get_mapping().get((service, username))
         return None
```

### Comparing `keyrings_envvars-1.0.2/src/keyrings/envvars/tests/conftest.py` & `keyrings_envvars-1.0.3/src/keyrings/envvars/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `keyrings_envvars-1.0.2/src/keyrings/envvars/tests/keyring_test.py` & `keyrings_envvars-1.0.3/src/keyrings/envvars/tests/keyring_test.py`

 * *Files identical despite different names*

### Comparing `keyrings_envvars-1.0.2/src/keyrings/envvars/tests/keyrings_envvars_test.py` & `keyrings_envvars-1.0.3/src/keyrings/envvars/tests/keyrings_envvars_test.py`

 * *Files identical despite different names*

### Comparing `keyrings_envvars-1.0.2/PKG-INFO` & `keyrings_envvars-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyrings.envvars
-Version: 1.0.2
+Version: 1.0.3
 Summary: keyring backend plugin to retrieve credentials from environment variables.
 Author-email: Tom Cassidy <wirelessduck+py@gmail.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -32,40 +32,44 @@
 Provides-Extra: pytest
 
 keyrings.envvars
 ================
 
 |PyPI| |Status| |Python Version| |License|
 
-|CI| |Codecov|
+|PyPI Downloads| |CI| |Codecov| |SonarCloud|
 
 |pre-commit| |Black|
 
-.. |PyPI| image:: https://img.shields.io/pypi/v/keyrings.envvars.svg
+.. |PyPI| image:: https://img.shields.io/pypi/v/keyrings.envvars
    :target: https://pypi.org/project/keyrings.envvars/
    :alt: PyPI
-.. |Status| image:: https://img.shields.io/pypi/status/keyrings.envvars.svg
+.. |Status| image:: https://img.shields.io/pypi/status/keyrings.envvars
    :target: https://pypi.org/project/keyrings.envvars/
    :alt: Status
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/keyrings.envvars
    :target: https://pypi.org/project/keyrings.envvars
    :alt: Python Version
+.. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/keyrings.envvars
+   :alt: PyPI - Downloads
 .. |License| image:: https://img.shields.io/pypi/l/keyrings.envvars
    :target: https://opensource.org/licenses/MIT
    :alt: License
 .. |CI| image:: https://github.com/wwuck/keyrings.envvars/workflows/CI/badge.svg
    :target: https://github.com/wwuck/keyrings.envvars/actions?workflow=CI
    :alt: CI
 .. |Codecov| image:: https://codecov.io/gh/wwuck/keyrings.envvars/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/wwuck/keyrings.envvars
    :alt: Codecov
+.. |SonarCloud| image:: https://sonarcloud.io/api/project_badges/measure?project=wwuck_keyrings.envvars&metric=alert_status
+   :alt: Sonar Coverage
 .. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
-.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000
    :target: https://github.com/psf/black
    :alt: Black
 
 
 *keyrings.envvars* is a keyring backend plugin for the keyring_ utility that provides credentials via environment variables.
```

