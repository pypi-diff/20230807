# Comparing `tmp/thipster-0.23.6.tar.gz` & `tmp/thipster-0.23.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.23.6.tar", last modified: Fri Aug  4 12:28:43 2023, max compression
+gzip compressed data, was "thipster-0.23.7.tar", last modified: Mon Aug  7 06:48:34 2023, max compression
```

## Comparing `thipster-0.23.6.tar` & `thipster-0.23.7.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.558070 thipster-0.23.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-04 12:28:23.000000 thipster-0.23.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-04 12:28:23.000000 thipster-0.23.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-04 12:28:43.558070 thipster-0.23.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-08-04 12:28:23.000000 thipster-0.23.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-04 12:28:23.000000 thipster-0.23.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-04 12:28:23.000000 thipster-0.23.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:28:43.558070 thipster-0.23.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-04 12:28:24.000000 thipster-0.23.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.546070 thipster-0.23.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.546070 thipster-0.23.6/tests/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/engine/test_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.546070 thipster-0.23.6/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.550070 thipster-0.23.6/tests/parser/dsl_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    19038 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/test_parsedfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/test_parserfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/parser/test_yamlparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.550070 thipster-0.23.6/tests/repository/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/repository/test_github_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/repository/test_local_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/repository/test_resourcemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-08-04 12:28:23.000000 thipster-0.23.6/tests/test_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.550070 thipster-0.23.6/thipster/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.550070 thipster-0.23.6/thipster/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/auth/google.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.554070 thipster-0.23.6/thipster/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/i_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/i_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/i_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/i_terraform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/parsed_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/engine/resource_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.554070 thipster-0.23.6/thipster/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.554070 thipster-0.23.6/thipster/parser/dsl_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    24580 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/parser_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.558070 thipster-0.23.6/thipster/repository/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/repository/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/repository/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/repository/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/repository/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.558070 thipster-0.23.6/thipster/terraform/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/terraform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26119 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/terraform/cdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-04 12:28:23.000000 thipster-0.23.6/thipster/terraform/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:28:43.550070 thipster-0.23.6/thipster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-04 12:28:43.000000 thipster-0.23.6/thipster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-04 12:28:43.000000 thipster-0.23.6/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:28:43.000000 thipster-0.23.6/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-04 12:28:43.000000 thipster-0.23.6/thipster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 12:28:43.000000 thipster-0.23.6/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.552600 thipster-0.23.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-07 06:48:16.000000 thipster-0.23.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-07 06:48:16.000000 thipster-0.23.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-07 06:48:34.552600 thipster-0.23.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-08-07 06:48:16.000000 thipster-0.23.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-07 06:48:16.000000 thipster-0.23.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-07 06:48:16.000000 thipster-0.23.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 06:48:34.552600 thipster-0.23.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-07 06:48:17.000000 thipster-0.23.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.548600 thipster-0.23.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.548600 thipster-0.23.7/tests/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/engine/test_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.548600 thipster-0.23.7/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.548600 thipster-0.23.7/tests/parser/dsl_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19038 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/test_parsedfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/test_parserfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/parser/test_yamlparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.548600 thipster-0.23.7/tests/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/repository/test_github_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/repository/test_local_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/repository/test_resourcemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-08-07 06:48:16.000000 thipster-0.23.7/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.548600 thipster-0.23.7/thipster/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.552600 thipster-0.23.7/thipster/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/auth/google.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.552600 thipster-0.23.7/thipster/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/i_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/i_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/i_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/i_terraform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/parsed_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/engine/resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.552600 thipster-0.23.7/thipster/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.552600 thipster-0.23.7/thipster/parser/dsl_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23855 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/parser_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.552600 thipster-0.23.7/thipster/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/repository/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/repository/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/repository/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/repository/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.552600 thipster-0.23.7/thipster/terraform/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/terraform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26119 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/terraform/cdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-07 06:48:16.000000 thipster-0.23.7/thipster/terraform/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:48:34.548600 thipster-0.23.7/thipster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-07 06:48:34.000000 thipster-0.23.7/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-07 06:48:34.000000 thipster-0.23.7/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:48:34.000000 thipster-0.23.7/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-07 06:48:34.000000 thipster-0.23.7/thipster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-07 06:48:34.000000 thipster-0.23.7/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.23.6/LICENSE` & `thipster-0.23.7/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/PKG-INFO` & `thipster-0.23.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.23.6
+Version: 0.23.7
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.23.6 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.23.7 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.23.6/README.md` & `thipster-0.23.7/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/pyproject.toml` & `thipster-0.23.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/setup.py` & `thipster-0.23.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('requirements').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.23.6'
+__version__ = '0.23.7'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as rm:
     readme = rm.read()
```

### Comparing `thipster-0.23.6/tests/engine/test_engine.py` & `thipster-0.23.7/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/tests/engine/test_generation.py` & `thipster-0.23.7/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/tests/parser/dsl_parser/test_ast.py` & `thipster-0.23.7/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.23.7/tests/parser/dsl_parser/test_dslparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.23.7/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/tests/parser/dsl_parser/test_token.py` & `thipster-0.23.7/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.23.7/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/tests/parser/test_parsedfile.py` & `thipster-0.23.7/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/tests/parser/test_parserfactory.py` & `thipster-0.23.7/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/tests/parser/test_yamlparser.py` & `thipster-0.23.7/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/tests/repository/test_github_repository.py` & `thipster-0.23.7/tests/repository/test_github_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/tests/repository/test_local_repository.py` & `thipster-0.23.7/tests/repository/test_local_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/tests/repository/test_resourcemodel.py` & `thipster-0.23.7/tests/repository/test_resourcemodel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/tests/test_e2e.py` & `thipster-0.23.7/tests/test_e2e.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
         tf.setup()
         try:
             tf.apply()
             yield tf.output()
         except Exception as e:
             raise e
-
         finally:
             tf.destroy()
 
     return _apply_output
 
 
 @pytest.fixture
```

### Comparing `thipster-0.23.6/tests/test_tools.py` & `thipster-0.23.7/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/auth/google.py` & `thipster-0.23.7/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/engine/engine.py` & `thipster-0.23.7/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/engine/i_parser.py` & `thipster-0.23.7/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/engine/i_repository.py` & `thipster-0.23.7/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/engine/i_terraform.py` & `thipster-0.23.7/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/engine/parsed_file.py` & `thipster-0.23.7/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/engine/resource_model.py` & `thipster-0.23.7/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/helpers.py` & `thipster-0.23.7/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/parser/dsl_parser/ast.py` & `thipster-0.23.7/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.23.7/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.23.7/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/parser/dsl_parser/lexer.py` & `thipster-0.23.7/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.23.7/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/parser/dsl_parser/parser.py` & `thipster-0.23.7/thipster/parser/dsl_parser/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module that contains the THipster DSL Parser."""
 import os
 from pathlib import Path
 
 from thipster.engine import ParserPort
 from thipster.engine.parsed_file import ParsedFile
 
-from .exceptions import DSLParserBaseError, DSLParserPathNotFoundError
+from .exceptions import DSLParserPathNotFoundError
 from .interpreter import Interpreter
 from .lexer import Lexer
 from .token_parser import TokenParser
 
 
 class DSLParser(ParserPort):
     """Parser for the THipster's DSL."""
@@ -59,21 +59,15 @@
             Path to run the parser into
 
         Returns
         -------
         ParsedFile
             A ParsedFile object with the content of all the files in the input path
         """
-        try:
-            files = DSLParser.__getfiles(path)
-            lexer = Lexer(files)
-            token_list = lexer.run()
-            parser = TokenParser(token_list)
-            ast = parser.run()
-
-            interpreter = Interpreter()
-            return interpreter.run(ast)
-
-        except DSLParserBaseError as e:
-            raise e
-        except Exception as e:
-            raise e
+        files = DSLParser.__getfiles(path)
+        lexer = Lexer(files)
+        token_list = lexer.run()
+        parser = TokenParser(token_list)
+        ast = parser.run()
+
+        interpreter = Interpreter()
+        return interpreter.run(ast)
```

### Comparing `thipster-0.23.6/thipster/parser/dsl_parser/token.py` & `thipster-0.23.7/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.23.7/thipster/parser/dsl_parser/token_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,35 +23,33 @@
         """
         self.__tokens = tokens
 
     def run(self) -> ast.FileNode:
         """Run the parser."""
         self.__rm_empty_lines()
         file_node = ast.FileNode()
-        try:
+
+        self.__trim_newlines()
+        while self.__get_next_type() != TT.EOF:
             self.__trim_newlines()
-            while self.__get_next_type() != TT.EOF:
-                self.__trim_newlines()
 
-                match self.__get_next_type():
-                    case TT.VAR:
-                        file_node.variables.append(
-                            self.__get_assignment(),
-                        )
-                    case TT.STRING:
-                        file_node.resources.append(self.__create_resource())
-                    case TT.OUTPUT:
-                        self.__get_outputs(file_node)
-                    case _:
-                        raise DSLSyntaxError(
-                            self.__next(), [TT.VAR, TT.STRING, TT.OUTPUT],
-                        )
-                self.__trim_newlines()
-        except Exception as e:
-            raise e
+            match self.__get_next_type():
+                case TT.VAR:
+                    file_node.variables.append(
+                        self.__get_assignment(),
+                    )
+                case TT.STRING:
+                    file_node.resources.append(self.__create_resource())
+                case TT.OUTPUT:
+                    self.__get_outputs(file_node)
+                case _:
+                    raise DSLSyntaxError(
+                        self.__next(), [TT.VAR, TT.STRING, TT.OUTPUT],
+                    )
+            self.__trim_newlines()
 
         return file_node
 
     def __next(self, expected: TT | list[TT] | None = None) -> Token:
         """Get next token and pop it from the list.
 
         Parameters
@@ -226,36 +224,30 @@
             )
 
     def __get_parameter(self, indent: int) -> ast.ParameterNode:
         r"""Create an AST Parameter node.
 
         Format: name, ":", (value, [if_else_ctrl] | [if_ctrl], "\\n", (list | dict)).
         """
-        try:
-            name = self.__next(TT.STRING)
-            self.__get_whitespaces()
-            self.__next(TT.COLON)
-            self.__get_whitespaces()
-        except DSLSyntaxError as e:
-            raise e
+        name = self.__next(TT.STRING)
+        self.__get_whitespaces()
+        self.__next(TT.COLON)
+        self.__get_whitespaces()
 
         next_token_type = self.__get_next_type()
 
         if next_token_type not in [
             TT.IF,
             TT.NEWLINE,
         ]:
             # value, [if_else_ctrl]
-            try:
-                value = self.__get_value()
-                self.__get_whitespaces()
-                if_else_ctrl = self.__get_if_else_ctrl()
-                self.__get_whitespaces()
-            except:
-                raise
+            value = self.__get_value()
+            self.__get_whitespaces()
+            if_else_ctrl = self.__get_if_else_ctrl()
+            self.__get_whitespaces()
 
             parameter = ast.ParameterNode(
                 name=ast.StringNode(name),
                 value=value,
             )
 
             if if_else_ctrl:
@@ -325,49 +317,46 @@
     def __get_list(self, indent: int, check_small_indent=True) -> ast.ListNode:
         """Create an AST List node.
 
         Format: { "-", (value, [if_else_ctrl], [amt_ctrl], NEWLINE | dict) }.
         """
         list_items = []
 
-        try:
-            small_indent = indent-1 if check_small_indent else indent
-            while self.__get_tabs(small_indent):
-                if not self.__check(TT.MINUS):
-                    if not check_small_indent:
-                        raise DSLSyntaxError(self.__next(), TT.TAB)
-                    small_indent = indent
-                    self.__next(TT.TAB)
-                    self.__next(TT.MINUS)
-                check_small_indent = False
-                self.__next(TT.WHITESPACE)
-                self.__get_whitespaces()
+        small_indent = indent-1 if check_small_indent else indent
+        while self.__get_tabs(small_indent):
+            if not self.__check(TT.MINUS):
+                if not check_small_indent:
+                    raise DSLSyntaxError(self.__next(), TT.TAB)
+                small_indent = indent
+                self.__next(TT.TAB)
+                self.__next(TT.MINUS)
+            check_small_indent = False
+            self.__next(TT.WHITESPACE)
+            self.__get_whitespaces()
 
-                value = self.__get_dict(indent+1, no_indent_first=True)\
-                    if self.__check_dict() else self.__get_value()
-                self.__get_whitespaces()
+            value = self.__get_dict(indent+1, no_indent_first=True)\
+                if self.__check_dict() else self.__get_value()
+            self.__get_whitespaces()
 
-                if_else_ctrl = self.__get_if_else_ctrl()
-                self.__get_whitespaces()
-                amount_ctrl = self.__get_nb_ctrl()
-                self.__get_whitespaces()
+            if_else_ctrl = self.__get_if_else_ctrl()
+            self.__get_whitespaces()
+            amount_ctrl = self.__get_nb_ctrl()
+            self.__get_whitespaces()
+
+            if if_else_ctrl:
+                if_else_ctrl.if_case = value
+                value = if_else_ctrl
 
-                if if_else_ctrl:
-                    if_else_ctrl.if_case = value
-                    value = if_else_ctrl
-
-                if amount_ctrl:
-                    amount_ctrl.node = value
-                    value = amount_ctrl
+            if amount_ctrl:
+                amount_ctrl.node = value
+                value = amount_ctrl
 
-                list_items.append(value)
+            list_items.append(value)
 
-                self.__get_newline()
-        except Exception as e:
-            raise e
+            self.__get_newline()
 
         self.__tokens.insert(
             0, Token(
                 position=self.__tokens[0].position,
                 token_type=TT.NEWLINE,
             ),
         )
@@ -420,23 +409,20 @@
     def __get_dict(self, indent: int, no_indent_first=False) -> ast.DictNode:
         """Create an AST Dict node.
 
         Format: { parameter, NEWLINE }.
         """
         parameters = []
 
-        try:
-            while self.__get_tabs(indent) or no_indent_first:
-                self.__get_whitespaces()
-                parameters.append(self.__get_parameter(indent))
-                self.__get_whitespaces()
-                self.__get_newline()
-                no_indent_first = False
-        except Exception as e:
-            raise e
+        while self.__get_tabs(indent) or no_indent_first:
+            self.__get_whitespaces()
+            parameters.append(self.__get_parameter(indent))
+            self.__get_whitespaces()
+            self.__get_newline()
+            no_indent_first = False
 
         self.__tokens.insert(
             0, Token(
                 position=self.__tokens[0].position,
                 token_type=TT.NEWLINE,
             ),
         )
@@ -444,28 +430,25 @@
         return ast.DictNode(parameters)
 
     def __get_nb_ctrl(self) -> ast.AmountNode | None:
         """Create an AST Amount node.
 
         Format: "amount", ":", int, ["#", var].
         """
-        try:
-            amount_token = self.__check(TT.AMOUNT)
-            if not amount_token:
-                return None
+        amount_token = self.__check(TT.AMOUNT)
+        if not amount_token:
+            return None
 
-            self.__get_whitespaces()
-            self.__next(TT.COLON)
+        self.__get_whitespaces()
+        self.__next(TT.COLON)
 
-            self.__get_whitespaces()
-            amount = self.__get_value()
+        self.__get_whitespaces()
+        amount = self.__get_value()
 
-            self.__get_whitespaces()
-        except DSLSyntaxError as e:
-            raise e
+        self.__get_whitespaces()
 
         amount_variable = self.__check(TT.VAR)
 
         return ast.AmountNode(
             position=amount_token,
             amount=amount,
             variable=ast.VariableDefinitionNode(
@@ -483,19 +466,16 @@
         Format: "if", condition.
         """
         condition = self.__check(TT.IF)
         if not condition:
             return None
 
         self.__get_whitespaces()
-        try:
-            condition = self.__get_comp_expr()
-            self.__get_whitespaces()
-        except DSLSyntaxError as e:
-            raise e
+        condition = self.__get_comp_expr()
+        self.__get_whitespaces()
 
         return ast.IfNode(
             condition=condition,
             if_case=None,
         )
 
     def __get_if_else_ctrl(self) -> ast.IfElseNode | None:
```

### Comparing `thipster-0.23.6/thipster/parser/exceptions.py` & `thipster-0.23.7/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/parser/parser_factory.py` & `thipster-0.23.7/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/parser/yaml_parser.py` & `thipster-0.23.7/thipster/parser/yaml_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,38 +86,31 @@
             Path to run the parser into
 
         Returns
         -------
         ParsedFile
             A ParsedFile object with the content of all the files in the input path
         """
-        try:
-            files = cls.__getfiles(path)
-            parsed_file = pf.ParsedFile()
-
-            for file in files:
-                filedir, filename = os.path.split(file)
-
-                environment = Environment(
-                    loader=FileSystemLoader(filedir),
-                    autoescape=True,
-                )
-                template = environment.get_template(filename)
-                rendered = template.render()
-                content = yaml.safe_load(rendered)
-
-                parsed_file.resources += cls.__convert(content)
-
-            return parsed_file
-        except yaml.YAMLError as exc:
-            raise exc
-        except YAMLParserBaseError as e:
-            raise e
-        except Exception as e:
-            raise e
+        files = cls.__getfiles(path)
+        parsed_file = pf.ParsedFile()
+
+        for file in files:
+            filedir, filename = os.path.split(file)
+
+            environment = Environment(
+                loader=FileSystemLoader(filedir),
+                autoescape=True,
+            )
+            template = environment.get_template(filename)
+            rendered = template.render()
+            content = yaml.safe_load(rendered)
+
+            parsed_file.resources += cls.__convert(content)
+
+        return parsed_file
 
     @classmethod
     def __convert(cls, file: dict) -> list[pf.ParsedResource]:
         """Convert a dictionnary into a list of ParsedResources.
 
         Parameters
         ----------
```

### Comparing `thipster-0.23.6/thipster/repository/exceptions.py` & `thipster-0.23.7/thipster/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/repository/github.py` & `thipster-0.23.7/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/repository/json.py` & `thipster-0.23.7/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/repository/local.py` & `thipster-0.23.7/thipster/repository/local.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/terraform/cdk.py` & `thipster-0.23.7/thipster/terraform/cdk.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster/terraform/exceptions.py` & `thipster-0.23.7/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.6/thipster.egg-info/PKG-INFO` & `thipster-0.23.7/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.23.6
+Version: 0.23.7
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.23.6 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.23.7 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.23.6/thipster.egg-info/SOURCES.txt` & `thipster-0.23.7/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

