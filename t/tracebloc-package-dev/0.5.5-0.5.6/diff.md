# Comparing `tmp/tracebloc_package-dev-0.5.5.tar.gz` & `tmp/tracebloc_package-dev-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.5.5.tar", last modified: Fri Aug  4 11:43:54 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.5.6.tar", last modified: Mon Aug  7 13:57:30 2023, max compression
```

## Comparing `tracebloc_package-dev-0.5.5.tar` & `tracebloc_package-dev-0.5.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-08-04 11:43:54.937171 tracebloc_package-dev-0.5.5/
--rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.5.5/LICENSE.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-08-04 11:43:54.937263 tracebloc_package-dev-0.5.5/PKG-INFO
--rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.5.5/README.md
--rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-08-04 11:43:54.937573 tracebloc_package-dev-0.5.5/setup.cfg
--rw-r--r--   0 divyasingh   (501) staff       (20)      949 2023-08-04 11:43:45.000000 tracebloc_package-dev-0.5.5/setup.py
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-08-04 11:43:54.935561 tracebloc_package-dev-0.5.5/tracebloc_package/
--rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.5.5/tracebloc_package/__init__.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     5669 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.5.5/tracebloc_package/check_parameters.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    29559 2023-08-04 06:55:34.000000 tracebloc_package-dev-0.5.5/tracebloc_package/functional_test.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    58421 2023-08-02 07:41:20.000000 tracebloc_package-dev-0.5.5/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.5.5/tracebloc_package/messages.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    11477 2023-08-04 06:55:34.000000 tracebloc_package-dev-0.5.5/tracebloc_package/upload.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    10427 2023-06-09 08:04:05.000000 tracebloc_package-dev-0.5.5/tracebloc_package/user.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     6860 2023-08-03 15:22:24.000000 tracebloc_package-dev-0.5.5/tracebloc_package/utils.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     3200 2023-06-09 08:04:05.000000 tracebloc_package-dev-0.5.5/tracebloc_package/weights.py
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-08-04 11:43:54.936993 tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/
--rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-08-04 11:43:54.000000 tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-08-04 11:43:54.000000 tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-08-04 11:43:54.000000 tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-08-04 11:43:54.000000 tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 divyasingh   (501) staff       (20)      119 2023-08-04 11:43:54.000000 tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-08-04 11:43:54.000000 tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-08-07 13:57:30.754644 tracebloc_package-dev-0.5.6/
+-rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.5.6/LICENSE.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-08-07 13:57:30.754721 tracebloc_package-dev-0.5.6/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.5.6/README.md
+-rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-08-07 13:57:30.754997 tracebloc_package-dev-0.5.6/setup.cfg
+-rw-r--r--   0 divyasingh   (501) staff       (20)      949 2023-08-07 13:55:56.000000 tracebloc_package-dev-0.5.6/setup.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-08-07 13:57:30.753286 tracebloc_package-dev-0.5.6/tracebloc_package/
+-rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.5.6/tracebloc_package/__init__.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     5669 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.5.6/tracebloc_package/check_parameters.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    29608 2023-08-07 13:47:52.000000 tracebloc_package-dev-0.5.6/tracebloc_package/functional_test.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    58421 2023-08-02 07:41:20.000000 tracebloc_package-dev-0.5.6/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.5.6/tracebloc_package/messages.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    11477 2023-08-04 06:55:34.000000 tracebloc_package-dev-0.5.6/tracebloc_package/upload.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    10427 2023-06-09 08:04:05.000000 tracebloc_package-dev-0.5.6/tracebloc_package/user.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     6860 2023-08-03 15:22:24.000000 tracebloc_package-dev-0.5.6/tracebloc_package/utils.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     3200 2023-06-09 08:04:05.000000 tracebloc_package-dev-0.5.6/tracebloc_package/weights.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-08-07 13:57:30.754504 tracebloc_package-dev-0.5.6/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-08-07 13:57:30.000000 tracebloc_package-dev-0.5.6/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-08-07 13:57:30.000000 tracebloc_package-dev-0.5.6/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-08-07 13:57:30.000000 tracebloc_package-dev-0.5.6/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-08-07 13:57:30.000000 tracebloc_package-dev-0.5.6/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 divyasingh   (501) staff       (20)      119 2023-08-07 13:57:30.000000 tracebloc_package-dev-0.5.6/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-08-07 13:57:30.000000 tracebloc_package-dev-0.5.6/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.5.5/LICENSE.txt` & `tracebloc_package-dev-0.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.5/PKG-INFO` & `tracebloc_package-dev-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.5.5
+Version: 0.5.6
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `tracebloc_package-dev-0.5.5/setup.py` & `tracebloc_package-dev-0.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.5.5",
+    version="0.5.6",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.5.5/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.5.6/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.5/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.5.6/tracebloc_package/functional_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,18 +52,18 @@
             if main_file and self.framework == TENSORFLOW_FRAMEWORK:
                 self.tmp_file = os.path.join(self.tmp_file_path, self.file_name)
                 if self.main_method == "":
                     self.load_model(temp_file)
                     self.add_method(temp_file, remove_lines)
                 else:
                     self.edit_file(temp_file, filelines, remove_lines)
-            elif self.framework == PYTORCH_FRAMEWORK:
+            elif self.framework == PYTORCH_FRAMEWORK and main_file:
                 self.tmp_file = os.path.join(self.tmp_file_path, self.file_name)
                 self.edit_file(temp_file, filelines, remove_lines)
-            else:
+            elif main_file and self.framework == "":
                 raise Exception("\nFramework argument missing in file")
         except Exception as e:
             raise e
 
     def get_variables(self, temp_file):
         main_file = False
         remove_lines = []
```

### Comparing `tracebloc_package-dev-0.5.5/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.5.6/tracebloc_package/linkModelDataSet.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.5/tracebloc_package/messages.py` & `tracebloc_package-dev-0.5.6/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.5/tracebloc_package/upload.py` & `tracebloc_package-dev-0.5.6/tracebloc_package/upload.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.5/tracebloc_package/user.py` & `tracebloc_package-dev-0.5.6/tracebloc_package/user.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.5/tracebloc_package/utils.py` & `tracebloc_package-dev-0.5.6/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.5/tracebloc_package/weights.py` & `tracebloc_package-dev-0.5.6/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.5.6/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.5.5
+Version: 0.5.6
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.5.6/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

