# Comparing `tmp/all_repos_envvar-1.0.0.tar.gz` & `tmp/all_repos_envvar-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "all_repos_envvar-1.0.0.tar", max compression
+gzip compressed data, was "all_repos_envvar-1.1.0.tar", max compression
```

## Comparing `all_repos_envvar-1.0.0.tar` & `all_repos_envvar-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-06-27 11:39:30.286209 all_repos_envvar-1.0.0/LICENSE
--rw-r--r--   0        0        0     4782 2023-06-27 11:39:30.286209 all_repos_envvar-1.0.0/README.md
--rw-r--r--   0        0        0     2072 2023-06-27 11:39:31.526219 all_repos_envvar-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-27 11:39:31.486219 all_repos_envvar-1.0.0/src/all_repos_envvar/__init__.py
--rw-r--r--   0        0        0      485 2023-06-27 11:39:30.286209 all_repos_envvar-1.0.0/src/all_repos_envvar/mixin.py
--rw-r--r--   0        0        0      167 2023-06-27 11:39:30.286209 all_repos_envvar-1.0.0/src/all_repos_envvar/push.py
--rw-r--r--   0        0        0        0 2023-06-27 11:39:30.286209 all_repos_envvar-1.0.0/src/all_repos_envvar/py.typed
--rw-r--r--   0        0        0      168 2023-06-27 11:39:30.286209 all_repos_envvar-1.0.0/src/all_repos_envvar/source.py
--rw-r--r--   0        0        0     6134 1970-01-01 00:00:00.000000 all_repos_envvar-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-07 14:53:54.165517 all_repos_envvar-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4782 2023-08-07 14:53:54.165517 all_repos_envvar-1.1.0/README.md
+-rw-r--r--   0        0        0     2286 2023-08-07 14:53:55.029509 all_repos_envvar-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-08-07 14:53:54.165517 all_repos_envvar-1.1.0/src/all_repos_envvar/__init__.py
+-rw-r--r--   0        0        0      485 2023-08-07 14:53:54.165517 all_repos_envvar-1.1.0/src/all_repos_envvar/mixin.py
+-rw-r--r--   0        0        0      167 2023-08-07 14:53:54.165517 all_repos_envvar-1.1.0/src/all_repos_envvar/push.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:53:54.165517 all_repos_envvar-1.1.0/src/all_repos_envvar/py.typed
+-rw-r--r--   0        0        0      168 2023-08-07 14:53:54.165517 all_repos_envvar-1.1.0/src/all_repos_envvar/source.py
+-rw-r--r--   0        0        0     6185 1970-01-01 00:00:00.000000 all_repos_envvar-1.1.0/PKG-INFO
```

### Comparing `all_repos_envvar-1.0.0/LICENSE` & `all_repos_envvar-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `all_repos_envvar-1.0.0/README.md` & `all_repos_envvar-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `all_repos_envvar-1.0.0/pyproject.toml` & `all_repos_envvar-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "all-repos-envvar"
-version = "1.0.0"
+version = "1.1.0"
 description = "An all-repos extension to read values from environment variables."
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/all-repos-envvar"
 documentation = "https://all-repos-envvar.readthedocs.io"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
+    "Programming Language :: Python :: 3.12",
 ]
 packages = [
     { include = "all_repos_envvar", from = "src" },
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/browniebroke/all-repos-envvar/issues"
@@ -31,18 +32,27 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.0"
 
 [tool.semantic_release]
 branch = "main"
-version_toml = "pyproject.toml:tool.poetry.version"
+version_toml = ["pyproject.toml:tool.poetry.version"]
 version_variable = "src/all_repos_envvar/__init__.py:__version__"
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
 addopts = "-v -Wdefault --cov=all_repos_envvar --cov-report=term-missing:skip-covered"
 pythonpath = ["src"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `all_repos_envvar-1.0.0/PKG-INFO` & `all_repos_envvar-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: all-repos-envvar
-Version: 1.0.0
+Version: 1.1.0
 Summary: An all-repos extension to read values from environment variables.
 Home-page: https://github.com/browniebroke/all-repos-envvar
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
 Requires-Dist: all-repos (>=1)
 Requires-Dist: environs (>=9.4,<10.0)
 Project-URL: Bug Tracker, https://github.com/browniebroke/all-repos-envvar/issues
 Project-URL: Changelog, https://all-repos-envvar.readthedocs.io/changelog.html
 Project-URL: Documentation, https://all-repos-envvar.readthedocs.io
 Project-URL: Mastodon, https://fosstodon.org/@browniebroke
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: all-repos-envvar Version: 1.0.0 Summary: An all-
+Metadata-Version: 2.1 Name: all-repos-envvar Version: 1.1.0 Summary: An all-
 repos extension to read values from environment variables. Home-page: https://
 github.com/browniebroke/all-repos-envvar License: MIT Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
-Dist: all-repos (>=1) Requires-Dist: environs (>=9.4,<10.0) Project-URL: Bug
-Tracker, https://github.com/browniebroke/all-repos-envvar/issues Project-URL:
-Changelog, https://all-repos-envvar.readthedocs.io/changelog.html Project-URL:
-Documentation, https://all-repos-envvar.readthedocs.io Project-URL: Mastodon,
-https://fosstodon.org/@browniebroke Project-URL: Repository, https://
-github.com/browniebroke/all-repos-envvar Project-URL: Twitter, https://
-twitter.com/_BrunoAlla Description-Content-Type: text/markdown # all-repos-
-envvar
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Topic :: Software Development :: Libraries Requires-Dist: all-repos (>=1)
+Requires-Dist: environs (>=9.4,<10.0) Project-URL: Bug Tracker, https://
+github.com/browniebroke/all-repos-envvar/issues Project-URL: Changelog, https:/
+/all-repos-envvar.readthedocs.io/changelog.html Project-URL: Documentation,
+https://all-repos-envvar.readthedocs.io Project-URL: Mastodon, https://
+fosstodon.org/@browniebroke Project-URL: Repository, https://github.com/
+browniebroke/all-repos-envvar Project-URL: Twitter, https://twitter.com/
+_BrunoAlla Description-Content-Type: text/markdown # all-repos-envvar
                     [CI_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 An all-repos extension to read values from environment variables. ##
 Installation Install this via pip (or your favourite package manager): `pip
 install all-repos-envvar` ## Usage This library should be installed alongside
 `all-repos` so that it's findable at import time. It provides a custom `source`
```

