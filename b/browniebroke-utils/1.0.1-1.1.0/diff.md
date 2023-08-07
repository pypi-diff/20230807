# Comparing `tmp/browniebroke_utils-1.0.1.tar.gz` & `tmp/browniebroke_utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browniebroke_utils-1.0.1.tar", max compression
+gzip compressed data, was "browniebroke_utils-1.1.0.tar", max compression
```

## Comparing `browniebroke_utils-1.0.1.tar` & `browniebroke_utils-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/LICENSE
--rw-r--r--   0        0        0     4519 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/README.md
--rw-r--r--   0        0        0     2196 2023-07-19 11:30:20.446077 browniebroke_utils-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/src/browniebroke_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/src/browniebroke_utils/py.typed
--rw-r--r--   0        0        0     1106 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/src/browniebroke_utils/setup_prettier.py
--rw-r--r--   0        0        0      343 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/src/browniebroke_utils/setup_pywatchers.py
--rw-r--r--   0        0        0      264 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/src/browniebroke_utils/templates/prettier/prettier.xml
--rw-r--r--   0        0        0      449 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/src/browniebroke_utils/templates/prettier/to_add.xml
--rw-r--r--   0        0        0     2731 2023-07-19 11:30:19.634081 browniebroke_utils-1.0.1/src/browniebroke_utils/templates/pywatchers/watchers.xml
--rw-r--r--   0        0        0     5771 1970-01-01 00:00:00.000000 browniebroke_utils-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-07 14:56:59.766009 browniebroke_utils-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4519 2023-08-07 14:56:59.766009 browniebroke_utils-1.1.0/README.md
+-rw-r--r--   0        0        0     2408 2023-08-07 14:57:00.918121 browniebroke_utils-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-08-07 14:56:59.766009 browniebroke_utils-1.1.0/src/browniebroke_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:56:59.766009 browniebroke_utils-1.1.0/src/browniebroke_utils/py.typed
+-rw-r--r--   0        0        0     1106 2023-08-07 14:56:59.766009 browniebroke_utils-1.1.0/src/browniebroke_utils/setup_prettier.py
+-rw-r--r--   0        0        0      343 2023-08-07 14:56:59.766009 browniebroke_utils-1.1.0/src/browniebroke_utils/setup_pywatchers.py
+-rw-r--r--   0        0        0      264 2023-08-07 14:56:59.766009 browniebroke_utils-1.1.0/src/browniebroke_utils/templates/prettier/prettier.xml
+-rw-r--r--   0        0        0      449 2023-08-07 14:56:59.766009 browniebroke_utils-1.1.0/src/browniebroke_utils/templates/prettier/to_add.xml
+-rw-r--r--   0        0        0     2731 2023-08-07 14:56:59.766009 browniebroke_utils-1.1.0/src/browniebroke_utils/templates/pywatchers/watchers.xml
+-rw-r--r--   0        0        0     5822 1970-01-01 00:00:00.000000 browniebroke_utils-1.1.0/PKG-INFO
```

### Comparing `browniebroke_utils-1.0.1/LICENSE` & `browniebroke_utils-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `browniebroke_utils-1.0.1/README.md` & `browniebroke_utils-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `browniebroke_utils-1.0.1/pyproject.toml` & `browniebroke_utils-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "browniebroke-utils"
-version = "1.0.1"
+version = "1.1.0"
 description = "A collections of small scripts."
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/browniebroke-utils"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
+    "Programming Language :: Python :: 3.12",
 ]
 packages = [
     { include = "browniebroke_utils", from = "src" },
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/browniebroke/browniebroke-utils/issues"
@@ -38,14 +39,23 @@
 
 [tool.semantic_release]
 branch = "main"
 version_toml = ["pyproject.toml:tool.poetry.version"]
 version_variable = "src/browniebroke_utils/__init__.py:__version__"
 build_command = "pip install poetry && poetry build"
 
+[tool.semantic_release.changelog]
+exclude_commit_patterns = [
+    "chore*",
+    "ci*",
+]
+
+[tool.semantic_release.changelog.environment]
+keep_trailing_newline = true
+
 [tool.pytest.ini_options]
 addopts = "-v -Wdefault --cov=browniebroke_utils --cov-report=term-missing:skip-covered"
 pythonpath = ["src"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `browniebroke_utils-1.0.1/src/browniebroke_utils/setup_prettier.py` & `browniebroke_utils-1.1.0/src/browniebroke_utils/setup_prettier.py`

 * *Files identical despite different names*

### Comparing `browniebroke_utils-1.0.1/src/browniebroke_utils/templates/pywatchers/watchers.xml` & `browniebroke_utils-1.1.0/src/browniebroke_utils/templates/pywatchers/watchers.xml`

 * *Files identical despite different names*

### Comparing `browniebroke_utils-1.0.1/PKG-INFO` & `browniebroke_utils-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browniebroke-utils
-Version: 1.0.1
+Version: 1.1.0
 Summary: A collections of small scripts.
 Home-page: https://github.com/browniebroke/browniebroke-utils
 License: MIT
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,14 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Bug Tracker, https://github.com/browniebroke/browniebroke-utils/issues
 Project-URL: Changelog, https://github.com/browniebroke/browniebroke-utils/blob/main/CHANGELOG.md
 Project-URL: Mastodon, https://fosstodon.org/@browniebroke
 Project-URL: Repository, https://github.com/browniebroke/browniebroke-utils
 Project-URL: Twitter, https://twitter.com/_BrunoAlla
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: browniebroke-utils Version: 1.0.1 Summary: A
+Metadata-Version: 2.1 Name: browniebroke-utils Version: 1.1.0 Summary: A
 collections of small scripts. Home-page: https://github.com/browniebroke/
 browniebroke-utils License: MIT Author: Bruno Alla Author-email:
 alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Topic :: Software Development :: Libraries Requires-Dist: xmltodict
-(>=0.13.0,<0.14.0) Project-URL: Bug Tracker, https://github.com/browniebroke/
-browniebroke-utils/issues Project-URL: Changelog, https://github.com/
-browniebroke/browniebroke-utils/blob/main/CHANGELOG.md Project-URL: Mastodon,
-https://fosstodon.org/@browniebroke Project-URL: Repository, https://
-github.com/browniebroke/browniebroke-utils Project-URL: Twitter, https://
-twitter.com/_BrunoAlla Description-Content-Type: text/markdown # Browniebroke
-Utils
+Programming Language :: Python :: 3.12 Classifier: Topic :: Software
+Development :: Libraries Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-
+URL: Bug Tracker, https://github.com/browniebroke/browniebroke-utils/issues
+Project-URL: Changelog, https://github.com/browniebroke/browniebroke-utils/
+blob/main/CHANGELOG.md Project-URL: Mastodon, https://fosstodon.org/
+@browniebroke Project-URL: Repository, https://github.com/browniebroke/
+browniebroke-utils Project-URL: Twitter, https://twitter.com/_BrunoAlla
+Description-Content-Type: text/markdown # Browniebroke Utils
                     [CI_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 A collections of small scripts. ## Installation Install this via pip (or your
 favourite package manager): `pip install browniebroke-utils` ## Usage This tool
 provides a few random scripts I use in my day to day work. ### `pych-prettier`
 Configure [Prettier](https://prettier.io/) as file watcher in the current
```

