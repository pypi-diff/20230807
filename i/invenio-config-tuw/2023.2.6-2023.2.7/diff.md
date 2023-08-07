# Comparing `tmp/invenio-config-tuw-2023.2.6.tar.gz` & `tmp/invenio-config-tuw-2023.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-config-tuw-2023.2.6.tar", last modified: Mon Jul 31 08:20:31 2023, max compression
+gzip compressed data, was "invenio-config-tuw-2023.2.7.tar", last modified: Mon Aug  7 11:44:47 2023, max compression
```

## Comparing `invenio-config-tuw-2023.2.6.tar` & `invenio-config-tuw-2023.2.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-31 08:20:31.541247 invenio-config-tuw-2023.2.6/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/.dockerignore
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      628 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.6/.editorconfig
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.6/.git-blame-ignore-revs
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-31 08:20:31.521247 invenio-config-tuw-2023.2.6/.tx/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1056 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/.tx/config
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      332 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.6/AUTHORS.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2603 2023-07-31 08:19:45.000000 invenio-config-tuw-2023.2.6/CHANGES.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3392 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.6/CONTRIBUTING.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      139 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/INSTALL.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/LICENSE
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1033 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.6/MANIFEST.in
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5540 2023-07-31 08:20:31.541247 invenio-config-tuw-2023.2.6/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1960 2022-08-09 11:57:39.000000 invenio-config-tuw-2023.2.6/README.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      536 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/babel.ini
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-31 08:20:31.529247 invenio-config-tuw-2023.2.6/docs/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7457 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/docs/Makefile
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      278 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/docs/api.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/docs/authors.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/docs/changes.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10226 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.6/docs/conf.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      290 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/docs/configuration.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      239 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/docs/contributing.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      817 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/docs/index.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/docs/installation.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/docs/license.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7005 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/docs/make.bat
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/docs/requirements.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/docs/usage.rst
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-31 08:20:31.533247 invenio-config-tuw-2023.2.6/invenio_config_tuw/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      408 2023-07-31 08:19:45.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/__init__.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-31 08:20:31.537247 invenio-config-tuw-2023.2.6/invenio_config_tuw/auth/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      540 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/auth/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1006 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/auth/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8845 2023-07-26 20:21:45.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/auth/handlers.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2540 2021-10-04 14:54:28.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/auth/utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7800 2023-07-26 20:21:45.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2623 2022-11-24 12:57:07.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/ext.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1337 2023-05-26 12:34:11.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/formatters.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3905 2023-07-26 20:21:45.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/forms.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-31 08:20:31.537247 invenio-config-tuw-2023.2.6/invenio_config_tuw/permissions/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      780 2022-07-18 13:04:23.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/permissions/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3170 2022-10-11 13:14:29.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/permissions/generators.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11136 2023-04-27 15:56:14.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/permissions/policies.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3862 2022-10-28 12:03:49.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/startup.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4599 2023-07-26 20:31:27.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/tasks.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-31 08:20:31.537247 invenio-config-tuw-2023.2.6/invenio_config_tuw/tiss/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      409 2023-07-26 14:21:51.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/tiss/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2404 2023-07-26 14:21:51.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/tiss/models.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1794 2023-07-26 14:21:51.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/tiss/utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2739 2023-04-24 16:03:59.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw/utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-31 08:20:31.533247 invenio-config-tuw-2023.2.6/invenio_config_tuw.egg-info/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5540 2023-07-31 08:20:31.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1401 2023-07-31 08:20:31.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-07-31 08:20:31.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      485 2023-07-31 08:20:31.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-07-31 08:20:31.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw.egg-info/not-zip-safe
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2023-07-31 08:20:31.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       19 2023-07-31 08:20:31.000000 invenio-config-tuw-2023.2.6/invenio_config_tuw.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.6/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      492 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/requirements-devel.txt
--rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      411 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.6/run-tests.sh
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2832 2023-07-31 08:20:31.541247 invenio-config-tuw-2023.2.6/setup.cfg
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.6/setup.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-31 08:20:31.541247 invenio-config-tuw-2023.2.6/tests/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2023-04-27 15:56:14.000000 invenio-config-tuw-2023.2.6/tests/conftest.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      789 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.6/tests/test_invenio_config_tuw.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-08-07 11:44:47.342774 invenio-config-tuw-2023.2.7/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/.dockerignore
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      628 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.7/.editorconfig
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.7/.git-blame-ignore-revs
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-08-07 11:44:47.326773 invenio-config-tuw-2023.2.7/.tx/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1056 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/.tx/config
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      332 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.7/AUTHORS.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2603 2023-08-07 11:43:58.000000 invenio-config-tuw-2023.2.7/CHANGES.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3392 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.7/CONTRIBUTING.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      139 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/INSTALL.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/LICENSE
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1033 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.7/MANIFEST.in
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5540 2023-08-07 11:44:47.342774 invenio-config-tuw-2023.2.7/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1960 2022-08-09 11:57:39.000000 invenio-config-tuw-2023.2.7/README.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      536 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/babel.ini
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-08-07 11:44:47.330773 invenio-config-tuw-2023.2.7/docs/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7457 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/docs/Makefile
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      278 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/docs/api.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/docs/authors.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/docs/changes.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10226 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.7/docs/conf.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      290 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/docs/configuration.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      239 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/docs/contributing.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      817 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/docs/index.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/docs/installation.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/docs/license.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7005 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/docs/make.bat
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/docs/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/docs/usage.rst
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-08-07 11:44:47.334773 invenio-config-tuw-2023.2.7/invenio_config_tuw/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      408 2023-08-07 11:43:58.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/__init__.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-08-07 11:44:47.338773 invenio-config-tuw-2023.2.7/invenio_config_tuw/auth/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      540 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/auth/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1006 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/auth/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8845 2023-07-26 20:21:45.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/auth/handlers.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2540 2021-10-04 14:54:28.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/auth/utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7800 2023-08-07 11:43:58.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2623 2022-11-24 12:57:07.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/ext.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1337 2023-05-26 12:34:11.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/formatters.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3905 2023-07-26 20:21:45.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/forms.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-08-07 11:44:47.338773 invenio-config-tuw-2023.2.7/invenio_config_tuw/permissions/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      780 2022-07-18 13:04:23.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/permissions/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3170 2022-10-11 13:14:29.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/permissions/generators.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11136 2023-08-07 11:43:58.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/permissions/policies.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3862 2022-10-28 12:03:49.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/startup.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4599 2023-07-26 20:31:27.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/tasks.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-08-07 11:44:47.342774 invenio-config-tuw-2023.2.7/invenio_config_tuw/tiss/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      409 2023-07-26 14:21:51.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/tiss/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2404 2023-07-26 14:21:51.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/tiss/models.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1794 2023-07-26 14:21:51.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/tiss/utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2739 2023-04-24 16:03:59.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw/utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-08-07 11:44:47.338773 invenio-config-tuw-2023.2.7/invenio_config_tuw.egg-info/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5540 2023-08-07 11:44:47.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1401 2023-08-07 11:44:47.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-08-07 11:44:47.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      491 2023-08-07 11:44:47.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-08-07 11:44:47.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw.egg-info/not-zip-safe
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2023-08-07 11:44:47.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       19 2023-08-07 11:44:47.000000 invenio-config-tuw-2023.2.7/invenio_config_tuw.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.7/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      492 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/requirements-devel.txt
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      411 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.7/run-tests.sh
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2838 2023-08-07 11:44:47.342774 invenio-config-tuw-2023.2.7/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.7/setup.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-08-07 11:44:47.342774 invenio-config-tuw-2023.2.7/tests/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2023-08-07 11:43:58.000000 invenio-config-tuw-2023.2.7/tests/conftest.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      789 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.7/tests/test_invenio_config_tuw.py
```

### Comparing `invenio-config-tuw-2023.2.6/.editorconfig` & `invenio-config-tuw-2023.2.7/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/.tx/config` & `invenio-config-tuw-2023.2.7/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/CHANGES.rst` & `invenio-config-tuw-2023.2.7/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24, updated 2023-07-31)
+Version 2023.2 (released 2023-04-24, updated 2023-08-07)
 
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
 - Add a null check for the current_user in the logging formatter
 - Prevent the logging formatter from blowing up outside of a request context
```

### Comparing `invenio-config-tuw-2023.2.6/CONTRIBUTING.rst` & `invenio-config-tuw-2023.2.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/LICENSE` & `invenio-config-tuw-2023.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/MANIFEST.in` & `invenio-config-tuw-2023.2.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/PKG-INFO` & `invenio-config-tuw-2023.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tuw
-Version: 2023.2.6
+Version: 2023.2.7
 Summary: "Invenio module containing some customizations and configuration for TU Wien."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-config-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio tu wien configuration
 Platform: any
@@ -94,15 +94,15 @@
     Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24, updated 2023-07-31)
+Version 2023.2 (released 2023-04-24, updated 2023-08-07)
 
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
 - Add a null check for the current_user in the logging formatter
 - Prevent the logging formatter from blowing up outside of a request context
```

### Comparing `invenio-config-tuw-2023.2.6/README.rst` & `invenio-config-tuw-2023.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/babel.ini` & `invenio-config-tuw-2023.2.7/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/docs/Makefile` & `invenio-config-tuw-2023.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/docs/conf.py` & `invenio-config-tuw-2023.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/docs/index.rst` & `invenio-config-tuw-2023.2.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/docs/make.bat` & `invenio-config-tuw-2023.2.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/auth/__init__.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/auth/config.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/auth/config.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/auth/handlers.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/auth/handlers.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/auth/utils.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/auth/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/config.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/config.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/ext.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/formatters.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/formatters.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/forms.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/forms.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/permissions/__init__.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/permissions/generators.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/permissions/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/permissions/policies.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/permissions/policies.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/startup.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/startup.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/tasks.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/tiss/models.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/tiss/models.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/tiss/utils.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/tiss/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw/utils.py` & `invenio-config-tuw-2023.2.7/invenio_config_tuw/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw.egg-info/PKG-INFO` & `invenio-config-tuw-2023.2.7/invenio_config_tuw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tuw
-Version: 2023.2.6
+Version: 2023.2.7
 Summary: "Invenio module containing some customizations and configuration for TU Wien."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-config-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio tu wien configuration
 Platform: any
@@ -94,15 +94,15 @@
     Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24, updated 2023-07-31)
+Version 2023.2 (released 2023-04-24, updated 2023-08-07)
 
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
 - Add a null check for the current_user in the logging formatter
 - Prevent the logging formatter from blowing up outside of a request context
```

### Comparing `invenio-config-tuw-2023.2.6/invenio_config_tuw.egg-info/SOURCES.txt` & `invenio-config-tuw-2023.2.7/invenio_config_tuw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/setup.cfg` & `invenio-config-tuw-2023.2.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 invenio_base.api_apps = 
 	invenio_config_tuw = invenio_config_tuw:InvenioConfigTUW
 invenio_base.blueprints = 
 	invenio_config_tuw_hacks = invenio_config_tuw.startup:blueprint
 invenio_base.api_blueprints = 
 	invenio_config_tuw_hacks = invenio_config_tuw.startup:blueprint
 invenio_celery.tasks = 
-	invenio_app_rdm = invenio_app_rdm.tasks
+	invenio_config_tuw = invenio_config_tuw.tasks
 invenio_config.module = 
 	zzz_invenio_config_tuw = invenio_config_tuw.config
 
 [build_sphinx]
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
```

### Comparing `invenio-config-tuw-2023.2.6/tests/conftest.py` & `invenio-config-tuw-2023.2.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.6/tests/test_invenio_config_tuw.py` & `invenio-config-tuw-2023.2.7/tests/test_invenio_config_tuw.py`

 * *Files identical despite different names*

