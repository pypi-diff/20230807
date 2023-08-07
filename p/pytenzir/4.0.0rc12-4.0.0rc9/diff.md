# Comparing `tmp/pytenzir-4.0.0rc12.tar.gz` & `tmp/pytenzir-4.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytenzir-4.0.0rc12.tar", max compression
+gzip compressed data, was "pytenzir-4.0.0rc9.tar", max compression
```

## Comparing `pytenzir-4.0.0rc12.tar` & `pytenzir-4.0.0rc9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1858 2023-08-04 10:32:02.469981 pytenzir-4.0.0rc12/README.md
--rw-r--r--   0        0        0     1539 2023-08-04 10:32:02.469981 pytenzir-4.0.0rc12/pyproject.toml
--rw-r--r--   0        0        0       81 2023-08-04 10:32:02.469981 pytenzir-4.0.0rc12/pytenzir/__init__.py
--rw-r--r--   0        0        0     5832 2023-08-04 10:32:02.469981 pytenzir-4.0.0rc12/pytenzir/apps/thehive.py
--rw-r--r--   0        0        0       74 2023-08-04 10:32:02.469981 pytenzir-4.0.0rc12/pytenzir/tenzir/__init__.py
--rw-r--r--   0        0        0     2913 2023-08-04 10:32:02.469981 pytenzir-4.0.0rc12/pytenzir/tenzir/cli.py
--rw-r--r--   0        0        0     3657 2023-08-04 10:32:02.469981 pytenzir-4.0.0rc12/pytenzir/tenzir/convert.py
--rw-r--r--   0        0        0     6170 2023-08-04 10:32:02.469981 pytenzir-4.0.0rc12/pytenzir/tenzir/tenzir.py
--rw-r--r--   0        0        0     7461 2023-08-04 10:32:02.469981 pytenzir-4.0.0rc12/pytenzir/utils/arrow.py
--rw-r--r--   0        0        0     2062 2023-08-04 10:32:02.469981 pytenzir-4.0.0rc12/pytenzir/utils/asyncio.py
--rw-r--r--   0        0        0      740 2023-08-04 10:32:02.469981 pytenzir-4.0.0rc12/pytenzir/utils/config.py
--rw-r--r--   0        0        0     1947 2023-08-04 10:32:02.469981 pytenzir-4.0.0rc12/pytenzir/utils/logging.py
--rw-r--r--   0        0        0     3112 1970-01-01 00:00:00.000000 pytenzir-4.0.0rc12/setup.py
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 pytenzir-4.0.0rc12/PKG-INFO
+-rw-r--r--   0        0        0     1858 2023-07-24 15:12:41.664579 pytenzir-4.0.0rc9/README.md
+-rw-r--r--   0        0        0     1538 2023-07-24 15:12:41.664579 pytenzir-4.0.0rc9/pyproject.toml
+-rw-r--r--   0        0        0       81 2023-07-24 15:12:41.664579 pytenzir-4.0.0rc9/pytenzir/__init__.py
+-rw-r--r--   0        0        0     5832 2023-07-24 15:12:41.664579 pytenzir-4.0.0rc9/pytenzir/apps/thehive.py
+-rw-r--r--   0        0        0       74 2023-07-24 15:12:41.664579 pytenzir-4.0.0rc9/pytenzir/tenzir/__init__.py
+-rw-r--r--   0        0        0     2913 2023-07-24 15:12:41.664579 pytenzir-4.0.0rc9/pytenzir/tenzir/cli.py
+-rw-r--r--   0        0        0     3657 2023-07-24 15:12:41.664579 pytenzir-4.0.0rc9/pytenzir/tenzir/convert.py
+-rw-r--r--   0        0        0     6170 2023-07-24 15:12:41.664579 pytenzir-4.0.0rc9/pytenzir/tenzir/tenzir.py
+-rw-r--r--   0        0        0     7461 2023-07-24 15:12:41.664579 pytenzir-4.0.0rc9/pytenzir/utils/arrow.py
+-rw-r--r--   0        0        0     2062 2023-07-24 15:12:41.664579 pytenzir-4.0.0rc9/pytenzir/utils/asyncio.py
+-rw-r--r--   0        0        0      740 2023-07-24 15:12:41.664579 pytenzir-4.0.0rc9/pytenzir/utils/config.py
+-rw-r--r--   0        0        0     1947 2023-07-24 15:12:41.664579 pytenzir-4.0.0rc9/pytenzir/utils/logging.py
+-rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 pytenzir-4.0.0rc9/setup.py
+-rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 pytenzir-4.0.0rc9/PKG-INFO
```

### Comparing `pytenzir-4.0.0rc12/README.md` & `pytenzir-4.0.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `pytenzir-4.0.0rc12/pyproject.toml` & `pytenzir-4.0.0rc9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytenzir"
-version = "4.0.0-rc12"
+version = "4.0.0-rc9"
 description = "A security telemetry engine for detection and response"
 authors = ["Tenzir <engineering@tenzir.com>"]
 maintainers = ["Tenzir <engineering@tenzir.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pytenzir-4.0.0rc12/pytenzir/apps/thehive.py` & `pytenzir-4.0.0rc9/pytenzir/apps/thehive.py`

 * *Files identical despite different names*

### Comparing `pytenzir-4.0.0rc12/pytenzir/tenzir/cli.py` & `pytenzir-4.0.0rc9/pytenzir/tenzir/cli.py`

 * *Files identical despite different names*

### Comparing `pytenzir-4.0.0rc12/pytenzir/tenzir/convert.py` & `pytenzir-4.0.0rc9/pytenzir/tenzir/convert.py`

 * *Files identical despite different names*

### Comparing `pytenzir-4.0.0rc12/pytenzir/tenzir/tenzir.py` & `pytenzir-4.0.0rc9/pytenzir/tenzir/tenzir.py`

 * *Files identical despite different names*

### Comparing `pytenzir-4.0.0rc12/pytenzir/utils/arrow.py` & `pytenzir-4.0.0rc9/pytenzir/utils/arrow.py`

 * *Files identical despite different names*

### Comparing `pytenzir-4.0.0rc12/pytenzir/utils/asyncio.py` & `pytenzir-4.0.0rc9/pytenzir/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `pytenzir-4.0.0rc12/pytenzir/utils/config.py` & `pytenzir-4.0.0rc9/pytenzir/utils/config.py`

 * *Files identical despite different names*

### Comparing `pytenzir-4.0.0rc12/pytenzir/utils/logging.py` & `pytenzir-4.0.0rc9/pytenzir/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pytenzir-4.0.0rc12/setup.py` & `pytenzir-4.0.0rc9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 entry_points = \
 {'console_scripts': ['app-thehive-count-alerts = '
                      'pytenzir.apps.thehive:count_alerts',
                      'app-thehive-run = pytenzir.apps.thehive:run']}
 
 setup_kwargs = {
     'name': 'pytenzir',
-    'version': '4.0.0rc12',
+    'version': '4.0.0rc9',
     'description': 'A security telemetry engine for detection and response',
     'long_description': '# Tenzir Python\n\nThe Python package of Tenzir provides a flexible control plane to integrate Tenzir\nwith other security tools.\n\n> **Note**\n> The Python effort is still highly experimental and subject to rapid change.\n> Please do not consider it for production use.\n\n## Usage\n\nTo get started, clone the Tenzir repository and install the Python package via\n[Poetry](https://python-poetry.org/docs/):\n\n```bash\ngit clone https://github.com/tenzir/tenzir.git\ncd tenzir/python\npoetry install\n```\n\n## Development\n\nWe recommend that you work with an editable installation, which is the default\nfor `poetry install`.\n\n### Unit Tests\n\nRun the unit tests via pytest:\n\n```bash\npoetry run pytest\n```\n\n### Integration Tests\n\nRun the integrations tests via Docker Compose and pytest:\n\n```bash\n./docker-poetry-run.sh pytest -v\n```\n\n## Packaging\n\nThe following instructions concern maintainers who want to publish the Python\npackage to PyPI.\n\n> **Note**\n> Our releasing scripts and CI run these steps automatically. You do not need to\n> intervene anywhere. The instructions below merely document the steps taken.\n\n### Bump the version\n\nPrior to releasing a new version, bump the version, e.g.:\n\n```bash\npoetry version 2.3.1\n```\n\nThis updates the `pyproject.toml` file.\n\n### Publish to Test PyPI\n\n1. Add a Test PyPi repository:\n\n   ```bash\n   poetry config repositories.test-pypi https://test.pypi.org/legacy/\n   ```\n\n2. Get the token from <https://test.pypi.org/manage/account/token/>.\n\n3. Store the token:\n\n  ```bash\n  poetry config pypi-token.test-pypi pypi-XXXXXXXX\n  ```\n\n4. Publish:\n  \n   ```bash\n   poetry publish --build -r test-pypi\n   ```\n\n### Publish to PyPI\n\n1. Get the token from <https://pypi.org/manage/account/token/>.\n\n2. Store the token:\n\n  ```bash\n  poetry config pypi-token.pypi pypi-XXXXXXXX\n  ```\n\n3. Publish\n\n   ```bash\n   poetry publish --build\n   ```\n',
     'author': 'Tenzir',
     'author_email': 'engineering@tenzir.com',
     'maintainer': 'Tenzir',
     'maintainer_email': 'engineering@tenzir.com',
     'url': 'https://tenzir.com',
```

### Comparing `pytenzir-4.0.0rc12/PKG-INFO` & `pytenzir-4.0.0rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytenzir
-Version: 4.0.0rc12
+Version: 4.0.0rc9
 Summary: A security telemetry engine for detection and response
 Home-page: https://tenzir.com
 License: BSD-3-Clause
 Author: Tenzir
 Author-email: engineering@tenzir.com
 Maintainer: Tenzir
 Maintainer-email: engineering@tenzir.com
```

