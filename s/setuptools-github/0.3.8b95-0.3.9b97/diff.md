# Comparing `tmp/setuptools-github-0.3.8b95.tar.gz` & `tmp/setuptools-github-0.3.9b97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.8b95.tar", last modified: Mon Aug  7 19:54:48 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.9b97.tar", last modified: Mon Aug  7 20:18:19 2023, max compression
```

## Comparing `setuptools-github-0.3.8b95.tar` & `setuptools-github-0.3.9b97.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:54:48.906384 setuptools-github-0.3.8b95/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-08-07 19:54:48.906384 setuptools-github-0.3.8b95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-08-07 19:54:48.000000 setuptools-github-0.3.8b95/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:54:48.906384 setuptools-github-0.3.8b95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:54:48.906384 setuptools-github-0.3.8b95/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-08-07 19:54:48.000000 setuptools-github-0.3.8b95/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-07 19:54:48.000000 setuptools-github-0.3.8b95/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:54:48.000000 setuptools-github-0.3.8b95/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-07 19:54:48.000000 setuptools-github-0.3.8b95/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-07 19:54:48.000000 setuptools-github-0.3.8b95/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 19:54:48.000000 setuptools-github-0.3.8b95/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:54:48.902383 setuptools-github-0.3.8b95/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:54:48.906384 setuptools-github-0.3.8b95/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-07 19:54:48.000000 setuptools-github-0.3.8b95/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9581 2023-08-07 19:54:48.000000 setuptools-github-0.3.8b95/src/setuptools_github/_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:54:48.906384 setuptools-github-0.3.8b95/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-08-07 19:54:12.000000 setuptools-github-0.3.8b95/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:18:19.096397 setuptools-github-0.3.9b97/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-08-07 20:18:19.096397 setuptools-github-0.3.9b97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-08-07 20:18:19.000000 setuptools-github-0.3.9b97/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 20:18:19.096397 setuptools-github-0.3.9b97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:18:19.096397 setuptools-github-0.3.9b97/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-08-07 20:18:19.000000 setuptools-github-0.3.9b97/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-07 20:18:19.000000 setuptools-github-0.3.9b97/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:18:19.000000 setuptools-github-0.3.9b97/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-07 20:18:19.000000 setuptools-github-0.3.9b97/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-07 20:18:19.000000 setuptools-github-0.3.9b97/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 20:18:19.000000 setuptools-github-0.3.9b97/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:18:19.092397 setuptools-github-0.3.9b97/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:18:19.096397 setuptools-github-0.3.9b97/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-07 20:18:19.000000 setuptools-github-0.3.9b97/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-08-07 20:18:19.000000 setuptools-github-0.3.9b97/src/setuptools_github/_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:18:19.096397 setuptools-github-0.3.9b97/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-08-07 20:17:34.000000 setuptools-github-0.3.9b97/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.8b95/LICENSE` & `setuptools-github-0.3.9b97/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.8b95/PKG-INFO` & `setuptools-github-0.3.9b97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.8b95
+Version: 0.3.9b97
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,16 +19,16 @@
 
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5789315544)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.8/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.8)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5789514622)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.9/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.9)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
```

### Comparing `setuptools-github-0.3.8b95/README.md` & `setuptools-github-0.3.9b97/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5789315544)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.8/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.8)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5789514622)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.9/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.9)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
```

### Comparing `setuptools-github-0.3.8b95/pyproject.toml` & `setuptools-github-0.3.9b97/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.8b95/setup.py` & `setuptools-github-0.3.9b97/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.8b95/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.9b97/setuptools_github.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.8b95
+Version: 0.3.9b97
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,16 +19,16 @@
 
 # setuptools-github
 
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
-[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5789315544)
-[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.8/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.8)
+[![Build](https://github.com/cav71/setuptools-github/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions/runs/5789514622)
+[![Codecov](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.9/graph/badge.svg?token=SIUMZ7MT5T)](https://codecov.io/gh/cav71/setuptools-github/tree/beta%2F0.3.9)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 ## Quick start
```

### Comparing `setuptools-github-0.3.8b95/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.9b97/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.8b95/src/setuptools_github/_build.py` & `setuptools-github-0.3.9b97/src/setuptools_github/_build.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,42 +3,42 @@
 action_ref = ''
 action_repository = ''
 actor = 'cav71'
 actor_id = '2042971'
 api_url = 'https://api.github.com'
 artifact_cache_size_limit = '10'
 base_ref = ''
-env = '/home/runner/work/_temp/_runner_file_commands/set_env_5f68d7fb-9e6d-47de-89bc-b42527cb350c'
-event = {'after': '9df889992f422a62cdd3ced41323eaba6e855ae3', 'base_ref': 'refs/heads/master', 'before': '139bd7e4c7b88052101b1a8524e68249b8fe8935', 'commits': [{'author': {'email': 'a.cavallo@cavallinux.eu', 'name': 'antonio', 'username': 'cav71'}, 'committer': {'email': 'a.cavallo@cavallinux.eu', 'name': 'antonio', 'username': 'cav71'}, 'distinct': False, 'id': '9df889992f422a62cdd3ced41323eaba6e855ae3', 'message': 'fix test', 'timestamp': '2023-08-07T21:53:39+02:00', 'tree_id': '3b1d92038f5d9c6eff69adb078dfcf4454d12466', 'url': 'https://github.com/cav71/setuptools-github/commit/9df889992f422a62cdd3ced41323eaba6e855ae3'}], 'compare': 'https://github.com/cav71/setuptools-github/compare/139bd7e4c7b8...9df889992f42', 'created': False, 'deleted': False, 'forced': False, 'head_commit': {'author': {'email': 'a.cavallo@cavallinux.eu', 'name': 'antonio', 'username': 'cav71'}, 'committer': {'email': 'a.cavallo@cavallinux.eu', 'name': 'antonio', 'username': 'cav71'}, 'distinct': False, 'id': '9df889992f422a62cdd3ced41323eaba6e855ae3', 'message': 'fix test', 'timestamp': '2023-08-07T21:53:39+02:00', 'tree_id': '3b1d92038f5d9c6eff69adb078dfcf4454d12466', 'url': 'https://github.com/cav71/setuptools-github/commit/9df889992f422a62cdd3ced41323eaba6e855ae3'}, 'pusher': {'email': 'a.cavallo@cavallinux.eu', 'name': 'cav71'}, 'ref': 'refs/heads/beta/0.3.8', 'repository': {'allow_forking': True, 'archive_url': 'https://api.github.com/repos/cav71/setuptools-github/{archive_format}{/ref}', 'archived': False, 'assignees_url': 'https://api.github.com/repos/cav71/setuptools-github/assignees{/user}', 'blobs_url': 'https://api.github.com/repos/cav71/setuptools-github/git/blobs{/sha}', 'branches_url': 'https://api.github.com/repos/cav71/setuptools-github/branches{/branch}', 'clone_url': 'https://github.com/cav71/setuptools-github.git', 'collaborators_url': 'https://api.github.com/repos/cav71/setuptools-github/collaborators{/collaborator}', 'comments_url': 'https://api.github.com/repos/cav71/setuptools-github/comments{/number}', 'commits_url': 'https://api.github.com/repos/cav71/setuptools-github/commits{/sha}', 'compare_url': 'https://api.github.com/repos/cav71/setuptools-github/compare/{base}...{head}', 'contents_url': 'https://api.github.com/repos/cav71/setuptools-github/contents/{+path}', 'contributors_url': 'https://api.github.com/repos/cav71/setuptools-github/contributors', 'created_at': 1631538103, 'default_branch': 'master', 'deployments_url': 'https://api.github.com/repos/cav71/setuptools-github/deployments', 'description': 'hooks to support github deployment', 'disabled': False, 'downloads_url': 'https://api.github.com/repos/cav71/setuptools-github/downloads', 'events_url': 'https://api.github.com/repos/cav71/setuptools-github/events', 'fork': False, 'forks': 0, 'forks_count': 0, 'forks_url': 'https://api.github.com/repos/cav71/setuptools-github/forks', 'full_name': 'cav71/setuptools-github', 'git_commits_url': 'https://api.github.com/repos/cav71/setuptools-github/git/commits{/sha}', 'git_refs_url': 'https://api.github.com/repos/cav71/setuptools-github/git/refs{/sha}', 'git_tags_url': 'https://api.github.com/repos/cav71/setuptools-github/git/tags{/sha}', 'git_url': 'git://github.com/cav71/setuptools-github.git', 'has_discussions': False, 'has_downloads': True, 'has_issues': True, 'has_pages': False, 'has_projects': True, 'has_wiki': True, 'homepage': None, 'hooks_url': 'https://api.github.com/repos/cav71/setuptools-github/hooks', 'html_url': 'https://github.com/cav71/setuptools-github', 'id': 405975487, 'is_template': False, 'issue_comment_url': 'https://api.github.com/repos/cav71/setuptools-github/issues/comments{/number}', 'issue_events_url': 'https://api.github.com/repos/cav71/setuptools-github/issues/events{/number}', 'issues_url': 'https://api.github.com/repos/cav71/setuptools-github/issues{/number}', 'keys_url': 'https://api.github.com/repos/cav71/setuptools-github/keys{/key_id}', 'labels_url': 'https://api.github.com/repos/cav71/setuptools-github/labels{/name}', 'language': 'Python', 'languages_url': 'https://api.github.com/repos/cav71/setuptools-github/languages', 'license': {'key': 'bsd-2-clause', 'name': 'BSD 2-Clause "Simplified" License', 'node_id': 'MDc6TGljZW5zZTQ=', 'spdx_id': 'BSD-2-Clause', 'url': 'https://api.github.com/licenses/bsd-2-clause'}, 'master_branch': 'master', 'merges_url': 'https://api.github.com/repos/cav71/setuptools-github/merges', 'milestones_url': 'https://api.github.com/repos/cav71/setuptools-github/milestones{/number}', 'mirror_url': None, 'name': 'setuptools-github', 'node_id': 'MDEwOlJlcG9zaXRvcnk0MDU5NzU0ODc=', 'notifications_url': 'https://api.github.com/repos/cav71/setuptools-github/notifications{?since,all,participating}', 'open_issues': 1, 'open_issues_count': 1, 'owner': {'avatar_url': 'https://avatars.githubusercontent.com/u/2042971?v=4', 'email': 'a.cavallo@cavallinux.eu', 'events_url': 'https://api.github.com/users/cav71/events{/privacy}', 'followers_url': 'https://api.github.com/users/cav71/followers', 'following_url': 'https://api.github.com/users/cav71/following{/other_user}', 'gists_url': 'https://api.github.com/users/cav71/gists{/gist_id}', 'gravatar_id': '', 'html_url': 'https://github.com/cav71', 'id': 2042971, 'login': 'cav71', 'name': 'cav71', 'node_id': 'MDQ6VXNlcjIwNDI5NzE=', 'organizations_url': 'https://api.github.com/users/cav71/orgs', 'received_events_url': 'https://api.github.com/users/cav71/received_events', 'repos_url': 'https://api.github.com/users/cav71/repos', 'site_admin': False, 'starred_url': 'https://api.github.com/users/cav71/starred{/owner}{/repo}', 'subscriptions_url': 'https://api.github.com/users/cav71/subscriptions', 'type': 'User', 'url': 'https://api.github.com/users/cav71'}, 'private': False, 'pulls_url': 'https://api.github.com/repos/cav71/setuptools-github/pulls{/number}', 'pushed_at': 1691438040, 'releases_url': 'https://api.github.com/repos/cav71/setuptools-github/releases{/id}', 'size': 361, 'ssh_url': 'git@github.com:cav71/setuptools-github.git', 'stargazers': 0, 'stargazers_count': 0, 'stargazers_url': 'https://api.github.com/repos/cav71/setuptools-github/stargazers', 'statuses_url': 'https://api.github.com/repos/cav71/setuptools-github/statuses/{sha}', 'subscribers_url': 'https://api.github.com/repos/cav71/setuptools-github/subscribers', 'subscription_url': 'https://api.github.com/repos/cav71/setuptools-github/subscription', 'svn_url': 'https://github.com/cav71/setuptools-github', 'tags_url': 'https://api.github.com/repos/cav71/setuptools-github/tags', 'teams_url': 'https://api.github.com/repos/cav71/setuptools-github/teams', 'topics': [], 'trees_url': 'https://api.github.com/repos/cav71/setuptools-github/git/trees{/sha}', 'updated_at': '2022-01-04T18:09:04Z', 'url': 'https://github.com/cav71/setuptools-github', 'visibility': 'public', 'watchers': 0, 'watchers_count': 0, 'web_commit_signoff_required': False}, 'sender': {'avatar_url': 'https://avatars.githubusercontent.com/u/2042971?v=4', 'events_url': 'https://api.github.com/users/cav71/events{/privacy}', 'followers_url': 'https://api.github.com/users/cav71/followers', 'following_url': 'https://api.github.com/users/cav71/following{/other_user}', 'gists_url': 'https://api.github.com/users/cav71/gists{/gist_id}', 'gravatar_id': '', 'html_url': 'https://github.com/cav71', 'id': 2042971, 'login': 'cav71', 'node_id': 'MDQ6VXNlcjIwNDI5NzE=', 'organizations_url': 'https://api.github.com/users/cav71/orgs', 'received_events_url': 'https://api.github.com/users/cav71/received_events', 'repos_url': 'https://api.github.com/users/cav71/repos', 'site_admin': False, 'starred_url': 'https://api.github.com/users/cav71/starred{/owner}{/repo}', 'subscriptions_url': 'https://api.github.com/users/cav71/subscriptions', 'type': 'User', 'url': 'https://api.github.com/users/cav71'}}
+env = '/home/runner/work/_temp/_runner_file_commands/set_env_5d7ccf4b-2e2e-4c3a-aa0c-5f7a543a07cc'
+event = {'after': '971cde0beef9e5a64cc43d51e9f2259b5c878f75', 'base_ref': 'refs/heads/master', 'before': '26138d18892737a60b939fd3203c9fba05b2416a', 'commits': [{'author': {'email': 'a.cavallo@cavallinux.eu', 'name': 'antonio', 'username': 'cav71'}, 'committer': {'email': 'a.cavallo@cavallinux.eu', 'name': 'antonio', 'username': 'cav71'}, 'distinct': False, 'id': '971cde0beef9e5a64cc43d51e9f2259b5c878f75', 'message': 'fix', 'timestamp': '2023-08-07T22:16:51+02:00', 'tree_id': '4ada180449617cc4fe5e6dc3b15abd5b5b93810c', 'url': 'https://github.com/cav71/setuptools-github/commit/971cde0beef9e5a64cc43d51e9f2259b5c878f75'}], 'compare': 'https://github.com/cav71/setuptools-github/compare/26138d188927...971cde0beef9', 'created': False, 'deleted': False, 'forced': False, 'head_commit': {'author': {'email': 'a.cavallo@cavallinux.eu', 'name': 'antonio', 'username': 'cav71'}, 'committer': {'email': 'a.cavallo@cavallinux.eu', 'name': 'antonio', 'username': 'cav71'}, 'distinct': False, 'id': '971cde0beef9e5a64cc43d51e9f2259b5c878f75', 'message': 'fix', 'timestamp': '2023-08-07T22:16:51+02:00', 'tree_id': '4ada180449617cc4fe5e6dc3b15abd5b5b93810c', 'url': 'https://github.com/cav71/setuptools-github/commit/971cde0beef9e5a64cc43d51e9f2259b5c878f75'}, 'pusher': {'email': 'a.cavallo@cavallinux.eu', 'name': 'cav71'}, 'ref': 'refs/heads/beta/0.3.9', 'repository': {'allow_forking': True, 'archive_url': 'https://api.github.com/repos/cav71/setuptools-github/{archive_format}{/ref}', 'archived': False, 'assignees_url': 'https://api.github.com/repos/cav71/setuptools-github/assignees{/user}', 'blobs_url': 'https://api.github.com/repos/cav71/setuptools-github/git/blobs{/sha}', 'branches_url': 'https://api.github.com/repos/cav71/setuptools-github/branches{/branch}', 'clone_url': 'https://github.com/cav71/setuptools-github.git', 'collaborators_url': 'https://api.github.com/repos/cav71/setuptools-github/collaborators{/collaborator}', 'comments_url': 'https://api.github.com/repos/cav71/setuptools-github/comments{/number}', 'commits_url': 'https://api.github.com/repos/cav71/setuptools-github/commits{/sha}', 'compare_url': 'https://api.github.com/repos/cav71/setuptools-github/compare/{base}...{head}', 'contents_url': 'https://api.github.com/repos/cav71/setuptools-github/contents/{+path}', 'contributors_url': 'https://api.github.com/repos/cav71/setuptools-github/contributors', 'created_at': 1631538103, 'default_branch': 'master', 'deployments_url': 'https://api.github.com/repos/cav71/setuptools-github/deployments', 'description': 'hooks to support github deployment', 'disabled': False, 'downloads_url': 'https://api.github.com/repos/cav71/setuptools-github/downloads', 'events_url': 'https://api.github.com/repos/cav71/setuptools-github/events', 'fork': False, 'forks': 0, 'forks_count': 0, 'forks_url': 'https://api.github.com/repos/cav71/setuptools-github/forks', 'full_name': 'cav71/setuptools-github', 'git_commits_url': 'https://api.github.com/repos/cav71/setuptools-github/git/commits{/sha}', 'git_refs_url': 'https://api.github.com/repos/cav71/setuptools-github/git/refs{/sha}', 'git_tags_url': 'https://api.github.com/repos/cav71/setuptools-github/git/tags{/sha}', 'git_url': 'git://github.com/cav71/setuptools-github.git', 'has_discussions': False, 'has_downloads': True, 'has_issues': True, 'has_pages': False, 'has_projects': True, 'has_wiki': True, 'homepage': None, 'hooks_url': 'https://api.github.com/repos/cav71/setuptools-github/hooks', 'html_url': 'https://github.com/cav71/setuptools-github', 'id': 405975487, 'is_template': False, 'issue_comment_url': 'https://api.github.com/repos/cav71/setuptools-github/issues/comments{/number}', 'issue_events_url': 'https://api.github.com/repos/cav71/setuptools-github/issues/events{/number}', 'issues_url': 'https://api.github.com/repos/cav71/setuptools-github/issues{/number}', 'keys_url': 'https://api.github.com/repos/cav71/setuptools-github/keys{/key_id}', 'labels_url': 'https://api.github.com/repos/cav71/setuptools-github/labels{/name}', 'language': 'Python', 'languages_url': 'https://api.github.com/repos/cav71/setuptools-github/languages', 'license': {'key': 'bsd-2-clause', 'name': 'BSD 2-Clause "Simplified" License', 'node_id': 'MDc6TGljZW5zZTQ=', 'spdx_id': 'BSD-2-Clause', 'url': 'https://api.github.com/licenses/bsd-2-clause'}, 'master_branch': 'master', 'merges_url': 'https://api.github.com/repos/cav71/setuptools-github/merges', 'milestones_url': 'https://api.github.com/repos/cav71/setuptools-github/milestones{/number}', 'mirror_url': None, 'name': 'setuptools-github', 'node_id': 'MDEwOlJlcG9zaXRvcnk0MDU5NzU0ODc=', 'notifications_url': 'https://api.github.com/repos/cav71/setuptools-github/notifications{?since,all,participating}', 'open_issues': 1, 'open_issues_count': 1, 'owner': {'avatar_url': 'https://avatars.githubusercontent.com/u/2042971?v=4', 'email': 'a.cavallo@cavallinux.eu', 'events_url': 'https://api.github.com/users/cav71/events{/privacy}', 'followers_url': 'https://api.github.com/users/cav71/followers', 'following_url': 'https://api.github.com/users/cav71/following{/other_user}', 'gists_url': 'https://api.github.com/users/cav71/gists{/gist_id}', 'gravatar_id': '', 'html_url': 'https://github.com/cav71', 'id': 2042971, 'login': 'cav71', 'name': 'cav71', 'node_id': 'MDQ6VXNlcjIwNDI5NzE=', 'organizations_url': 'https://api.github.com/users/cav71/orgs', 'received_events_url': 'https://api.github.com/users/cav71/received_events', 'repos_url': 'https://api.github.com/users/cav71/repos', 'site_admin': False, 'starred_url': 'https://api.github.com/users/cav71/starred{/owner}{/repo}', 'subscriptions_url': 'https://api.github.com/users/cav71/subscriptions', 'type': 'User', 'url': 'https://api.github.com/users/cav71'}, 'private': False, 'pulls_url': 'https://api.github.com/repos/cav71/setuptools-github/pulls{/number}', 'pushed_at': 1691439437, 'releases_url': 'https://api.github.com/repos/cav71/setuptools-github/releases{/id}', 'size': 361, 'ssh_url': 'git@github.com:cav71/setuptools-github.git', 'stargazers': 0, 'stargazers_count': 0, 'stargazers_url': 'https://api.github.com/repos/cav71/setuptools-github/stargazers', 'statuses_url': 'https://api.github.com/repos/cav71/setuptools-github/statuses/{sha}', 'subscribers_url': 'https://api.github.com/repos/cav71/setuptools-github/subscribers', 'subscription_url': 'https://api.github.com/repos/cav71/setuptools-github/subscription', 'svn_url': 'https://github.com/cav71/setuptools-github', 'tags_url': 'https://api.github.com/repos/cav71/setuptools-github/tags', 'teams_url': 'https://api.github.com/repos/cav71/setuptools-github/teams', 'topics': [], 'trees_url': 'https://api.github.com/repos/cav71/setuptools-github/git/trees{/sha}', 'updated_at': '2022-01-04T18:09:04Z', 'url': 'https://github.com/cav71/setuptools-github', 'visibility': 'public', 'watchers': 0, 'watchers_count': 0, 'web_commit_signoff_required': False}, 'sender': {'avatar_url': 'https://avatars.githubusercontent.com/u/2042971?v=4', 'events_url': 'https://api.github.com/users/cav71/events{/privacy}', 'followers_url': 'https://api.github.com/users/cav71/followers', 'following_url': 'https://api.github.com/users/cav71/following{/other_user}', 'gists_url': 'https://api.github.com/users/cav71/gists{/gist_id}', 'gravatar_id': '', 'html_url': 'https://github.com/cav71', 'id': 2042971, 'login': 'cav71', 'node_id': 'MDQ6VXNlcjIwNDI5NzE=', 'organizations_url': 'https://api.github.com/users/cav71/orgs', 'received_events_url': 'https://api.github.com/users/cav71/received_events', 'repos_url': 'https://api.github.com/users/cav71/repos', 'site_admin': False, 'starred_url': 'https://api.github.com/users/cav71/starred{/owner}{/repo}', 'subscriptions_url': 'https://api.github.com/users/cav71/subscriptions', 'type': 'User', 'url': 'https://api.github.com/users/cav71'}}
 event_name = 'push'
 event_path = '/home/runner/work/_temp/_github_workflow/event.json'
 graphql_url = 'https://api.github.com/graphql'
 head_ref = ''
 job = 'build'
-output = '/home/runner/work/_temp/_runner_file_commands/set_output_5f68d7fb-9e6d-47de-89bc-b42527cb350c'
-path = '/home/runner/work/_temp/_runner_file_commands/add_path_5f68d7fb-9e6d-47de-89bc-b42527cb350c'
-ref = 'refs/heads/beta/0.3.8'
-ref_name = 'beta/0.3.8'
+output = '/home/runner/work/_temp/_runner_file_commands/set_output_5d7ccf4b-2e2e-4c3a-aa0c-5f7a543a07cc'
+path = '/home/runner/work/_temp/_runner_file_commands/add_path_5d7ccf4b-2e2e-4c3a-aa0c-5f7a543a07cc'
+ref = 'refs/heads/beta/0.3.9'
+ref_name = 'beta/0.3.9'
 ref_protected = False
 ref_type = 'branch'
 repo-self-hosted-runners-disabled = False
 repository = 'cav71/setuptools-github'
 repositoryUrl = 'git://github.com/cav71/setuptools-github.git'
 repository_id = '405975487'
 repository_owner = 'cav71'
 repository_owner_id = '2042971'
 repository_visibility = 'public'
 retention_days = '90'
 run_attempt = '1'
-run_id = '5789315544'
-run_number = '95'
+run_id = '5789514622'
+run_number = '97'
 secret_source = 'Actions'
 server_url = 'https://github.com'
-sha = '9df889992f422a62cdd3ced41323eaba6e855ae3'
-state = '/home/runner/work/_temp/_runner_file_commands/save_state_5f68d7fb-9e6d-47de-89bc-b42527cb350c'
-step_summary = '/home/runner/work/_temp/_runner_file_commands/step_summary_5f68d7fb-9e6d-47de-89bc-b42527cb350c'
-token = 'ghs_mAuqBeO6cC2LijxN7yaKMaxPrfZfZP132thp'
+sha = '971cde0beef9e5a64cc43d51e9f2259b5c878f75'
+state = '/home/runner/work/_temp/_runner_file_commands/save_state_5d7ccf4b-2e2e-4c3a-aa0c-5f7a543a07cc'
+step_summary = '/home/runner/work/_temp/_runner_file_commands/step_summary_5d7ccf4b-2e2e-4c3a-aa0c-5f7a543a07cc'
+token = 'ghs_Po6ZSPwRzrZ13hK3JQmPL2XoueRhqF1cPqkj'
 triggering_actor = 'cav71'
 workflow = 'Beta build'
-workflow_ref = 'cav71/setuptools-github/.github/workflows/beta.yml@refs/heads/beta/0.3.8'
-workflow_sha = '9df889992f422a62cdd3ced41323eaba6e855ae3'
+workflow_ref = 'cav71/setuptools-github/.github/workflows/beta.yml@refs/heads/beta/0.3.9'
+workflow_sha = '971cde0beef9e5a64cc43d51e9f2259b5c878f75'
 workspace = '/home/runner/work/setuptools-github/setuptools-github'
```

### Comparing `setuptools-github-0.3.8b95/src/setuptools_github/cli.py` & `setuptools-github-0.3.9b97/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.8b95/src/setuptools_github/scm.py` & `setuptools-github-0.3.9b97/src/setuptools_github/scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.8b95/src/setuptools_github/script.py` & `setuptools-github-0.3.9b97/src/setuptools_github/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 
         for branch in [*options.repo.branches.local, *options.repo.branches.remote]:
             if not branch.endswith(f"beta/{version}"):
                 continue
             options.error(f"branch '{branch}' already present")
         log.info("creating branch '%s'", f"/beta/{version}")
         options.repo.branch(f"beta/{version}", master)
-        options.repo(["checkout", master])
         print(  # noqa: T201
             tools.indent(
                 f"""
         The release branch beta/{version} has been created.
 
         To complete the release:
             git push origin beta/{version}
```

### Comparing `setuptools-github-0.3.8b95/src/setuptools_github/tools.py` & `setuptools-github-0.3.9b97/src/setuptools_github/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,15 +297,16 @@
             )
         return result, {}
 
     dirty = False
     if github_dump:
         gdata = json.loads(github_dump) if isinstance(github_dump, str) else github_dump
     elif record_path and record_path.exists():
-        gdata = loadmod(record_path).data
+        mod = loadmod(record_path)
+        gdata = {k: getattr(mod, k) for k in dir(mod) if not k.startswith("_")}
     elif repo:
         gdata = {
             "ref": repo.head.name,
             "sha": repo.head.target.hex[:7],
             "run_number": 0,
             "run_id": 0,
         }
```

### Comparing `setuptools-github-0.3.8b95/tests/conftest.py` & `setuptools-github-0.3.9b97/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.8b95/tests/test_cli.py` & `setuptools-github-0.3.9b97/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.8b95/tests/test_conftest.py` & `setuptools-github-0.3.9b97/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.8b95/tests/test_scm.py` & `setuptools-github-0.3.9b97/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.8b95/tests/test_script.py` & `setuptools-github-0.3.9b97/tests/test_script.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         repo=repo,
         mode="make-beta",
         error=errorfn,
         master="master"
     )
     script.main.__wrapped__(options)
     assert set(repo.branches.local) == {"master", "beta/0.0.0"}
+    repo(["checkout", "master"])
 
     try:
         script.main.__wrapped__(options)
     except MyError as exc:
         assert exc.args[0].startswith("branch 'beta/0.0.0' already present")
```

### Comparing `setuptools-github-0.3.8b95/tests/test_tools.py` & `setuptools-github-0.3.9b97/tests/test_tools.py`

 * *Files identical despite different names*

