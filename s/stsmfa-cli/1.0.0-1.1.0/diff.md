# Comparing `tmp/stsmfa_cli-1.0.0.tar.gz` & `tmp/stsmfa_cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stsmfa_cli-1.0.0.tar", max compression
+gzip compressed data, was "stsmfa_cli-1.1.0.tar", max compression
```

## Comparing `stsmfa_cli-1.0.0.tar` & `stsmfa_cli-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-06-27 11:13:20.585278 stsmfa_cli-1.0.0/LICENSE
--rw-r--r--   0        0        0     4969 2023-06-27 11:13:20.585278 stsmfa_cli-1.0.0/README.md
--rw-r--r--   0        0        0     2093 2023-06-27 11:13:21.461276 stsmfa_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-27 11:13:21.425276 stsmfa_cli-1.0.0/src/stsmfa/__init__.py
--rw-r--r--   0        0        0       59 2023-06-27 11:13:20.589278 stsmfa_cli-1.0.0/src/stsmfa/__maIn__.py
--rw-r--r--   0        0        0     2036 2023-06-27 11:13:20.589278 stsmfa_cli-1.0.0/src/stsmfa/cli.py
--rw-r--r--   0        0        0        0 2023-06-27 11:13:20.589278 stsmfa_cli-1.0.0/src/stsmfa/py.typed
--rw-r--r--   0        0        0     6169 1970-01-01 00:00:00.000000 stsmfa_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-07 15:13:27.079918 stsmfa_cli-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4969 2023-08-07 15:13:27.079918 stsmfa_cli-1.1.0/README.md
+-rw-r--r--   0        0        0     2307 2023-08-07 15:13:28.507931 stsmfa_cli-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-08-07 15:13:27.079918 stsmfa_cli-1.1.0/src/stsmfa/__init__.py
+-rw-r--r--   0        0        0       59 2023-08-07 15:13:27.079918 stsmfa_cli-1.1.0/src/stsmfa/__maIn__.py
+-rw-r--r--   0        0        0     2036 2023-08-07 15:13:27.079918 stsmfa_cli-1.1.0/src/stsmfa/cli.py
+-rw-r--r--   0        0        0        0 2023-08-07 15:13:27.079918 stsmfa_cli-1.1.0/src/stsmfa/py.typed
+-rw-r--r--   0        0        0     6220 1970-01-01 00:00:00.000000 stsmfa_cli-1.1.0/PKG-INFO
```

### Comparing `stsmfa_cli-1.0.0/LICENSE` & `stsmfa_cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stsmfa_cli-1.0.0/README.md` & `stsmfa_cli-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `stsmfa_cli-1.0.0/pyproject.toml` & `stsmfa_cli-1.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "stsmfa-cli"
-version = "1.0.0"
+version = "1.1.0"
 description = "A small CLI to help with creating AWS profile for MFA protected sessions"
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/stsmfa-cli"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
+    "Programming Language :: Python :: 3.12",
 ]
 packages = [
     { include = "stsmfa", from = "src" },
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/browniebroke/stsmfa-cli/issues"
@@ -34,18 +35,27 @@
 pytest = "^7.0"
 pytest-cov = "^4.0"
 pyfakefs = "^5.0.0"
 pytest-mock = "^3.10.0"
 
 [tool.semantic_release]
 branch = "main"
-version_toml = "pyproject.toml:tool.poetry.version"
+version_toml = ["pyproject.toml:tool.poetry.version"]
 version_variable = "src/stsmfa/__init__.py:__version__"
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
 addopts = "-v -Wdefault --cov=stsmfa --cov-report=term-missing:skip-covered"
 pythonpath = ["src"]
 
 [tool.coverage.run]
 branch = true
 omit = [
```

### Comparing `stsmfa_cli-1.0.0/src/stsmfa/cli.py` & `stsmfa_cli-1.1.0/src/stsmfa/cli.py`

 * *Files identical despite different names*

### Comparing `stsmfa_cli-1.0.0/PKG-INFO` & `stsmfa_cli-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stsmfa-cli
-Version: 1.0.0
+Version: 1.1.0
 Summary: A small CLI to help with creating AWS profile for MFA protected sessions
 Home-page: https://github.com/browniebroke/stsmfa-cli
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
 Requires-Dist: boto3 (>=1.26,<2.0)
 Requires-Dist: rich (>=10.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/browniebroke/stsmfa-cli/issues
 Project-URL: Changelog, https://github.com/browniebroke/stsmfa-cli/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/browniebroke/stsmfa-cli
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: stsmfa-cli Version: 1.0.0 Summary: A small CLI to
+Metadata-Version: 2.1 Name: stsmfa-cli Version: 1.1.0 Summary: A small CLI to
 help with creating AWS profile for MFA protected sessions Home-page: https://
 github.com/browniebroke/stsmfa-cli License: MIT Author: Bruno Alla Author-
 email: alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
-Dist: boto3 (>=1.26,<2.0) Requires-Dist: rich (>=10.0) Requires-Dist: typer
-(>=0.9.0,<0.10.0) Project-URL: Bug Tracker, https://github.com/browniebroke/
-stsmfa-cli/issues Project-URL: Changelog, https://github.com/browniebroke/
-stsmfa-cli/blob/main/CHANGELOG.md Project-URL: Repository, https://github.com/
-browniebroke/stsmfa-cli Description-Content-Type: text/markdown # STS MFA CLI
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Topic :: Software Development :: Libraries Requires-Dist: boto3 (>=1.26,<2.0)
+Requires-Dist: rich (>=10.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Project-
+URL: Bug Tracker, https://github.com/browniebroke/stsmfa-cli/issues Project-
+URL: Changelog, https://github.com/browniebroke/stsmfa-cli/blob/main/
+CHANGELOG.md Project-URL: Repository, https://github.com/browniebroke/stsmfa-
+cli Description-Content-Type: text/markdown # STS MFA CLI
                     [CI_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 Creating temporary profiles for multi-factor auth (MFA) protected accounts
 using AWS STS is too hard. This is a small CLI that helps with that. ##
 Installation Via Homebrew: ```bash brew install browniebroke/tap/stsmfa-cli ```
 Via pip, pipx, or your favourite Python package manager: ```bash pip install
```

