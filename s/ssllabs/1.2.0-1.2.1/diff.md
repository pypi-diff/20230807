# Comparing `tmp/ssllabs-1.2.0.tar.gz` & `tmp/ssllabs-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssllabs-1.2.0.tar", last modified: Mon Mar  6 14:33:52 2023, max compression
+gzip compressed data, was "ssllabs-1.2.1.tar", last modified: Mon Aug  7 20:04:29 2023, max compression
```

## Comparing `ssllabs-1.2.0.tar` & `ssllabs-1.2.1.tar`

### file list

```diff
@@ -1,93 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:52.331025 ssllabs-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:52.315024 ssllabs-1.2.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-06 14:33:32.000000 ssllabs-1.2.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-03-06 14:33:32.000000 ssllabs-1.2.0/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-06 14:33:32.000000 ssllabs-1.2.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-06 14:33:32.000000 ssllabs-1.2.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:52.315024 ssllabs-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-03-06 14:33:32.000000 ssllabs-1.2.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-03-06 14:33:32.000000 ssllabs-1.2.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:52.315024 ssllabs-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-06 14:33:32.000000 ssllabs-1.2.0/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-06 14:33:32.000000 ssllabs-1.2.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-03-06 14:33:32.000000 ssllabs-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-06 14:33:32.000000 ssllabs-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-06 14:33:32.000000 ssllabs-1.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-06 14:33:32.000000 ssllabs-1.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-06 14:33:32.000000 ssllabs-1.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-06 14:33:52.327024 ssllabs-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-03-06 14:33:32.000000 ssllabs-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:52.319024 ssllabs-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-06 14:33:32.000000 ssllabs-1.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-06 14:33:32.000000 ssllabs-1.2.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:52.319024 ssllabs-1.2.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-06 14:33:32.000000 ssllabs-1.2.0/docs/_templates/docs-navbar.html
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-06 14:33:32.000000 ssllabs-1.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-06 14:33:32.000000 ssllabs-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-06 14:33:32.000000 ssllabs-1.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:52.319024 ssllabs-1.2.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-06 14:33:32.000000 ssllabs-1.2.0/docs/source/ssllabs.api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-03-06 14:33:32.000000 ssllabs-1.2.0/docs/source/ssllabs.data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-06 14:33:32.000000 ssllabs-1.2.0/docs/source/ssllabs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-06 14:33:32.000000 ssllabs-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 14:33:52.331025 ssllabs-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-06 14:33:32.000000 ssllabs-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:52.319024 ssllabs-1.2.0/ssllabs/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:52.319024 ssllabs-1.2.0/ssllabs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/api/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/api/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/api/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/api/root_certs_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/api/status_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:52.327024 ssllabs-1.2.0/ssllabs/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/caa_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/caa_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/cert.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/certificate_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/drown_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/endpoint_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/host.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/hpkp_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/hsts_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/hsts_preload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/http_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/named_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/named_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/protocol_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/sim_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/sim_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/static_pkp_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/status_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/suite.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/trust.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/data/trust_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-03-06 14:33:32.000000 ssllabs-1.2.0/ssllabs/ssllabs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:52.319024 ssllabs-1.2.0/ssllabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-06 14:33:52.000000 ssllabs-1.2.0/ssllabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-03-06 14:33:52.000000 ssllabs-1.2.0/ssllabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:33:52.000000 ssllabs-1.2.0/ssllabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-06 14:33:52.000000 ssllabs-1.2.0/ssllabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-06 14:33:52.000000 ssllabs-1.2.0/ssllabs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:52.327024 ssllabs-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-06 14:33:32.000000 ssllabs-1.2.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:32.000000 ssllabs-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-06 14:33:32.000000 ssllabs-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-06 14:33:32.000000 ssllabs-1.2.0/tests/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:33:52.327024 ssllabs-1.2.0/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-03-06 14:33:32.000000 ssllabs-1.2.0/tests/test_data/analyze.json
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-06 14:33:32.000000 ssllabs-1.2.0/tests/test_data/analyze_running.json
--rw-r--r--   0 runner    (1001) docker     (123)   109150 2023-03-06 14:33:32.000000 ssllabs-1.2.0/tests/test_data/endpoint.json
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-06 14:33:32.000000 ssllabs-1.2.0/tests/test_data/info.json
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-06 14:33:32.000000 ssllabs-1.2.0/tests/test_data/info_max_assessments.json
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-06 14:33:32.000000 ssllabs-1.2.0/tests/test_data/info_running_assessments.json
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-06 14:33:32.000000 ssllabs-1.2.0/tests/test_data/root_certs.json
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-03-06 14:33:32.000000 ssllabs-1.2.0/tests/test_data/status_codes.json
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-03-06 14:33:32.000000 ssllabs-1.2.0/tests/test_ssllabs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:29.180268 ssllabs-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:29.172268 ssllabs-1.2.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-07 20:04:11.000000 ssllabs-1.2.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-07 20:04:11.000000 ssllabs-1.2.1/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-07 20:04:11.000000 ssllabs-1.2.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 20:04:11.000000 ssllabs-1.2.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:29.172268 ssllabs-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-08-07 20:04:11.000000 ssllabs-1.2.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-08-07 20:04:11.000000 ssllabs-1.2.1/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-07 20:04:11.000000 ssllabs-1.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:29.172268 ssllabs-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-07 20:04:11.000000 ssllabs-1.2.1/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-07 20:04:11.000000 ssllabs-1.2.1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-07 20:04:11.000000 ssllabs-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-07 20:04:11.000000 ssllabs-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-07 20:04:11.000000 ssllabs-1.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-07 20:04:11.000000 ssllabs-1.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-07 20:04:11.000000 ssllabs-1.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-07 20:04:29.180268 ssllabs-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-08-07 20:04:11.000000 ssllabs-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:29.176268 ssllabs-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-07 20:04:11.000000 ssllabs-1.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-07 20:04:11.000000 ssllabs-1.2.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:29.176268 ssllabs-1.2.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-08-07 20:04:11.000000 ssllabs-1.2.1/docs/_templates/docs-navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 20:04:11.000000 ssllabs-1.2.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-07 20:04:11.000000 ssllabs-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 20:04:11.000000 ssllabs-1.2.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:29.176268 ssllabs-1.2.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-07 20:04:11.000000 ssllabs-1.2.1/docs/source/ssllabs.api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-08-07 20:04:11.000000 ssllabs-1.2.1/docs/source/ssllabs.data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-07 20:04:11.000000 ssllabs-1.2.1/docs/source/ssllabs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 20:04:11.000000 ssllabs-1.2.1/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 20:04:11.000000 ssllabs-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 20:04:29.184268 ssllabs-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-07 20:04:11.000000 ssllabs-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:29.176268 ssllabs-1.2.1/ssllabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:29.176268 ssllabs-1.2.1/ssllabs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/api/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/api/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/api/root_certs_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/api/status_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:29.180268 ssllabs-1.2.1/ssllabs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/caa_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/caa_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/certificate_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/drown_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/endpoint_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/hpkp_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/hsts_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/hsts_preload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/http_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/named_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/named_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/protocol_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/sim_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/sim_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/static_pkp_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/trust.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/data/trust_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-08-07 20:04:11.000000 ssllabs-1.2.1/ssllabs/ssllabs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:29.176268 ssllabs-1.2.1/ssllabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-07 20:04:29.000000 ssllabs-1.2.1/ssllabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-08-07 20:04:29.000000 ssllabs-1.2.1/ssllabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:04:29.000000 ssllabs-1.2.1/ssllabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-07 20:04:29.000000 ssllabs-1.2.1/ssllabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-07 20:04:29.000000 ssllabs-1.2.1/ssllabs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:29.180268 ssllabs-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-07 20:04:11.000000 ssllabs-1.2.1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:11.000000 ssllabs-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-07 20:04:11.000000 ssllabs-1.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-07 20:04:11.000000 ssllabs-1.2.1/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:04:29.180268 ssllabs-1.2.1/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-08-07 20:04:11.000000 ssllabs-1.2.1/tests/test_data/analyze.json
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-07 20:04:11.000000 ssllabs-1.2.1/tests/test_data/analyze_running.json
+-rw-r--r--   0 runner    (1001) docker     (123)   109150 2023-08-07 20:04:11.000000 ssllabs-1.2.1/tests/test_data/endpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-07 20:04:11.000000 ssllabs-1.2.1/tests/test_data/info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-07 20:04:11.000000 ssllabs-1.2.1/tests/test_data/info_max_assessments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-07 20:04:11.000000 ssllabs-1.2.1/tests/test_data/info_running_assessments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-08-07 20:04:11.000000 ssllabs-1.2.1/tests/test_data/root_certs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-08-07 20:04:11.000000 ssllabs-1.2.1/tests/test_data/status_codes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-08-07 20:04:11.000000 ssllabs-1.2.1/tests/test_ssllabs.py
```

### Comparing `ssllabs-1.2.0/.devcontainer/devcontainer.json` & `ssllabs-1.2.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/.github/CODE_OF_CONDUCT.md` & `ssllabs-1.2.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/.github/CONTRIBUTING.md` & `ssllabs-1.2.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/.github/workflows/pythonpackage.yml` & `ssllabs-1.2.1/.github/workflows/pythonpackage.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Python package
 
-on: [push]
+on: [push, pull_request]
 
 jobs:
 
   format:
     name: Check formatting
     runs-on: ubuntu-latest
     steps:
```

### Comparing `ssllabs-1.2.0/.github/workflows/pythonpublish.yml` & `ssllabs-1.2.1/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/.gitignore` & `ssllabs-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/CHANGELOG.md` & `ssllabs-1.2.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [v1.2.1] - 2023/08/07
+
+### Fixed
+
+- Set fromCache explicitly to not always trigger a new analysis
+
 ## [v1.2.0] - 2023/03/06
 
 ### Added
 
 - Allow using cached results
 
 ## [v1.1.0] - 2023/02/16
```

### Comparing `ssllabs-1.2.0/LICENSE.md` & `ssllabs-1.2.1/LICENSE.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 devolo AG
+Copyright (c) 2023 devolo GmbH
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ssllabs-1.2.0/PKG-INFO` & `ssllabs-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssllabs
-Version: 1.2.0
+Version: 1.2.1
 Summary: Qualys SSL Labs API in Python
 Home-page: https://github.com/devolo/ssllabs
 Author: Markus Bong, Guido Schmitz
 Author-email: m.bong@famabo.de, guido.schmitz@fedaix.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssllabs-1.2.0/README.md` & `ssllabs-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,18 @@
     return await ssllabs.status_codes()
 
 asyncio.run(status_codes())
 ```
 
 This will give you a [StatusCodes object](https://github.com/ssllabs/ssllabs-scan/blob/master/ssllabs-api-docs-v3.md#statuscodes) as dataclass.
 
+### Example to print the grade of multiple servers
+
+If you are just interested in the grade of servers, you can take [this example](https://github.com/devolo/ssllabs/blob/master/example.py) as a starting point. Just exchange the list of hosts you want to query.
+
 ## Low level usage
 
 If the high level methods do not match your use case, you can access each [API call](https://github.com/ssllabs/ssllabs-scan/blob/master/ssllabs-api-docs-v3.md#protocol-calls).
 
 ```python
 import asyncio
```

### Comparing `ssllabs-1.2.0/docs/Makefile` & `ssllabs-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/docs/README.md` & `ssllabs-1.2.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/docs/_templates/docs-navbar.html` & `ssllabs-1.2.1/docs/_templates/docs-navbar.html`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/docs/conf.py` & `ssllabs-1.2.1/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 sys.path.insert(0, os.path.abspath("../"))
 
 version = get_distribution("ssllabs").version
 
 # -- Project information -----------------------------------------------------
 
 project = get_distribution("ssllabs").project_name
-copyright = "2021, devolo AG"
+copyright = "2023, devolo GmbH"
 author = "Markus Bong, Guido Schmitz"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named "sphinx.ext.*") or your custom
 # ones.
```

### Comparing `ssllabs-1.2.0/docs/source/ssllabs.api.rst` & `ssllabs-1.2.1/docs/source/ssllabs.api.rst`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/docs/source/ssllabs.data.rst` & `ssllabs-1.2.1/docs/source/ssllabs.data.rst`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/setup.py` & `ssllabs-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/api/_api.py` & `ssllabs-1.2.1/ssllabs/api/_api.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/api/analyze.py` & `ssllabs-1.2.1/ssllabs/api/analyze.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/api/endpoint.py` & `ssllabs-1.2.1/ssllabs/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/api/info.py` & `ssllabs-1.2.1/ssllabs/api/info.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/api/root_certs_raw.py` & `ssllabs-1.2.1/ssllabs/api/root_certs_raw.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/api/status_codes.py` & `ssllabs-1.2.1/ssllabs/api/status_codes.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/cert.py` & `ssllabs-1.2.1/ssllabs/data/cert.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/certificate_chain.py` & `ssllabs-1.2.1/ssllabs/data/certificate_chain.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/drown_hosts.py` & `ssllabs-1.2.1/ssllabs/data/drown_hosts.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/endpoint.py` & `ssllabs-1.2.1/ssllabs/data/endpoint.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/endpoint_details.py` & `ssllabs-1.2.1/ssllabs/data/endpoint_details.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/host.py` & `ssllabs-1.2.1/ssllabs/data/host.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/hpkp_policy.py` & `ssllabs-1.2.1/ssllabs/data/hpkp_policy.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/hsts_policy.py` & `ssllabs-1.2.1/ssllabs/data/hsts_policy.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/hsts_preload.py` & `ssllabs-1.2.1/ssllabs/data/hsts_preload.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/http_transaction.py` & `ssllabs-1.2.1/ssllabs/data/http_transaction.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/info.py` & `ssllabs-1.2.1/ssllabs/data/info.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/protocol.py` & `ssllabs-1.2.1/ssllabs/data/protocol.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/protocol_suites.py` & `ssllabs-1.2.1/ssllabs/data/protocol_suites.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/sim_client.py` & `ssllabs-1.2.1/ssllabs/data/sim_client.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/simulation.py` & `ssllabs-1.2.1/ssllabs/data/simulation.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/static_pkp_policy.py` & `ssllabs-1.2.1/ssllabs/data/static_pkp_policy.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/suite.py` & `ssllabs-1.2.1/ssllabs/data/suite.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/data/trust_path.py` & `ssllabs-1.2.1/ssllabs/data/trust_path.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/ssllabs/ssllabs.py` & `ssllabs-1.2.1/ssllabs/ssllabs.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         if info.currentAssessments != 0:
             await asyncio.sleep(info.newAssessmentCoolOff / 1000)
 
         a = Analyze(self._client)
         host_object = await a.get(
             host=host,
             startNew="off" if from_cache else "on",
+            fromCache="on" if from_cache else "off",
             publish="on" if publish else "off",
             ignoreMismatch="on" if ignore_mismatch else "off",
             maxAge=max_age,
         )
         self._semaphore.release()
         while host_object.status not in ["READY", "ERROR"]:
             self._logger.debug("Assessment of %s not ready yet.", host)
```

### Comparing `ssllabs-1.2.0/ssllabs.egg-info/PKG-INFO` & `ssllabs-1.2.1/ssllabs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssllabs
-Version: 1.2.0
+Version: 1.2.1
 Summary: Qualys SSL Labs API in Python
 Home-page: https://github.com/devolo/ssllabs
 Author: Markus Bong, Guido Schmitz
 Author-email: m.bong@famabo.de, guido.schmitz@fedaix.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssllabs-1.2.0/ssllabs.egg-info/SOURCES.txt` & `ssllabs-1.2.1/ssllabs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 .git-blame-ignore-revs
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 CHANGELOG.md
 LICENSE.md
 README.md
+example.py
 pyproject.toml
 setup.py
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .github/CODE_OF_CONDUCT.md
 .github/CONTRIBUTING.md
+.github/dependabot.yml
 .github/workflows/pythonpackage.yml
 .github/workflows/pythonpublish.yml
 docs/Makefile
 docs/README.md
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
```

### Comparing `ssllabs-1.2.0/tests/conftest.py` & `ssllabs-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/tests/test_api.py` & `ssllabs-1.2.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/tests/test_data/analyze.json` & `ssllabs-1.2.1/tests/test_data/analyze.json`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/tests/test_data/endpoint.json` & `ssllabs-1.2.1/tests/test_data/endpoint.json`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/tests/test_data/root_certs.json` & `ssllabs-1.2.1/tests/test_data/root_certs.json`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/tests/test_data/status_codes.json` & `ssllabs-1.2.1/tests/test_data/status_codes.json`

 * *Files identical despite different names*

### Comparing `ssllabs-1.2.0/tests/test_ssllabs.py` & `ssllabs-1.2.1/tests/test_ssllabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,22 @@
         ), patch(
             "ssllabs.api.analyze.Analyze.get",
             new=AsyncMock(return_value=from_dict(data_class=HostData, data=request.cls.analyze)),
         ) as get:
             ssllabs = Ssllabs()
             api_data = await ssllabs.analyze(host="devolo.de")
             assert dataclasses.asdict(api_data) == request.cls.analyze
-            get.assert_called_with(host="devolo.de", ignoreMismatch="off", publish="off", startNew="on", maxAge=None)
+            get.assert_called_with(
+                host="devolo.de", ignoreMismatch="off", publish="off", startNew="on", fromCache="off", maxAge=None
+            )
             api_data = await ssllabs.analyze(host="devolo.de", from_cache=True, max_age=1)
             assert dataclasses.asdict(api_data) == request.cls.analyze
-            get.assert_called_with(host="devolo.de", ignoreMismatch="off", publish="off", startNew="off", maxAge=1)
+            get.assert_called_with(
+                host="devolo.de", ignoreMismatch="off", publish="off", startNew="off", fromCache="on", maxAge=1
+            )
 
     @pytest.mark.asyncio
     async def test_analyze_not_ready_yet(self, request, mocker):
         with patch("asyncio.sleep", new=AsyncMock()), patch(
             "ssllabs.api.info.Info.get", new=AsyncMock(return_value=from_dict(data_class=InfoData, data=request.cls.info))
         ), patch(
             "ssllabs.api.analyze.Analyze.get",
```

