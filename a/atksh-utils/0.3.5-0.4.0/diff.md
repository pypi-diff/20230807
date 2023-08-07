# Comparing `tmp/atksh-utils-0.3.5.tar.gz` & `tmp/atksh-utils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.3.5.tar", last modified: Sun Aug  6 07:33:55 2023, max compression
+gzip compressed data, was "atksh-utils-0.4.0.tar", last modified: Mon Aug  7 01:20:23 2023, max compression
```

## Comparing `atksh-utils-0.3.5.tar` & `atksh-utils-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:33:55.257208 atksh-utils-0.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:33:55.257208 atksh-utils-0.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:33:55.257208 atksh-utils-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-06 07:33:45.000000 atksh-utils-0.3.5/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-06 07:33:45.000000 atksh-utils-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-06 07:33:45.000000 atksh-utils-0.3.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-06 07:33:45.000000 atksh-utils-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-06 07:33:55.257208 atksh-utils-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-06 07:33:45.000000 atksh-utils-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-06 07:33:45.000000 atksh-utils-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-06 07:33:55.261208 atksh-utils-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:33:55.257208 atksh-utils-0.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:33:55.257208 atksh-utils-0.3.5/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:33:45.000000 atksh-utils-0.3.5/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:33:55.257208 atksh-utils-0.3.5/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-06 07:33:45.000000 atksh-utils-0.3.5/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-08-06 07:33:45.000000 atksh-utils-0.3.5/src/atksh_utils/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-06 07:33:45.000000 atksh-utils-0.3.5/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-06 07:33:45.000000 atksh-utils-0.3.5/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-06 07:33:45.000000 atksh-utils-0.3.5/src/atksh_utils/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-06 07:33:55.000000 atksh-utils-0.3.5/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:33:55.257208 atksh-utils-0.3.5/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-06 07:33:55.000000 atksh-utils-0.3.5/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-06 07:33:55.000000 atksh-utils-0.3.5/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:33:55.000000 atksh-utils-0.3.5/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-06 07:33:55.000000 atksh-utils-0.3.5/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-06 07:33:55.000000 atksh-utils-0.3.5/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:33:55.257208 atksh-utils-0.3.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:33:55.257208 atksh-utils-0.3.5/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-06 07:33:45.000000 atksh-utils-0.3.5/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-06 07:33:45.000000 atksh-utils-0.3.5/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.640003 atksh-utils-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.636003 atksh-utils-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.636003 atksh-utils-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-07 01:20:23.640003 atksh-utils-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 01:20:23.640003 atksh-utils-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.636003 atksh-utils-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.636003 atksh-utils-0.4.0/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.640003 atksh-utils-0.4.0/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/src/atksh_utils/openai/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1616 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/src/atksh_utils/openai/askgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/src/atksh_utils/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-07 01:20:23.000000 atksh-utils-0.4.0/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.636003 atksh-utils-0.4.0/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-07 01:20:23.000000 atksh-utils-0.4.0/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-07 01:20:23.000000 atksh-utils-0.4.0/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 01:20:23.000000 atksh-utils-0.4.0/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 01:20:23.000000 atksh-utils-0.4.0/src/atksh_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-07 01:20:23.000000 atksh-utils-0.4.0/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 01:20:23.000000 atksh-utils-0.4.0/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.636003 atksh-utils-0.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.640003 atksh-utils-0.4.0/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.3.5/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.4.0/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.5/.gitignore` & `atksh-utils-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.5/LICENSE` & `atksh-utils-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.5/PKG-INFO` & `atksh-utils-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.3.5
+Version: 0.4.0
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.3.5/README.md` & `atksh-utils-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.5/pyproject.toml` & `atksh-utils-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 description = "atksh's utils"
 dynamic = ["version"]
 license = {file = "LICENSE"}
 name = "atksh-utils"
 readme = "README.md"
 requires-python = ">=3.7"
 
+[project.scripts]
+askgpt = "atksh_utils.openai.askgpt:ask"
+
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [tool.setuptools.dynamic]
 version = {attr = "atksh_utils.version.__version__"}
 
 [tool.setuptools_scm]
```

### Comparing `atksh-utils-0.3.5/src/atksh_utils/openai/api.py` & `atksh-utils-0.4.0/src/atksh_utils/openai/api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.5/src/atksh_utils/openai/functional.py` & `atksh-utils-0.4.0/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.5/src/atksh_utils/openai/prompt.py` & `atksh-utils-0.4.0/src/atksh_utils/openai/prompt.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.5/src/atksh_utils/openai/tool.py` & `atksh-utils-0.4.0/src/atksh_utils/openai/tool.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.5/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.4.0/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.3.5
+Version: 0.4.0
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.3.5/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.4.0/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 setup.cfg
 .github/workflows/publish_to_pypi.yaml
 src/atksh_utils/__init__.py
 src/atksh_utils/version.py
 src/atksh_utils.egg-info/PKG-INFO
 src/atksh_utils.egg-info/SOURCES.txt
 src/atksh_utils.egg-info/dependency_links.txt
+src/atksh_utils.egg-info/entry_points.txt
 src/atksh_utils.egg-info/requires.txt
 src/atksh_utils.egg-info/top_level.txt
 src/atksh_utils/openai/__init__.py
 src/atksh_utils/openai/api.py
+src/atksh_utils/openai/askgpt.py
 src/atksh_utils/openai/functional.py
 src/atksh_utils/openai/prompt.py
 src/atksh_utils/openai/tool.py
 tests/openai/test_api.py
 tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.3.5/tests/openai/test_api.py` & `atksh-utils-0.4.0/tests/openai/test_api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.5/tests/openai/test_functional.py` & `atksh-utils-0.4.0/tests/openai/test_functional.py`

 * *Files identical despite different names*

