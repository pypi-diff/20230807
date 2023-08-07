# Comparing `tmp/bump-my-version-0.9.1.tar.gz` & `tmp/bump-my-version-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bump-my-version-0.9.1.tar", last modified: Thu Aug  3 12:58:49 2023, max compression
+gzip compressed data, was "bump-my-version-0.9.2.tar", last modified: Mon Aug  7 14:13:59 2023, max compression
```

## Comparing `bump-my-version-0.9.1.tar` & `bump-my-version-0.9.2.tar`

### file list

```diff
@@ -1,67 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:49.558560 bump-my-version-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-08-03 12:58:49.558560 bump-my-version-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:49.554560 bump-my-version-0.9.1/bump_my_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-08-03 12:58:49.000000 bump-my-version-0.9.1/bump_my_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-03 12:58:49.000000 bump-my-version-0.9.1/bump_my_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:58:49.000000 bump-my-version-0.9.1/bump_my_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-03 12:58:49.000000 bump-my-version-0.9.1/bump_my_version.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-03 12:58:49.000000 bump-my-version-0.9.1/bump_my_version.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-03 12:58:49.000000 bump-my-version-0.9.1/bump_my_version.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:49.554560 bump-my-version-0.9.1/bumpversion/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/bump.py
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/show.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/version_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/bumpversion/yaml_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-03 12:58:49.558560 bump-my-version-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:49.558560 bump-my-version-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:49.558560 bump-my-version-0.9.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/fixtures/basic_cfg.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/fixtures/basic_cfg.toml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/fixtures/basic_cfg_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/fixtures/basic_cfg_expected.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/fixtures/basic_cfg_expected.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/fixtures/basic_cfg_expected_full.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:49.558560 bump-my-version-0.9.1/tests/fixtures/glob/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:49.558560 bump-my-version-0.9.1/tests/fixtures/glob/directory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/fixtures/glob/directory/file3.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/fixtures/glob/file1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/fixtures/glob/file2.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/fixtures/glob/not-text.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:49.558560 bump-my-version-0.9.1/tests/fixtures/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/fixtures/interpolation/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/fixtures/interpolation/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/fixtures/interpolation/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/fixtures/pep440.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/test_autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/test_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)    18732 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/test_show.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/test_version_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-03 12:58:23.000000 bump-my-version-0.9.1/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.077245 bump-my-version-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    23198 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-08-07 14:13:59.077245 bump-my-version-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.069244 bump-my-version-0.9.2/bump_my_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-08-07 14:13:59.000000 bump-my-version-0.9.2/bump_my_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-07 14:13:59.000000 bump-my-version-0.9.2/bump_my_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:13:59.000000 bump-my-version-0.9.2/bump_my_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 14:13:59.000000 bump-my-version-0.9.2/bump_my_version.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-07 14:13:59.000000 bump-my-version-0.9.2/bump_my_version.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 14:13:59.000000 bump-my-version-0.9.2/bump_my_version.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.073244 bump-my-version-0.9.2/bumpversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/version_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/bumpversion/yaml_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-07 14:13:59.077245 bump-my-version-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.073244 bump-my-version-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.073244 bump-my-version-0.9.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/basic_cfg.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/basic_cfg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected_full.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.073244 bump-my-version-0.9.2/tests/fixtures/csharp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/csharp/.bumpversion.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/csharp/AssemblyInfo.cs
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/csharp/FULL_VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/csharp/Version.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.077245 bump-my-version-0.9.2/tests/fixtures/glob/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.077245 bump-my-version-0.9.2/tests/fixtures/glob/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/glob/directory/file3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/glob/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/glob/file2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/glob/not-text.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:13:59.077245 bump-my-version-0.9.2/tests/fixtures/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/interpolation/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/interpolation/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/interpolation/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/fixtures/pep440.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18732 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16079 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_version_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-07 14:13:39.000000 bump-my-version-0.9.2/tests/test_yaml.py
```

### Comparing `bump-my-version-0.9.1/CHANGELOG.md` & `bump-my-version-0.9.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## 0.9.2 (2023-08-07)
+[Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.9.1...0.9.2)
+
+### Fixes
+
+- Fixed modified context when committing. [130bbe0](https://github.com/callowayproject/bump-my-version/commit/130bbe0dc9cbc436ed2d4a74878937fc784fbccd)
+    
+  - Resets the context before committing and tagging
+  - Fixes #14
+
 ## 0.9.1 (2023-08-03)
 [Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.9.0...0.9.1)
 
 ### Other
 
 - [pre-commit.ci] auto fixes from pre-commit.com hooks. [4b457d0](https://github.com/callowayproject/bump-my-version/commit/4b457d0d15b881612de7e8970f729f5ea0556c9d)
```

### Comparing `bump-my-version-0.9.1/CODE_OF_CONDUCT.md` & `bump-my-version-0.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/CONTRIBUTING.md` & `bump-my-version-0.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/LICENSE` & `bump-my-version-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/PKG-INFO` & `bump-my-version-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.9.1
+Version: 0.9.2
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bump-my-version-0.9.1/README.md` & `bump-my-version-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/bump_my_version.egg-info/PKG-INFO` & `bump-my-version-0.9.2/bump_my_version.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.9.1
+Version: 0.9.2
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bump-my-version-0.9.1/bump_my_version.egg-info/SOURCES.txt` & `bump-my-version-0.9.2/bump_my_version.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,18 @@
 tests/fixtures/basic_cfg.cfg
 tests/fixtures/basic_cfg.toml
 tests/fixtures/basic_cfg_expected.json
 tests/fixtures/basic_cfg_expected.txt
 tests/fixtures/basic_cfg_expected.yaml
 tests/fixtures/basic_cfg_expected_full.json
 tests/fixtures/pep440.toml
+tests/fixtures/csharp/.bumpversion.toml
+tests/fixtures/csharp/AssemblyInfo.cs
+tests/fixtures/csharp/FULL_VERSION.txt
+tests/fixtures/csharp/Version.csv
 tests/fixtures/glob/file1.txt
 tests/fixtures/glob/file2.txt
 tests/fixtures/glob/not-text.md
 tests/fixtures/glob/directory/file3.txt
 tests/fixtures/interpolation/.bumpversion.cfg
 tests/fixtures/interpolation/pyproject.toml
 tests/fixtures/interpolation/setup.cfg
```

### Comparing `bump-my-version-0.9.1/bumpversion/aliases.py` & `bump-my-version-0.9.2/bumpversion/aliases.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/bumpversion/autocast.py` & `bump-my-version-0.9.2/bumpversion/autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/bumpversion/bump.py` & `bump-my-version-0.9.2/bumpversion/bump.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,17 +77,18 @@
     if dry_run:
         logger.info("Dry run active, won't touch any files.")
 
     ctx = get_context(config, version, next_version)
 
     configured_files = resolve_file_config(config.files, config.version_config)
     modify_files(configured_files, version, next_version, ctx, dry_run)
-
     update_config_file(config_file, config.current_version, next_version_str, dry_run)
 
+    ctx = get_context(config, version, next_version)
+    ctx["new_version"] = next_version_str
     commit_and_tag(config, config_file, configured_files, ctx, dry_run)
 
 
 def commit_and_tag(
     config: Config,
     config_file: Optional[Path],
     configured_files: List["ConfiguredFile"],
```

### Comparing `bump-my-version-0.9.1/bumpversion/cli.py` & `bump-my-version-0.9.2/bumpversion/cli.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/bumpversion/config.py` & `bump-my-version-0.9.2/bumpversion/config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/bumpversion/exceptions.py` & `bump-my-version-0.9.2/bumpversion/exceptions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/bumpversion/files.py` & `bump-my-version-0.9.2/bumpversion/files.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/bumpversion/functions.py` & `bump-my-version-0.9.2/bumpversion/functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/bumpversion/logging.py` & `bump-my-version-0.9.2/bumpversion/logging.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/bumpversion/scm.py` & `bump-my-version-0.9.2/bumpversion/scm.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/bumpversion/show.py` & `bump-my-version-0.9.2/bumpversion/show.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/bumpversion/utils.py` & `bump-my-version-0.9.2/bumpversion/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         {"current_version": config.current_version},
         {"now": datetime.datetime.now(), "utcnow": datetime.datetime.utcnow()},
         prefixed_environ(),
         asdict(config.scm_info),
         {c: c for c in ("#", ";")},
     )
     if current_version:
-        ctx.new_child({f"current_{part}": current_version[part].value for part in current_version})
+        ctx = ctx.new_child({f"current_{part}": current_version[part].value for part in current_version})
     if new_version:
-        ctx.new_child({f"new_{part}": new_version[part].value for part in new_version})
+        ctx = ctx.new_child({f"new_{part}": new_version[part].value for part in new_version})
     return ctx
 
 
 def get_overrides(**kwargs) -> dict:
     """Return a dictionary containing only the overridden key-values."""
     return {key: val for key, val in kwargs.items() if val is not None}
```

### Comparing `bump-my-version-0.9.1/bumpversion/version_part.py` & `bump-my-version-0.9.2/bumpversion/version_part.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/bumpversion/yaml_dump.py` & `bump-my-version-0.9.2/bumpversion/yaml_dump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/pyproject.toml` & `bump-my-version-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 [tool.ruff.isort]
 order-by-type = true
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.bumpversion]
-current_version = "0.9.1"
+current_version = "0.9.2"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "{new_version}"
 allow_dirty = true
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.(?P<dev>dev\\d+))?"
 serialize = [
```

### Comparing `bump-my-version-0.9.1/tests/conftest.py` & `bump-my-version-0.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/fixtures/basic_cfg.cfg` & `bump-my-version-0.9.2/tests/fixtures/basic_cfg.cfg`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/fixtures/basic_cfg.toml` & `bump-my-version-0.9.2/tests/fixtures/basic_cfg.toml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/fixtures/basic_cfg_expected.json` & `bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected.json`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/fixtures/basic_cfg_expected.txt` & `bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected.txt`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/fixtures/basic_cfg_expected.yaml` & `bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected.yaml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/fixtures/basic_cfg_expected_full.json` & `bump-my-version-0.9.2/tests/fixtures/basic_cfg_expected_full.json`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/fixtures/pep440.toml` & `bump-my-version-0.9.2/tests/fixtures/pep440.toml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/test_autocast.py` & `bump-my-version-0.9.2/tests/test_autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/test_bump.py` & `bump-my-version-0.9.2/tests/test_bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/test_cli.py` & `bump-my-version-0.9.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/test_config.py` & `bump-my-version-0.9.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/test_files.py` & `bump-my-version-0.9.2/tests/test_files.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """File processing tests."""
 import os
+import shutil
 from datetime import datetime, timezone
 from pathlib import Path
 from textwrap import dedent
 
 import pytest
 from pytest import param
 
-from bumpversion import exceptions, files
+from bumpversion import exceptions, files, config, bump
 from bumpversion.utils import get_context
 from bumpversion.exceptions import VersionNotFoundError
+from bumpversion.version_part import VersionConfig
 from tests.conftest import get_config_data, inside_dir
 
 
 @pytest.mark.parametrize(
     ["glob_pattern", "file_list"],
     [
         param("*.txt", {Path("file1.txt"), Path("file2.txt")}, id="simple-glob"),
@@ -150,79 +152,54 @@
 
     assert full_vers_path.read_text() == "2.0.1"
     assert maj_vers_path.read_text() == "2"
     assert readme_path.read_text() == "MyAwesomeSoftware(TM) v2.0"
     assert build_num_path.read_text() == "2.0.1+jane+38945"
 
 
-def test_raises_correct_missing_version_string(tmp_path: Path):
-    full_vers_path = tmp_path / "FULL_VERSION.txt"
-    full_vers_path.write_text("3.1.0-rc+build.1031")
-    assembly_path = tmp_path / "AssemblyInfo.cs"
-    assembly_path.write_text(
-        '[assembly: AssemblyFileVersion("3.1.0-rc+build.1031")]\n' '[assembly: AssemblyVersion("3.1.1031.0")]'
-    )
-    csv_path = tmp_path / "Version.csv"
-    csv_path.write_text("1;3-1;0;rc;build.1031")
-
-    overrides = {
-        "current_version": "3.1.0-rc+build.1031",
-        "parse": r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(-(?P<release>[0-9A-Za-z]+))?(\+build\.(?P<build>.[0-9A-Za-z]+))?",
-        "serialize": ["{major}.{minor}.{patch}-{release}+build.{build}", "{major}.{minor}.{patch}+build.{build}"],
-        "commit": True,
-        "message": "Bump version: {current_version} -> {new_version}",
-        "tag": False,
-        "tag_name": "{new_version}",
-        "tag_message": "Version {new_version}",
-        "allow_dirty": True,
-        "files": [
-            {
-                "filename": str(full_vers_path),
-            },
-            {
-                "filename": str(assembly_path),
-                "search": '[assembly: AssemblyFileVersion("{current_version}")]',
-                "replace": '[assembly: AssemblyFileVersion("{new_version}")]',
-            },
-            {
-                "filename": str(assembly_path),
-                "parse": r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<build>\d+)\.(?P<patch>\d+)",
-                "serialize": ["{major}.{minor}.{build}.{patch}"],
-                "search": '[assembly: AssemblyVersion("{current_version}")]',
-                "replace": '[assembly: AssemblyVersion("{new_version}")]',
-            },
-            {
-                "filename": str(csv_path),
-                "parse": r"(?P<major>\d+);(?P<minor>\d+);(?P<patch>\d+);(?P<release>[0-9A-Za-z]+)?;(build\.(?P<build>.[0-9A-Za-z]+))?",
-                "serialize": [
-                    "{major};{minor};{patch};{release};build.{build}",
-                    "{major};{minor};{patch};;build.{build}",
-                ],
-                "search": "1;{current_version}",
-                "replace": "1;{new_version}",
-            },
-        ],
-        "parts": {
-            "release": {"values": ["beta", "rc", "final"], "optional_value": "final"},
-            "build": {
-                "first_value": 1000,
-                "independent": True,
-            },
-        },
-    }
-    conf, version_config, current_version = get_config_data(overrides)
-    major_version = current_version.bump("patch", version_config.order)
+def test_raises_correct_missing_version_string(tmp_path: Path, fixtures_path: Path):
+    """When a file is missing the version string, the error should indicate the correct serialization missing."""
+    csharp_path = fixtures_path / "csharp"
+    dst_path: Path = shutil.copytree(csharp_path, tmp_path / "csharp")
+
+    with inside_dir(dst_path):
+        conf = config.get_configuration(config_file=dst_path.joinpath(".bumpversion.toml"))
+        version_config = VersionConfig(conf.parse, conf.serialize, conf.search, conf.replace, conf.parts)
+        current_version = version_config.parse(conf.current_version)
+        dst_path.joinpath("Version.csv").write_text("1;3-1;0;rc;build.1031")
+
+        major_version = current_version.bump("patch", version_config.order)
+        ctx = get_context(conf)
+
+        configured_files = [files.ConfiguredFile(file_cfg, version_config) for file_cfg in conf.files]
+
+        with pytest.raises(VersionNotFoundError) as e:
+            files.modify_files(configured_files, current_version, major_version, ctx)
+            assert e.message.startswith("Did not find '1;3;1;0;rc;build.1031'")
+
+
+def test_uses_correct_serialization_for_tag_and_commit_messages(git_repo: Path, fixtures_path: Path, caplog):
+    """The tag and commit messages should use the root configured serialization."""
+    import subprocess
+    import logging
 
-    ctx = get_context(conf)
+    caplog.set_level(logging.INFO)
 
-    configured_files = [files.ConfiguredFile(file_cfg, version_config) for file_cfg in conf.files]
+    csharp_path = fixtures_path / "csharp"
+    dst_path: Path = shutil.copytree(csharp_path, git_repo / "csharp")
+    subprocess.check_call(["git", "add", "."], cwd=git_repo)
+    subprocess.check_call(["git", "commit", "-m", "Initial commit"], cwd=git_repo)
+    subprocess.check_call(["git", "tag", "3.1.0-rc+build.1031"], cwd=git_repo)
+
+    with inside_dir(dst_path):
+        config_file = dst_path.joinpath(".bumpversion.toml")
+        conf = config.get_configuration(config_file=config_file)
+        bump.do_bump("patch", None, conf, config_file, dry_run=True)
 
-    with pytest.raises(VersionNotFoundError) as e:
-        files.modify_files(configured_files, current_version, major_version, ctx)
-        assert e.message.startswith("Did not find '1;3;1;0;rc;build.1031'")
+    assert "Bump version: 3.1.0-rc+build.1031 -> 3.1.1" in caplog.text
 
 
 def test_search_replace_to_avoid_updating_unconcerned_lines(tmp_path: Path, caplog):
     import logging
 
     caplog.set_level(logging.DEBUG)
     req_path = tmp_path / "requirements.txt"
```

### Comparing `bump-my-version-0.9.1/tests/test_functions.py` & `bump-my-version-0.9.2/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/test_scm.py` & `bump-my-version-0.9.2/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/test_show.py` & `bump-my-version-0.9.2/tests/test_show.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/test_version_part.py` & `bump-my-version-0.9.2/tests/test_version_part.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.9.1/tests/test_yaml.py` & `bump-my-version-0.9.2/tests/test_yaml.py`

 * *Files identical despite different names*

