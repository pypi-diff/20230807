# Comparing `tmp/python_jsonschema_objects-0.4.3.tar.gz` & `tmp/python_jsonschema_objects-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_jsonschema_objects-0.4.3.tar", last modified: Thu Aug  3 13:46:29 2023, max compression
+gzip compressed data, was "python_jsonschema_objects-0.4.4.tar", last modified: Mon Aug  7 00:02:02 2023, max compression
```

## Comparing `python_jsonschema_objects-0.4.3.tar` & `python_jsonschema_objects-0.4.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:46:29.600027 python_jsonschema_objects-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-03 13:46:29.600027 python_jsonschema_objects-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/development.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:46:29.592027 python_jsonschema_objects-0.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/docs/Introduction.md
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/docs/apidoc.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:46:29.600027 python_jsonschema_objects-0.4.3/python_jsonschema_objects/
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-03 13:46:29.600027 python_jsonschema_objects-0.4.3/python_jsonschema_objects/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    27287 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects/classbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects/descriptors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:46:29.596027 python_jsonschema_objects-0.4.3/python_jsonschema_objects/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects/markdown_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects/pattern_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects/wrapper_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:46:29.596027 python_jsonschema_objects-0.4.3/python_jsonschema_objects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-03 13:46:29.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-08-03 13:46:29.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 13:46:29.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 13:46:29.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-03 13:46:29.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 13:46:29.000000 python_jsonschema_objects-0.4.3/python_jsonschema_objects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-03 13:46:29.600027 python_jsonschema_objects-0.4.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2075 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:46:29.600027 python_jsonschema_objects-0.4.3/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:46:29.600027 python_jsonschema_objects-0.4.3/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/resources/query.json
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/resources/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_array_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_circular_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_default_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_feature_151.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_feature_177.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_nested_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_nondefault_resolver_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_pattern_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    14710 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_pytest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_114.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_126.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_133.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_143.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_156.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_165.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_17.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_185.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_208.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_213.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_214.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_232.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_49.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_8.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_87.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_88.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_89.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_regression_90.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_util_pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/test_wrong_exception_protocolbase_getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/thing-one.json
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/test/thing-two.json
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)    62474 2023-08-03 13:46:25.000000 python_jsonschema_objects-0.4.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:02:02.647560 python_jsonschema_objects-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-07 00:02:02.647560 python_jsonschema_objects-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/development.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:02:02.639560 python_jsonschema_objects-0.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/docs/Introduction.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/docs/apidoc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:02:02.651560 python_jsonschema_objects-0.4.4/python_jsonschema_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-07 00:02:02.651560 python_jsonschema_objects-0.4.4/python_jsonschema_objects/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27287 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects/classbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects/descriptors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:02:02.643560 python_jsonschema_objects-0.4.4/python_jsonschema_objects/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects/markdown_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects/pattern_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects/wrapper_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:02:02.643560 python_jsonschema_objects-0.4.4/python_jsonschema_objects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-07 00:02:02.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-08-07 00:02:02.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 00:02:02.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 00:02:02.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-07 00:02:02.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 00:02:02.000000 python_jsonschema_objects-0.4.4/python_jsonschema_objects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-07 00:02:02.651560 python_jsonschema_objects-0.4.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2074 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:02:02.647560 python_jsonschema_objects-0.4.4/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:02:02.647560 python_jsonschema_objects-0.4.4/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/resources/query.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/resources/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_array_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_circular_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_feature_151.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_feature_177.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_nested_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_nondefault_resolver_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_pattern_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14710 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_pytest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_114.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_126.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_133.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_143.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_156.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_165.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_185.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_208.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_213.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_214.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_232.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_49.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_87.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_88.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_89.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_regression_90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_util_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/test_wrong_exception_protocolbase_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/thing-one.json
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/test/thing-two.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    62474 2023-08-07 00:01:52.000000 python_jsonschema_objects-0.4.4/versioneer.py
```

### Comparing `python_jsonschema_objects-0.4.3/LICENSE` & `python_jsonschema_objects-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/PKG-INFO` & `python_jsonschema_objects-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python_jsonschema_objects
-Version: 0.4.3
+Version: 0.4.4
 Summary: An object wrapper for JSON Schema definitions
 Home-page: http://python-jsonschema-objects.readthedocs.org/
 Author: Chris Wacek
 Author-email: cwacek@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `python_jsonschema_objects-0.4.3/README.md` & `python_jsonschema_objects-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/conftest.py` & `python_jsonschema_objects-0.4.4/conftest.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/docs/Introduction.md` & `python_jsonschema_objects-0.4.4/docs/Introduction.md`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/docs/Makefile` & `python_jsonschema_objects-0.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/docs/conf.py` & `python_jsonschema_objects-0.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/docs/index.rst` & `python_jsonschema_objects-0.4.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/python_jsonschema_objects/__init__.py` & `python_jsonschema_objects-0.4.4/python_jsonschema_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/python_jsonschema_objects/classbuilder.py` & `python_jsonschema_objects-0.4.4/python_jsonschema_objects/classbuilder.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/python_jsonschema_objects/descriptors.py` & `python_jsonschema_objects-0.4.4/python_jsonschema_objects/descriptors.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/python_jsonschema_objects/examples/README.md` & `python_jsonschema_objects-0.4.4/python_jsonschema_objects/examples/README.md`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/python_jsonschema_objects/literals.py` & `python_jsonschema_objects-0.4.4/python_jsonschema_objects/literals.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/python_jsonschema_objects/markdown_support.py` & `python_jsonschema_objects-0.4.4/python_jsonschema_objects/markdown_support.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/python_jsonschema_objects/pattern_properties.py` & `python_jsonschema_objects-0.4.4/python_jsonschema_objects/pattern_properties.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/python_jsonschema_objects/util.py` & `python_jsonschema_objects-0.4.4/python_jsonschema_objects/util.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/python_jsonschema_objects/validators.py` & `python_jsonschema_objects-0.4.4/python_jsonschema_objects/validators.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/python_jsonschema_objects/wrapper_types.py` & `python_jsonschema_objects-0.4.4/python_jsonschema_objects/wrapper_types.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/python_jsonschema_objects.egg-info/PKG-INFO` & `python_jsonschema_objects-0.4.4/python_jsonschema_objects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-jsonschema-objects
-Version: 0.4.3
+Version: 0.4.4
 Summary: An object wrapper for JSON Schema definitions
 Home-page: http://python-jsonschema-objects.readthedocs.org/
 Author: Chris Wacek
 Author-email: cwacek@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `python_jsonschema_objects-0.4.3/python_jsonschema_objects.egg-info/SOURCES.txt` & `python_jsonschema_objects-0.4.4/python_jsonschema_objects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/setup.py` & `python_jsonschema_objects-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         package_data={"python_jsonschema_objects.examples": ["README.md"]},
         zip_safe=False,
         url="http://python-jsonschema-objects.readthedocs.org/",
         setup_requires=["setuptools>=18.0.0"],
         install_requires=[
             "inflection>=0.2",
             "Markdown>=2.4",
-            "jsonschema>=2.3,<4.1.8",
+            "jsonschema>=2.3,<4.18",
             "six>=1.5.2",
         ],
         cmdclass=versioneer.get_cmdclass(),
         classifiers=[
             "Programming Language :: Python :: 2",
             "Programming Language :: Python :: 2.7",
             "Programming Language :: Python :: 3",
```

### Comparing `python_jsonschema_objects-0.4.3/test/resources/query.json` & `python_jsonschema_objects-0.4.4/test/resources/query.json`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/resources/schema.json` & `python_jsonschema_objects-0.4.4/test/resources/schema.json`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_array_validation.py` & `python_jsonschema_objects-0.4.4/test/test_array_validation.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_circular_references.py` & `python_jsonschema_objects-0.4.4/test/test_circular_references.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_default_values.py` & `python_jsonschema_objects-0.4.4/test/test_default_values.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_feature_151.py` & `python_jsonschema_objects-0.4.4/test/test_feature_151.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_feature_177.py` & `python_jsonschema_objects-0.4.4/test/test_feature_177.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_nested_arrays.py` & `python_jsonschema_objects-0.4.4/test/test_nested_arrays.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_nondefault_resolver_validator.py` & `python_jsonschema_objects-0.4.4/test/test_nondefault_resolver_validator.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_pattern_properties.py` & `python_jsonschema_objects-0.4.4/test/test_pattern_properties.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_pytest.py` & `python_jsonschema_objects-0.4.4/test/test_pytest.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_114.py` & `python_jsonschema_objects-0.4.4/test/test_regression_114.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_126.py` & `python_jsonschema_objects-0.4.4/test/test_regression_126.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_133.py` & `python_jsonschema_objects-0.4.4/test/test_regression_133.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_143.py` & `python_jsonschema_objects-0.4.4/test/test_regression_143.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_156.py` & `python_jsonschema_objects-0.4.4/test/test_regression_156.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_165.py` & `python_jsonschema_objects-0.4.4/test/test_regression_165.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_17.py` & `python_jsonschema_objects-0.4.4/test/test_regression_17.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_185.py` & `python_jsonschema_objects-0.4.4/test/test_regression_185.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_208.py` & `python_jsonschema_objects-0.4.4/test/test_regression_208.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_213.py` & `python_jsonschema_objects-0.4.4/test/test_regression_213.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_214.py` & `python_jsonschema_objects-0.4.4/test/test_regression_214.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_232.py` & `python_jsonschema_objects-0.4.4/test/test_regression_232.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_49.py` & `python_jsonschema_objects-0.4.4/test/test_regression_49.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_8.py` & `python_jsonschema_objects-0.4.4/test/test_regression_8.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_88.py` & `python_jsonschema_objects-0.4.4/test/test_regression_88.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_regression_90.py` & `python_jsonschema_objects-0.4.4/test/test_regression_90.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_util_pytest.py` & `python_jsonschema_objects-0.4.4/test/test_util_pytest.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/test_wrong_exception_protocolbase_getitem.py` & `python_jsonschema_objects-0.4.4/test/test_wrong_exception_protocolbase_getitem.py`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/thing-one.json` & `python_jsonschema_objects-0.4.4/test/thing-one.json`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/test/thing-two.json` & `python_jsonschema_objects-0.4.4/test/thing-two.json`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/tox.ini` & `python_jsonschema_objects-0.4.4/tox.ini`

 * *Files identical despite different names*

### Comparing `python_jsonschema_objects-0.4.3/versioneer.py` & `python_jsonschema_objects-0.4.4/versioneer.py`

 * *Files identical despite different names*

