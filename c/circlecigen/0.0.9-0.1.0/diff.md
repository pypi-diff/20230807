# Comparing `tmp/circlecigen-0.0.9.tar.gz` & `tmp/circlecigen-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circlecigen-0.0.9.tar", last modified: Thu Jun 29 20:41:44 2023, max compression
+gzip compressed data, was "circlecigen-0.1.0.tar", last modified: Mon Aug  7 00:22:42 2023, max compression
```

## Comparing `circlecigen-0.0.9.tar` & `circlecigen-0.1.0.tar`

### file list

```diff
@@ -1,61 +1,67 @@
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:44.124463 circlecigen-0.0.9/
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:44.120463 circlecigen-0.0.9/.circleci/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3995 2023-06-29 20:41:39.000000 circlecigen-0.0.9/.circleci/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-06-29 20:41:39.000000 circlecigen-0.0.9/.codeclimate.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-29 20:41:39.000000 circlecigen-0.0.9/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-06-29 20:41:39.000000 circlecigen-0.0.9/.pre-commit-config.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-06-29 20:41:39.000000 circlecigen-0.0.9/.pylintrc
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-06-29 20:41:39.000000 circlecigen-0.0.9/.python-version
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-06-29 20:41:39.000000 circlecigen-0.0.9/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26085 2023-06-29 20:41:44.124463 circlecigen-0.0.9/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2023-06-29 20:41:39.000000 circlecigen-0.0.9/Pipfile
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25450 2023-06-29 20:41:39.000000 circlecigen-0.0.9/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:39.000000 circlecigen-0.0.9/__init__.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:44.120463 circlecigen-0.0.9/circlecigen.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26085 2023-06-29 20:41:44.000000 circlecigen-0.0.9/circlecigen.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1224 2023-06-29 20:41:44.000000 circlecigen-0.0.9/circlecigen.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-29 20:41:44.000000 circlecigen-0.0.9/circlecigen.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2023-06-29 20:41:44.000000 circlecigen-0.0.9/circlecigen.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2023-06-29 20:41:44.000000 circlecigen-0.0.9/circlecigen.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2023-06-29 20:41:44.000000 circlecigen-0.0.9/circlecigen.egg-info/top_level.txt
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:44.120463 circlecigen-0.0.9/env_test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      370 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/custom.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/default.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/dev.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6273 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/multi.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      147 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/nonprod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      147 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/nonprod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/nonprod.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      593 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/post-approve.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      315 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/pre-approve.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/prod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/prod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/prod.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3684 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/template_generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      313 2023-06-29 20:41:39.000000 circlecigen-0.0.9/notes.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-06-29 20:41:39.000000 circlecigen-0.0.9/op.env
--rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-06-29 20:41:39.000000 circlecigen-0.0.9/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-06-29 20:41:39.000000 circlecigen-0.0.9/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-29 20:41:44.124463 circlecigen-0.0.9/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      847 2023-06-29 20:41:39.000000 circlecigen-0.0.9/setup.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:44.120463 circlecigen-0.0.9/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:39.000000 circlecigen-0.0.9/src/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-06-29 20:41:44.000000 circlecigen-0.0.9/src/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3028 2023-06-29 20:41:39.000000 circlecigen-0.0.9/src/circlecigen.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6770 2023-06-29 20:41:39.000000 circlecigen-0.0.9/src/template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2430 2023-06-29 20:41:39.000000 circlecigen-0.0.9/src/tfvars.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-06-29 20:41:39.000000 circlecigen-0.0.9/src/utils.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:44.124463 circlecigen-0.0.9/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6273 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/generated_config_setup.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      147 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/nonprod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      147 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/nonprod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/prod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/prod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3684 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/template_generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2536 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/test_circlecigen.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3444 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/test_template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2340 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/test_tfvars.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1490 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/test_utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-07 00:22:42.265418 circlecigen-0.1.0/
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-07 00:22:42.261418 circlecigen-0.1.0/.circleci/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3995 2023-08-07 00:22:36.000000 circlecigen-0.1.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-08-07 00:22:36.000000 circlecigen-0.1.0/.codeclimate.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      157 2023-08-07 00:22:36.000000 circlecigen-0.1.0/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-08-07 00:22:36.000000 circlecigen-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-08-07 00:22:36.000000 circlecigen-0.1.0/.pylintrc
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-08-07 00:22:36.000000 circlecigen-0.1.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26085 2023-08-07 00:22:42.265418 circlecigen-0.1.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2023-08-07 00:22:36.000000 circlecigen-0.1.0/Pipfile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25450 2023-08-07 00:22:36.000000 circlecigen-0.1.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-07 00:22:36.000000 circlecigen-0.1.0/__init__.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-07 00:22:42.261418 circlecigen-0.1.0/circlecigen.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26085 2023-08-07 00:22:42.000000 circlecigen-0.1.0/circlecigen.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1393 2023-08-07 00:22:42.000000 circlecigen-0.1.0/circlecigen.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-08-07 00:22:42.000000 circlecigen-0.1.0/circlecigen.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2023-08-07 00:22:42.000000 circlecigen-0.1.0/circlecigen.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2023-08-07 00:22:42.000000 circlecigen-0.1.0/circlecigen.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2023-08-07 00:22:42.000000 circlecigen-0.1.0/circlecigen.egg-info/top_level.txt
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-07 00:22:42.261418 circlecigen-0.1.0/env_test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      370 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/custom.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/default.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/dev.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6273 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/multi.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      147 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/nonprod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      147 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/nonprod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/nonprod.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      593 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/post-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      315 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/pre-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/prod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/prod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/prod.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3684 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test/template_generated_config.yml
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-07 00:22:42.261418 circlecigen-0.1.0/env_test_role/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test_role/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      230 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test_role/post-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      183 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test_role/pre-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3316 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test_role/role_generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      193 2023-08-07 00:22:36.000000 circlecigen-0.1.0/env_test_role/versions.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      313 2023-08-07 00:22:36.000000 circlecigen-0.1.0/notes.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-08-07 00:22:36.000000 circlecigen-0.1.0/op.env
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-08-07 00:22:36.000000 circlecigen-0.1.0/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      366 2023-08-07 00:22:36.000000 circlecigen-0.1.0/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-08-07 00:22:42.265418 circlecigen-0.1.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      847 2023-08-07 00:22:36.000000 circlecigen-0.1.0/setup.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-07 00:22:42.265418 circlecigen-0.1.0/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-08-07 00:22:36.000000 circlecigen-0.1.0/src/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-08-07 00:22:42.000000 circlecigen-0.1.0/src/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3181 2023-08-07 00:22:36.000000 circlecigen-0.1.0/src/circlecigen.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7824 2023-08-07 00:22:36.000000 circlecigen-0.1.0/src/template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2430 2023-08-07 00:22:36.000000 circlecigen-0.1.0/src/tfvars.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-08-07 00:22:36.000000 circlecigen-0.1.0/src/utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-07 00:22:42.265418 circlecigen-0.1.0/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6273 2023-08-07 00:22:36.000000 circlecigen-0.1.0/test/generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2023-08-07 00:22:36.000000 circlecigen-0.1.0/test/generated_config_setup.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      147 2023-08-07 00:22:36.000000 circlecigen-0.1.0/test/nonprod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      147 2023-08-07 00:22:36.000000 circlecigen-0.1.0/test/nonprod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-08-07 00:22:36.000000 circlecigen-0.1.0/test/prod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-08-07 00:22:36.000000 circlecigen-0.1.0/test/prod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3316 2023-08-07 00:22:36.000000 circlecigen-0.1.0/test/role_generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3684 2023-08-07 00:22:36.000000 circlecigen-0.1.0/test/template_generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2536 2023-08-07 00:22:36.000000 circlecigen-0.1.0/test/test_circlecigen.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4231 2023-08-07 00:22:36.000000 circlecigen-0.1.0/test/test_template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2340 2023-08-07 00:22:36.000000 circlecigen-0.1.0/test/test_tfvars.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1490 2023-08-07 00:22:36.000000 circlecigen-0.1.0/test/test_utils.py
```

### Comparing `circlecigen-0.0.9/.circleci/config.yml` & `circlecigen-0.1.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/.pre-commit-config.yaml` & `circlecigen-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/.pylintrc` & `circlecigen-0.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/LICENSE` & `circlecigen-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/PKG-INFO` & `circlecigen-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circlecigen
-Version: 0.0.9
+Version: 0.1.0
 Summary: Opinionated generation of continuation pipelines
 Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
 Author: Nic Cheneweth
 Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
 Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
 Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: circlecigen Version: 0.0.9 Summary: Opinionated
+Metadata-Version: 2.1 Name: circlecigen Version: 0.1.0 Summary: Opinionated
 generation of continuation pipelines Home-page: https://github.com/
 ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
 thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
 circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
 circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `circlecigen-0.0.9/README.md` & `circlecigen-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/circlecigen.egg-info/PKG-INFO` & `circlecigen-0.1.0/circlecigen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circlecigen
-Version: 0.0.9
+Version: 0.1.0
 Summary: Opinionated generation of continuation pipelines
 Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
 Author: Nic Cheneweth
 Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
 Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
 Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: circlecigen Version: 0.0.9 Summary: Opinionated
+Metadata-Version: 2.1 Name: circlecigen Version: 0.1.0 Summary: Opinionated
 generation of continuation pipelines Home-page: https://github.com/
 ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
 thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
 circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
 circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `circlecigen-0.0.9/circlecigen.egg-info/SOURCES.txt` & `circlecigen-0.1.0/circlecigen.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 .codeclimate.yml
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
-.python-version
 LICENSE
 Pipfile
 README.md
 __init__.py
 notes.txt
 op.env
 pyproject.toml
@@ -30,24 +29,30 @@
 env_test/nonprod.json
 env_test/post-approve.yml
 env_test/pre-approve.yml
 env_test/prod-us-east-2.tfvars.json
 env_test/prod-us-west-2.tfvars.json
 env_test/prod.json
 env_test/template_generated_config.yml
+env_test_role/config.yml
+env_test_role/post-approve.yml
+env_test_role/pre-approve.yml
+env_test_role/role_generated_config.yml
+env_test_role/versions.json
 src/__init__.py
 src/_version.py
 src/circlecigen.py
 src/template.py
 src/tfvars.py
 src/utils.py
 test/generated_config.yml
 test/generated_config_setup.yml
 test/nonprod-us-east-2.tfvars.json
 test/nonprod-us-west-2.tfvars.json
 test/prod-us-east-2.tfvars.json
 test/prod-us-west-2.tfvars.json
+test/role_generated_config.yml
 test/template_generated_config.yml
 test/test_circlecigen.py
 test/test_template.py
 test/test_tfvars.py
 test/test_utils.py
```

### Comparing `circlecigen-0.0.9/env_test/config.yml` & `circlecigen-0.1.0/env_test/config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/env_test/generated_config.yml` & `circlecigen-0.1.0/env_test/generated_config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/env_test/multi.json` & `circlecigen-0.1.0/env_test/multi.json`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/env_test/post-approve.yml` & `circlecigen-0.1.0/env_test/post-approve.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/env_test/template_generated_config.yml` & `circlecigen-0.1.0/env_test/template_generated_config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/pyproject.toml` & `circlecigen-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/setup.py` & `circlecigen-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/src/circlecigen.py` & `circlecigen-0.1.0/src/circlecigen.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,18 @@
     help="Generate tfvars.json files for all role/instances. Default is true")
 @click.option("--workflow", default="continuation-generated-workflow",
     help="Name for generated config. Default continuation-generated-workflow",
     callback=validate_filename_arg)
 @click.option("--pipepath", default=".circleci",
     help="Override default config.yml location for testing",
     callback=validate_filepath_arg)
+@click.option("--roleonly", default=True,
+    help="Generate pipeline for role only workflow. Default is false")
 @click.argument('pipeline', nargs=1)
-def cli(pipeline, outfile, envpath, multifile, defaultparams, tfvars, workflow, pipepath, template):
+def cli(pipeline, outfile, envpath, multifile, defaultparams, tfvars, workflow, pipepath, template, roleonly):
     """
 
     Inputs 
 
       .circleci/pre_approve.yml
       .circleci/post_approve.yml
       .circleci/custom_template.yml (optional)
@@ -75,9 +77,10 @@
         click.echo("Not generating tfvars.json files")
     generate_config(pipeline,
                     pipepath,
                     outfile,
                     envpath,
                     read_json_file(envpath, multifile),
                     workflow,
-                    template
+                    template,
+                    roleonly
                     )
```

### Comparing `circlecigen-0.0.9/src/template.py` & `circlecigen-0.1.0/src/template.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """
 
 PRIOR_APPROVAL="""
           requires:
             - approve {} changes
 """
 
-def generate_config(use_pipeline, pipepath, outfile, envpath, environs, workflow, template):
+def generate_config(use_pipeline, pipepath, outfile, envpath, environs, workflow, template, roleonly):
     """create generated_config.yaml for continuation orb"""
 
     # use the specified filter to generate a pipeline only for the desired trigger
     pipeline = environs[use_pipeline]
 
     # copy everything but the jobs and workflows from config.yml into generated_config.yml
     # pipepath = where to find config.yml, default .circleci
@@ -44,82 +44,105 @@
     approve_vars["filter"] = pipeline["filter"]
 
     # all pre-approval jobs created accept for the first role must wait for
     # the prior role approval set this as blank to start then populate
     # with the list of all instance plans jobs in the role
     priorapprovalrequired = ""
     approvalrequiredjobs = ""
-
     # open the outfile for appeand and start processing roles/instances
     with open(f"{pipepath}/{outfile}", 'a', encoding="utf-8") as f:
         for role in pipeline:
             # skip the filter definition
             if role == "filter":
                 continue
 
             if custom:
                 generate_custom_jobs(f, envpath, custom, pipeline, role)
             else:
                 # when the approval template is generated, it must be populated with
                 # a list of all instances for which a pre-approval template will be
                 # generated. That is returned by this job.
-                approvalrequiredjobs = generate_pre_approval_jobs(f, envpath, pre, pipeline, role, priorapprovalrequired)
+                approvalrequiredjobs = generate_pre_approval_jobs(f, envpath, pre, pipeline, role, roleonly, priorapprovalrequired)
 
                 # generate approval job for the current role, a human will trigger the post- phase
                 generate_approval_jobs(f, approve, approve_vars, approvalrequiredjobs, role)
-                generate_post_approval_jobs(f, envpath, post, pipeline, role)
+                generate_post_approval_jobs(f, envpath, post, pipeline, role, roleonly)
 
                 # record the current role, to provide 'requires:' list in any subsequent pre- jobs
                 priorapprovalrequired = role
 
-def generate_pre_approval_jobs(f, envpath, pre, pipeline, role, priorapprovalrequired):
-    # generate a pre-approval job for each instance in the role,
+def generate_pre_approval_jobs(f, envpath, pre, pipeline, role, roleonly, priorapprovalrequired):
+    # generate a pre-approval job for each instance in the role, or for each role if roleonly
     # if a pre-approval.yml file exists
     if pre:
         approvalrequiredjobs = "requires:"
-        for instance in pipeline[role]:
-            instance_vars=read_json_file(envpath, f"{instance}.tfvars.json")
-            instance_vars.update({
+        if roleonly:
+            role_vars=read_json_file(envpath, "versions.json")
+            role_vars.update({
                 "filters": pipeline["filter"],
                 "role": role,
                 "envpath": envpath
             })
             if priorapprovalrequired:
-                instance_vars.update({
+                role_vars.update({
                     "priorapprovalrequired": PRIOR_APPROVAL.format(priorapprovalrequired)
                 })
-            approvalrequiredjobs += f"\n            - plan {instance} change"
-            f.write(pre.render(instance_vars))
+            approvalrequiredjobs += f"\n            - plan {role} change"
+            f.write(pre.render(role_vars))
+        else:
+            for instance in pipeline[role]:
+                instance_vars=read_json_file(envpath, f"{instance}.tfvars.json")
+                instance_vars.update({
+                    "filters": pipeline["filter"],
+                    "role": role,
+                    "envpath": envpath
+                })
+                if priorapprovalrequired:
+                    instance_vars.update({
+                        "priorapprovalrequired": PRIOR_APPROVAL.format(priorapprovalrequired)
+                    })
+                approvalrequiredjobs += f"\n            - plan {instance} change"
+                f.write(pre.render(instance_vars))
 
         if priorapprovalrequired:
-            for prior_role_instance in pipeline[priorapprovalrequired].keys():
-                approvalrequiredjobs += f"\n            - apply {prior_role_instance} change plan"
+            if not roleonly:
+                for prior_role_instance in pipeline[priorapprovalrequired].keys():
+                    approvalrequiredjobs += f"\n            - apply {prior_role_instance} change plan"
 
         return approvalrequiredjobs
     return None
 
 def generate_approval_jobs(f, approve, approve_vars, approvalrequiredjobs, role):
     approve_vars.update ({
         "role": role,
         "approvalrequiredjobs": approvalrequiredjobs
     })
     f.write(approve.render(approve_vars))
 
-def generate_post_approval_jobs(f, envpath, post, pipeline, role):
+def generate_post_approval_jobs(f, envpath, post, pipeline, role, roleonly):
     # generate a post-approval job for each instance in the role,
     # if a post-approval.yml file exists
     if post:
-        for instance in pipeline[role]:
-            instance_vars=read_json_file(envpath, f"{instance}.tfvars.json")
-            instance_vars.update({
+        if roleonly:
+            role_vars=read_json_file(envpath, "versions.json")
+            role_vars.update({
                 "filters": pipeline["filter"],
                 "role": role,
                 "envpath": envpath
             })
-            f.write(post.render(instance_vars))
+            f.write(post.render(role_vars))
+        else:
+            for instance in pipeline[role]:
+                instance_vars=read_json_file(envpath, f"{instance}.tfvars.json")
+                instance_vars.update({
+                    "filters": pipeline["filter"],
+                    "role": role,
+                    "envpath": envpath
+                })
+                f.write(post.render(instance_vars))
 
 
 def generate_custom_jobs(f, envpath, custom, pipeline, role):
     # generate a custom job for each instance in the role,
     # if a custom template file (specified by the --template flag) exists
     for instance in pipeline[role]:
         instance_vars=read_json_file(envpath, f"{instance}.tfvars.json")
```

### Comparing `circlecigen-0.0.9/src/tfvars.py` & `circlecigen-0.1.0/src/tfvars.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/src/utils.py` & `circlecigen-0.1.0/src/utils.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/test/generated_config.yml` & `circlecigen-0.1.0/test/generated_config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/test/generated_config_setup.yml` & `circlecigen-0.1.0/test/generated_config_setup.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/test/template_generated_config.yml` & `circlecigen-0.1.0/test/template_generated_config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/test/test_circlecigen.py` & `circlecigen-0.1.0/test/test_circlecigen.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/test/test_template.py` & `circlecigen-0.1.0/test/test_template.py`

 * *Files 17% similar despite different names*

```diff
@@ -78,30 +78,48 @@
 def test_generate_config():
     mock_pipeline = "release"
     mock_pipepath = "env_test"
     mock_envpath = "env_test"
     mock_outfile = "generated_config.yml"
     mock_workflow = "continuation-generated-workflow"
     mock_template = None
+    mock_roleonly = False
 
-    generate_config(mock_pipeline, mock_pipepath, mock_outfile, mock_envpath, mock_multi, mock_workflow, mock_template)
+    generate_config(mock_pipeline, mock_pipepath, mock_outfile, mock_envpath, mock_multi, mock_workflow, mock_template, mock_roleonly)
     assert os.path.isfile(os.path.join(mock_pipepath, mock_outfile))
     assert filecmp.cmp(os.path.join(mock_pipepath,
                        mock_outfile),
                        os.path.join("test",
                        mock_outfile))
 
 
 def test_generate_config_with_custom_template():
     mock_pipeline = "release"
     mock_pipepath = "env_test"
     mock_envpath = "env_test"
     mock_outfile = "template_generated_config.yml"
     mock_workflow = "continuation-generated-workflow"
     mock_template = "custom.yml"
+    mock_roleonly = False
 
-    generate_config(mock_pipeline, mock_pipepath, mock_outfile, mock_envpath, mock_multi, mock_workflow, mock_template)
+    generate_config(mock_pipeline, mock_pipepath, mock_outfile, mock_envpath, mock_multi, mock_workflow, mock_template, mock_roleonly)
+    assert os.path.isfile(os.path.join(mock_pipepath, mock_outfile))
+    assert filecmp.cmp(os.path.join(mock_pipepath,
+                                    mock_outfile),
+                       os.path.join("test",
+                                    mock_outfile))
+
+def test_generate_config_with_roleonly():
+    mock_pipeline = "release"
+    mock_pipepath = "env_test_role"
+    mock_envpath = "env_test_role"
+    mock_outfile = "role_generated_config.yml"
+    mock_workflow = "continuation-generated-workflow"
+    mock_template = "custom.yml"
+    mock_roleonly = True
+
+    generate_config(mock_pipeline, mock_pipepath, mock_outfile, mock_envpath, mock_multi, mock_workflow, mock_template, mock_roleonly)
     assert os.path.isfile(os.path.join(mock_pipepath, mock_outfile))
     assert filecmp.cmp(os.path.join(mock_pipepath,
                                     mock_outfile),
                        os.path.join("test",
                                     mock_outfile))
```

### Comparing `circlecigen-0.0.9/test/test_tfvars.py` & `circlecigen-0.1.0/test/test_tfvars.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.9/test/test_utils.py` & `circlecigen-0.1.0/test/test_utils.py`

 * *Files identical despite different names*

