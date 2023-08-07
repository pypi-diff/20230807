# Comparing `tmp/atksh-utils-0.4.0.tar.gz` & `tmp/atksh-utils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.4.0.tar", last modified: Mon Aug  7 01:20:23 2023, max compression
+gzip compressed data, was "atksh-utils-0.4.1.tar", last modified: Mon Aug  7 01:24:59 2023, max compression
```

## Comparing `atksh-utils-0.4.0.tar` & `atksh-utils-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.640003 atksh-utils-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.636003 atksh-utils-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.636003 atksh-utils-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-07 01:20:23.640003 atksh-utils-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 01:20:23.640003 atksh-utils-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.636003 atksh-utils-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.636003 atksh-utils-0.4.0/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.640003 atksh-utils-0.4.0/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/src/atksh_utils/openai/api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1616 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/src/atksh_utils/openai/askgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/src/atksh_utils/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-07 01:20:23.000000 atksh-utils-0.4.0/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.636003 atksh-utils-0.4.0/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-07 01:20:23.000000 atksh-utils-0.4.0/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-07 01:20:23.000000 atksh-utils-0.4.0/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 01:20:23.000000 atksh-utils-0.4.0/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 01:20:23.000000 atksh-utils-0.4.0/src/atksh_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-07 01:20:23.000000 atksh-utils-0.4.0/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 01:20:23.000000 atksh-utils-0.4.0/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.636003 atksh-utils-0.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:20:23.640003 atksh-utils-0.4.0/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-07 01:20:11.000000 atksh-utils-0.4.0/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.128282 atksh-utils-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.124282 atksh-utils-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.124282 atksh-utils-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-07 01:24:59.128282 atksh-utils-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 01:24:59.128282 atksh-utils-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.124282 atksh-utils-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.124282 atksh-utils-0.4.1/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.128282 atksh-utils-0.4.1/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/src/atksh_utils/openai/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1763 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/src/atksh_utils/openai/askgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/src/atksh_utils/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-07 01:24:58.000000 atksh-utils-0.4.1/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.128282 atksh-utils-0.4.1/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-07 01:24:59.000000 atksh-utils-0.4.1/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-07 01:24:59.000000 atksh-utils-0.4.1/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 01:24:59.000000 atksh-utils-0.4.1/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 01:24:59.000000 atksh-utils-0.4.1/src/atksh_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-07 01:24:59.000000 atksh-utils-0.4.1/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 01:24:59.000000 atksh-utils-0.4.1/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.124282 atksh-utils-0.4.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.128282 atksh-utils-0.4.1/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.4.0/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.4.1/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.0/.gitignore` & `atksh-utils-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.0/LICENSE` & `atksh-utils-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.0/PKG-INFO` & `atksh-utils-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.4.0
+Version: 0.4.1
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.4.0/README.md` & `atksh-utils-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.0/pyproject.toml` & `atksh-utils-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.0/src/atksh_utils/openai/api.py` & `atksh-utils-0.4.1/src/atksh_utils/openai/api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.0/src/atksh_utils/openai/askgpt.py` & `atksh-utils-0.4.1/src/atksh_utils/openai/askgpt.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,18 @@
         else:
             info = chunk["choices"][0]
             if info["finish_reason"] == "function_call":
                 function_name = message["function_call"]["name"]
                 function_call_args = json.loads(message["function_call"]["arguments"])
                 pretty_args = []
                 for arg, value in function_call_args.items():
-                    pretty_args.append(f"\t{arg}={value}")
+                    if "\n" not in value:
+                        pretty_args.append(f"\t{arg}={value}")
+                    else:
+                        pretty_args.append(f'\t{arg}=\n"""\n{value}\n"""')
                 pretty_args = ",\n".join(pretty_args)
                 text = f"{function_name}(\n{pretty_args}\n)"
                 print("function_call:")
                 print(text)
                 print()
         return
     token = chunk["choices"][0]["delta"].get("content", "")
```

### Comparing `atksh-utils-0.4.0/src/atksh_utils/openai/functional.py` & `atksh-utils-0.4.1/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.0/src/atksh_utils/openai/prompt.py` & `atksh-utils-0.4.1/src/atksh_utils/openai/prompt.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.0/src/atksh_utils/openai/tool.py` & `atksh-utils-0.4.1/src/atksh_utils/openai/tool.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.0/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.4.1/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.4.0
+Version: 0.4.1
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.4.0/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.4.1/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.0/tests/openai/test_api.py` & `atksh-utils-0.4.1/tests/openai/test_api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.0/tests/openai/test_functional.py` & `atksh-utils-0.4.1/tests/openai/test_functional.py`

 * *Files identical despite different names*

