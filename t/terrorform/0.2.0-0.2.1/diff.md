# Comparing `tmp/terrorform-0.2.0.tar.gz` & `tmp/terrorform-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrorform-0.2.0.tar", last modified: Tue Aug 30 15:58:00 2022, max compression
+gzip compressed data, was "terrorform-0.2.1.tar", last modified: Mon Aug  7 20:46:09 2023, max compression
```

## Comparing `terrorform-0.2.0.tar` & `terrorform-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-08-30 15:58:00.414921 terrorform-0.2.0/
--rw-r--r--   0 ben        (501) staff       (20)     1060 2022-06-15 17:39:11.000000 terrorform-0.2.0/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)     2206 2022-08-30 15:58:00.414551 terrorform-0.2.0/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     1895 2022-06-17 05:19:03.000000 terrorform-0.2.0/README.md
--rw-r--r--   0 ben        (501) staff       (20)       38 2022-08-30 15:58:00.415014 terrorform-0.2.0/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)      557 2022-08-30 15:56:55.000000 terrorform-0.2.0/setup.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-08-30 15:58:00.412667 terrorform-0.2.0/terrorform/
--rw-r--r--   0 ben        (501) staff       (20)       87 2022-08-02 18:13:30.000000 terrorform-0.2.0/terrorform/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     6301 2022-08-30 15:55:19.000000 terrorform-0.2.0/terrorform/terrorform.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-08-30 15:58:00.414213 terrorform-0.2.0/terrorform.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     2206 2022-08-30 15:58:00.000000 terrorform-0.2.0/terrorform.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      243 2022-08-30 15:58:00.000000 terrorform-0.2.0/terrorform.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2022-08-30 15:58:00.000000 terrorform-0.2.0/terrorform.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)        7 2022-08-30 15:58:00.000000 terrorform-0.2.0/terrorform.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       11 2022-08-30 15:58:00.000000 terrorform-0.2.0/terrorform.egg-info/top_level.txt
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-08-07 20:46:09.517560 terrorform-0.2.1/
+-rw-r--r--   0 ben        (501) staff       (20)     1060 2023-08-07 20:18:16.000000 terrorform-0.2.1/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)     2187 2023-08-07 20:46:09.517469 terrorform-0.2.1/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     1895 2023-08-07 20:18:16.000000 terrorform-0.2.1/README.md
+-rw-r--r--   0 ben        (501) staff       (20)       38 2023-08-07 20:46:09.517597 terrorform-0.2.1/setup.cfg
+-rw-r--r--   0 ben        (501) staff       (20)      557 2023-08-07 20:46:02.000000 terrorform-0.2.1/setup.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-08-07 20:46:09.516704 terrorform-0.2.1/terrorform/
+-rw-r--r--   0 ben        (501) staff       (20)       87 2023-08-07 20:18:16.000000 terrorform-0.2.1/terrorform/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     6321 2023-08-07 20:19:17.000000 terrorform-0.2.1/terrorform/terrorform.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-08-07 20:46:09.517310 terrorform-0.2.1/terrorform.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     2187 2023-08-07 20:46:09.000000 terrorform-0.2.1/terrorform.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      243 2023-08-07 20:46:09.000000 terrorform-0.2.1/terrorform.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-08-07 20:46:09.000000 terrorform-0.2.1/terrorform.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)        7 2023-08-07 20:46:09.000000 terrorform-0.2.1/terrorform.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       11 2023-08-07 20:46:09.000000 terrorform-0.2.1/terrorform.egg-info/top_level.txt
```

### Comparing `terrorform-0.2.0/LICENSE` & `terrorform-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terrorform-0.2.0/PKG-INFO` & `terrorform-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: terrorform
-Version: 0.2.0
+Version: 0.2.1
 Summary: Terraform wrapper for python
 Home-page: https://github.com/bengetch/terrorform
 Author: bengetch
 Author-email: bengetch@gmail.com
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## terrorform
 
 Python wrapper for [Terraform](https://www.terraform.io/)
@@ -81,8 +80,7 @@
 ### Testing
 
 Tests are run using `pytest`:
 
 ```shell
 python -m pytest tests.py
 ```
-
```

### Comparing `terrorform-0.2.0/README.md` & `terrorform-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `terrorform-0.2.0/setup.py` & `terrorform-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="terrorform",
-    version="0.2.0",
+    version="0.2.1",
     packages=find_packages(),
     include_package_data=True,
     install_requires=["pytest"],
     license="MIT",
     url="https://github.com/bengetch/terrorform",
     author="bengetch",
     author_email="bengetch@gmail.com",
```

### Comparing `terrorform-0.2.0/terrorform/terrorform.py` & `terrorform-0.2.1/terrorform/terrorform.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 TERRORFORM_OPTIONS = {
     # non-global options for terraform need to be placed *after* the workflow keyword
     # when using the CLI, while global options are placed *before* the workflow keyword
     # TODO: this list is not exhaustive, but Terraform documentation doesn't appear to
     #  provide a centralized global parameter list. Will need to look into it more.
     "NON_GLOBAL_KW_OPTIONS": [
         "-input", "-lock", "-lock-timeout", "-refresh", "-replace", "-target",
-        "-var", "-var-file", "-parallelism", "-state", "-state-out", "-backup"
+        "-var", "-var-file", "-parallelism", "-state", "-state-out", "-backup",
+        "-backend"
     ],
     # Suppress user prompts for approval at runtime for apply and destroy workflows.
     # Overriding this flag is not recommended, as the prompt itself will not actually
     # display at runtime, and the program will hang for an indefinite period of time
     # before crashing.
     "AUTO_APPROVE": True,
     # Prevent terraform from placing state locking on .tfstate files.
```

### Comparing `terrorform-0.2.0/terrorform.egg-info/PKG-INFO` & `terrorform-0.2.1/terrorform.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: terrorform
-Version: 0.2.0
+Version: 0.2.1
 Summary: Terraform wrapper for python
 Home-page: https://github.com/bengetch/terrorform
 Author: bengetch
 Author-email: bengetch@gmail.com
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## terrorform
 
 Python wrapper for [Terraform](https://www.terraform.io/)
@@ -81,8 +80,7 @@
 ### Testing
 
 Tests are run using `pytest`:
 
 ```shell
 python -m pytest tests.py
 ```
-
```

