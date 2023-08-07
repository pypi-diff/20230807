# Comparing `tmp/django_codemod-2.0.0.tar.gz` & `tmp/django_codemod-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_codemod-2.0.0.tar", max compression
+gzip compressed data, was "django_codemod-2.1.0.tar", max compression
```

## Comparing `django_codemod-2.0.0.tar` & `django_codemod-2.1.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1068 2023-06-27 12:18:53.930551 django_codemod-2.0.0/LICENSE
--rw-r--r--   0        0        0     9809 2023-06-27 12:18:53.930551 django_codemod-2.0.0/README.md
--rw-r--r--   0        0        0     2340 2023-06-27 12:18:55.098557 django_codemod-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-27 12:18:55.066557 django_codemod-2.0.0/src/django_codemod/__init__.py
--rw-r--r--   0        0        0     8612 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/cli.py
--rw-r--r--   0        0        0      710 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/commands.py
--rw-r--r--   0        0        0      448 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/constants.py
--rw-r--r--   0        0        0      116 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/feature_flags.py
--rw-r--r--   0        0        0     3640 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/path_utils.py
--rw-r--r--   0        0        0        0 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/utils/__init__.py
--rw-r--r--   0        0        0     1378 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/utils/calls.py
--rw-r--r--   0        0        0     3367 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/__init__.py
--rw-r--r--   0        0        0     5978 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/admin.py
--rw-r--r--   0        0        0    14945 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/base.py
--rw-r--r--   0        0        0      379 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/core.py
--rw-r--r--   0        0        0     1222 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/crypto.py
--rw-r--r--   0        0        0     1107 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/decorators.py
--rw-r--r--   0        0        0     1042 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/encoding.py
--rw-r--r--   0        0        0     1459 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/exceptions.py
--rw-r--r--   0        0        0      699 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/forms.py
--rw-r--r--   0        0        0      415 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/html.py
--rw-r--r--   0        0        0     3240 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/http.py
--rw-r--r--   0        0        0      413 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/lru_cache.py
--rw-r--r--   0        0        0     7917 2023-06-27 12:18:53.930551 django_codemod-2.0.0/src/django_codemod/visitors/models.py
--rw-r--r--   0        0        0      390 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/os_utils.py
--rw-r--r--   0        0        0      422 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/paginator.py
--rw-r--r--   0        0        0     1116 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/postgres_fields.py
--rw-r--r--   0        0        0      648 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/shortcuts.py
--rw-r--r--   0        0        0     3974 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/signals.py
--rw-r--r--   0        0        0     1339 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/template_context.py
--rw-r--r--   0        0        0     5774 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/template_tags.py
--rw-r--r--   0        0        0     1259 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/timezone.py
--rw-r--r--   0        0        0     1654 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/translations.py
--rw-r--r--   0        0        0     4170 2023-06-27 12:18:53.934551 django_codemod-2.0.0/src/django_codemod/visitors/urls.py
--rw-r--r--   0        0        0        0 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0     6320 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/test_cli.py
--rwxr-xr-x   0        0        0      737 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/test_e2e.sh
--rw-r--r--   0        0        0     6959 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/test_path_utils.py
--rw-r--r--   0        0        0        0 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/__init__.py
--rw-r--r--   0        0        0      484 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/base.py
--rw-r--r--   0        0        0     7083 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_admin.py
--rw-r--r--   0        0        0    14132 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_base.py
--rw-r--r--   0        0        0      951 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_core.py
--rw-r--r--   0        0        0     2264 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_crypto.py
--rw-r--r--   0        0        0     1894 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_decorators.py
--rw-r--r--   0        0        0     1704 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_encoding.py
--rw-r--r--   0        0        0     2071 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_exceptions.py
--rw-r--r--   0        0        0      954 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_forms.py
--rw-r--r--   0        0        0      559 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_html.py
--rw-r--r--   0        0        0     5449 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_http.py
--rw-r--r--   0        0        0      531 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_lru_cache.py
--rw-r--r--   0        0        0    11944 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_models.py
--rw-r--r--   0        0        0      514 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_os_utils.py
--rw-r--r--   0        0        0     1351 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_paginator.py
--rw-r--r--   0        0        0     2560 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_postgres_fields.py
--rw-r--r--   0        0        0      671 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_shortcuts.py
--rw-r--r--   0        0        0     4162 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_signals.py
--rw-r--r--   0        0        0     1957 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_template_context.py
--rw-r--r--   0        0        0     4713 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_template_tags.py
--rw-r--r--   0        0        0     2409 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_timezone.py
--rw-r--r--   0        0        0     4501 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_translations.py
--rw-r--r--   0        0        0     6971 2023-06-27 12:18:53.934551 django_codemod-2.0.0/tests/visitors/test_urls.py
--rw-r--r--   0        0        0    11280 1970-01-01 00:00:00.000000 django_codemod-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-07 15:00:30.165863 django_codemod-2.1.0/LICENSE
+-rw-r--r--   0        0        0     9809 2023-08-07 15:00:30.165863 django_codemod-2.1.0/README.md
+-rw-r--r--   0        0        0     2548 2023-08-07 15:00:32.253884 django_codemod-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/__init__.py
+-rw-r--r--   0        0        0     8612 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/cli.py
+-rw-r--r--   0        0        0      710 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/commands.py
+-rw-r--r--   0        0        0      448 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/constants.py
+-rw-r--r--   0        0        0      116 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/feature_flags.py
+-rw-r--r--   0        0        0     3640 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/path_utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/utils/__init__.py
+-rw-r--r--   0        0        0     1378 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/utils/calls.py
+-rw-r--r--   0        0        0     3367 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/__init__.py
+-rw-r--r--   0        0        0     5978 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/admin.py
+-rw-r--r--   0        0        0    14945 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/base.py
+-rw-r--r--   0        0        0      379 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/core.py
+-rw-r--r--   0        0        0     1222 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/crypto.py
+-rw-r--r--   0        0        0     1107 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/decorators.py
+-rw-r--r--   0        0        0     1042 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/encoding.py
+-rw-r--r--   0        0        0     1459 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/exceptions.py
+-rw-r--r--   0        0        0      699 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/forms.py
+-rw-r--r--   0        0        0      415 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/html.py
+-rw-r--r--   0        0        0     3240 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/http.py
+-rw-r--r--   0        0        0      413 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/lru_cache.py
+-rw-r--r--   0        0        0     7917 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/models.py
+-rw-r--r--   0        0        0      390 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/os_utils.py
+-rw-r--r--   0        0        0      422 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/paginator.py
+-rw-r--r--   0        0        0     1116 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/postgres_fields.py
+-rw-r--r--   0        0        0      648 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/shortcuts.py
+-rw-r--r--   0        0        0     3974 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/signals.py
+-rw-r--r--   0        0        0     1339 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/template_context.py
+-rw-r--r--   0        0        0     5774 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/template_tags.py
+-rw-r--r--   0        0        0     1259 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/timezone.py
+-rw-r--r--   0        0        0     1654 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/translations.py
+-rw-r--r--   0        0        0     4170 2023-08-07 15:00:30.169863 django_codemod-2.1.0/src/django_codemod/visitors/urls.py
+-rw-r--r--   0        0        0        0 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     6320 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/test_cli.py
+-rwxr-xr-x   0        0        0      737 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/test_e2e.sh
+-rw-r--r--   0        0        0     6959 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/test_path_utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/__init__.py
+-rw-r--r--   0        0        0      484 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/base.py
+-rw-r--r--   0        0        0     7083 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/test_admin.py
+-rw-r--r--   0        0        0    14132 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/test_base.py
+-rw-r--r--   0        0        0      951 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/test_core.py
+-rw-r--r--   0        0        0     2264 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/test_crypto.py
+-rw-r--r--   0        0        0     1894 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/test_decorators.py
+-rw-r--r--   0        0        0     1704 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/test_encoding.py
+-rw-r--r--   0        0        0     2071 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/test_exceptions.py
+-rw-r--r--   0        0        0      954 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/test_forms.py
+-rw-r--r--   0        0        0      559 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/test_html.py
+-rw-r--r--   0        0        0     5449 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/test_http.py
+-rw-r--r--   0        0        0      531 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/test_lru_cache.py
+-rw-r--r--   0        0        0    11944 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/test_models.py
+-rw-r--r--   0        0        0      514 2023-08-07 15:00:30.169863 django_codemod-2.1.0/tests/visitors/test_os_utils.py
+-rw-r--r--   0        0        0     1351 2023-08-07 15:00:30.173863 django_codemod-2.1.0/tests/visitors/test_paginator.py
+-rw-r--r--   0        0        0     2560 2023-08-07 15:00:30.173863 django_codemod-2.1.0/tests/visitors/test_postgres_fields.py
+-rw-r--r--   0        0        0      671 2023-08-07 15:00:30.173863 django_codemod-2.1.0/tests/visitors/test_shortcuts.py
+-rw-r--r--   0        0        0     4162 2023-08-07 15:00:30.173863 django_codemod-2.1.0/tests/visitors/test_signals.py
+-rw-r--r--   0        0        0     1957 2023-08-07 15:00:30.173863 django_codemod-2.1.0/tests/visitors/test_template_context.py
+-rw-r--r--   0        0        0     4713 2023-08-07 15:00:30.173863 django_codemod-2.1.0/tests/visitors/test_template_tags.py
+-rw-r--r--   0        0        0     2409 2023-08-07 15:00:30.173863 django_codemod-2.1.0/tests/visitors/test_timezone.py
+-rw-r--r--   0        0        0     4501 2023-08-07 15:00:30.173863 django_codemod-2.1.0/tests/visitors/test_translations.py
+-rw-r--r--   0        0        0     6971 2023-08-07 15:00:30.173863 django_codemod-2.1.0/tests/visitors/test_urls.py
+-rw-r--r--   0        0        0    11331 1970-01-01 00:00:00.000000 django_codemod-2.1.0/PKG-INFO
```

### Comparing `django_codemod-2.0.0/LICENSE` & `django_codemod-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/README.md` & `django_codemod-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/pyproject.toml` & `django_codemod-2.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "django-codemod"
-version = "2.0.0"
+version = "2.1.0"
 description = "A command line tool to automatically fix Django deprecations."
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["django", "codemod", "libCST"]
 repository = "https://github.com/browniebroke/django-codemod"
 documentation = "https://django-codemod.readthedocs.io"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
+    "Programming Language :: Python :: 3.12",
 ]
 packages = [
     { include = "django_codemod", from = "src" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.urls]
@@ -45,22 +46,31 @@
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
-sphinx-rtd-theme = ">=1.0"
+furo = ">=2023.5.20"
 
 [tool.semantic_release]
 branch = "main"
-version_toml = "pyproject.toml:tool.poetry.version"
+version_toml = ["pyproject.toml:tool.poetry.version"]
 version_variable = "src/django_codemod/__init__.py:__version__"
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
 addopts = "-v -Wdefault --cov=django_codemod --cov-report=term-missing:skip-covered"
 pythonpath = ["src"]
 
 [tool.isort]
 profile = "black"
 known_first_party = ["django_codemod", "tests"]
```

### Comparing `django_codemod-2.0.0/src/django_codemod/cli.py` & `django_codemod-2.1.0/src/django_codemod/cli.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/commands.py` & `django_codemod-2.1.0/src/django_codemod/commands.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/path_utils.py` & `django_codemod-2.1.0/src/django_codemod/path_utils.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/utils/calls.py` & `django_codemod-2.1.0/src/django_codemod/utils/calls.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/__init__.py` & `django_codemod-2.1.0/src/django_codemod/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/admin.py` & `django_codemod-2.1.0/src/django_codemod/visitors/admin.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/base.py` & `django_codemod-2.1.0/src/django_codemod/visitors/base.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/crypto.py` & `django_codemod-2.1.0/src/django_codemod/visitors/crypto.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/decorators.py` & `django_codemod-2.1.0/src/django_codemod/visitors/decorators.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/encoding.py` & `django_codemod-2.1.0/src/django_codemod/visitors/encoding.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/exceptions.py` & `django_codemod-2.1.0/src/django_codemod/visitors/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/forms.py` & `django_codemod-2.1.0/src/django_codemod/visitors/forms.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/http.py` & `django_codemod-2.1.0/src/django_codemod/visitors/http.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/models.py` & `django_codemod-2.1.0/src/django_codemod/visitors/models.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/postgres_fields.py` & `django_codemod-2.1.0/src/django_codemod/visitors/postgres_fields.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/shortcuts.py` & `django_codemod-2.1.0/src/django_codemod/visitors/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/signals.py` & `django_codemod-2.1.0/src/django_codemod/visitors/signals.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/template_context.py` & `django_codemod-2.1.0/src/django_codemod/visitors/template_context.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/template_tags.py` & `django_codemod-2.1.0/src/django_codemod/visitors/template_tags.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/timezone.py` & `django_codemod-2.1.0/src/django_codemod/visitors/timezone.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/translations.py` & `django_codemod-2.1.0/src/django_codemod/visitors/translations.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/src/django_codemod/visitors/urls.py` & `django_codemod-2.1.0/src/django_codemod/visitors/urls.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/test_cli.py` & `django_codemod-2.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/test_e2e.sh` & `django_codemod-2.1.0/tests/test_e2e.sh`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/test_path_utils.py` & `django_codemod-2.1.0/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_admin.py` & `django_codemod-2.1.0/tests/visitors/test_admin.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_base.py` & `django_codemod-2.1.0/tests/visitors/test_base.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_core.py` & `django_codemod-2.1.0/tests/visitors/test_core.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_crypto.py` & `django_codemod-2.1.0/tests/visitors/test_crypto.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_decorators.py` & `django_codemod-2.1.0/tests/visitors/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_encoding.py` & `django_codemod-2.1.0/tests/visitors/test_encoding.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_exceptions.py` & `django_codemod-2.1.0/tests/visitors/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_forms.py` & `django_codemod-2.1.0/tests/visitors/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_html.py` & `django_codemod-2.1.0/tests/visitors/test_html.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_http.py` & `django_codemod-2.1.0/tests/visitors/test_http.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_lru_cache.py` & `django_codemod-2.1.0/tests/visitors/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_models.py` & `django_codemod-2.1.0/tests/visitors/test_models.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_os_utils.py` & `django_codemod-2.1.0/tests/visitors/test_os_utils.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_paginator.py` & `django_codemod-2.1.0/tests/visitors/test_paginator.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_postgres_fields.py` & `django_codemod-2.1.0/tests/visitors/test_postgres_fields.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_shortcuts.py` & `django_codemod-2.1.0/tests/visitors/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_signals.py` & `django_codemod-2.1.0/tests/visitors/test_signals.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_template_context.py` & `django_codemod-2.1.0/tests/visitors/test_template_context.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_template_tags.py` & `django_codemod-2.1.0/tests/visitors/test_template_tags.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_timezone.py` & `django_codemod-2.1.0/tests/visitors/test_timezone.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_translations.py` & `django_codemod-2.1.0/tests/visitors/test_translations.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/tests/visitors/test_urls.py` & `django_codemod-2.1.0/tests/visitors/test_urls.py`

 * *Files identical despite different names*

### Comparing `django_codemod-2.0.0/PKG-INFO` & `django_codemod-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-codemod
-Version: 2.0.0
+Version: 2.1.0
 Summary: A command line tool to automatically fix Django deprecations.
 Home-page: https://github.com/browniebroke/django-codemod
 License: MIT
 Keywords: django,codemod,libCST
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -14,14 +14,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: click (<9)
 Requires-Dist: libcst (==1.0.1)
 Requires-Dist: pathspec (>=0.6,<1)
 Requires-Dist: rich (>=10)
 Requires-Dist: rich-click (>=1.0)
 Project-URL: Bug Tracker, https://github.com/browniebroke/django-codemod/issues
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: django-codemod Version: 2.0.0 Summary: A command
+Metadata-Version: 2.1 Name: django-codemod Version: 2.1.0 Summary: A command
 line tool to automatically fix Django deprecations. Home-page: https://
 github.com/browniebroke/django-codemod License: MIT Keywords:
 django,codemod,libCST Author: Bruno Alla Author-email: alla.brunoo@gmail.com
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Software Development :: Libraries Requires-Dist: click (<9) Requires-Dist:
-libcst (==1.0.1) Requires-Dist: pathspec (>=0.6,<1) Requires-Dist: rich (>=10)
-Requires-Dist: rich-click (>=1.0) Project-URL: Bug Tracker, https://github.com/
-browniebroke/django-codemod/issues Project-URL: Changelog, https://django-
-codemod.readthedocs.io/en/stable/changelog.html Project-URL: Documentation,
-https://django-codemod.readthedocs.io Project-URL: Mastodon, https://
-fosstodon.org/@browniebroke Project-URL: Repository, https://github.com/
-browniebroke/django-codemod Project-URL: Twitter, https://twitter.com/
-_BrunoAlla Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Software Development ::
+Libraries Requires-Dist: click (<9) Requires-Dist: libcst (==1.0.1) Requires-
+Dist: pathspec (>=0.6,<1) Requires-Dist: rich (>=10) Requires-Dist: rich-click
+(>=1.0) Project-URL: Bug Tracker, https://github.com/browniebroke/django-
+codemod/issues Project-URL: Changelog, https://django-codemod.readthedocs.io/
+en/stable/changelog.html Project-URL: Documentation, https://django-
+codemod.readthedocs.io Project-URL: Mastodon, https://fosstodon.org/
+@browniebroke Project-URL: Repository, https://github.com/browniebroke/django-
+codemod Project-URL: Twitter, https://twitter.com/_BrunoAlla Description-
+Content-Type: text/markdown
                                [Django Codemod]
  [CI_Status] [Documentation_Status] [Test_coverage_percentage] [pre-commit.ci
                                     status]
                          [Poetry] [black] [pre-commit]
                   [PyPi_Status] [pyversions] [license] [LoC]
 A tool to help upgrade Django projects to newer version of the framework by
 automatically fixing deprecations. ## The problem When maintaining a Django
```

